# Comparing `tmp/syncany-0.2.6.tar.gz` & `tmp/syncany-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syncany-0.2.6.tar", last modified: Tue Apr 25 09:43:43 2023, max compression
+gzip compressed data, was "syncany-0.2.7.tar", last modified: Fri Apr 28 09:59:18 2023, max compression
```

## Comparing `syncany-0.2.6.tar` & `syncany-0.2.7.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-25 09:43:43.802862 syncany-0.2.6/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1063 2022-08-13 12:36:15.000000 syncany-0.2.6/LICENSE
--rwxrwxrwx   0 snower    (1000) snower    (1000)     7103 2023-04-25 09:43:43.804884 syncany-0.2.6/PKG-INFO
--rwxrwxrwx   0 snower    (1000) snower    (1000)     5832 2022-08-13 12:36:15.000000 syncany-0.2.6/README.md
--rwxrwxrwx   0 snower    (1000) snower    (1000)       67 2023-04-25 09:43:43.814860 syncany-0.2.6/setup.cfg
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1928 2023-04-21 09:56:25.000000 syncany-0.2.6/setup.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-25 09:43:38.384634 syncany-0.2.6/syncany/
--rwxrwxrwx   0 snower    (1000) snower    (1000)      607 2023-04-21 09:56:25.000000 syncany-0.2.6/syncany/__init__.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-25 09:43:39.166440 syncany-0.2.6/syncany/calculaters/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4962 2023-04-25 03:51:51.000000 syncany-0.2.6/syncany/calculaters/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    39302 2023-04-19 07:06:22.000000 syncany-0.2.6/syncany/calculaters/builtin.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4394 2023-03-24 09:30:00.000000 syncany-0.2.6/syncany/calculaters/calculater.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     7999 2023-03-27 08:30:23.000000 syncany-0.2.6/syncany/calculaters/convert_calculater.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4573 2023-03-23 03:10:08.000000 syncany-0.2.6/syncany/calculaters/datetime_calculater.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2328 2023-04-25 04:06:56.000000 syncany-0.2.6/syncany/calculaters/import_calculater.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     3167 2023-03-23 03:10:08.000000 syncany-0.2.6/syncany/calculaters/textline_calculater.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    13907 2023-04-21 10:27:56.000000 syncany-0.2.6/syncany/calculaters/transform_calculater.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-25 09:43:40.173724 syncany-0.2.6/syncany/database/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     5187 2023-04-25 03:51:51.000000 syncany-0.2.6/syncany/database/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     8756 2023-03-24 06:27:35.000000 syncany-0.2.6/syncany/database/beanstalk.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    15594 2023-04-25 03:41:03.000000 syncany-0.2.6/syncany/database/clickhouse.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    15749 2023-04-25 02:15:32.000000 syncany-0.2.6/syncany/database/csv.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    10626 2023-02-23 11:47:13.000000 syncany-0.2.6/syncany/database/database.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    12481 2023-02-24 09:33:28.000000 syncany-0.2.6/syncany/database/elasticsearch.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    14490 2023-04-25 02:15:32.000000 syncany-0.2.6/syncany/database/excel.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    14218 2023-02-22 05:00:17.000000 syncany-0.2.6/syncany/database/http.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    17931 2023-02-24 09:33:28.000000 syncany-0.2.6/syncany/database/influxdb.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    12051 2023-04-25 02:15:32.000000 syncany-0.2.6/syncany/database/json.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    11954 2023-04-25 02:15:32.000000 syncany-0.2.6/syncany/database/memory.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    14642 2023-04-25 03:15:38.000000 syncany-0.2.6/syncany/database/mongodb.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    14723 2023-04-25 03:35:50.000000 syncany-0.2.6/syncany/database/mysql.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    14858 2023-04-25 03:37:13.000000 syncany-0.2.6/syncany/database/postgresql.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    18023 2023-04-25 02:22:52.000000 syncany-0.2.6/syncany/database/redis.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    13949 2023-03-28 03:39:46.000000 syncany-0.2.6/syncany/database/sqlite.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    15489 2023-04-25 03:39:10.000000 syncany-0.2.6/syncany/database/sqlserver.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    17928 2023-04-23 08:27:57.000000 syncany-0.2.6/syncany/database/textline.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      685 2022-08-23 12:03:29.000000 syncany-0.2.6/syncany/errors.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-25 09:43:40.338267 syncany-0.2.6/syncany/filters/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2275 2023-04-25 03:51:51.000000 syncany-0.2.6/syncany/filters/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    19439 2023-04-01 08:20:13.000000 syncany-0.2.6/syncany/filters/builtin.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      309 2022-08-13 12:36:15.000000 syncany-0.2.6/syncany/filters/filter.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1957 2023-02-16 02:10:09.000000 syncany-0.2.6/syncany/hook.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-25 09:43:40.738422 syncany-0.2.6/syncany/loaders/
--rwxrwxrwx   0 snower    (1000) snower    (1000)      927 2023-03-25 04:34:57.000000 syncany-0.2.6/syncany/loaders/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1401 2023-02-10 08:39:32.000000 syncany-0.2.6/syncany/loaders/cache.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1148 2023-03-21 06:16:11.000000 syncany-0.2.6/syncany/loaders/const.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     6106 2023-03-29 08:52:57.000000 syncany-0.2.6/syncany/loaders/db.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     9117 2023-03-30 02:17:02.000000 syncany-0.2.6/syncany/loaders/db_join.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1752 2023-02-24 04:31:16.000000 syncany-0.2.6/syncany/loaders/db_pull.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     8751 2023-04-20 05:37:24.000000 syncany-0.2.6/syncany/loaders/loader.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      214 2022-08-13 12:36:15.000000 syncany-0.2.6/syncany/logger.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    13966 2023-03-24 04:36:02.000000 syncany-0.2.6/syncany/main.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-25 09:43:41.161332 syncany-0.2.6/syncany/outputers/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1161 2023-03-25 04:34:57.000000 syncany-0.2.6/syncany/outputers/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1491 2023-02-24 04:31:16.000000 syncany-0.2.6/syncany/outputers/db.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1962 2023-04-25 03:15:38.000000 syncany-0.2.6/syncany/outputers/db_delete_insert.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      932 2023-04-25 03:15:38.000000 syncany-0.2.6/syncany/outputers/db_insert.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     5697 2023-04-25 03:15:38.000000 syncany-0.2.6/syncany/outputers/db_update_delete_insert.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4210 2023-04-25 03:15:38.000000 syncany-0.2.6/syncany/outputers/db_update_insert.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2864 2023-03-22 02:35:53.000000 syncany-0.2.6/syncany/outputers/outputer.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-25 09:43:41.439635 syncany-0.2.6/syncany/taskers/
--rwxrwxrwx   0 snower    (1000) snower    (1000)       52 2022-08-13 12:36:15.000000 syncany-0.2.6/syncany/taskers/__init__.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-25 09:43:41.936438 syncany-0.2.6/syncany/taskers/config/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1794 2023-03-25 04:34:57.000000 syncany-0.2.6/syncany/taskers/config/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      405 2022-08-23 12:07:09.000000 syncany-0.2.6/syncany/taskers/config/file_reader.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      937 2022-08-23 12:07:09.000000 syncany-0.2.6/syncany/taskers/config/http_reader.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      195 2022-08-13 12:36:15.000000 syncany-0.2.6/syncany/taskers/config/json_parser.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      208 2022-08-13 12:36:15.000000 syncany-0.2.6/syncany/taskers/config/parser.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      204 2022-08-23 11:55:44.000000 syncany-0.2.6/syncany/taskers/config/reader.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     5006 2022-08-13 12:36:15.000000 syncany-0.2.6/syncany/taskers/config/yaml_parser.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1377 2023-02-24 02:44:01.000000 syncany-0.2.6/syncany/taskers/context.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-25 09:43:42.425049 syncany-0.2.6/syncany/taskers/core/
--rwxrwxrwx   0 snower    (1000) snower    (1000)    73072 2023-04-25 04:03:27.000000 syncany-0.2.6/syncany/taskers/core/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2192 2023-03-21 06:17:51.000000 syncany-0.2.6/syncany/taskers/core/loader_creater.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      256 2022-08-13 12:36:15.000000 syncany-0.2.6/syncany/taskers/core/option.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2592 2023-02-10 08:39:32.000000 syncany-0.2.6/syncany/taskers/core/outputer_creater.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4736 2022-08-13 12:36:15.000000 syncany-0.2.6/syncany/taskers/core/states.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    15689 2023-02-25 11:47:43.000000 syncany-0.2.6/syncany/taskers/core/valuer_compiler.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    40757 2023-03-24 06:10:54.000000 syncany-0.2.6/syncany/taskers/core/valuer_creater.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      760 2023-02-25 12:43:51.000000 syncany-0.2.6/syncany/taskers/iterator.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      245 2022-08-13 12:36:15.000000 syncany-0.2.6/syncany/taskers/manager.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     7122 2023-04-20 05:48:37.000000 syncany-0.2.6/syncany/taskers/tasker.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    11025 2023-04-20 03:35:47.000000 syncany-0.2.6/syncany/utils.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-25 09:43:43.748890 syncany-0.2.6/syncany/valuers/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2098 2023-03-25 04:34:57.000000 syncany-0.2.6/syncany/valuers/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4574 2023-03-29 08:52:57.000000 syncany-0.2.6/syncany/valuers/aggregate.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     3714 2023-03-29 08:52:57.000000 syncany-0.2.6/syncany/valuers/assign.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     5209 2023-03-29 08:52:57.000000 syncany-0.2.6/syncany/valuers/cache.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     3956 2023-03-29 08:52:57.000000 syncany-0.2.6/syncany/valuers/calculate.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     6445 2023-03-29 08:52:57.000000 syncany-0.2.6/syncany/valuers/call.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     5526 2023-03-29 08:52:57.000000 syncany-0.2.6/syncany/valuers/case.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4729 2023-03-29 08:52:57.000000 syncany-0.2.6/syncany/valuers/condition.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      548 2023-03-29 08:52:57.000000 syncany-0.2.6/syncany/valuers/const.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2965 2023-03-30 01:52:08.000000 syncany-0.2.6/syncany/valuers/data.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     5059 2023-03-29 08:52:57.000000 syncany-0.2.6/syncany/valuers/db_join.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2043 2023-03-29 08:52:57.000000 syncany-0.2.6/syncany/valuers/db_load.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1877 2023-03-29 08:52:57.000000 syncany-0.2.6/syncany/valuers/function.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     6018 2023-03-29 08:52:57.000000 syncany-0.2.6/syncany/valuers/generator.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     3468 2023-03-29 08:52:57.000000 syncany-0.2.6/syncany/valuers/inherit.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     3379 2023-03-29 08:52:57.000000 syncany-0.2.6/syncany/valuers/let.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    12327 2023-03-29 08:52:57.000000 syncany-0.2.6/syncany/valuers/loop.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     7510 2023-03-29 08:52:57.000000 syncany-0.2.6/syncany/valuers/make.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    10283 2023-03-29 08:52:57.000000 syncany-0.2.6/syncany/valuers/match.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1247 2023-03-29 08:52:57.000000 syncany-0.2.6/syncany/valuers/schema.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4336 2023-03-29 08:52:57.000000 syncany-0.2.6/syncany/valuers/state.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     6066 2023-03-30 01:52:08.000000 syncany-0.2.6/syncany/valuers/valuer.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-25 09:43:38.687664 syncany-0.2.6/syncany.egg-info/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     7103 2023-04-25 09:43:35.000000 syncany-0.2.6/syncany.egg-info/PKG-INFO
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2889 2023-04-25 09:43:37.000000 syncany-0.2.6/syncany.egg-info/SOURCES.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2023-04-25 09:43:35.000000 syncany-0.2.6/syncany.egg-info/dependency_links.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)       47 2023-04-25 09:43:36.000000 syncany-0.2.6/syncany.egg-info/entry_points.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2022-08-15 03:43:33.000000 syncany-0.2.6/syncany.egg-info/not-zip-safe
--rwxrwxrwx   0 snower    (1000) snower    (1000)      371 2023-04-25 09:43:36.000000 syncany-0.2.6/syncany.egg-info/requires.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)        8 2023-04-25 09:43:36.000000 syncany-0.2.6/syncany.egg-info/top_level.txt
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-28 09:59:18.148139 syncany-0.2.7/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1063 2022-08-13 12:36:15.000000 syncany-0.2.7/LICENSE
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     7103 2023-04-28 09:59:18.150139 syncany-0.2.7/PKG-INFO
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     5832 2022-08-13 12:36:15.000000 syncany-0.2.7/README.md
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       67 2023-04-28 09:59:18.161559 syncany-0.2.7/setup.cfg
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1928 2023-04-26 02:13:49.000000 syncany-0.2.7/setup.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-28 09:59:11.950712 syncany-0.2.7/syncany/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      607 2023-04-26 02:13:50.000000 syncany-0.2.7/syncany/__init__.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-28 09:59:12.689719 syncany-0.2.7/syncany/calculaters/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4962 2023-04-25 03:51:51.000000 syncany-0.2.7/syncany/calculaters/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    39895 2023-04-28 09:52:26.000000 syncany-0.2.7/syncany/calculaters/builtin.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4394 2023-03-24 09:30:00.000000 syncany-0.2.7/syncany/calculaters/calculater.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     7999 2023-03-27 08:30:23.000000 syncany-0.2.7/syncany/calculaters/convert_calculater.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4573 2023-03-23 03:10:08.000000 syncany-0.2.7/syncany/calculaters/datetime_calculater.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2731 2023-04-27 09:47:49.000000 syncany-0.2.7/syncany/calculaters/import_calculater.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     3167 2023-03-23 03:10:08.000000 syncany-0.2.7/syncany/calculaters/textline_calculater.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    13898 2023-04-27 03:28:48.000000 syncany-0.2.7/syncany/calculaters/transform_calculater.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-28 09:59:13.962514 syncany-0.2.7/syncany/database/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     5187 2023-04-25 03:51:51.000000 syncany-0.2.7/syncany/database/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     8756 2023-03-24 06:27:35.000000 syncany-0.2.7/syncany/database/beanstalk.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    15594 2023-04-25 03:41:03.000000 syncany-0.2.7/syncany/database/clickhouse.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    15749 2023-04-25 02:15:32.000000 syncany-0.2.7/syncany/database/csv.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    10484 2023-04-26 02:09:40.000000 syncany-0.2.7/syncany/database/database.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    12481 2023-02-24 09:33:28.000000 syncany-0.2.7/syncany/database/elasticsearch.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    14490 2023-04-25 02:15:32.000000 syncany-0.2.7/syncany/database/excel.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    14218 2023-02-22 05:00:17.000000 syncany-0.2.7/syncany/database/http.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    17931 2023-02-24 09:33:28.000000 syncany-0.2.7/syncany/database/influxdb.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    12051 2023-04-25 02:15:32.000000 syncany-0.2.7/syncany/database/json.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    11954 2023-04-25 02:15:32.000000 syncany-0.2.7/syncany/database/memory.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    14642 2023-04-25 03:15:38.000000 syncany-0.2.7/syncany/database/mongodb.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    14723 2023-04-25 03:35:50.000000 syncany-0.2.7/syncany/database/mysql.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    14858 2023-04-25 03:37:13.000000 syncany-0.2.7/syncany/database/postgresql.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    18023 2023-04-25 02:22:52.000000 syncany-0.2.7/syncany/database/redis.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    13949 2023-03-28 03:39:46.000000 syncany-0.2.7/syncany/database/sqlite.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    15489 2023-04-25 03:39:10.000000 syncany-0.2.7/syncany/database/sqlserver.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    17928 2023-04-23 08:27:57.000000 syncany-0.2.7/syncany/database/textline.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      685 2022-08-23 12:03:29.000000 syncany-0.2.7/syncany/errors.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-28 09:59:14.145793 syncany-0.2.7/syncany/filters/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2275 2023-04-25 03:51:51.000000 syncany-0.2.7/syncany/filters/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    19439 2023-04-01 08:20:13.000000 syncany-0.2.7/syncany/filters/builtin.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      309 2022-08-13 12:36:15.000000 syncany-0.2.7/syncany/filters/filter.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1957 2023-02-16 02:10:09.000000 syncany-0.2.7/syncany/hook.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-28 09:59:14.588097 syncany-0.2.7/syncany/loaders/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      927 2023-03-25 04:34:57.000000 syncany-0.2.7/syncany/loaders/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1403 2023-04-27 03:37:21.000000 syncany-0.2.7/syncany/loaders/cache.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1001 2023-04-27 10:25:51.000000 syncany-0.2.7/syncany/loaders/const.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     6275 2023-04-27 09:34:08.000000 syncany-0.2.7/syncany/loaders/db.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     8832 2023-04-28 01:46:51.000000 syncany-0.2.7/syncany/loaders/db_join.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1754 2023-04-27 03:37:21.000000 syncany-0.2.7/syncany/loaders/db_pull.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     8749 2023-04-27 03:37:21.000000 syncany-0.2.7/syncany/loaders/loader.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      214 2022-08-13 12:36:15.000000 syncany-0.2.7/syncany/logger.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    13966 2023-03-24 04:36:02.000000 syncany-0.2.7/syncany/main.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-28 09:59:15.149055 syncany-0.2.7/syncany/outputers/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1161 2023-03-25 04:34:57.000000 syncany-0.2.7/syncany/outputers/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1491 2023-02-24 04:31:16.000000 syncany-0.2.7/syncany/outputers/db.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1962 2023-04-25 03:15:38.000000 syncany-0.2.7/syncany/outputers/db_delete_insert.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      932 2023-04-25 03:15:38.000000 syncany-0.2.7/syncany/outputers/db_insert.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     5697 2023-04-25 03:15:38.000000 syncany-0.2.7/syncany/outputers/db_update_delete_insert.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4210 2023-04-25 03:15:38.000000 syncany-0.2.7/syncany/outputers/db_update_insert.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2864 2023-03-22 02:35:53.000000 syncany-0.2.7/syncany/outputers/outputer.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-28 09:59:15.450759 syncany-0.2.7/syncany/taskers/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       52 2022-08-13 12:36:15.000000 syncany-0.2.7/syncany/taskers/__init__.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-28 09:59:16.005719 syncany-0.2.7/syncany/taskers/config/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1794 2023-03-25 04:34:57.000000 syncany-0.2.7/syncany/taskers/config/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      405 2022-08-23 12:07:09.000000 syncany-0.2.7/syncany/taskers/config/file_reader.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      937 2022-08-23 12:07:09.000000 syncany-0.2.7/syncany/taskers/config/http_reader.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      195 2022-08-13 12:36:15.000000 syncany-0.2.7/syncany/taskers/config/json_parser.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      208 2022-08-13 12:36:15.000000 syncany-0.2.7/syncany/taskers/config/parser.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      204 2022-08-23 11:55:44.000000 syncany-0.2.7/syncany/taskers/config/reader.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     5006 2022-08-13 12:36:15.000000 syncany-0.2.7/syncany/taskers/config/yaml_parser.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1377 2023-02-24 02:44:01.000000 syncany-0.2.7/syncany/taskers/context.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-28 09:59:16.571060 syncany-0.2.7/syncany/taskers/core/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    73215 2023-04-27 03:12:59.000000 syncany-0.2.7/syncany/taskers/core/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2192 2023-03-21 06:17:51.000000 syncany-0.2.7/syncany/taskers/core/loader_creater.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      256 2022-08-13 12:36:15.000000 syncany-0.2.7/syncany/taskers/core/option.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2592 2023-02-10 08:39:32.000000 syncany-0.2.7/syncany/taskers/core/outputer_creater.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4736 2022-08-13 12:36:15.000000 syncany-0.2.7/syncany/taskers/core/states.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    15689 2023-02-25 11:47:43.000000 syncany-0.2.7/syncany/taskers/core/valuer_compiler.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    42975 2023-04-28 01:45:52.000000 syncany-0.2.7/syncany/taskers/core/valuer_creater.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      760 2023-02-25 12:43:51.000000 syncany-0.2.7/syncany/taskers/iterator.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      245 2022-08-13 12:36:15.000000 syncany-0.2.7/syncany/taskers/manager.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     7122 2023-04-20 05:48:37.000000 syncany-0.2.7/syncany/taskers/tasker.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    11025 2023-04-20 03:35:47.000000 syncany-0.2.7/syncany/utils.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-28 09:59:18.095853 syncany-0.2.7/syncany/valuers/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2193 2023-04-27 03:26:45.000000 syncany-0.2.7/syncany/valuers/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     5565 2023-04-27 07:59:50.000000 syncany-0.2.7/syncany/valuers/aggregate.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     5094 2023-04-27 07:59:50.000000 syncany-0.2.7/syncany/valuers/assign.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     7021 2023-04-27 06:17:05.000000 syncany-0.2.7/syncany/valuers/cache.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     5314 2023-04-27 08:52:53.000000 syncany-0.2.7/syncany/valuers/calculate.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     8936 2023-04-27 06:17:04.000000 syncany-0.2.7/syncany/valuers/call.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     6980 2023-04-28 06:13:22.000000 syncany-0.2.7/syncany/valuers/case.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     6243 2023-04-28 06:13:22.000000 syncany-0.2.7/syncany/valuers/condition.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      548 2023-04-27 03:12:59.000000 syncany-0.2.7/syncany/valuers/const.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4916 2023-04-28 05:47:00.000000 syncany-0.2.7/syncany/valuers/data.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     9997 2023-04-28 03:45:24.000000 syncany-0.2.7/syncany/valuers/db_join.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     3424 2023-04-27 04:30:58.000000 syncany-0.2.7/syncany/valuers/db_load.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     3082 2023-04-27 04:30:58.000000 syncany-0.2.7/syncany/valuers/function.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     8557 2023-04-27 08:06:54.000000 syncany-0.2.7/syncany/valuers/generator.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     5960 2023-04-28 06:00:35.000000 syncany-0.2.7/syncany/valuers/inherit.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     5129 2023-04-27 06:17:05.000000 syncany-0.2.7/syncany/valuers/let.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    16860 2023-04-27 06:17:04.000000 syncany-0.2.7/syncany/valuers/loop.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     8197 2023-04-28 06:13:22.000000 syncany-0.2.7/syncany/valuers/make.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    12466 2023-04-28 06:13:22.000000 syncany-0.2.7/syncany/valuers/match.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2308 2023-04-27 06:17:04.000000 syncany-0.2.7/syncany/valuers/schema.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     5717 2023-04-27 06:17:04.000000 syncany-0.2.7/syncany/valuers/state.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     7804 2023-04-28 05:47:00.000000 syncany-0.2.7/syncany/valuers/valuer.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-04-28 09:59:12.201116 syncany-0.2.7/syncany.egg-info/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     7103 2023-04-28 09:59:09.000000 syncany-0.2.7/syncany.egg-info/PKG-INFO
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2889 2023-04-28 09:59:11.000000 syncany-0.2.7/syncany.egg-info/SOURCES.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2023-04-28 09:59:09.000000 syncany-0.2.7/syncany.egg-info/dependency_links.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       47 2023-04-28 09:59:09.000000 syncany-0.2.7/syncany.egg-info/entry_points.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2022-08-15 03:43:33.000000 syncany-0.2.7/syncany.egg-info/not-zip-safe
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      371 2023-04-28 09:59:09.000000 syncany-0.2.7/syncany.egg-info/requires.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)        8 2023-04-28 09:59:09.000000 syncany-0.2.7/syncany.egg-info/top_level.txt
```

### Comparing `syncany-0.2.6/LICENSE` & `syncany-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `syncany-0.2.6/PKG-INFO` & `syncany-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncany
-Version: 0.2.6
+Version: 0.2.7
 Summary: 简单易用的数据同步转换导出框架
 Home-page: https://github.com/snower/syncany
 Author: snower
 Author-email: sujian199@gmail.com
 License: MIT
 Description: # syncany
```

### Comparing `syncany-0.2.6/README.md` & `syncany-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `syncany-0.2.6/setup.py` & `syncany-0.2.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # 18/8/6
 # create by: snower
 
 import sys
 import os
 from setuptools import find_packages, setup
 
-version = "0.2.6"
+version = "0.2.7"
 
 if os.path.exists("README.md"):
     if sys.version_info[0] >= 3:
         try:
             with open("README.md", encoding="utf-8") as fp:
                 long_description = fp.read()
         except Exception as e:
```

### Comparing `syncany-0.2.6/syncany/__init__.py` & `syncany-0.2.7/syncany/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 # 18/8/6
 # create by: snower
 
-version = "0.2.6"
-version_info = (0, 2, 6)
+version = "0.2.7"
+version_info = (0, 2, 7)
 
 from .loaders import Loader, register_loader
 from .outputers import Outputer, register_outputer
 from .valuers import Valuer, register_valuer
 from .filters import Filter, register_filter
 from .database import DataBase, register_database
 from .calculaters import Calculater, TypeFormatCalculater, TypingCalculater, MathematicalCalculater, \
```

### Comparing `syncany-0.2.6/syncany/calculaters/__init__.py` & `syncany-0.2.7/syncany/calculaters/__init__.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.6/syncany/calculaters/builtin.py` & `syncany-0.2.7/syncany/calculaters/builtin.py`

 * *Files 6% similar despite different names*

```diff
@@ -927,15 +927,15 @@
 
 
 class SortCalculater(Calculater):
     def calculate(self, *args):
         if not args:
             return None
 
-        if not isinstance(args[0], list):
+        if not isinstance(args[0], list) or not args[0]:
             return args[0]
         if len(args) == 2 and not isinstance(args[1], bool):
             return sorted_by_keys(args[0], keys=args[1], reverse=False)
 
         keys = args[2] if len(args) >= 3 else None
         return sorted_by_keys(args[0], keys=keys,
                               reverse=True if len(args) >= 2 and args[1] else False)
@@ -961,123 +961,130 @@
                     return getattr(args[0], func_name)(*tuple(args[1:]))
                 except:
                     return ''
         return ''
 
 
 class ArrayCalculater(Calculater):
-    def to_map(self, args):
-        if len(args) == 2 and isinstance(args[0], list) and isinstance(args[1], str):
-            result = {}
-            for v in args[0]:
-                if not isinstance(v, dict) or args[1] not in v:
-                    continue
-                vk = v[args[1]]
-                if vk in result:
-                    if not isinstance(result[vk], list):
-                        result[vk] = [result[vk], v]
-                    else:
-                        result[vk].append(v)
-                else:
-                    result[vk] = v
-            return result
+    def __init__(self, *args, **kwargs):
+        super(ArrayCalculater, self).__init__(*args, **kwargs)
 
-        if len(args) == 1 and isinstance(args[0], list):
-            if len(args[0]) == 1 and isinstance(args[0][0], dict):
-                return args[0]
-            return {"index" + str(i): args[0][i] for i in range(len(args[0]))}
-
-        if isinstance(args[0], dict):
-            if len(args) == 2 and isinstance(args[1], str):
-                if args[1] in args[0]:
-                    return {args[0][args[1]]: args[0]}
-                return {}
-            return args[0]
-        return {}
+        func_name = self.name[7:]
+        if func_name == "map":
+            self.func = self.array_map
+        elif func_name == "flat":
+            self.func = self.array_flat
+        elif func_name == "contains":
+            self.func = lambda data, value: value in data
+        elif func_name == "sum":
+            self.func = lambda data: sum(data)
+        elif func_name == "max":
+            self.func = lambda data: max(data)
+        elif func_name == "min":
+            self.func = lambda data: max(data)
+        elif func_name == "avg":
+            self.func = lambda data: sum(data) / len(data)
+        elif func_name == "join":
+            self.func = lambda data, sep: str(sep).join([str(value) for value in data])
+        elif func_name == "first":
+            self.func = lambda data: data[0]
+        elif func_name == "last":
+            self.func = lambda data: data[-1]
+        elif func_name == "gt":
+            self.func = lambda data, value: [value for value in data if value is not None and value > value]
+        elif func_name == "gte":
+            self.func = lambda data, value: [value for value in data if value is not None and value >= value]
+        elif func_name == "lt":
+            self.func = lambda data, value: [value for value in data if value is not None and value < value]
+        elif func_name == "lte":
+            self.func = lambda data, value: [value for value in data if value is not None and value <= value]
+        elif func_name == "eq":
+            self.func = lambda data, value: [value for value in data if value is not None and value == value]
+        elif func_name == "neq":
+            self.func = lambda data, value: [value for value in data if value is not None and value != value]
+        elif func_name == "slice":
+            self.func = self.array_slice
+        else:
+            if hasattr([], func_name):
+                def ary_func(data, *data_args):
+                    try:
+                        if func_name in ("append", "clear", "extend", "insert", "reverse", "sort"):
+                            getattr(data, func_name)(*data_args)
+                            return data
+                        return getattr(data, func_name)(*data_args)
+                    except:
+                        return None
+                self.func = ary_func
+            else:
+                self.func = lambda data, *data_args: None
 
-    def flat(self, args):
+    def array_slice(self, data, *args):
+        if not args:
+            return data[:]
         if len(args) == 1:
-            if isinstance(args[0], list):
-                result = []
-                for d in args[0]:
-                    if isinstance(d, list):
-                        result.extend(d)
-                    else:
-                        result.append(d)
-                return result
-            return [args[0]]
+            return data[args[0]:]
+        if len(args) == 2:
+            return data[args[0]: args[1]]
+        return data[args[0]: args[1]: args[2]]
 
-        result = []
-        for d in args:
-            if isinstance(d, list):
-                result.extend(d)
+    def array_map(self, data, *args):
+        if not args:
+            if len(data) == 1 and isinstance(data[0], dict):
+                return data[0]
+            return {"index" + str(i): data[i] for i in range(len(data))}
+
+        result = {}
+        for value in data:
+            if not isinstance(value, dict) or args[0] not in value:
+                continue
+            vk = value[args[0]]
+            vv = value.get(args[1]) if len(args) >= 2 else value
+            if vk in result:
+                if not isinstance(result[vk], list):
+                    result[vk] = [result[vk], vv]
+                else:
+                    result[vk].append(vv)
             else:
-                result.append(d)
+                result[vk] = vv
+        return result
+
+    def array_flat(self, data, *args):
+        if not args:
+            result = []
+            for value in data:
+                if isinstance(value, list):
+                    result.extend(value)
+                else:
+                    result.append(value)
+            return result
+
+        result = []
+        for key in args:
+            for value in data:
+                if not isinstance(value, dict) or key not in value:
+                    continue
+                value = data[key]
+                if isinstance(value, list):
+                    result.extend(value)
+                else:
+                    result.append(value)
+            data = result
         return result
 
     def calculate(self, *args):
         if not args:
             return None
-
-        func_name = self.name[7:]
-        if func_name == "map":
-            return self.to_map(args)
-        if func_name == "flat":
-            return self.flat(args)
         data = args[0] if isinstance(args[0], list) else [args[0]]
         if not data:
+            return []
+        try:
+            return self.func(data, *args[1:])
+        except:
             return None
 
-        if func_name == "contains":
-            return args[1] in data
-        if func_name == "sum":
-            return sum(data)
-        if func_name == "max":
-            return max(*tuple(data))
-        if func_name == "min":
-            return max(*tuple(data))
-        if func_name == "avg":
-            return sum(data) / len(data)
-        if func_name == "join":
-            return str(args[1]).join([str(value) for value in data])
-        if func_name == "first":
-            return data[0]
-        if func_name == "last":
-            return data[-1]
-        if func_name == "gt":
-            return [value for value in data if value is not None and value > args[1]]
-        if func_name == "gte":
-            return [value for value in data if value is not None and value >= args[1]]
-        if func_name == "lt":
-            return [value for value in data if value is not None and value < args[1]]
-        if func_name == "lte":
-            return [value for value in data if value is not None and value <= args[1]]
-        if func_name == "eq":
-            return [value for value in data if value is not None and value == args[1]]
-        if func_name == "neq":
-            return [value for value in data if value is not None and value != args[1]]
-        if func_name == "slice":
-            if len(args) == 1:
-                return data[:]
-            if len(args) == 2:
-                return data[args[1]:]
-            if len(args) == 3:
-                return data[args[1]: args[2]]
-            return data[args[1]: args[2]: args[3]]
-
-        if hasattr(data, func_name):
-            try:
-                result = getattr(data, func_name)(*tuple(args[1:]))
-                if func_name in ("append", "clear", "extend", "insert", "reverse", "sort"):
-                    return data
-                return result
-            except:
-                return None
-        return None
-
 
 class MapCalculater(Calculater):
     def calculate(self, *args):
         if not args:
             return None
 
         func_name = self.name[5:]
```

### Comparing `syncany-0.2.6/syncany/calculaters/calculater.py` & `syncany-0.2.7/syncany/calculaters/calculater.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.6/syncany/calculaters/convert_calculater.py` & `syncany-0.2.7/syncany/calculaters/convert_calculater.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.6/syncany/calculaters/datetime_calculater.py` & `syncany-0.2.7/syncany/calculaters/datetime_calculater.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.6/syncany/calculaters/import_calculater.py` & `syncany-0.2.7/syncany/calculaters/import_calculater.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,49 +4,60 @@
 
 import types
 import traceback
 from ..logger import get_logger
 from .calculater import Calculater
 
 
+IMPORT_MODULES = {}
+
+
 class ImportCalculater(Calculater):
-    def calculate(self, *args):
+    def __init__(self, *args):
+        super(ImportCalculater, self).__init__(*args)
+
         if len(self._import_name) + 2 < len(self.name):
-            calculate_name = self.name[(len(self._import_name) + 2):]
-            attr_names = calculate_name.split(".")
-            module_or_func = self._import_module
+            self.calculate_name = self.name[(len(self._import_name) + 2):]
+            attr_names = self.calculate_name.split(".")
+            self.module_or_func = self._import_module
             for attr_name in attr_names:
-                if not hasattr(module_or_func, attr_name):
-                    raise NotImplementedError("%s not implemented %s" % (self._import_module, calculate_name))
-                module_or_func = getattr(module_or_func, attr_name)
-            if not callable(module_or_func):
-                if not args:
-                    return module_or_func
-                raise NotImplementedError("%s not callable %s" % (self._import_module, calculate_name))
+                if not hasattr(self.module_or_func, attr_name):
+                    raise NotImplementedError("%s not implemented %s" % (self._import_module, self.calculate_name))
+                self.module_or_func = getattr(self.module_or_func, attr_name)
         else:
-            calculate_name = self.name
+            self.calculate_name = self.name
             if not callable(self._import_module):
                 raise NotImplementedError("%s not callable %s" % (self._import_module, self.name))
-            module_or_func = self._import_module
+            self.module_or_func = self._import_module
 
+    def calculate(self, *args):
         try:
             if not args:
-                return module_or_func()
+                if not callable(self.module_or_func):
+                    return self.module_or_func
+                return self.module_or_func()
+
+            if not callable(self.module_or_func):
+                raise NotImplementedError("%s not callable %s" % (self._import_module, self.calculate_name))
             if len(args) == 1 and isinstance(args[0], list) and args[0] and isinstance(args[0][0], dict):
                 try:
-                    return module_or_func(*tuple(args[0]))
+                    return self.module_or_func(*tuple(args[0]))
                 except TypeError:
                     pass
-            return module_or_func(*args)
+            return self.module_or_func(*args)
         except Exception as e:
-            get_logger().warning("import calculater execute %s(%s) error: %s\n%s", calculate_name, args, e,
+            get_logger().warning("import calculater execute %s(%s) error: %s\n%s", self.calculate_name, args, e,
                                  traceback.format_exc())
             return None
 
 
 def create_import_calculater(name, module_or_func):
+    module_id = (name, id(module_or_func))
+    if module_id in IMPORT_MODULES:
+        return IMPORT_MODULES[module_id]
     class_name = "".join([n[:1].upper() + n[1:] for n in name.split("_")]) + "ImportCalculater"
     if isinstance(module_or_func, (types.FunctionType, types.BuiltinFunctionType, types.LambdaType)):
         import_module = lambda self, *args, **kwargs: module_or_func(*args, **kwargs)
     else:
         import_module = module_or_func
-    return type(class_name, (ImportCalculater,), dict(_import_name=name, _import_module=import_module))
+    IMPORT_MODULES[module_id] = type(class_name, (ImportCalculater,), dict(_import_name=name, _import_module=import_module))
+    return IMPORT_MODULES[module_id]
```

### Comparing `syncany-0.2.6/syncany/calculaters/textline_calculater.py` & `syncany-0.2.7/syncany/calculaters/textline_calculater.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.6/syncany/calculaters/transform_calculater.py` & `syncany-0.2.7/syncany/calculaters/transform_calculater.py`

 * *Files 1% similar despite different names*

```diff
@@ -344,15 +344,15 @@
         for data in result:
             for key in keys:
                 if key in data:
                     continue
                 if not valuer:
                     data[key] = 0
                     continue
-                data[key] = valuer.reinit().fill(None).get()
+                data[key] = valuer.fill(None).get()
 
         for key in keys:
             if key in tasker.outputer.schema:
                 continue
             valuer = tasker.create_valuer(tasker.valuer_compiler.compile_data_valuer(key, None))
             if not valuer:
                 continue
```

### Comparing `syncany-0.2.6/syncany/database/__init__.py` & `syncany-0.2.7/syncany/database/__init__.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.6/syncany/database/beanstalk.py` & `syncany-0.2.7/syncany/database/beanstalk.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.6/syncany/database/clickhouse.py` & `syncany-0.2.7/syncany/database/clickhouse.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.6/syncany/database/csv.py` & `syncany-0.2.7/syncany/database/csv.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.6/syncany/database/database.py` & `syncany-0.2.7/syncany/database/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # -*- coding: utf-8 -*-
 # 18/8/6
 # create by: snower
 
 import time
-import hashlib
 from collections import deque
 import threading
 
 
 class QueryBuilder(object):
     def __init__(self, db, name, primary_keys, fields):
         self.db = db
@@ -167,19 +166,15 @@
         self.config = config
         self.config_key = None
         self.database_driver = None
 
     def get_config_key(self):
         if self.config_key is not None:
             return self.config_key
-
-        cs = []
-        for key in sorted(self.config.keys()):
-            cs.append("%s=%s" % (key, self.config[key]))
-        self.config_key = hashlib.md5("&".join(cs).encode("utf-8")).hexdigest()
+        self.config_key = "%s::%s" % (self.__class__.__name__, self.name)
         return self.config_key
 
     def build_factory(self):
         raise NotImplementedError()
 
     def acquire_driver(self):
         if self.database_driver:
```

### Comparing `syncany-0.2.6/syncany/database/elasticsearch.py` & `syncany-0.2.7/syncany/database/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.6/syncany/database/excel.py` & `syncany-0.2.7/syncany/database/excel.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.6/syncany/database/http.py` & `syncany-0.2.7/syncany/database/http.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.6/syncany/database/influxdb.py` & `syncany-0.2.7/syncany/database/influxdb.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.6/syncany/database/json.py` & `syncany-0.2.7/syncany/database/json.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.6/syncany/database/memory.py` & `syncany-0.2.7/syncany/database/memory.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.6/syncany/database/mongodb.py` & `syncany-0.2.7/syncany/database/mongodb.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.6/syncany/database/mysql.py` & `syncany-0.2.7/syncany/database/mysql.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.6/syncany/database/postgresql.py` & `syncany-0.2.7/syncany/database/postgresql.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.6/syncany/database/redis.py` & `syncany-0.2.7/syncany/database/redis.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.6/syncany/database/sqlite.py` & `syncany-0.2.7/syncany/database/sqlite.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.6/syncany/database/sqlserver.py` & `syncany-0.2.7/syncany/database/sqlserver.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.6/syncany/database/textline.py` & `syncany-0.2.7/syncany/database/textline.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.6/syncany/errors.py` & `syncany-0.2.7/syncany/errors.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.6/syncany/filters/__init__.py` & `syncany-0.2.7/syncany/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.6/syncany/filters/builtin.py` & `syncany-0.2.7/syncany/filters/builtin.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.6/syncany/hook.py` & `syncany-0.2.7/syncany/hook.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.6/syncany/loaders/__init__.py` & `syncany-0.2.7/syncany/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.6/syncany/loaders/cache.py` & `syncany-0.2.7/syncany/loaders/cache.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*-
 # 2021/11/8
 # create by: snower
 
 from ..database import DatabaseInstanceBuilder
 
+
 class CacheLoader(object):
     def __init__(self, name, db, config):
         self.name = name
         self.db = db
         self.prefix_key = "syncany"
         self.exprie_seconds = 86400
         self.config = config
```

### Comparing `syncany-0.2.6/syncany/loaders/const.py` & `syncany-0.2.7/syncany/loaders/const.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # -*- coding: utf-8 -*-
 # 18/8/6
 # create by: snower
 
 from .loader import Loader
 
+
 class ConstLoader(Loader):
     def __init__(self, datas, *args, **kwargs):
         super(ConstLoader, self).__init__(*args, **kwargs)
 
         self.const_datas = datas
-        self.last_data = datas[-1]
+        self.last_data = datas[-1] if datas else None
 
     def clone(self):
         loader = self.__class__(self.const_datas, self.primary_keys, self.valuer_type)
         schema = {}
         for key, valuer in self.schema.items():
             schema[key] = valuer.clone()
         loader.schema = schema
@@ -22,15 +23,9 @@
         loader.intercepts = [intercept.clone() for intercept in self.intercepts]
         loader.key_matchers = [matcher.clone() for matcher in self.key_matchers]
         return loader
 
     def load(self, timeout=None):
         if self.loaded:
             return
-
-        for data in self.const_datas:
-            values = {}
-            for key, field in self.schema.items():
-                values[key] = field.clone().fill(data)
-            self.datas.append(values)
-
+        self.datas = self.const_datas[:]
         self.loaded = True
```

### Comparing `syncany-0.2.6/syncany/loaders/db.py` & `syncany-0.2.7/syncany/loaders/db.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
 # 18/8/6
 # create by: snower
 
-import types
 import copy
 from collections import defaultdict, deque
 from .loader import Loader
-from ..valuers.valuer import LoadAllFieldsException
+from ..valuers.valuer import Contexter, ContextRunner, LoadAllFieldsException
+
 
 class DBLoader(Loader):
     def __init__(self, db, name, *args, **kwargs):
         super(DBLoader, self).__init__(*args, **kwargs)
 
         self.db = db
         self.name = name
@@ -109,53 +109,57 @@
         if self.geted:
             return self.datas
         if not self.loaded:
             self.load()
 
         if not self.compiled:
             if not self.key_matchers:
-                require_loaded_schema_items = [(key, field) for key, field in self.schema.items() if field.require_loaded()]
+                require_loaded_schema_items = [(key, field, field.contexter if hasattr(field, "contexter") else None)
+                                               for key, field in self.schema.items() if field.require_loaded()]
                 if not require_loaded_schema_items:
                     if not self.valuer_type:
                         return self.fast_get()
                     return super(DBLoader, self).get()
                 for i in range(len(self.datas)):
-                    values = {key: value for key, value in self.datas[i].items()}
-                    for key, field in require_loaded_schema_items:
-                        values[key] = field.clone().fill(self.datas[i])
-                    self.datas[i] = values
+                    data, contexter_values = copy.copy(self.datas[i]), {}
+                    for key, field, contexter in require_loaded_schema_items:
+                        if contexter is None:
+                            contexter = Contexter()
+                            field = field.clone(contexter)
+                        data[key] = ContextRunner(contexter, field, contexter_values).fill(data)
+                    self.datas[i] = data
             else:
                 for i in range(len(self.datas)):
-                    values = {}
+                    data = {}
                     for key, value in self.datas[i].items():
                         if key in self.schema:
-                            values[key] = self.schema[key].clone().fill(self.datas[i])
-                        else:
-                            for key_matcher in self.key_matchers:
-                                if key_matcher.match(key):
-                                    valuer = key_matcher.create_key(key)
-                                    self.schema[key] = valuer
-                                    values[key] = valuer.clone().fill(self.datas[i])
-                    self.datas[i] = values
+                            data[key] = value
+                            continue
+                        for key_matcher in self.key_matchers:
+                            if not key_matcher.match(key):
+                                continue
+                            self.schema[key] = key_matcher.create_key(key)
+                            data[key] = value
+                            break
+                    self.datas[i] = data
+
         return super(DBLoader, self).get()
 
     def fast_get(self):
         if not self.intercepts:
             for i in range(len(self.datas)):
                 data = self.datas[i]
-                self.datas[i] = {name: valuer.reinit().fill(data).get()
-                                 for name, valuer in self.schema.items()}
+                self.datas[i] = {name: valuer.fill(data).get() for name, valuer in self.schema.items()}
             self.geted = True
             return self.datas
 
         datas, self.datas = deque(self.datas), []
         while datas:
             data = datas.popleft()
-            odata = {name: valuer.reinit().fill(data).get()
-                     for name, valuer in self.schema.items()}
+            odata = {name: valuer.fill(data).get() for name, valuer in self.schema.items()}
             if self.check_intercepts(odata):
                 continue
             self.datas.append(odata)
         self.geted = True
         return self.datas
 
     def statistics(self):
```

### Comparing `syncany-0.2.6/syncany/loaders/db_join.py` & `syncany-0.2.7/syncany/valuers/db_join.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,251 +1,235 @@
 # -*- coding: utf-8 -*-
 # 18/8/6
 # create by: snower
 
-from collections import defaultdict
-from .db import DBLoader
-from ..valuers.valuer import LoadAllFieldsException
-
-class DBJoinMatcher(object):
-    def __init__(self, keys, values):
-        self.keys = keys
-        self.values = values
-        self.data = None
-        self.valuers = []
-
-    def clone(self):
-        matcher = self.__class__(self.keys, self.values)
-        return matcher
-
-    def fill(self, values):
-        self.data = values
-        for valuer in self.valuers:
-            valuer.fill(self.data)
+from .data import Valuer
 
-    def add_valuer(self, valuer):
-        self.valuers.append(valuer)
 
-    def get(self):
-        return self.data
-
-class GroupDBJoinMatcher(object):
-    def __init__(self, return_valuer):
+class DBJoinValuer(Valuer):
+    def __init__(self, loader, foreign_keys, foreign_filters, args_valuers, return_valuer, inherit_valuers, *args, **kwargs):
+        self.loader = loader
+        self.foreign_keys = foreign_keys
+        self.args_valuers = args_valuers
         self.return_valuer = return_valuer
-        self.valuers = []
-        self.datas = None
-
-    def add_valuer(self, valuer):
-        self.valuers.append(valuer)
+        self.inherit_valuers = inherit_valuers
+        self.foreign_filters = foreign_filters
+        super(DBJoinValuer, self).__init__(*args, **kwargs)
+
+    def add_inherit_valuer(self, valuer):
+        self.inherit_valuers.append(valuer)
+
+    def clone(self, contexter=None):
+        args_valuers = [args_valuer.clone(contexter) for args_valuer in self.args_valuers] if self.args_valuers else None
+        return_valuer = self.return_valuer.clone(contexter)
+        inherit_valuers = [inherit_valuer.clone(contexter) for inherit_valuer in self.inherit_valuers] \
+            if self.inherit_valuers else None
+        if contexter is not None:
+            return ContextDBJoinValuer(self.loader, self.foreign_keys, self.foreign_filters,
+                                       args_valuers, return_valuer, inherit_valuers, self.key, self.filter,
+                                       from_valuer=self, contexter=contexter)
+        if isinstance(self, ContextDBJoinValuer):
+            return ContextDBJoinValuer(self.loader, self.foreign_keys, self.foreign_filters,
+                                       args_valuers, return_valuer, inherit_valuers, self.key, self.filter,
+                                       from_valuer=self, contexter=self.contexter)
+        return self.__class__(self.loader, self.foreign_keys, self.foreign_filters,
+                              args_valuers, return_valuer, inherit_valuers, self.key, self.filter, from_valuer=self)
+
+    def fill(self, data):
+        if self.inherit_valuers:
+            for inherit_valuer in self.inherit_valuers:
+                inherit_valuer.fill(data)
+
+        join_values, max_value_size, has_join_value = [], 0, False
+        if self.args_valuers:
+            for args_valuer in self.args_valuers:
+                join_value = args_valuer.fill(data).get()
+                if isinstance(join_value, list):
+                    if len(join_value) > max_value_size:
+                        max_value_size = len(join_value)
+                    has_join_value = True
+                else:
+                    max_value_size, has_join_value = max_value_size or 1, join_value is not None
+                join_values.append(join_value)
+        else:
+            if self.key:
+                super(DBJoinValuer, self).fill(data)
+            join_value = self.value
+            for _ in self.foreign_keys:
+                if isinstance(join_value, list):
+                    if len(join_value) > max_value_size:
+                        max_value_size = len(join_value)
+                    has_join_value = True
+                else:
+                    max_value_size, has_join_value = max_value_size or 1, join_value is not None
+                join_values.append(join_value)
 
-    def fill(self, valuer, data):
-        if self.datas is not None:
-            return self
-        for valuer in self.valuers:
-            if valuer.loaded is False:
-                return self
-
-        self.datas = []
-        for valuer in self.valuers:
-            if valuer.loaded is not True:
-                continue
-            value = valuer.get()
-            if isinstance(value, list):
-                self.datas.extend(value)
-            else:
-                self.datas.append(value)
-        self.return_valuer.fill(self.datas)
+        if max_value_size > 1:
+            group_macther = self.loader.create_group_macther(self.return_valuer)
+            for i in range(max_value_size):
+                ds, has_value = [], False
+                for join_value in join_values:
+                    if not isinstance(join_value, list):
+                        ds.append(join_value)
+                        has_value = True if join_value is not None else has_value
+                    else:
+                        ds.append(join_value[i] if i < len(join_value) else None)
+                        has_value = True if i < len(join_value) else has_value
+                if not has_value:
+                    continue
+                matcher = self.loader.create_macther(self.foreign_keys, ds)
+                return_valuer = DBJoinGroupMatchValuer(group_macther, "*")
+                matcher.add_valuer(return_valuer)
+                group_macther.add_valuer(return_valuer)
+        elif has_join_value:
+            matcher = self.loader.create_macther(self.foreign_keys, join_values)
+            matcher.valuer, matcher.contexter_values = self.return_valuer, None
+
+        self.loader.wait_try_load_count += 1
+        if self.loader.wait_try_load_count >= 64:
+            self.loader.try_load()
+            self.loader.wait_try_load_count = 0
+        return self
 
     def get(self):
-        if self.datas is not None:
-            return self.datas
+        self.loader.load()
+        return self.return_valuer.get()
 
-        self.datas = []
-        for valuer in self.valuers:
-            if valuer.loaded is not True:
-                continue
-            value = valuer.get()
-            if isinstance(value, list):
-                self.datas.extend(value)
-            else:
-                self.datas.append(value)
-        self.return_valuer.fill(self.datas)
-        return self.datas
-
-class DBJoinLoader(DBLoader):
-    def __init__(self, *args, **kwargs):
-        self.join_batch = kwargs.pop("join_batch", 10000) or 0xffffffff
-        super(DBJoinLoader, self).__init__(*args, **kwargs)
-
-        self.data_keys = {}
-        self.unload_primary_keys = set([])
-        self.load_primary_keys = set([])
-        self.matchers = defaultdict(list)
-
-    def clone(self):
-        loader = super(DBJoinLoader, self).clone()
-        loader.join_batch = self.join_batch
-        if len(self.data_keys) < self.join_batch:
-            loader.data_keys = self.data_keys
-        return loader
-
-    def next(self):
-        if not self.loaded:
-            return True
-        return False
-
-    def is_dynamic_schema(self):
-        return False
-
-    def is_streaming(self):
+    def childs(self):
+        valuers = []
+        if self.args_valuers:
+            for args_valuer in self.args_valuers:
+                valuers.append(args_valuer)
+        if self.return_valuer:
+            valuers.append(self.return_valuer)
+        if self.inherit_valuers:
+            for inherit_valuer in self.inherit_valuers:
+                valuers.append(inherit_valuer)
+        return valuers
+
+    def get_fields(self):
+        fields = []
+
+        if self.args_valuers:
+            for args_valuer in self.args_valuers:
+                for field in args_valuer.get_fields():
+                    fields.append(field)
+
+        if self.inherit_valuers:
+            for inherit_valuer in self.inherit_valuers:
+                for field in inherit_valuer.get_fields():
+                    fields.append(field)
+        return fields
+
+    def get_final_filter(self):
+        if self.return_valuer:
+            return self.return_valuer.get_final_filter()
         return None
 
-    def set_streaming(self, is_streaming=None):
-        pass
-
-    def create_group_macther(self, return_valuer):
-        return GroupDBJoinMatcher(return_valuer)
-
-    def create_macther(self, keys, values):
-        matcher = DBJoinMatcher(keys, values)
-        if len(self.primary_keys) == 1:
-            self.matchers[values[0]].append(matcher)
-            if values[0] not in self.data_keys:
-                self.unload_primary_keys.add(values[0])
-            else:
-                self.load_primary_keys.add(values[0])
-        else:
-            data_key = tuple(values)
-            self.matchers[data_key].append(matcher)
-            if data_key not in self.data_keys:
-                self.unload_primary_keys.add(data_key)
-            else:
-                self.load_primary_keys.add(data_key)
+    def require_loaded(self):
+        return True
 
-        self.loaded = False
-        return matcher
 
-    def load_join(self):
-        if self.loaded:
+class ContextDBJoinValuer(DBJoinValuer):
+    def __init__(self, *args, **kwargs):
+        self.contexter = kwargs.pop("contexter")
+        self.value_context_id = (id(self), "value")
+        super(ContextDBJoinValuer, self).__init__(*args, **kwargs)
+
+    @property
+    def value(self):
+        try:
+            return self.contexter.values[self.value_context_id]
+        except KeyError:
+            return None
+
+    @value.setter
+    def value(self, v):
+        if v is None:
+            if self.value_context_id in self.contexter.values:
+                self.contexter.values.pop(self.value_context_id)
             return
+        self.contexter.values[self.value_context_id] = v
 
-        if self.unload_primary_keys:
-            fields = set([])
-            if not self.key_matchers:
-                for key, exp, value in self.filters:
-                    if not key:
-                        continue
-                    fields.add(key)
-                try:
-                    for name, valuer in self.schema.items():
-                        for field in valuer.get_fields():
-                            fields.add(field)
-                except LoadAllFieldsException:
-                    fields = []
-
-            query = self.db.query(self.name, self.primary_keys, list(fields))
-            for key, exp, value in self.filters:
-                if key is None:
-                    getattr(query, "filter_%s" % exp)(value)
+    def fill(self, data):
+        if self.inherit_valuers:
+            for inherit_valuer in self.inherit_valuers:
+                inherit_valuer.fill(data)
+
+        join_values, max_value_size, has_join_value = [], 0, False
+        if self.args_valuers:
+            for args_valuer in self.args_valuers:
+                join_value = args_valuer.fill(data).get()
+                if isinstance(join_value, list):
+                    if len(join_value) > max_value_size:
+                        max_value_size = len(join_value)
+                    has_join_value = True
                 else:
-                    getattr(query, "filter_%s" % exp)(key, value)
-
-            if len(self.primary_keys) == 1:
-                query.filter_in(self.primary_keys[0], list(self.unload_primary_keys))
-            else:
-                for j in range(len(self.primary_keys)):
-                    query.filter_in(self.primary_keys[j], list({primary_value[j] for primary_value
-                                                                in self.unload_primary_keys}))
-            datas, query = query.commit(), None
-
-            if not self.key_matchers:
-                for i in range(len(datas)):
-                    data = datas[i]
-                    primary_key = self.get_data_primary_key(data)
-                    values = {key: field.reinit().fill(data).get() for key, field in self.schema.items()}
-
-                    if primary_key not in self.data_keys:
-                        self.data_keys[primary_key] = [values]
-                    elif primary_key in self.unload_primary_keys:
-                        self.data_keys[primary_key].append(values)
-                    datas[i] = values
-            else:
-                for i in range(len(datas)):
-                    data, values = datas[i], {}
-                    primary_key = self.get_data_primary_key(data)
-                    for key, value in data.items():
-                        if key in self.schema:
-                            values[key] = self.schema[key].reinit().fill(data).get()
-                        else:
-                            for key_matcher in self.key_matchers:
-                                if key_matcher.match(key):
-                                    valuer = key_matcher.create_key(key)
-                                    self.schema[key] = valuer
-                                    values[key] = valuer.reinit().fill(data).get()
-
-                    if primary_key not in self.data_keys:
-                        self.data_keys[primary_key] = [values]
-                    elif primary_key in self.unload_primary_keys:
-                        self.data_keys[primary_key].append(values)
-                    datas[i] = values
-
-            self.datas = datas
-            self.loader_state["query_count"] += 1
-            self.loader_state["load_count"] += len(datas)
-
-        if self.matchers:
-            for primary_key in self.load_primary_keys:
-                if primary_key not in self.matchers:
-                    continue
-                values = self.data_keys.get(primary_key, None)
-                if values and len(values) == 1:
-                    for matcher in self.matchers[primary_key]:
-                        matcher.fill(values[0])
+                    max_value_size, has_join_value = max_value_size or 1, join_value is not None
+                join_values.append(join_value)
+        else:
+            if self.key:
+                super(DBJoinValuer, self).fill(data)
+            join_value = self.value
+            for _ in self.foreign_keys:
+                if isinstance(join_value, list):
+                    if len(join_value) > max_value_size:
+                        max_value_size = len(join_value)
+                    has_join_value = True
                 else:
-                    for matcher in self.matchers[primary_key]:
-                        matcher.fill(values)
-                self.matchers.pop(primary_key)
+                    max_value_size, has_join_value = max_value_size or 1, join_value is not None
+                join_values.append(join_value)
 
-            for primary_key in self.unload_primary_keys:
-                if primary_key not in self.matchers:
+        if max_value_size > 1:
+            group_macther = self.loader.create_group_macther(self.return_valuer)
+            for i in range(max_value_size):
+                ds, has_value = [], False
+                for join_value in join_values:
+                    if not isinstance(join_value, list):
+                        ds.append(join_value)
+                        has_value = True if join_value is not None else has_value
+                    else:
+                        ds.append(join_value[i] if i < len(join_value) else None)
+                        has_value = True if i < len(join_value) else has_value
+                if not has_value:
                     continue
-                values = self.data_keys.get(primary_key, None)
-                if values and len(values) == 1:
-                    for matcher in self.matchers[primary_key]:
-                        matcher.fill(values[0])
-                else:
-                    for matcher in self.matchers[primary_key]:
-                        matcher.fill(values)
-                self.matchers.pop(primary_key)
-
-        self.unload_primary_keys = set([])
-        self.load_primary_keys = set([])
-        self.loaded = True
+                matcher = self.loader.create_macther(self.foreign_keys, ds)
+                return_valuer = DBJoinGroupMatchValuer(group_macther, "*")
+                matcher.add_valuer(return_valuer)
+                group_macther.add_valuer(return_valuer)
+        elif has_join_value:
+            matcher = self.loader.create_macther(self.foreign_keys, join_values)
+            matcher.valuer, matcher.contexter_values = self.return_valuer, self.contexter.values
+
+        self.loader.wait_try_load_count += 1
+        if self.loader.wait_try_load_count >= 64:
+            contexter_values = self.contexter.values
+            try:
+                self.loader.try_load()
+            finally:
+                self.contexter.values = contexter_values
+            self.loader.wait_try_load_count = 0
+        return self
 
-    def try_load(self):
-        if self.loaded:
-            return
-        if len(self.unload_primary_keys) >= self.join_batch:
-            return self.load_join()
-        if not self.load_primary_keys:
-            return
+    def get(self):
+        contexter_values = self.contexter.values
+        try:
+            self.loader.load()
+        finally:
+            self.contexter.values = contexter_values
+        return self.return_valuer.get()
+
+
+class DBJoinGroupMatchValuer(Valuer):
+    def __init__(self, matcher, *args, **kwargs):
+        self.matcher = matcher
+        self.loaded = False
+        super(DBJoinGroupMatchValuer, self).__init__(*args, **kwargs)
+
+    def clone(self, contexter=None):
+        return self.__class__(self.matcher, self.key, self.filter)
 
-        for primary_key in self.load_primary_keys:
-            if primary_key not in self.matchers:
-                continue
-            values = self.data_keys.get(primary_key, None)
-            if values and len(values) == 1:
-                for matcher in self.matchers[primary_key]:
-                    matcher.fill(values[0])
-            else:
-                for matcher in self.matchers[primary_key]:
-                    matcher.fill(values)
-            self.matchers.pop(primary_key)
-
-        self.load_primary_keys.clear()
-        if not self.unload_primary_keys:
-            self.loaded = True
-
-    def load(self, timeout=None):
-        self.load_join()
-        if len(self.data_keys) >= self.join_batch:
-            self.datas, self.data_keys = [], {}
+    def fill(self, data):
+        super(DBJoinGroupMatchValuer, self).fill(data)
+        self.loaded = None if data is None else True
+        self.matcher.fill(self, data)
+        return self
```

### Comparing `syncany-0.2.6/syncany/loaders/db_pull.py` & `syncany-0.2.7/syncany/loaders/db_pull.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # 2021/3/3
 # create by: snower
 
 import time
 import threading
 from .db import DBLoader
 
+
 class DBPullLoader(DBLoader):
     def __init__(self, *args, **kwargs):
         super(DBPullLoader, self).__init__(*args, **kwargs)
 
         self.last_load_time = 0
         self.start_loaded = False
         self.wait_event = None
```

### Comparing `syncany-0.2.6/syncany/loaders/loader.py` & `syncany-0.2.7/syncany/loaders/loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # -*- coding: utf-8 -*-
 # 18/8/6
 # create by: snower
 
 import types
 import re
 from collections import defaultdict, deque
-from ..valuers import Valuer
+from ..valuers import ContextRunner
+
 
 class KeyMatcher(object):
     def __init__(self, matcher, valuer):
         if isinstance(matcher, str):
             self.matcher = re.compile(matcher)
         else:
             self.matcher = matcher
@@ -33,14 +34,15 @@
         for key_event in self.key_events:
             key_event(key, valuer)
         return valuer
 
     def add_key_event(self, event):
         self.key_events.append(event)
 
+
 class Loader(object):
     def __init__(self, primary_keys, valuer_type=0, **kwargs):
         self.primary_keys = primary_keys
         self.valuer_type = valuer_type
         self.schema = {}
         self.filters = []
         self.orders = []
@@ -104,29 +106,29 @@
             self.load()
 
         datas, self.datas = deque(self.datas), []
         if not self.valuer_type:
             while datas:
                 data, odata = datas.popleft(), {}
                 for name, valuer in self.schema.items():
-                    if name not in data or not isinstance(data[name], Valuer):
-                        odata[name] = valuer.reinit().fill(data).get()
+                    if name not in data or not isinstance(data[name], ContextRunner):
+                        odata[name] = valuer.fill(data).get()
                     else:
                         odata[name] = data[name].get()
                 if self.intercepts and self.check_intercepts(odata):
                     continue
                 self.datas.append(odata)
             self.geted = True
             return self.datas
 
         while datas:
             data, odata, oyields, ofuncs = datas.popleft(), {}, {}, {}
             for name, valuer in self.schema.items():
-                if name not in data or not isinstance(data[name], Valuer):
-                    value = valuer.reinit().fill(data).get()
+                if name not in data or not isinstance(data[name], ContextRunner):
+                    value = valuer.fill(data).get()
                 else:
                     value = data[name].get()
                 if isinstance(value, types.FunctionType):
                     ofuncs[name] = value
                     odata[name] = None
                     continue
                 if isinstance(value, types.GeneratorType):
@@ -180,15 +182,15 @@
                     self.datas.append(odata)
         self.geted = True
         return self.datas
 
     def check_intercepts(self, data):
         intercept_stoped = False
         for intercept in self.intercepts:
-            intercept_result = intercept.reinit().fill(data).get()
+            intercept_result = intercept.fill(data).get()
             if intercept_result is not None and not intercept_result:
                 intercept_stoped = True
                 break
         return intercept_stoped
 
     def add_filter(self, key, exp, value):
         self.filters.append([key, exp, value])
```

### Comparing `syncany-0.2.6/syncany/main.py` & `syncany-0.2.7/syncany/main.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.6/syncany/outputers/__init__.py` & `syncany-0.2.7/syncany/outputers/__init__.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.6/syncany/outputers/db.py` & `syncany-0.2.7/syncany/outputers/db.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.6/syncany/outputers/db_delete_insert.py` & `syncany-0.2.7/syncany/outputers/db_delete_insert.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.6/syncany/outputers/db_insert.py` & `syncany-0.2.7/syncany/outputers/db_insert.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.6/syncany/outputers/db_update_delete_insert.py` & `syncany-0.2.7/syncany/outputers/db_update_delete_insert.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.6/syncany/outputers/db_update_insert.py` & `syncany-0.2.7/syncany/outputers/db_update_insert.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.6/syncany/outputers/outputer.py` & `syncany-0.2.7/syncany/outputers/outputer.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.6/syncany/taskers/config/__init__.py` & `syncany-0.2.7/syncany/taskers/config/__init__.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.6/syncany/taskers/config/http_reader.py` & `syncany-0.2.7/syncany/taskers/config/http_reader.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.6/syncany/taskers/config/yaml_parser.py` & `syncany-0.2.7/syncany/taskers/config/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.6/syncany/taskers/context.py` & `syncany-0.2.7/syncany/taskers/context.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.6/syncany/taskers/core/__init__.py` & `syncany-0.2.7/syncany/taskers/core/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from ...logger import get_logger
 from ..tasker import Tasker
 from ..config import load_config
 from .states import States
 from .option import DataValuerOutputerOption
 from ...calculaters.import_calculater import create_import_calculater
 from ...utils import get_expression_name, gen_runner_id
+from ...valuers import Contexter
 from .valuer_compiler import ValuerCompiler
 from .valuer_creater import ValuerCreater
 from .loader_creater import LoaderCreater
 from .outputer_creater import OutputerCreater
 from ...loaders.cache import CacheLoader
 from ...hook import PipelinesHooker
 from ...errors import LoaderUnknownException, OutputerUnknownException, \
@@ -777,14 +778,16 @@
             for name, valuer in self.schema.items():
                 inherit_valuers, yield_valuers = [], []
                 valuer = self.create_valuer(valuer, schema_field_name=name, inherit_valuers=inherit_valuers,
                                             join_loaders=self.join_loaders, yield_valuers=yield_valuers,
                                             aggregate_valuers=aggregate_valuers, define_valuers={},
                                             global_variables=self.global_variables, global_states=self.states)
                 if valuer:
+                    if valuer.require_loaded():
+                        valuer = valuer.clone(Contexter())
                     self.loader.add_valuer(name, valuer)
                 if inherit_valuers:
                     raise OverflowError(name + " inherit out of range")
                 if yield_valuers:
                     loader_config["valuer_type"] |= 0x01
                 if aggregate_valuers:
                     loader_config["valuer_type"] |= 0x02
```

### Comparing `syncany-0.2.6/syncany/taskers/core/loader_creater.py` & `syncany-0.2.7/syncany/taskers/core/loader_creater.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.6/syncany/taskers/core/outputer_creater.py` & `syncany-0.2.7/syncany/taskers/core/outputer_creater.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.6/syncany/taskers/core/states.py` & `syncany-0.2.7/syncany/taskers/core/states.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.6/syncany/taskers/core/valuer_compiler.py` & `syncany-0.2.7/syncany/taskers/core/valuer_compiler.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.6/syncany/taskers/core/valuer_creater.py` & `syncany-0.2.7/syncany/taskers/core/valuer_creater.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,770 +1,797 @@
-# -*- coding: utf-8 -*-
-# 18/8/15
-# create by: snower
-
-from ...valuers.valuer import LoadAllFieldsException
-from ...errors import CacheUnknownException, ValuerUnknownException
-
-
-class LoaderJoinWarp(object):
-    __loader = None
-
-    def __init__(self, loader):
-        self.__loader = loader
-
-    def __getattr__(self, item):
-        if self.__loader is None or item == "_LoaderJoinWarp__loader":
-            return super(LoaderJoinWarp, self).__getattr__(item)
-        return getattr(self.__loader, item)
-
-    def __setattr__(self, key, value):
-        if self.__loader is None or key == "_LoaderJoinWarp__loader":
-            return super(LoaderJoinWarp, self).__setattr__(key, value)
-        return setattr(self.__loader, key, value)
-
-    def __str__(self):
-        return str(self.__loader)
-
-    def __repr__(self):
-        return repr(self.__loader)
-
-    def clone(self):
-        self.__loader = self.__loader.clone()
-        return self
-
-    def add_valuer(self, name, valuer):
-        return self.__loader.add_valuer(name, valuer)
-
-    def add_intercept(self, intercept):
-        return self.__loader.add_intercept(intercept)
-
-    def add_key_matcher(self, matcher, valuer):
-        return self.__loader.add_key_matcher(matcher, valuer)
-
-    def get_data_primary_key(self, data):
-        return self.__loader.get_data_primary_key(data)
-
-    def next(self):
-        return self.__loader.next()
-
-    def is_dynamic_schema(self):
-        return self.__loader.is_dynamic_schema()
-
-    def is_streaming(self):
-        return self.__loader.is_streaming()
-
-    def set_streaming(self, is_streaming=None):
-        return self.__loader.set_streaming(is_streaming)
-
-    def create_group_macther(self, return_valuer):
-        return self.__loader.create_group_macther(return_valuer)
-
-    def create_macther(self, keys, values):
-        return self.__loader.create_macther(keys, values)
-
-    def try_load(self):
-        return self.__loader.try_load()
-
-    def load(self, timeout=None):
-        return self.__loader.load(timeout)
-
-    def statistics(self):
-        return self.__loader.statistics()
-
-class ValuerCreater(object):
-    def __init__(self, tasker):
-        self.tasker = tasker
-
-    def find_valuer_driver(self, *args, **kwargs):
-        return self.tasker.find_valuer_driver(*args, **kwargs)
-
-    def find_filter_driver(self, *args, **kwargs):
-        return self.tasker.find_filter_driver(*args, **kwargs)
-
-    def find_calculater_driver(self, *args, **kwargs):
-        return self.tasker.find_calculater_driver(*args, **kwargs)
-
-    def create_valuer(self, *args, **kwargs):
-        return self.tasker.create_valuer(*args, **kwargs)
-
-    def create_loader(self, *args, **kwargs):
-        return self.tasker.create_loader(*args, **kwargs)
-
-    def create_join_loader(self, config, join_loaders, renew=False):
-        def format_value_cache_key(value):
-            if isinstance(value, dict):
-                return "{" + ", ".join(["%s: %s" % (format_value_cache_key(key), format_value_cache_key(value[key]))
-                                        for key in sorted(value.keys())]) + "}"
-            if isinstance(value, (tuple, list, set)):
-                try:
-                    return "[" + ", ".join([format_value_cache_key(v) for v in sorted(list(value))]) + "]"
-                except:
-                    return "[" + ", ".join([format_value_cache_key(v) for v in value]) + "]"
-            return str(value)
-
-        loader_cache_key, loader_cache_foreign_filters = None, ""
-        if join_loaders is not None:
-            if config["foreign_filters"]:
-                loader_cache_foreign_filters = "&".join(sorted(["%s__%s=%s" % (name, exp, format_value_cache_key(valuer))
-                                                                for name, exp, valuer, _, _ in config["foreign_filters"]]))
-            loader_cache_key = "::".join([config["loader"]["name"], config["loader"]["database"],
-                                          "+".join(sorted(config["foreign_keys"])),
-                                          loader_cache_foreign_filters])
-            if not renew and loader_cache_key in join_loaders:
-                return join_loaders[loader_cache_key]
-
-        loader = self.create_loader(config["loader"], config["foreign_keys"])
-        if config["foreign_filters"]:
-            for name, exp, valuer, filter_cls, filter_args in config["foreign_filters"]:
-                inherit_valuers, yield_valuers, aggregate_valuers = [], [], []
-                valuer = self.create_valuer(valuer, schema_field_name="",
-                                            inherit_valuers=inherit_valuers, join_loaders=self.tasker.join_loaders,
-                                            yield_valuers=yield_valuers, aggregate_valuers=aggregate_valuers,
-                                            define_valuers={},
-                                            global_variables=dict(**self.tasker.config["variables"]),
-                                            global_states=self.tasker.states)
-
-                def add_foreign_filter(name, exp, valuer):
-                    def _():
-                        value = self.tasker.execute_valuer(valuer, self.tasker.arguments)
-                        if filter_cls:
-                            if exp == "in" and isinstance(value, list):
-                                value = [filter_cls(filter_args).filter(v) for v in value]
-                            else:
-                                value = filter_cls(filter_args).filter(value)
-                        if exp == "eq":
-                            loader.add_filter(name, exp, value)
-                        else:
-                            getattr(loader, "filter_" + exp)(name, value)
-                    return _
-                self.tasker.add_init_executer(add_foreign_filter(name, exp, valuer))
-        loader = LoaderJoinWarp(loader)
-        if loader_cache_key is not None:
-            if loader_cache_key in join_loaders:
-                join_loaders[loader_cache_key + "#" + str(id(join_loaders[loader_cache_key]))] = join_loaders[loader_cache_key]
-            join_loaders[loader_cache_key] = loader
-        return loader
-
-    def compile_data_valuer(self, *args, **kwargs):
-        return self.tasker.valuer_compiler.compile_data_valuer(*args, **kwargs)
-
-    def create_const_valuer(self, config, **kwargs):
-        valuer_cls = self.find_valuer_driver(config["name"])
-        if not valuer_cls:
-            raise ValuerUnknownException(config["name"] + " is unknown")
-        filter_cls = self.find_filter_driver(config["filter"]["name"]) if "filter" in config and config["filter"] else None
-        filter = filter_cls(config["filter"]["args"]) if filter_cls else None
-        return valuer_cls(config["value"], "", filter)
-
-    def create_data_valuer(self, config, inherit_valuers=None, **kwargs):
-        valuer_cls = self.find_valuer_driver(config["name"])
-        if not valuer_cls:
-            raise ValuerUnknownException(config["name"] + " is unknown")
-
-        return_inherit_valuers = []
-        return_valuer = self.create_valuer(config["return_valuer"], inherit_valuers=return_inherit_valuers, **kwargs) \
-            if "return_valuer" in config and config["return_valuer"] else None
-
-        filter_cls = self.find_filter_driver(config["filter"]["name"]) if "filter" in config and config["filter"] else None
-        filter = filter_cls(config["filter"]["args"]) if filter_cls else None
-
-        current_inherit_valuers = []
-        for inherit_valuer in return_inherit_valuers:
-            inherit_valuer["reflen"] -= 1
-            if inherit_valuer["reflen"] == 0:
-                current_inherit_valuers.append(inherit_valuer["valuer"])
-            elif inherit_valuer["reflen"] > 0 and inherit_valuers is not None:
-                inherit_valuers.append(inherit_valuer)
-
-        return valuer_cls(return_valuer, current_inherit_valuers, config["key"], filter)
-
-    def create_inherit_valuer(self, config, inherit_valuers=None, **kwargs):
-        valuer_cls = self.find_valuer_driver(config["name"])
-        if not valuer_cls:
-            raise ValuerUnknownException(config["name"] + " is unknown")
-        filter_cls = self.find_filter_driver(config["filter"]["name"]) if "filter" in config and config["filter"] else None
-        filter = filter_cls(config["filter"]["args"]) if filter_cls else None
-        value_valuer = self.create_valuer(config["value_valuer"], inherit_valuers=inherit_valuers, **kwargs)
-        inherit_valuer = valuer_cls(value_valuer, config["key"], filter)
-        if inherit_valuers is not None:
-            inherit_valuers.append({
-                "reflen": config["reflen"],
-                "valuer": inherit_valuer,
-            })
-        return inherit_valuer.get_inherit_child_valuer()
-
-    def create_db_load_valuer(self, config, inherit_valuers=None, join_loaders=None, **kwargs):
-        valuer_cls = self.find_valuer_driver(config["name"])
-        if not valuer_cls:
-            raise ValuerUnknownException(config["name"] + " is unknown")
-
-        loader = self.create_join_loader(config, join_loaders)
-        return_inherit_valuers = []
-        return_valuer = self.create_valuer(config["return_valuer"], inherit_valuers=return_inherit_valuers, join_loaders=join_loaders, **kwargs)
-        filter_cls = self.find_filter_driver(config["filter"]["name"]) if "filter" in config and config["filter"] else None
-        filter = filter_cls(config["filter"]["args"]) if filter_cls else None
-
-        for foreign_key in config["foreign_keys"]:
-            if foreign_key not in loader.schema:
-                if loader.loaded:
-                    loader = self.create_join_loader(config, join_loaders, True)
-                loader.add_valuer(foreign_key, self.create_valuer(self.compile_data_valuer(foreign_key, None)))
-
-        try:
-            for key in return_valuer.get_fields():
-                if key not in loader.schema:
-                    if loader.loaded:
-                        loader = self.create_join_loader(config, join_loaders, True)
-                    loader.add_valuer(key, self.create_valuer(self.compile_data_valuer(key, None)))
-        except LoadAllFieldsException:
-            if loader.loaded:
-                loader = self.create_join_loader(config, join_loaders, True)
-            loader.schema.clear()
-            loader.add_key_matcher(".*", self.create_valuer(self.compile_data_valuer("", None)))
-
-        current_inherit_valuers = []
-        for inherit_valuer in return_inherit_valuers:
-            inherit_valuer["reflen"] -= 1
-            if inherit_valuer["reflen"] == 0:
-                current_inherit_valuers.append(inherit_valuer["valuer"])
-            elif inherit_valuer["reflen"] > 0 and inherit_valuers is not None:
-                inherit_valuers.append(inherit_valuer)
-
-        return valuer_cls(loader, config["foreign_keys"], config["foreign_filters"], return_valuer,
-                          current_inherit_valuers, config["key"], filter)
-
-    def create_db_join_valuer(self, config, inherit_valuers=None, join_loaders=None, **kwargs):
-        valuer_cls = self.find_valuer_driver(config["name"])
-        if not valuer_cls:
-            raise ValuerUnknownException(config["name"] + " is unknown")
-
-        loader = self.create_join_loader(config, join_loaders)
-        args_valuers = [self.create_valuer(args_valuer, inherit_valuers=inherit_valuers,
-                                           join_loaders=join_loaders, **kwargs) for args_valuer in config["args_valuers"]] \
-            if config["args_valuers"] else None
-        return_inherit_valuers = []
-        return_valuer = self.create_valuer(config["return_valuer"], inherit_valuers=return_inherit_valuers, join_loaders=join_loaders, **kwargs)
-        filter_cls = self.find_filter_driver(config["filter"]["name"]) if "filter" in config and config["filter"] else None
-        filter = filter_cls(config["filter"]["args"]) if filter_cls else None
-
-        for foreign_key in config["foreign_keys"]:
-            if foreign_key not in loader.schema:
-                if loader.loaded:
-                    loader = self.create_join_loader(config, join_loaders, True)
-                loader.add_valuer(foreign_key, self.create_valuer(self.compile_data_valuer(foreign_key, None)))
-
-        try:
-            for key in return_valuer.get_fields():
-                if key not in loader.schema:
-                    if loader.loaded:
-                        loader = self.create_join_loader(config, join_loaders, True)
-                    loader.add_valuer(key, self.create_valuer(self.compile_data_valuer(key, None)))
-        except LoadAllFieldsException:
-            if loader.loaded:
-                loader = self.create_join_loader(config, join_loaders, True)
-            loader.schema.clear()
-            loader.add_key_matcher(".*", self.create_valuer(self.compile_data_valuer("", None)))
-
-        current_inherit_valuers = []
-        for inherit_valuer in return_inherit_valuers:
-            inherit_valuer["reflen"] -= 1
-            if inherit_valuer["reflen"] == 0:
-                current_inherit_valuers.append(inherit_valuer["valuer"])
-            elif inherit_valuer["reflen"] > 0 and inherit_valuers is not None:
-                inherit_valuers.append(inherit_valuer)
-
-        return valuer_cls(loader, config["foreign_keys"], config["foreign_filters"], args_valuers, return_valuer,
-                          current_inherit_valuers, config["key"], filter)
-
-    def create_case_valuer(self, config, inherit_valuers=None, **kwargs):
-        valuer_cls = self.find_valuer_driver(config["name"])
-        if not valuer_cls:
-            raise ValuerUnknownException(config["name"] + " is unknown")
-
-        if "value_valuer" in config and config["value_valuer"]:
-            value_valuer = self.create_valuer(config["value_valuer"], inherit_valuers=inherit_valuers, **kwargs)
-        else:
-            value_valuer = None
-
-        case_valuers = {}
-        for key, valuer_config in config["case_valuers"].items():
-            case_valuers[key] = self.create_valuer(valuer_config, inherit_valuers=inherit_valuers, **kwargs)
-
-        default_case_valuer = self.create_valuer(config["default_valuer"], inherit_valuers=inherit_valuers, **kwargs) \
-            if "default_valuer" in config and config["default_valuer"] else None
-
-        return_inherit_valuers = []
-        return_valuer = self.create_valuer(config["return_valuer"], inherit_valuers=return_inherit_valuers, **kwargs) \
-            if "return_valuer" in config and config["return_valuer"] else None
-
-        current_inherit_valuers = []
-        for inherit_valuer in return_inherit_valuers:
-            inherit_valuer["reflen"] -= 1
-            if inherit_valuer["reflen"] == 0:
-                current_inherit_valuers.append(inherit_valuer["valuer"])
-            elif inherit_valuer["reflen"] > 0 and inherit_valuers is not None:
-                inherit_valuers.append(inherit_valuer)
-
-        return valuer_cls(case_valuers, default_case_valuer, value_valuer, return_valuer, current_inherit_valuers, config["key"], None)
-
-    def create_calculate_valuer(self, config, inherit_valuers=None, **kwargs):
-        valuer_cls = self.find_valuer_driver(config["name"])
-        if not valuer_cls:
-            raise ValuerUnknownException(config["name"] + " is unknown")
-
-        args_valuers = []
-        for valuer_config in config["args_valuers"]:
-            args_valuers.append(self.create_valuer(valuer_config, inherit_valuers=inherit_valuers, **kwargs))
-        calculater = self.find_calculater_driver(config["key"])
-
-        filter_cls = self.find_filter_driver(config["filter"]["name"]) if "filter" in config and config["filter"] else None
-        filter = filter_cls(config["filter"]["args"]) if filter_cls else None
-
-        return_inherit_valuers = []
-        return_valuer = self.create_valuer(config["return_valuer"], inherit_valuers=return_inherit_valuers, **kwargs) \
-            if "return_valuer" in config and config["return_valuer"] else None
-
-        current_inherit_valuers = []
-        for inherit_valuer in return_inherit_valuers:
-            inherit_valuer["reflen"] -= 1
-            if inherit_valuer["reflen"] == 0:
-                current_inherit_valuers.append(inherit_valuer["valuer"])
-            elif inherit_valuer["reflen"] > 0 and inherit_valuers is not None:
-                inherit_valuers.append(inherit_valuer)
-
-        return valuer_cls(calculater.instance(config['key']), args_valuers, return_valuer, current_inherit_valuers, "", filter)
-
-    def create_schema_valuer(self, config, **kwargs):
-        valuer_cls = self.find_valuer_driver(config["name"])
-        if not valuer_cls:
-            raise ValuerUnknownException(config["name"] + " is unknown")
-        schema_valuers = {}
-        for key, valuer_config in config["schema_valuers"].items():
-            schema_valuers[key] = self.create_valuer(valuer_config, **kwargs)
-        return valuer_cls(schema_valuers, config["key"], None)
-
-    def create_make_valuer(self, config, inherit_valuers=None, **kwargs):
-        valuer_cls = self.find_valuer_driver(config["name"])
-        if not valuer_cls:
-            raise ValuerUnknownException(config["name"] + " is unknown")
-        if isinstance(config["value_valuer"], dict):
-            if "name" in config["value_valuer"] and isinstance(config["value_valuer"]["name"], str):
-                value_valuer = self.create_valuer(config["value_valuer"], inherit_valuers=inherit_valuers, **kwargs)
-            else:
-                value_valuer = {key: (self.create_valuer(key_config, inherit_valuers=inherit_valuers, **kwargs),
-                                      self.create_valuer(value_config, inherit_valuers=inherit_valuers, **kwargs))
-                                for key, (key_config, value_config) in config["value_valuer"].items()}
-        elif isinstance(config["value_valuer"], list):
-            value_valuer = [self.create_valuer(value_config, inherit_valuers=inherit_valuers, **kwargs)
-                            for value_config in config["value_valuer"]]
-        else:
-            value_valuer = None
-
-        return_inherit_valuers = []
-        return_valuer = self.create_valuer(config["return_valuer"], inherit_valuers=return_inherit_valuers, **kwargs) \
-            if "return_valuer" in config and config["return_valuer"] else None
-
-        current_inherit_valuers = []
-        for inherit_valuer in return_inherit_valuers:
-            inherit_valuer["reflen"] -= 1
-            if inherit_valuer["reflen"] == 0:
-                current_inherit_valuers.append(inherit_valuer["valuer"])
-            elif inherit_valuer["reflen"] > 0 and inherit_valuers is not None:
-                inherit_valuers.append(inherit_valuer)
-        return valuer_cls(value_valuer, return_valuer, current_inherit_valuers, config["key"], None)
-
-    def create_let_valuer(self, config, inherit_valuers=None, **kwargs):
-        valuer_cls = self.find_valuer_driver(config["name"])
-        if not valuer_cls:
-            raise ValuerUnknownException(config["name"] + " is unknown")
-        key_valuer = self.create_valuer(config["key_valuer"], inherit_valuers=inherit_valuers, **kwargs) \
-            if "key_valuer" in config and config["key_valuer"] else None
-
-        return_inherit_valuers = []
-        return_valuer = self.create_valuer(config["return_valuer"], inherit_valuers=return_inherit_valuers, **kwargs) \
-            if "return_valuer" in config and config["return_valuer"] else None
-
-        filter_cls = self.find_filter_driver(config["filter"]["name"]) if "filter" in config and config["filter"] else None
-        filter = filter_cls(config["filter"]["args"]) if filter_cls else None
-
-        current_inherit_valuers = []
-        for inherit_valuer in return_inherit_valuers:
-            inherit_valuer["reflen"] -= 1
-            if inherit_valuer["reflen"] == 0:
-                current_inherit_valuers.append(inherit_valuer["valuer"])
-            elif inherit_valuer["reflen"] > 0 and inherit_valuers is not None:
-                inherit_valuers.append(inherit_valuer)
-        return valuer_cls(key_valuer, return_valuer, current_inherit_valuers, config["key"], filter)
-
-    def create_yield_valuer(self, config, inherit_valuers=None, yield_valuers=None, **kwargs):
-        valuer_cls = self.find_valuer_driver(config["name"])
-        if not valuer_cls:
-            raise ValuerUnknownException(config["name"] + " is unknown")
-        value_valuer = self.create_valuer(config["value_valuer"], inherit_valuers=inherit_valuers,
-                                          yield_valuers=yield_valuers, **kwargs) \
-            if "value_valuer" in config and config["value_valuer"] else None
-
-        return_inherit_valuers = []
-        return_valuer = self.create_valuer(config["return_valuer"], inherit_valuers=return_inherit_valuers,
-                                           yield_valuers=yield_valuers, **kwargs) \
-            if "return_valuer" in config and config["return_valuer"] else None
-
-        filter_cls = self.find_filter_driver(config["filter"]["name"]) if "filter" in config and config["filter"] else None
-        filter = filter_cls(config["filter"]["args"]) if filter_cls else None
-
-        current_inherit_valuers = []
-        for inherit_valuer in return_inherit_valuers:
-            inherit_valuer["reflen"] -= 1
-            if inherit_valuer["reflen"] == 0:
-                current_inherit_valuers.append(inherit_valuer["valuer"])
-            elif inherit_valuer["reflen"] > 0 and inherit_valuers is not None:
-                inherit_valuers.append(inherit_valuer)
-        yield_valuer = valuer_cls(value_valuer, return_valuer, current_inherit_valuers, config["key"], filter)
-        if yield_valuers is not None:
-            yield_valuers.append(yield_valuer)
-        return yield_valuer
-
-    def create_aggregate_valuer(self, config, schema_field_name=None, inherit_valuers=None, aggregate_valuers=None, **kwargs):
-        valuer_cls = self.find_valuer_driver(config["name"])
-        if not valuer_cls:
-            raise ValuerUnknownException(config["name"] + " is unknown")
-
-        key_child_aggregate_valuers = []
-        key_valuer = self.create_valuer(config["key_valuer"], schema_field_name=schema_field_name,
-                                        inherit_valuers=inherit_valuers,
-                                        aggregate_valuers=key_child_aggregate_valuers, **kwargs) \
-            if "key_valuer" in config and config["key_valuer"] else None
-        if key_child_aggregate_valuers:
-            raise SyntaxError("aggregate conflict")
-
-        calculate_child_aggregate_valuers = []
-        calculate_inherit_valuers = []
-        calculate_valuer = self.create_valuer(config["calculate_valuer"], schema_field_name=schema_field_name,
-                                              inherit_valuers=calculate_inherit_valuers,
-                                              aggregate_valuers=calculate_child_aggregate_valuers, **kwargs) \
-            if "calculate_valuer" in config and config["calculate_valuer"] else None
-
-        current_inherit_valuers = []
-        for inherit_valuer in calculate_inherit_valuers:
-            inherit_valuer["reflen"] -= 1
-            if inherit_valuer["reflen"] == 0:
-                current_inherit_valuers.append(inherit_valuer["valuer"])
-            elif inherit_valuer["reflen"] > 0 and inherit_valuers is not None:
-                inherit_valuers.append(inherit_valuer)
-
-        manager = aggregate_valuers[0].get_manager() if aggregate_valuers else None
-        aggregate_valuer = valuer_cls(key_valuer, calculate_valuer, current_inherit_valuers, manager, schema_field_name, None)
-        if aggregate_valuers is not None:
-            aggregate_valuers.append(aggregate_valuer)
-        return aggregate_valuer
-
-    def create_call_valuer(self, config, inherit_valuers=None, define_valuers=None, **kwargs):
-        valuer_cls = self.find_valuer_driver(config["name"])
-        if not valuer_cls:
-            raise ValuerUnknownException(config["name"] + " is unknown")
-        value_valuer = self.create_valuer(config["value_valuer"], inherit_valuers=inherit_valuers, **kwargs) \
-            if "value_valuer" in config and config["value_valuer"] else None
-
-        calculate_inherit_valuers = []
-        calculate_valuer = self.create_valuer(config["calculate_valuer"], inherit_valuers=calculate_inherit_valuers,
-                                              define_valuers=define_valuers, **kwargs) \
-            if "calculate_valuer" in config and config["calculate_valuer"] else None
-
-        current_inherit_valuers = []
-        if not calculate_inherit_valuers:
-            if define_valuers and config["key"] in define_valuers:
-                calculate_valuer = define_valuers[config["key"]]
-            else:
-                define_valuers[config["key"]] = calculate_valuer
-        else:
-            for inherit_valuer in calculate_inherit_valuers:
-                inherit_valuer["reflen"] -= 1
-                if inherit_valuer["reflen"] == 0:
-                    current_inherit_valuers.append(inherit_valuer["valuer"])
-                elif inherit_valuer["reflen"] > 0 and inherit_valuers is not None:
-                    inherit_valuers.append(inherit_valuer)
-
-        return_inherit_valuers = []
-        return_valuer = self.create_valuer(config["return_valuer"], inherit_valuers=return_inherit_valuers,
-                                           define_valuers=define_valuers, **kwargs) \
-            if "return_valuer" in config and config["return_valuer"] else None
-
-        for inherit_valuer in return_inherit_valuers:
-            inherit_valuer["reflen"] -= 1
-            if inherit_valuer["reflen"] == 0:
-                current_inherit_valuers.append(inherit_valuer["valuer"])
-            elif inherit_valuer["reflen"] > 0 and inherit_valuers is not None:
-                inherit_valuers.append(inherit_valuer)
-
-        return valuer_cls(value_valuer, calculate_valuer, return_valuer, current_inherit_valuers, None, config['key'], None)
-
-    def create_assign_valuer(self, config, inherit_valuers=None, global_variables=None, **kwargs):
-        valuer_cls = self.find_valuer_driver(config["name"])
-        if not valuer_cls:
-            raise ValuerUnknownException(config["name"] + " is unknown")
-
-        calculate_inherit_valuers = []
-        calculate_valuer = self.create_valuer(config["calculate_valuer"], inherit_valuers=calculate_inherit_valuers,
-                                              global_variables=global_variables, **kwargs) \
-            if "calculate_valuer" in config and config["calculate_valuer"] else None
-
-        return_inherit_valuers = []
-        return_valuer = self.create_valuer(config["return_valuer"], inherit_valuers=return_inherit_valuers,
-                                           global_variables=global_variables, **kwargs) \
-            if "return_valuer" in config and config["return_valuer"] else None
-
-        filter_cls = self.find_filter_driver(config["filter"]["name"]) if "filter" in config and config["filter"] else None
-        filter = filter_cls(config["filter"]["args"]) if filter_cls else None
-
-        current_inherit_valuers = []
-        for inherit_valuer in calculate_inherit_valuers:
-            inherit_valuer["reflen"] -= 1
-            if inherit_valuer["reflen"] == 0:
-                current_inherit_valuers.append(inherit_valuer["valuer"])
-            elif inherit_valuer["reflen"] > 0 and inherit_valuers is not None:
-                inherit_valuers.append(inherit_valuer)
-
-        for inherit_valuer in return_inherit_valuers:
-            inherit_valuer["reflen"] -= 1
-            if inherit_valuer["reflen"] == 0:
-                current_inherit_valuers.append(inherit_valuer["valuer"])
-            elif inherit_valuer["reflen"] > 0 and inherit_valuers is not None:
-                inherit_valuers.append(inherit_valuer)
-
-        return valuer_cls(global_variables, calculate_valuer, return_valuer, current_inherit_valuers, config['key'], filter)
-
-    def create_lambda_valuer(self, config, inherit_valuers=None, **kwargs):
-        valuer_cls = self.find_valuer_driver(config["name"])
-        if not valuer_cls:
-            raise ValuerUnknownException(config["name"] + " is unknown")
-
-        calculate_inherit_valuers = []
-        calculate_valuer = self.create_valuer(config["calculate_valuer"], inherit_valuers=calculate_inherit_valuers,
-                                              **kwargs) if "calculate_valuer" in config and config["calculate_valuer"] else None
-
-        current_inherit_valuers = []
-        for inherit_valuer in calculate_inherit_valuers:
-            inherit_valuer["reflen"] -= 1
-            if inherit_valuer["reflen"] == 0:
-                current_inherit_valuers.append(inherit_valuer["valuer"])
-            elif inherit_valuer["reflen"] > 0 and inherit_valuers is not None:
-                inherit_valuers.append(inherit_valuer)
-
-        return valuer_cls(calculate_valuer, current_inherit_valuers, config['key'], None)
-
-    def create_foreach_valuer(self, config, inherit_valuers=None, **kwargs):
-        valuer_cls = self.find_valuer_driver(config["name"])
-        if not valuer_cls:
-            raise ValuerUnknownException(config["name"] + " is unknown")
-        value_valuer = self.create_valuer(config["value_valuer"], inherit_valuers=inherit_valuers, **kwargs) \
-            if "value_valuer" in config and config["value_valuer"] else None
-
-        calculate_inherit_valuers = []
-        calculate_valuer = self.create_valuer(config["calculate_valuer"], inherit_valuers=calculate_inherit_valuers, **kwargs) \
-            if "calculate_valuer" in config and config["calculate_valuer"] else None
-
-        return_inherit_valuers = []
-        return_valuer = self.create_valuer(config["return_valuer"], inherit_valuers=return_inherit_valuers, **kwargs) \
-            if "return_valuer" in config and config["return_valuer"] else None
-
-        current_inherit_valuers = []
-        for inherit_valuer in calculate_inherit_valuers:
-            inherit_valuer["reflen"] -= 1
-            if inherit_valuer["reflen"] == 0:
-                current_inherit_valuers.append(inherit_valuer["valuer"])
-            elif inherit_valuer["reflen"] > 0 and inherit_valuers is not None:
-                inherit_valuers.append(inherit_valuer)
-
-        for inherit_valuer in return_inherit_valuers:
-            inherit_valuer["reflen"] -= 1
-            if inherit_valuer["reflen"] == 0:
-                current_inherit_valuers.append(inherit_valuer["valuer"])
-            elif inherit_valuer["reflen"] > 0 and inherit_valuers is not None:
-                inherit_valuers.append(inherit_valuer)
-
-        return valuer_cls(value_valuer, calculate_valuer, return_valuer, current_inherit_valuers,
-                          config['key'], None)
-
-    def create_break_valuer(self, config, inherit_valuers=None, **kwargs):
-        valuer_cls = self.find_valuer_driver(config["name"])
-        if not valuer_cls:
-            raise ValuerUnknownException(config["name"] + " is unknown")
-
-        return_inherit_valuers = []
-        return_valuer = self.create_valuer(config["return_valuer"], inherit_valuers=return_inherit_valuers, **kwargs) \
-            if "return_valuer" in config and config["return_valuer"] else None
-
-        current_inherit_valuers = []
-        for inherit_valuer in return_inherit_valuers:
-            inherit_valuer["reflen"] -= 1
-            if inherit_valuer["reflen"] == 0:
-                current_inherit_valuers.append(inherit_valuer["valuer"])
-            elif inherit_valuer["reflen"] > 0 and inherit_valuers is not None:
-                inherit_valuers.append(inherit_valuer)
-
-        return valuer_cls(return_valuer, current_inherit_valuers, config['key'], None)
-
-    def create_continue_valuer(self, config, inherit_valuers=None, **kwargs):
-        valuer_cls = self.find_valuer_driver(config["name"])
-        if not valuer_cls:
-            raise ValuerUnknownException(config["name"] + " is unknown")
-
-        return_inherit_valuers = []
-        return_valuer = self.create_valuer(config["return_valuer"], inherit_valuers=return_inherit_valuers, **kwargs) \
-            if "return_valuer" in config and config["return_valuer"] else None
-
-        current_inherit_valuers = []
-        for inherit_valuer in return_inherit_valuers:
-            inherit_valuer["reflen"] -= 1
-            if inherit_valuer["reflen"] == 0:
-                current_inherit_valuers.append(inherit_valuer["valuer"])
-            elif inherit_valuer["reflen"] > 0 and inherit_valuers is not None:
-                inherit_valuers.append(inherit_valuer)
-        return valuer_cls(return_valuer, current_inherit_valuers, config['key'], None)
-
-
-    def create_if_valuer(self, config, inherit_valuers=None, **kwargs):
-        valuer_cls = self.find_valuer_driver(config["name"])
-        if not valuer_cls:
-            raise ValuerUnknownException(config["name"] + " is unknown")
-
-        if "value_valuer" in config and config["value_valuer"]:
-            value_valuer = self.create_valuer(config["value_valuer"], inherit_valuers=inherit_valuers, **kwargs)
-        else:
-            value_valuer = None
-
-        true_valuer = self.create_valuer(config["true_valuer"], inherit_valuers=inherit_valuers, **kwargs) \
-            if "true_valuer" in config and config["true_valuer"] else None
-
-        false_valuer = self.create_valuer(config["false_valuer"], inherit_valuers=inherit_valuers, **kwargs) \
-            if "false_valuer" in config and config["false_valuer"] else None
-
-        return_inherit_valuers = []
-        return_valuer = self.create_valuer(config["return_valuer"], inherit_valuers=return_inherit_valuers, **kwargs) \
-            if "return_valuer" in config and config["return_valuer"] else None
-
-        current_inherit_valuers = []
-        for inherit_valuer in return_inherit_valuers:
-            inherit_valuer["reflen"] -= 1
-            if inherit_valuer["reflen"] == 0:
-                current_inherit_valuers.append(inherit_valuer["valuer"])
-            elif inherit_valuer["reflen"] > 0 and inherit_valuers is not None:
-                inherit_valuers.append(inherit_valuer)
-
-        return valuer_cls(true_valuer, false_valuer, value_valuer, return_valuer, current_inherit_valuers, config["key"], None)
-
-    def create_match_valuer(self, config, inherit_valuers=None, **kwargs):
-        valuer_cls = self.find_valuer_driver(config["name"])
-        if not valuer_cls:
-            raise ValuerUnknownException(config["name"] + " is unknown")
-
-        if "value_valuer" in config and config["value_valuer"]:
-            value_valuer = self.create_valuer(config["value_valuer"], inherit_valuers=inherit_valuers, **kwargs)
-        else:
-            value_valuer = None
-
-        match_valuers, match_inherit_valuers = {}, []
-        for key, valuer_config in config["match_valuers"].items():
-            match_valuers[key] = self.create_valuer(valuer_config, inherit_valuers=match_inherit_valuers, **kwargs)
-
-        default_match_valuer = self.create_valuer(config["default_valuer"], inherit_valuers=inherit_valuers, **kwargs) \
-            if "default_valuer" in config and config["default_valuer"] else None
-
-        return_inherit_valuers = []
-        return_valuer = self.create_valuer(config["return_valuer"], inherit_valuers=return_inherit_valuers, **kwargs) \
-            if "return_valuer" in config and config["return_valuer"] else None
-
-        current_inherit_valuers = []
-        for inherit_valuer in match_inherit_valuers:
-            inherit_valuer["reflen"] -= 1
-            if inherit_valuer["reflen"] == 0:
-                current_inherit_valuers.append(inherit_valuer["valuer"])
-            elif inherit_valuer["reflen"] > 0 and inherit_valuers is not None:
-                inherit_valuers.append(inherit_valuer)
-
-        for inherit_valuer in return_inherit_valuers:
-            inherit_valuer["reflen"] -= 1
-            if inherit_valuer["reflen"] == 0:
-                current_inherit_valuers.append(inherit_valuer["valuer"])
-            elif inherit_valuer["reflen"] > 0 and inherit_valuers is not None:
-                inherit_valuers.append(inherit_valuer)
-
-        return valuer_cls(match_valuers, default_match_valuer, value_valuer, return_valuer, current_inherit_valuers, config["key"], None)
-
-    def create_state_valuer(self, config, inherit_valuers=None, global_states=None, **kwargs):
-        valuer_cls = self.find_valuer_driver(config["name"])
-        if not valuer_cls:
-            raise ValuerUnknownException(config["name"] + " is unknown")
-
-        calculate_inherit_valuers = []
-        calculate_valuer = self.create_valuer(config["calculate_valuer"], inherit_valuers=calculate_inherit_valuers,
-                                              global_states=global_states, **kwargs) \
-            if "calculate_valuer" in config and config["calculate_valuer"] else None
-
-        default_inherit_valuers = []
-        default_valuer = self.create_valuer(config["default_valuer"], inherit_valuers=default_inherit_valuers,
-                                              global_states=global_states, **kwargs) \
-            if "default_valuer" in config and config["default_valuer"] else None
-
-        return_inherit_valuers = []
-        return_valuer = self.create_valuer(config["return_valuer"], inherit_valuers=return_inherit_valuers,
-                                           global_states=global_states, **kwargs) \
-            if "return_valuer" in config and config["return_valuer"] else None
-
-        filter_cls = self.find_filter_driver(config["filter"]["name"]) if "filter" in config and config["filter"] else None
-        filter = filter_cls(config["filter"]["args"]) if filter_cls else None
-
-        current_inherit_valuers = []
-        for inherit_valuer in calculate_inherit_valuers:
-            inherit_valuer["reflen"] -= 1
-            if inherit_valuer["reflen"] == 0:
-                current_inherit_valuers.append(inherit_valuer["valuer"])
-            elif inherit_valuer["reflen"] > 0 and inherit_valuers is not None:
-                inherit_valuers.append(inherit_valuer)
-
-        for inherit_valuer in default_inherit_valuers:
-            inherit_valuer["reflen"] -= 1
-            if inherit_valuer["reflen"] == 0:
-                current_inherit_valuers.append(inherit_valuer["valuer"])
-            elif inherit_valuer["reflen"] > 0 and inherit_valuers is not None:
-                inherit_valuers.append(inherit_valuer)
-
-        for inherit_valuer in return_inherit_valuers:
-            inherit_valuer["reflen"] -= 1
-            if inherit_valuer["reflen"] == 0:
-                current_inherit_valuers.append(inherit_valuer["valuer"])
-            elif inherit_valuer["reflen"] > 0 and inherit_valuers is not None:
-                inherit_valuers.append(inherit_valuer)
-
-        return valuer_cls(global_states, calculate_valuer, default_valuer, return_valuer, current_inherit_valuers, config['key'], filter)
-
-    def create_cache_valuer(self, config, inherit_valuers=None, **kwargs):
-        valuer_cls = self.find_valuer_driver(config["name"])
-        if not valuer_cls:
-            raise ValuerUnknownException(config["name"] + " is unknown")
-        if config["key"] not in self.tasker.caches:
-            raise CacheUnknownException(config["key"] + " is unknown")
-
-        key_valuer = self.create_valuer(config["key_valuer"], inherit_valuers=inherit_valuers, **kwargs) \
-            if "key_valuer" in config and config["key_valuer"] else None
-
-        calculate_valuer = self.create_valuer(config["calculate_valuer"], inherit_valuers=inherit_valuers, **kwargs) \
-            if "calculate_valuer" in config and config["calculate_valuer"] else None
-
-        return_inherit_valuers = []
-        return_valuer = self.create_valuer(config["return_valuer"], inherit_valuers=return_inherit_valuers, **kwargs) \
-            if "return_valuer" in config and config["return_valuer"] else None
-
-        filter_cls = self.find_filter_driver(config["filter"]["name"]) if "filter" in config and config["filter"] else None
-        filter = filter_cls(config["filter"]["args"]) if filter_cls else None
-
-        current_inherit_valuers = []
-        for inherit_valuer in return_inherit_valuers:
-            inherit_valuer["reflen"] -= 1
-            if inherit_valuer["reflen"] == 0:
-                current_inherit_valuers.append(inherit_valuer["valuer"])
-            elif inherit_valuer["reflen"] > 0 and inherit_valuers is not None:
-                inherit_valuers.append(inherit_valuer)
-
-        return valuer_cls(self.tasker.caches[config["key"]], key_valuer, calculate_valuer, return_valuer,
+# -*- coding: utf-8 -*-
+# 18/8/15
+# create by: snower
+
+from ...valuers.valuer import LoadAllFieldsException
+from ...errors import CacheUnknownException, ValuerUnknownException
+
+
+class LoaderJoinWarp(object):
+    __loader = None
+    wait_try_load_count = 0
+
+    def __init__(self, loader):
+        self.__loader = loader
+        self.wait_try_load_count = 0
+        if hasattr(self.__loader, "create_group_macther"):
+            self.create_group_macther = self.__loader.create_group_macther
+        if hasattr(self.__loader, "create_macther"):
+            self.create_macther = self.__loader.create_macther
+        if hasattr(self.__loader, "try_load"):
+            self.try_load = self.__loader.try_load
+        if hasattr(self.__loader, "load"):
+            self.load = self.__loader.load
+
+    def __getattr__(self, item):
+        if self.__loader is None or item == "_LoaderJoinWarp__loader":
+            return super(LoaderJoinWarp, self).__getattr__(item)
+        return getattr(self.__loader, item)
+
+    def __setattr__(self, key, value):
+        if self.__loader is None or key == "_LoaderJoinWarp__loader":
+            return super(LoaderJoinWarp, self).__setattr__(key, value)
+        return setattr(self.__loader, key, value)
+
+    def __str__(self):
+        return str(self.__loader)
+
+    def __repr__(self):
+        return repr(self.__loader)
+
+    def clone(self):
+        self.__loader = self.__loader.clone()
+        self.wait_try_load_count = 0
+        if hasattr(self.__loader, "create_group_macther"):
+            self.create_group_macther = self.__loader.create_group_macther
+        else:
+            self.create_group_macther = lambda *args, **kwargs: self.__loader.create_group_macther(*args, **kwargs)
+        if hasattr(self.__loader, "create_macther"):
+            self.create_macther = self.__loader.create_macther
+        else:
+            self.create_macther = lambda *args, **kwargs: self.__loader.create_macther(*args, **kwargs)
+        if hasattr(self.__loader, "try_load"):
+            self.try_load = self.__loader.try_load
+        else:
+            self.try_load = lambda *args, **kwargs: self.__loader.try_load(*args, **kwargs)
+        if hasattr(self.__loader, "load"):
+            self.load = self.__loader.load
+        else:
+            self.load = lambda *args, **kwargs: self.__loader.load(*args, **kwargs)
+        return self
+
+    def add_valuer(self, name, valuer):
+        return self.__loader.add_valuer(name, valuer)
+
+    def add_intercept(self, intercept):
+        return self.__loader.add_intercept(intercept)
+
+    def add_key_matcher(self, matcher, valuer):
+        return self.__loader.add_key_matcher(matcher, valuer)
+
+    def get_data_primary_key(self, data):
+        return self.__loader.get_data_primary_key(data)
+
+    def next(self):
+        return self.__loader.next()
+
+    def is_dynamic_schema(self):
+        return self.__loader.is_dynamic_schema()
+
+    def is_streaming(self):
+        return self.__loader.is_streaming()
+
+    def set_streaming(self, is_streaming=None):
+        return self.__loader.set_streaming(is_streaming)
+
+    def create_group_macther(self, return_valuer):
+        return self.__loader.create_group_macther(return_valuer)
+
+    def create_macther(self, keys, values):
+        return self.__loader.create_macther(keys, values)
+
+    def try_load(self):
+        return self.__loader.try_load()
+
+    def load(self, timeout=None):
+        return self.__loader.load(timeout)
+
+    def statistics(self):
+        return self.__loader.statistics()
+
+class ValuerCreater(object):
+    def __init__(self, tasker):
+        self.tasker = tasker
+
+    def find_valuer_driver(self, *args, **kwargs):
+        return self.tasker.find_valuer_driver(*args, **kwargs)
+
+    def find_filter_driver(self, *args, **kwargs):
+        return self.tasker.find_filter_driver(*args, **kwargs)
+
+    def find_calculater_driver(self, *args, **kwargs):
+        return self.tasker.find_calculater_driver(*args, **kwargs)
+
+    def create_valuer(self, *args, **kwargs):
+        return self.tasker.create_valuer(*args, **kwargs)
+
+    def create_loader(self, *args, **kwargs):
+        return self.tasker.create_loader(*args, **kwargs)
+
+    def create_join_loader(self, config, join_loaders, renew=False):
+        def format_value_cache_key(value):
+            if isinstance(value, dict):
+                return "{" + ", ".join(["%s: %s" % (format_value_cache_key(key), format_value_cache_key(value[key]))
+                                        for key in sorted(value.keys())]) + "}"
+            if isinstance(value, (tuple, list, set)):
+                try:
+                    return "[" + ", ".join([format_value_cache_key(v) for v in sorted(list(value))]) + "]"
+                except:
+                    return "[" + ", ".join([format_value_cache_key(v) for v in value]) + "]"
+            return str(value)
+
+        loader_cache_key, loader_cache_foreign_filters = None, ""
+        if join_loaders is not None:
+            if config["foreign_filters"]:
+                loader_cache_foreign_filters = "&".join(sorted(["%s__%s=%s" % (name, exp, format_value_cache_key(valuer))
+                                                                for name, exp, valuer, _, _ in config["foreign_filters"]]))
+            loader_cache_key = "::".join([config["loader"]["name"], config["loader"]["database"],
+                                          "+".join(sorted(config["foreign_keys"])),
+                                          loader_cache_foreign_filters])
+            if not renew and loader_cache_key in join_loaders:
+                return join_loaders[loader_cache_key]
+
+        loader = self.create_loader(config["loader"], config["foreign_keys"])
+        if config["foreign_filters"]:
+            for name, exp, valuer, filter_cls, filter_args in config["foreign_filters"]:
+                inherit_valuers, yield_valuers, aggregate_valuers = [], [], []
+                valuer = self.create_valuer(valuer, schema_field_name="",
+                                            inherit_valuers=inherit_valuers, join_loaders=self.tasker.join_loaders,
+                                            yield_valuers=yield_valuers, aggregate_valuers=aggregate_valuers,
+                                            define_valuers={},
+                                            global_variables=dict(**self.tasker.config["variables"]),
+                                            global_states=self.tasker.states)
+
+                def add_foreign_filter(name, exp, valuer):
+                    def _():
+                        value = self.tasker.execute_valuer(valuer, self.tasker.arguments)
+                        if filter_cls:
+                            if exp == "in" and isinstance(value, list):
+                                value = [filter_cls(filter_args).filter(v) for v in value]
+                            else:
+                                value = filter_cls(filter_args).filter(value)
+                        if exp == "eq":
+                            loader.add_filter(name, exp, value)
+                        else:
+                            getattr(loader, "filter_" + exp)(name, value)
+                    return _
+                self.tasker.add_init_executer(add_foreign_filter(name, exp, valuer))
+        loader = LoaderJoinWarp(loader)
+        if loader_cache_key is not None:
+            if loader_cache_key in join_loaders:
+                join_loaders[loader_cache_key + "#" + str(id(join_loaders[loader_cache_key]))] = join_loaders[loader_cache_key]
+            join_loaders[loader_cache_key] = loader
+        return loader
+
+    def compile_data_valuer(self, *args, **kwargs):
+        return self.tasker.valuer_compiler.compile_data_valuer(*args, **kwargs)
+
+    def create_const_valuer(self, config, **kwargs):
+        valuer_cls = self.find_valuer_driver(config["name"])
+        if not valuer_cls:
+            raise ValuerUnknownException(config["name"] + " is unknown")
+        filter_cls = self.find_filter_driver(config["filter"]["name"]) if "filter" in config and config["filter"] else None
+        filter = filter_cls(config["filter"]["args"]) if filter_cls else None
+        return valuer_cls(config["value"], "", filter)
+
+    def create_data_valuer(self, config, inherit_valuers=None, **kwargs):
+        valuer_cls = self.find_valuer_driver(config["name"])
+        if not valuer_cls:
+            raise ValuerUnknownException(config["name"] + " is unknown")
+
+        return_inherit_valuers = []
+        return_valuer = self.create_valuer(config["return_valuer"], inherit_valuers=return_inherit_valuers, **kwargs) \
+            if "return_valuer" in config and config["return_valuer"] else None
+
+        filter_cls = self.find_filter_driver(config["filter"]["name"]) if "filter" in config and config["filter"] else None
+        filter = filter_cls(config["filter"]["args"]) if filter_cls else None
+
+        current_inherit_valuers = []
+        for inherit_valuer in return_inherit_valuers:
+            inherit_valuer["reflen"] -= 1
+            if inherit_valuer["reflen"] == 0:
+                current_inherit_valuers.append(inherit_valuer["valuer"])
+            elif inherit_valuer["reflen"] > 0 and inherit_valuers is not None:
+                inherit_valuers.append(inherit_valuer)
+
+        return valuer_cls(return_valuer, current_inherit_valuers, config["key"], filter)
+
+    def create_inherit_valuer(self, config, inherit_valuers=None, **kwargs):
+        valuer_cls = self.find_valuer_driver(config["name"])
+        if not valuer_cls:
+            raise ValuerUnknownException(config["name"] + " is unknown")
+        filter_cls = self.find_filter_driver(config["filter"]["name"]) if "filter" in config and config["filter"] else None
+        filter = filter_cls(config["filter"]["args"]) if filter_cls else None
+        value_valuer = self.create_valuer(config["value_valuer"], inherit_valuers=inherit_valuers, **kwargs)
+        inherit_valuer = valuer_cls(value_valuer, config["key"], filter)
+        if inherit_valuers is not None:
+            inherit_valuers.append({
+                "reflen": config["reflen"],
+                "valuer": inherit_valuer,
+            })
+        return inherit_valuer.get_inherit_child_valuer()
+
+    def create_db_load_valuer(self, config, inherit_valuers=None, join_loaders=None, **kwargs):
+        valuer_cls = self.find_valuer_driver(config["name"])
+        if not valuer_cls:
+            raise ValuerUnknownException(config["name"] + " is unknown")
+
+        loader = self.create_join_loader(config, join_loaders)
+        return_inherit_valuers = []
+        return_valuer = self.create_valuer(config["return_valuer"], inherit_valuers=return_inherit_valuers, join_loaders=join_loaders, **kwargs)
+        filter_cls = self.find_filter_driver(config["filter"]["name"]) if "filter" in config and config["filter"] else None
+        filter = filter_cls(config["filter"]["args"]) if filter_cls else None
+
+        for foreign_key in config["foreign_keys"]:
+            if foreign_key not in loader.schema:
+                if loader.loaded:
+                    loader = self.create_join_loader(config, join_loaders, True)
+                loader.add_valuer(foreign_key, self.create_valuer(self.compile_data_valuer(foreign_key, None)))
+
+        try:
+            for key in return_valuer.get_fields():
+                if key not in loader.schema:
+                    if loader.loaded:
+                        loader = self.create_join_loader(config, join_loaders, True)
+                    loader.add_valuer(key, self.create_valuer(self.compile_data_valuer(key, None)))
+        except LoadAllFieldsException:
+            if loader.loaded:
+                loader = self.create_join_loader(config, join_loaders, True)
+            loader.schema.clear()
+            loader.add_key_matcher(".*", self.create_valuer(self.compile_data_valuer("", None)))
+
+        current_inherit_valuers = []
+        for inherit_valuer in return_inherit_valuers:
+            inherit_valuer["reflen"] -= 1
+            if inherit_valuer["reflen"] == 0:
+                current_inherit_valuers.append(inherit_valuer["valuer"])
+            elif inherit_valuer["reflen"] > 0 and inherit_valuers is not None:
+                inherit_valuers.append(inherit_valuer)
+
+        return valuer_cls(loader, config["foreign_keys"], config["foreign_filters"], return_valuer,
+                          current_inherit_valuers, config["key"], filter)
+
+    def create_db_join_valuer(self, config, inherit_valuers=None, join_loaders=None, **kwargs):
+        valuer_cls = self.find_valuer_driver(config["name"])
+        if not valuer_cls:
+            raise ValuerUnknownException(config["name"] + " is unknown")
+
+        loader = self.create_join_loader(config, join_loaders)
+        args_valuers = [self.create_valuer(args_valuer, inherit_valuers=inherit_valuers,
+                                           join_loaders=join_loaders, **kwargs) for args_valuer in config["args_valuers"]] \
+            if config["args_valuers"] else None
+        return_inherit_valuers = []
+        return_valuer = self.create_valuer(config["return_valuer"], inherit_valuers=return_inherit_valuers, join_loaders=join_loaders, **kwargs)
+        filter_cls = self.find_filter_driver(config["filter"]["name"]) if "filter" in config and config["filter"] else None
+        filter = filter_cls(config["filter"]["args"]) if filter_cls else None
+
+        for foreign_key in config["foreign_keys"]:
+            if foreign_key not in loader.schema:
+                if loader.loaded:
+                    loader = self.create_join_loader(config, join_loaders, True)
+                loader.add_valuer(foreign_key, self.create_valuer(self.compile_data_valuer(foreign_key, None)))
+
+        try:
+            for key in return_valuer.get_fields():
+                if key not in loader.schema:
+                    if loader.loaded:
+                        loader = self.create_join_loader(config, join_loaders, True)
+                    loader.add_valuer(key, self.create_valuer(self.compile_data_valuer(key, None)))
+        except LoadAllFieldsException:
+            if loader.loaded:
+                loader = self.create_join_loader(config, join_loaders, True)
+            loader.schema.clear()
+            loader.add_key_matcher(".*", self.create_valuer(self.compile_data_valuer("", None)))
+
+        current_inherit_valuers = []
+        for inherit_valuer in return_inherit_valuers:
+            inherit_valuer["reflen"] -= 1
+            if inherit_valuer["reflen"] == 0:
+                current_inherit_valuers.append(inherit_valuer["valuer"])
+            elif inherit_valuer["reflen"] > 0 and inherit_valuers is not None:
+                inherit_valuers.append(inherit_valuer)
+
+        return valuer_cls(loader, config["foreign_keys"], config["foreign_filters"], args_valuers, return_valuer,
+                          current_inherit_valuers, config["key"], filter)
+
+    def create_case_valuer(self, config, inherit_valuers=None, **kwargs):
+        valuer_cls = self.find_valuer_driver(config["name"])
+        if not valuer_cls:
+            raise ValuerUnknownException(config["name"] + " is unknown")
+
+        if "value_valuer" in config and config["value_valuer"]:
+            value_valuer = self.create_valuer(config["value_valuer"], inherit_valuers=inherit_valuers, **kwargs)
+        else:
+            value_valuer = None
+
+        case_valuers = {}
+        for key, valuer_config in config["case_valuers"].items():
+            case_valuers[key] = self.create_valuer(valuer_config, inherit_valuers=inherit_valuers, **kwargs)
+
+        default_case_valuer = self.create_valuer(config["default_valuer"], inherit_valuers=inherit_valuers, **kwargs) \
+            if "default_valuer" in config and config["default_valuer"] else None
+
+        return_inherit_valuers = []
+        return_valuer = self.create_valuer(config["return_valuer"], inherit_valuers=return_inherit_valuers, **kwargs) \
+            if "return_valuer" in config and config["return_valuer"] else None
+
+        current_inherit_valuers = []
+        for inherit_valuer in return_inherit_valuers:
+            inherit_valuer["reflen"] -= 1
+            if inherit_valuer["reflen"] == 0:
+                current_inherit_valuers.append(inherit_valuer["valuer"])
+            elif inherit_valuer["reflen"] > 0 and inherit_valuers is not None:
+                inherit_valuers.append(inherit_valuer)
+
+        return valuer_cls(case_valuers, default_case_valuer, value_valuer, return_valuer, current_inherit_valuers, config["key"], None)
+
+    def create_calculate_valuer(self, config, inherit_valuers=None, **kwargs):
+        valuer_cls = self.find_valuer_driver(config["name"])
+        if not valuer_cls:
+            raise ValuerUnknownException(config["name"] + " is unknown")
+
+        args_valuers = []
+        for valuer_config in config["args_valuers"]:
+            args_valuers.append(self.create_valuer(valuer_config, inherit_valuers=inherit_valuers, **kwargs))
+        calculater = self.find_calculater_driver(config["key"])
+
+        filter_cls = self.find_filter_driver(config["filter"]["name"]) if "filter" in config and config["filter"] else None
+        filter = filter_cls(config["filter"]["args"]) if filter_cls else None
+
+        return_inherit_valuers = []
+        return_valuer = self.create_valuer(config["return_valuer"], inherit_valuers=return_inherit_valuers, **kwargs) \
+            if "return_valuer" in config and config["return_valuer"] else None
+
+        current_inherit_valuers = []
+        for inherit_valuer in return_inherit_valuers:
+            inherit_valuer["reflen"] -= 1
+            if inherit_valuer["reflen"] == 0:
+                current_inherit_valuers.append(inherit_valuer["valuer"])
+            elif inherit_valuer["reflen"] > 0 and inherit_valuers is not None:
+                inherit_valuers.append(inherit_valuer)
+
+        return valuer_cls(calculater.instance(config['key']), args_valuers, return_valuer, current_inherit_valuers, "", filter)
+
+    def create_schema_valuer(self, config, **kwargs):
+        valuer_cls = self.find_valuer_driver(config["name"])
+        if not valuer_cls:
+            raise ValuerUnknownException(config["name"] + " is unknown")
+        schema_valuers = {}
+        for key, valuer_config in config["schema_valuers"].items():
+            schema_valuers[key] = self.create_valuer(valuer_config, **kwargs)
+        return valuer_cls(schema_valuers, config["key"], None)
+
+    def create_make_valuer(self, config, inherit_valuers=None, **kwargs):
+        valuer_cls = self.find_valuer_driver(config["name"])
+        if not valuer_cls:
+            raise ValuerUnknownException(config["name"] + " is unknown")
+        if isinstance(config["value_valuer"], dict):
+            if "name" in config["value_valuer"] and isinstance(config["value_valuer"]["name"], str):
+                value_valuer = self.create_valuer(config["value_valuer"], inherit_valuers=inherit_valuers, **kwargs)
+            else:
+                value_valuer = {key: (self.create_valuer(key_config, inherit_valuers=inherit_valuers, **kwargs),
+                                      self.create_valuer(value_config, inherit_valuers=inherit_valuers, **kwargs))
+                                for key, (key_config, value_config) in config["value_valuer"].items()}
+        elif isinstance(config["value_valuer"], list):
+            value_valuer = [self.create_valuer(value_config, inherit_valuers=inherit_valuers, **kwargs)
+                            for value_config in config["value_valuer"]]
+        else:
+            value_valuer = None
+
+        return_inherit_valuers = []
+        return_valuer = self.create_valuer(config["return_valuer"], inherit_valuers=return_inherit_valuers, **kwargs) \
+            if "return_valuer" in config and config["return_valuer"] else None
+
+        current_inherit_valuers = []
+        for inherit_valuer in return_inherit_valuers:
+            inherit_valuer["reflen"] -= 1
+            if inherit_valuer["reflen"] == 0:
+                current_inherit_valuers.append(inherit_valuer["valuer"])
+            elif inherit_valuer["reflen"] > 0 and inherit_valuers is not None:
+                inherit_valuers.append(inherit_valuer)
+        return valuer_cls(value_valuer, return_valuer, current_inherit_valuers, config["key"], None)
+
+    def create_let_valuer(self, config, inherit_valuers=None, **kwargs):
+        valuer_cls = self.find_valuer_driver(config["name"])
+        if not valuer_cls:
+            raise ValuerUnknownException(config["name"] + " is unknown")
+        key_valuer = self.create_valuer(config["key_valuer"], inherit_valuers=inherit_valuers, **kwargs) \
+            if "key_valuer" in config and config["key_valuer"] else None
+
+        return_inherit_valuers = []
+        return_valuer = self.create_valuer(config["return_valuer"], inherit_valuers=return_inherit_valuers, **kwargs) \
+            if "return_valuer" in config and config["return_valuer"] else None
+
+        filter_cls = self.find_filter_driver(config["filter"]["name"]) if "filter" in config and config["filter"] else None
+        filter = filter_cls(config["filter"]["args"]) if filter_cls else None
+
+        current_inherit_valuers = []
+        for inherit_valuer in return_inherit_valuers:
+            inherit_valuer["reflen"] -= 1
+            if inherit_valuer["reflen"] == 0:
+                current_inherit_valuers.append(inherit_valuer["valuer"])
+            elif inherit_valuer["reflen"] > 0 and inherit_valuers is not None:
+                inherit_valuers.append(inherit_valuer)
+        return valuer_cls(key_valuer, return_valuer, current_inherit_valuers, config["key"], filter)
+
+    def create_yield_valuer(self, config, inherit_valuers=None, yield_valuers=None, **kwargs):
+        valuer_cls = self.find_valuer_driver(config["name"])
+        if not valuer_cls:
+            raise ValuerUnknownException(config["name"] + " is unknown")
+        value_valuer = self.create_valuer(config["value_valuer"], inherit_valuers=inherit_valuers,
+                                          yield_valuers=yield_valuers, **kwargs) \
+            if "value_valuer" in config and config["value_valuer"] else None
+
+        return_inherit_valuers = []
+        return_valuer = self.create_valuer(config["return_valuer"], inherit_valuers=return_inherit_valuers,
+                                           yield_valuers=yield_valuers, **kwargs) \
+            if "return_valuer" in config and config["return_valuer"] else None
+
+        filter_cls = self.find_filter_driver(config["filter"]["name"]) if "filter" in config and config["filter"] else None
+        filter = filter_cls(config["filter"]["args"]) if filter_cls else None
+
+        current_inherit_valuers = []
+        for inherit_valuer in return_inherit_valuers:
+            inherit_valuer["reflen"] -= 1
+            if inherit_valuer["reflen"] == 0:
+                current_inherit_valuers.append(inherit_valuer["valuer"])
+            elif inherit_valuer["reflen"] > 0 and inherit_valuers is not None:
+                inherit_valuers.append(inherit_valuer)
+        yield_valuer = valuer_cls(value_valuer, return_valuer, current_inherit_valuers, config["key"], filter)
+        if yield_valuers is not None:
+            yield_valuers.append(yield_valuer)
+        return yield_valuer
+
+    def create_aggregate_valuer(self, config, schema_field_name=None, inherit_valuers=None, aggregate_valuers=None, **kwargs):
+        valuer_cls = self.find_valuer_driver(config["name"])
+        if not valuer_cls:
+            raise ValuerUnknownException(config["name"] + " is unknown")
+
+        key_child_aggregate_valuers = []
+        key_valuer = self.create_valuer(config["key_valuer"], schema_field_name=schema_field_name,
+                                        inherit_valuers=inherit_valuers,
+                                        aggregate_valuers=key_child_aggregate_valuers, **kwargs) \
+            if "key_valuer" in config and config["key_valuer"] else None
+        if key_child_aggregate_valuers:
+            raise SyntaxError("aggregate conflict")
+
+        calculate_child_aggregate_valuers = []
+        calculate_inherit_valuers = []
+        calculate_valuer = self.create_valuer(config["calculate_valuer"], schema_field_name=schema_field_name,
+                                              inherit_valuers=calculate_inherit_valuers,
+                                              aggregate_valuers=calculate_child_aggregate_valuers, **kwargs) \
+            if "calculate_valuer" in config and config["calculate_valuer"] else None
+
+        current_inherit_valuers = []
+        for inherit_valuer in calculate_inherit_valuers:
+            inherit_valuer["reflen"] -= 1
+            if inherit_valuer["reflen"] == 0:
+                current_inherit_valuers.append(inherit_valuer["valuer"])
+            elif inherit_valuer["reflen"] > 0 and inherit_valuers is not None:
+                inherit_valuers.append(inherit_valuer)
+
+        manager = aggregate_valuers[0].get_manager() if aggregate_valuers else None
+        aggregate_valuer = valuer_cls(key_valuer, calculate_valuer, current_inherit_valuers, manager, schema_field_name, None)
+        if aggregate_valuers is not None:
+            aggregate_valuers.append(aggregate_valuer)
+        return aggregate_valuer
+
+    def create_call_valuer(self, config, inherit_valuers=None, define_valuers=None, **kwargs):
+        valuer_cls = self.find_valuer_driver(config["name"])
+        if not valuer_cls:
+            raise ValuerUnknownException(config["name"] + " is unknown")
+        value_valuer = self.create_valuer(config["value_valuer"], inherit_valuers=inherit_valuers, **kwargs) \
+            if "value_valuer" in config and config["value_valuer"] else None
+
+        calculate_inherit_valuers = []
+        calculate_valuer = self.create_valuer(config["calculate_valuer"], inherit_valuers=calculate_inherit_valuers,
+                                              define_valuers=define_valuers, **kwargs) \
+            if "calculate_valuer" in config and config["calculate_valuer"] else None
+
+        current_inherit_valuers = []
+        if not calculate_inherit_valuers:
+            if define_valuers and config["key"] in define_valuers:
+                calculate_valuer = define_valuers[config["key"]]
+            else:
+                define_valuers[config["key"]] = calculate_valuer
+        else:
+            for inherit_valuer in calculate_inherit_valuers:
+                inherit_valuer["reflen"] -= 1
+                if inherit_valuer["reflen"] == 0:
+                    current_inherit_valuers.append(inherit_valuer["valuer"])
+                elif inherit_valuer["reflen"] > 0 and inherit_valuers is not None:
+                    inherit_valuers.append(inherit_valuer)
+
+        return_inherit_valuers = []
+        return_valuer = self.create_valuer(config["return_valuer"], inherit_valuers=return_inherit_valuers,
+                                           define_valuers=define_valuers, **kwargs) \
+            if "return_valuer" in config and config["return_valuer"] else None
+
+        for inherit_valuer in return_inherit_valuers:
+            inherit_valuer["reflen"] -= 1
+            if inherit_valuer["reflen"] == 0:
+                current_inherit_valuers.append(inherit_valuer["valuer"])
+            elif inherit_valuer["reflen"] > 0 and inherit_valuers is not None:
+                inherit_valuers.append(inherit_valuer)
+
+        return valuer_cls(value_valuer, calculate_valuer, return_valuer, current_inherit_valuers, None, config['key'], None)
+
+    def create_assign_valuer(self, config, inherit_valuers=None, global_variables=None, **kwargs):
+        valuer_cls = self.find_valuer_driver(config["name"])
+        if not valuer_cls:
+            raise ValuerUnknownException(config["name"] + " is unknown")
+
+        calculate_inherit_valuers = []
+        calculate_valuer = self.create_valuer(config["calculate_valuer"], inherit_valuers=calculate_inherit_valuers,
+                                              global_variables=global_variables, **kwargs) \
+            if "calculate_valuer" in config and config["calculate_valuer"] else None
+
+        return_inherit_valuers = []
+        return_valuer = self.create_valuer(config["return_valuer"], inherit_valuers=return_inherit_valuers,
+                                           global_variables=global_variables, **kwargs) \
+            if "return_valuer" in config and config["return_valuer"] else None
+
+        filter_cls = self.find_filter_driver(config["filter"]["name"]) if "filter" in config and config["filter"] else None
+        filter = filter_cls(config["filter"]["args"]) if filter_cls else None
+
+        current_inherit_valuers = []
+        for inherit_valuer in calculate_inherit_valuers:
+            inherit_valuer["reflen"] -= 1
+            if inherit_valuer["reflen"] == 0:
+                current_inherit_valuers.append(inherit_valuer["valuer"])
+            elif inherit_valuer["reflen"] > 0 and inherit_valuers is not None:
+                inherit_valuers.append(inherit_valuer)
+
+        for inherit_valuer in return_inherit_valuers:
+            inherit_valuer["reflen"] -= 1
+            if inherit_valuer["reflen"] == 0:
+                current_inherit_valuers.append(inherit_valuer["valuer"])
+            elif inherit_valuer["reflen"] > 0 and inherit_valuers is not None:
+                inherit_valuers.append(inherit_valuer)
+
+        return valuer_cls(global_variables, calculate_valuer, return_valuer, current_inherit_valuers, config['key'], filter)
+
+    def create_lambda_valuer(self, config, inherit_valuers=None, **kwargs):
+        valuer_cls = self.find_valuer_driver(config["name"])
+        if not valuer_cls:
+            raise ValuerUnknownException(config["name"] + " is unknown")
+
+        calculate_inherit_valuers = []
+        calculate_valuer = self.create_valuer(config["calculate_valuer"], inherit_valuers=calculate_inherit_valuers,
+                                              **kwargs) if "calculate_valuer" in config and config["calculate_valuer"] else None
+
+        current_inherit_valuers = []
+        for inherit_valuer in calculate_inherit_valuers:
+            inherit_valuer["reflen"] -= 1
+            if inherit_valuer["reflen"] == 0:
+                current_inherit_valuers.append(inherit_valuer["valuer"])
+            elif inherit_valuer["reflen"] > 0 and inherit_valuers is not None:
+                inherit_valuers.append(inherit_valuer)
+
+        return valuer_cls(calculate_valuer, current_inherit_valuers, config['key'], None)
+
+    def create_foreach_valuer(self, config, inherit_valuers=None, **kwargs):
+        valuer_cls = self.find_valuer_driver(config["name"])
+        if not valuer_cls:
+            raise ValuerUnknownException(config["name"] + " is unknown")
+        value_valuer = self.create_valuer(config["value_valuer"], inherit_valuers=inherit_valuers, **kwargs) \
+            if "value_valuer" in config and config["value_valuer"] else None
+
+        calculate_inherit_valuers = []
+        calculate_valuer = self.create_valuer(config["calculate_valuer"], inherit_valuers=calculate_inherit_valuers, **kwargs) \
+            if "calculate_valuer" in config and config["calculate_valuer"] else None
+
+        return_inherit_valuers = []
+        return_valuer = self.create_valuer(config["return_valuer"], inherit_valuers=return_inherit_valuers, **kwargs) \
+            if "return_valuer" in config and config["return_valuer"] else None
+
+        current_inherit_valuers = []
+        for inherit_valuer in calculate_inherit_valuers:
+            inherit_valuer["reflen"] -= 1
+            if inherit_valuer["reflen"] == 0:
+                current_inherit_valuers.append(inherit_valuer["valuer"])
+            elif inherit_valuer["reflen"] > 0 and inherit_valuers is not None:
+                inherit_valuers.append(inherit_valuer)
+
+        for inherit_valuer in return_inherit_valuers:
+            inherit_valuer["reflen"] -= 1
+            if inherit_valuer["reflen"] == 0:
+                current_inherit_valuers.append(inherit_valuer["valuer"])
+            elif inherit_valuer["reflen"] > 0 and inherit_valuers is not None:
+                inherit_valuers.append(inherit_valuer)
+
+        return valuer_cls(value_valuer, calculate_valuer, return_valuer, current_inherit_valuers,
+                          config['key'], None)
+
+    def create_break_valuer(self, config, inherit_valuers=None, **kwargs):
+        valuer_cls = self.find_valuer_driver(config["name"])
+        if not valuer_cls:
+            raise ValuerUnknownException(config["name"] + " is unknown")
+
+        return_inherit_valuers = []
+        return_valuer = self.create_valuer(config["return_valuer"], inherit_valuers=return_inherit_valuers, **kwargs) \
+            if "return_valuer" in config and config["return_valuer"] else None
+
+        current_inherit_valuers = []
+        for inherit_valuer in return_inherit_valuers:
+            inherit_valuer["reflen"] -= 1
+            if inherit_valuer["reflen"] == 0:
+                current_inherit_valuers.append(inherit_valuer["valuer"])
+            elif inherit_valuer["reflen"] > 0 and inherit_valuers is not None:
+                inherit_valuers.append(inherit_valuer)
+
+        return valuer_cls(return_valuer, current_inherit_valuers, config['key'], None)
+
+    def create_continue_valuer(self, config, inherit_valuers=None, **kwargs):
+        valuer_cls = self.find_valuer_driver(config["name"])
+        if not valuer_cls:
+            raise ValuerUnknownException(config["name"] + " is unknown")
+
+        return_inherit_valuers = []
+        return_valuer = self.create_valuer(config["return_valuer"], inherit_valuers=return_inherit_valuers, **kwargs) \
+            if "return_valuer" in config and config["return_valuer"] else None
+
+        current_inherit_valuers = []
+        for inherit_valuer in return_inherit_valuers:
+            inherit_valuer["reflen"] -= 1
+            if inherit_valuer["reflen"] == 0:
+                current_inherit_valuers.append(inherit_valuer["valuer"])
+            elif inherit_valuer["reflen"] > 0 and inherit_valuers is not None:
+                inherit_valuers.append(inherit_valuer)
+        return valuer_cls(return_valuer, current_inherit_valuers, config['key'], None)
+
+
+    def create_if_valuer(self, config, inherit_valuers=None, **kwargs):
+        valuer_cls = self.find_valuer_driver(config["name"])
+        if not valuer_cls:
+            raise ValuerUnknownException(config["name"] + " is unknown")
+
+        if "value_valuer" in config and config["value_valuer"]:
+            value_valuer = self.create_valuer(config["value_valuer"], inherit_valuers=inherit_valuers, **kwargs)
+        else:
+            value_valuer = None
+
+        true_valuer = self.create_valuer(config["true_valuer"], inherit_valuers=inherit_valuers, **kwargs) \
+            if "true_valuer" in config and config["true_valuer"] else None
+
+        false_valuer = self.create_valuer(config["false_valuer"], inherit_valuers=inherit_valuers, **kwargs) \
+            if "false_valuer" in config and config["false_valuer"] else None
+
+        return_inherit_valuers = []
+        return_valuer = self.create_valuer(config["return_valuer"], inherit_valuers=return_inherit_valuers, **kwargs) \
+            if "return_valuer" in config and config["return_valuer"] else None
+
+        current_inherit_valuers = []
+        for inherit_valuer in return_inherit_valuers:
+            inherit_valuer["reflen"] -= 1
+            if inherit_valuer["reflen"] == 0:
+                current_inherit_valuers.append(inherit_valuer["valuer"])
+            elif inherit_valuer["reflen"] > 0 and inherit_valuers is not None:
+                inherit_valuers.append(inherit_valuer)
+
+        return valuer_cls(true_valuer, false_valuer, value_valuer, return_valuer, current_inherit_valuers, config["key"], None)
+
+    def create_match_valuer(self, config, inherit_valuers=None, **kwargs):
+        valuer_cls = self.find_valuer_driver(config["name"])
+        if not valuer_cls:
+            raise ValuerUnknownException(config["name"] + " is unknown")
+
+        if "value_valuer" in config and config["value_valuer"]:
+            value_valuer = self.create_valuer(config["value_valuer"], inherit_valuers=inherit_valuers, **kwargs)
+        else:
+            value_valuer = None
+
+        match_valuers, match_inherit_valuers = {}, []
+        for key, valuer_config in config["match_valuers"].items():
+            match_valuers[key] = self.create_valuer(valuer_config, inherit_valuers=match_inherit_valuers, **kwargs)
+
+        default_match_valuer = self.create_valuer(config["default_valuer"], inherit_valuers=inherit_valuers, **kwargs) \
+            if "default_valuer" in config and config["default_valuer"] else None
+
+        return_inherit_valuers = []
+        return_valuer = self.create_valuer(config["return_valuer"], inherit_valuers=return_inherit_valuers, **kwargs) \
+            if "return_valuer" in config and config["return_valuer"] else None
+
+        current_inherit_valuers = []
+        for inherit_valuer in match_inherit_valuers:
+            inherit_valuer["reflen"] -= 1
+            if inherit_valuer["reflen"] == 0:
+                current_inherit_valuers.append(inherit_valuer["valuer"])
+            elif inherit_valuer["reflen"] > 0 and inherit_valuers is not None:
+                inherit_valuers.append(inherit_valuer)
+
+        for inherit_valuer in return_inherit_valuers:
+            inherit_valuer["reflen"] -= 1
+            if inherit_valuer["reflen"] == 0:
+                current_inherit_valuers.append(inherit_valuer["valuer"])
+            elif inherit_valuer["reflen"] > 0 and inherit_valuers is not None:
+                inherit_valuers.append(inherit_valuer)
+
+        return valuer_cls(match_valuers, default_match_valuer, value_valuer, return_valuer, current_inherit_valuers, config["key"], None)
+
+    def create_state_valuer(self, config, inherit_valuers=None, global_states=None, **kwargs):
+        valuer_cls = self.find_valuer_driver(config["name"])
+        if not valuer_cls:
+            raise ValuerUnknownException(config["name"] + " is unknown")
+
+        calculate_inherit_valuers = []
+        calculate_valuer = self.create_valuer(config["calculate_valuer"], inherit_valuers=calculate_inherit_valuers,
+                                              global_states=global_states, **kwargs) \
+            if "calculate_valuer" in config and config["calculate_valuer"] else None
+
+        default_inherit_valuers = []
+        default_valuer = self.create_valuer(config["default_valuer"], inherit_valuers=default_inherit_valuers,
+                                              global_states=global_states, **kwargs) \
+            if "default_valuer" in config and config["default_valuer"] else None
+
+        return_inherit_valuers = []
+        return_valuer = self.create_valuer(config["return_valuer"], inherit_valuers=return_inherit_valuers,
+                                           global_states=global_states, **kwargs) \
+            if "return_valuer" in config and config["return_valuer"] else None
+
+        filter_cls = self.find_filter_driver(config["filter"]["name"]) if "filter" in config and config["filter"] else None
+        filter = filter_cls(config["filter"]["args"]) if filter_cls else None
+
+        current_inherit_valuers = []
+        for inherit_valuer in calculate_inherit_valuers:
+            inherit_valuer["reflen"] -= 1
+            if inherit_valuer["reflen"] == 0:
+                current_inherit_valuers.append(inherit_valuer["valuer"])
+            elif inherit_valuer["reflen"] > 0 and inherit_valuers is not None:
+                inherit_valuers.append(inherit_valuer)
+
+        for inherit_valuer in default_inherit_valuers:
+            inherit_valuer["reflen"] -= 1
+            if inherit_valuer["reflen"] == 0:
+                current_inherit_valuers.append(inherit_valuer["valuer"])
+            elif inherit_valuer["reflen"] > 0 and inherit_valuers is not None:
+                inherit_valuers.append(inherit_valuer)
+
+        for inherit_valuer in return_inherit_valuers:
+            inherit_valuer["reflen"] -= 1
+            if inherit_valuer["reflen"] == 0:
+                current_inherit_valuers.append(inherit_valuer["valuer"])
+            elif inherit_valuer["reflen"] > 0 and inherit_valuers is not None:
+                inherit_valuers.append(inherit_valuer)
+
+        return valuer_cls(global_states, calculate_valuer, default_valuer, return_valuer, current_inherit_valuers, config['key'], filter)
+
+    def create_cache_valuer(self, config, inherit_valuers=None, **kwargs):
+        valuer_cls = self.find_valuer_driver(config["name"])
+        if not valuer_cls:
+            raise ValuerUnknownException(config["name"] + " is unknown")
+        if config["key"] not in self.tasker.caches:
+            raise CacheUnknownException(config["key"] + " is unknown")
+
+        key_valuer = self.create_valuer(config["key_valuer"], inherit_valuers=inherit_valuers, **kwargs) \
+            if "key_valuer" in config and config["key_valuer"] else None
+
+        calculate_valuer = self.create_valuer(config["calculate_valuer"], inherit_valuers=inherit_valuers, **kwargs) \
+            if "calculate_valuer" in config and config["calculate_valuer"] else None
+
+        return_inherit_valuers = []
+        return_valuer = self.create_valuer(config["return_valuer"], inherit_valuers=return_inherit_valuers, **kwargs) \
+            if "return_valuer" in config and config["return_valuer"] else None
+
+        filter_cls = self.find_filter_driver(config["filter"]["name"]) if "filter" in config and config["filter"] else None
+        filter = filter_cls(config["filter"]["args"]) if filter_cls else None
+
+        current_inherit_valuers = []
+        for inherit_valuer in return_inherit_valuers:
+            inherit_valuer["reflen"] -= 1
+            if inherit_valuer["reflen"] == 0:
+                current_inherit_valuers.append(inherit_valuer["valuer"])
+            elif inherit_valuer["reflen"] > 0 and inherit_valuers is not None:
+                inherit_valuers.append(inherit_valuer)
+
+        return valuer_cls(self.tasker.caches[config["key"]], key_valuer, calculate_valuer, return_valuer,
                                              current_inherit_valuers, config['key'], filter)
```

### Comparing `syncany-0.2.6/syncany/taskers/iterator.py` & `syncany-0.2.7/syncany/taskers/iterator.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.6/syncany/taskers/tasker.py` & `syncany-0.2.7/syncany/taskers/tasker.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.6/syncany/utils.py` & `syncany-0.2.7/syncany/utils.py`

 * *Files identical despite different names*

### Comparing `syncany-0.2.6/syncany/valuers/__init__.py` & `syncany-0.2.7/syncany/valuers/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-# -*- coding: utf-8 -*-
-# 18/8/6
-# create by: snower
-
-from .valuer import Valuer
-from .const import ConstValuer
-from .data import DataValuer
-from .inherit import InheritValuer
-from .db_load import DBLoadValuer
-from .db_join import DBJoinValuer
-from .case import CaseValuer
-from .calculate import CalculateValuer
-from .schema import SchemaValuer
-from .make import MakeValuer
-from .let import LetValuer
-from .generator import YieldValuer
-from .aggregate import AggregateValuer
-from .call import CallValuer
-from .assign import AssignValuer
-from .function import LambdaValuer
-from .loop import ForeachValuer, BreakValuer, ContinueValuer
-from .condition import IfValuer
-from .match import MatchValuer
-from .state import StateValuer
-from .cache import CacheValuer
-from ..errors import ValuerUnknownException
-
-VALUERS = {
-    "const_valuer": ConstValuer,
-    "data_valuer": DataValuer,
-    "inherit_valuer": InheritValuer,
-    "db_load_valuer": DBLoadValuer,
-    "db_join_valuer": DBJoinValuer,
-    "case_valuer": CaseValuer,
-    "calculate_valuer": CalculateValuer,
-    "schema_valuer": SchemaValuer,
-    "make_valuer": MakeValuer,
-    "let_valuer": LetValuer,
-    "yield_valuer": YieldValuer,
-    "aggregate_valuer": AggregateValuer,
-    "call_valuer": CallValuer,
-    "assign_valuer": AssignValuer,
-    "lambda_valuer": LambdaValuer,
-    "foreach_valuer": ForeachValuer,
-    "break_valuer": BreakValuer,
-    "continue_valuer": ContinueValuer,
-    "if_valuer": IfValuer,
-    "match_valuer": MatchValuer,
-    "state_valuer": StateValuer,
-    "cache_valuer": CacheValuer,
-}
-
-def find_valuer(name):
-    if name not in VALUERS:
-        raise ValuerUnknownException("%s is unknown valuer" % name)
-    return VALUERS[name]
-
-def register_valuer(name, valuer=None):
-    if valuer is None:
-        def _(valuer):
-            if not issubclass(valuer, Valuer):
-                raise TypeError("is not Valuer")
-            VALUERS[name] = valuer
-            return valuer
-        return _
-
-    if not issubclass(valuer, Valuer):
-        raise TypeError("is not Valuer")
-    VALUERS[name] = valuer
+# -*- coding: utf-8 -*-
+# 18/8/6
+# create by: snower
+
+from .valuer import Valuer, Contexter, ContextRunner
+from .const import ConstValuer
+from .data import DataValuer
+from .inherit import InheritValuer
+from .db_load import DBLoadValuer
+from .db_join import DBJoinValuer
+from .case import CaseValuer
+from .calculate import CalculateValuer
+from .schema import SchemaValuer
+from .make import MakeValuer
+from .let import LetValuer
+from .generator import YieldValuer
+from .aggregate import AggregateValuer
+from .call import CallValuer
+from .assign import AssignValuer
+from .function import LambdaValuer
+from .loop import ForeachValuer, BreakValuer, ContinueValuer
+from .condition import IfValuer
+from .match import MatchValuer
+from .state import StateValuer
+from .cache import CacheValuer
+from ..errors import ValuerUnknownException
+
+VALUERS = {
+    "const_valuer": ConstValuer,
+    "data_valuer": DataValuer,
+    "inherit_valuer": InheritValuer,
+    "db_load_valuer": DBLoadValuer,
+    "db_join_valuer": DBJoinValuer,
+    "case_valuer": CaseValuer,
+    "calculate_valuer": CalculateValuer,
+    "schema_valuer": SchemaValuer,
+    "make_valuer": MakeValuer,
+    "let_valuer": LetValuer,
+    "yield_valuer": YieldValuer,
+    "aggregate_valuer": AggregateValuer,
+    "call_valuer": CallValuer,
+    "assign_valuer": AssignValuer,
+    "lambda_valuer": LambdaValuer,
+    "foreach_valuer": ForeachValuer,
+    "break_valuer": BreakValuer,
+    "continue_valuer": ContinueValuer,
+    "if_valuer": IfValuer,
+    "match_valuer": MatchValuer,
+    "state_valuer": StateValuer,
+    "cache_valuer": CacheValuer,
+}
+
+def find_valuer(name):
+    if name not in VALUERS:
+        raise ValuerUnknownException("%s is unknown valuer" % name)
+    return VALUERS[name]
+
+def register_valuer(name, valuer=None):
+    if valuer is None:
+        def _(valuer):
+            if not issubclass(valuer, Valuer):
+                raise TypeError("is not Valuer")
+            VALUERS[name] = valuer
+            return valuer
+        return _
+
+    if not issubclass(valuer, Valuer):
+        raise TypeError("is not Valuer")
+    VALUERS[name] = valuer
     return valuer
```

### Comparing `syncany-0.2.6/syncany/valuers/aggregate.py` & `syncany-0.2.7/syncany/valuers/data.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,134 +1,139 @@
 # -*- coding: utf-8 -*-
-# 2020/7/2
+# 18/8/6
 # create by: snower
 
-from .valuer import Valuer
+import datetime
+from ..utils import ensure_timezone
+from ..filters import ArrayFilter
+from .valuer import Valuer, LoadAllFieldsException
 
-class AggregateData(object):
-    def __init__(self, data, state):
-        self.data = data
-        self.state = state
-
-class AggregateManager(object):
-    def __init__(self):
-        self.datas = {}
-
-    def loaded(self, key, name):
-        if key not in self.datas:
-            return False
-        if name not in self.datas[key].state:
-            return False
-        return True
 
-    def get(self, key):
-        if key not in self.datas:
-            return None
-        return self.datas[key].data
-
-    def set(self, key, name, value):
-        if key not in self.datas:
-            return None
-        self.datas[key].data[name] = value
-
-    def add(self, key, name, data, value):
-        if key in self.datas:
-            aggregate_value = self.datas[key]
-            aggregate_value.state[name] = True
-        else:
-            aggregate_value = AggregateData(data, {name: True})
-            self.datas[key] = aggregate_value
-        aggregate_value.data[name] = value
-
-    def reset(self):
-        self.datas = {}
-
-class AggregateValuer(Valuer):
-    def __init__(self, key_valuer, calculate_valuer, inherit_valuers, aggregate_manager, *args, **kwargs):
-        self.key_valuer = key_valuer
-        self.calculate_valuer = calculate_valuer
+class DataValuer(Valuer):
+    def __init__(self, return_valuer, inherit_valuers, *args, **kwargs):
+        self.return_valuer = return_valuer
         self.inherit_valuers = inherit_valuers
-        self.aggregate_manager = aggregate_manager or AggregateManager()
-        super(AggregateValuer, self).__init__(*args, **kwargs)
+        super(DataValuer, self).__init__(*args, **kwargs)
 
-        self.key_value = None
-        self.loader_loaded = False
+        self.option = None
 
-    def get_manager(self):
-        return self.aggregate_manager
+    def new_init(self):
+        super(DataValuer, self).new_init()
+        if self.key in self.KEY_GETTER_CACHES:
+            self.key_getters = self.KEY_GETTER_CACHES[self.key]
+        else:
+            self.parse_key()
 
     def add_inherit_valuer(self, valuer):
         self.inherit_valuers.append(valuer)
 
-    def clone(self):
-        key_valuer = self.key_valuer.clone() if self.key_valuer else None
-        calculate_valuer = self.calculate_valuer.clone() if self.calculate_valuer else None
-        inherit_valuers = [inherit_valuer.clone() for inherit_valuer in self.inherit_valuers] if self.inherit_valuers else None
-        return self.__class__(key_valuer, calculate_valuer, inherit_valuers, self.aggregate_manager, self.key,
-                              self.filter, from_valuer=self)
-
-    def reinit(self):
-        self.key_value = None
-        self.loader_loaded = False
-        return super(AggregateValuer, self).reinit()
+    def clone(self, contexter=None):
+        return_valuer = self.return_valuer.clone(contexter) if self.return_valuer else None
+        inherit_valuers = [inherit_valuer.clone(contexter) for inherit_valuer in self.inherit_valuers] \
+            if self.inherit_valuers else None
+        if contexter is not None:
+            valuer = ContextDataValuer(return_valuer, inherit_valuers, self.key, self.filter, from_valuer=self,
+                                       contexter=contexter)
+        elif isinstance(self, ContextDataValuer):
+            valuer = ContextDataValuer(return_valuer, inherit_valuers, self.key, self.filter, from_valuer=self,
+                                       contexter=self.contexter)
+        else:
+            valuer = self.__class__(return_valuer, inherit_valuers, self.key, self.filter, from_valuer=self)
+        valuer.option = self.option
+        return valuer
 
     def fill(self, data):
         if self.inherit_valuers:
             for inherit_valuer in self.inherit_valuers:
                 inherit_valuer.fill(data)
 
-        if self.key_valuer:
-            self.key_valuer.fill(data)
+        if isinstance(data, dict) and self.key in data:
+            value = self.do_filter(data[self.key])
+        elif data is None or not self.key:
+            value = self.do_filter(None)
+        elif self.key == "*":
+            value = self.do_filter(data)
+        else:
+            if not self.key_getters:
+                if self.key in self.KEY_GETTER_CACHES:
+                    self.key_getters = self.KEY_GETTER_CACHES[self.key]
+                else:
+                    self.parse_key()
+            try:
+                key_getter_index, key_getter_len = 0, len(self.key_getters)
+                while key_getter_index < key_getter_len:
+                    data, index = self.key_getters[key_getter_index](data)
+                    if data is None:
+                        break
+                    key_getter_index += index
+                value = self.do_filter(data)
+            except:
+                value = self.do_filter(None)
+
+        if self.return_valuer:
+            self.return_valuer.fill(value)
+        else:
+            self.value = value
         return self
 
     def get(self):
-        self.key_value = self.key_valuer.get() if self.key_valuer else ""
-
-        def calculate_value(data):
-            self.loader_loaded = self.aggregate_manager.loaded(self.key_value, self.key)
-            if self.loader_loaded:
-                cdata = self.aggregate_manager.get(self.key_value)
-                self.calculate_valuer.fill(cdata)
-                self.do_filter(self.calculate_valuer.get())
-                self.aggregate_manager.set(self.key_value, self.key, self.value)
-                raise StopIteration
-
-            self.calculate_valuer.fill(data)
-            self.do_filter(self.calculate_valuer.get())
-            self.aggregate_manager.add(self.key_value, self.key, data, self.value)
-            return self.value
-        return calculate_value
-
-    def reset(self):
-        self.aggregate_manager.reset()
-        super(AggregateValuer, self).reset()
+        if self.return_valuer:
+            return self.return_valuer.get()
+        return self.value
+
+    def do_filter(self, value):
+        if not self.filter:
+            if isinstance(value, datetime.datetime):
+                value = ensure_timezone(value)
+            return value
+
+        if isinstance(value, list):
+            if isinstance(self.filter, ArrayFilter):
+                return value
+            return [self.filter.filter(v) for v in value]
+        return self.filter.filter(value)
 
     def childs(self):
-        childs = []
-        if self.key_valuer:
-            childs.append(self.key_valuer)
-        if self.calculate_valuer:
-            childs.append(self.calculate_valuer)
-        if self.inherit_valuers:
-            for inherit_valuer in self.inherit_valuers:
-                childs.append(inherit_valuer)
-        return childs
+        if self.return_valuer:
+            return [self.return_valuer]
+        return []
 
     def get_fields(self):
-        fields = []
-        if self.key_valuer:
-            for field in self.key_valuer.get_fields():
-                fields.append(field)
-
-        if self.inherit_valuers:
-            for inherit_valuer in self.inherit_valuers:
-                for field in inherit_valuer.get_fields():
-                    fields.append(field)
-        return fields
+        if not self.key or self.key == "*":
+            if self.return_valuer:
+                return self.return_valuer.get_fields()
+            raise LoadAllFieldsException()
+
+        keys = [key for key in self.key.split(".") if key and key[0] != ":"]
+        if not keys:
+            return []
+        return keys
 
     def get_final_filter(self):
-        if self.filter:
-            return self.filter
+        if self.return_valuer:
+            return self.return_valuer.get_final_filter()
+        return self.filter
+
+    def require_loaded(self):
+        return False
+
+
+class ContextDataValuer(DataValuer):
+    def __init__(self, *args, **kwargs):
+        self.contexter = kwargs.pop("contexter")
+        self.value_context_id = (id(self), "value")
+        super(ContextDataValuer, self).__init__(*args, **kwargs)
+
+    @property
+    def value(self):
+        try:
+            return self.contexter.values[self.value_context_id]
+        except KeyError:
+            return None
 
-        if self.calculate_valuer:
-            return self.calculate_valuer.get_final_filter()
-        return None
+    @value.setter
+    def value(self, v):
+        if v is None:
+            if self.value_context_id in self.contexter.values:
+                self.contexter.values.pop(self.value_context_id)
+            return
+        self.contexter.values[self.value_context_id] = v
```

### Comparing `syncany-0.2.6/syncany/valuers/assign.py` & `syncany-0.2.7/syncany/valuers/function.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,95 +1,86 @@
 # -*- coding: utf-8 -*-
-# 2020/7/3
+# 2021/2/4
 # create by: snower
 
 from .valuer import Valuer
 
-class AssignValuer(Valuer):
-    def __init__(self, global_value, calculate_valuer, return_valuer, inherit_valuers, *args, **kwargs):
-        self.global_value = global_value
+
+class LambdaFunction(object):
+    def __init__(self, calculate_valuer):
         self.calculate_valuer = calculate_valuer
-        self.return_valuer = return_valuer
-        self.inherit_valuers = inherit_valuers
-        super(AssignValuer, self).__init__(*args, **kwargs)
 
-    def new_init(self):
-        super(AssignValuer, self).new_init()
-        self.calculate_wait_loaded = self.calculate_valuer and self.calculate_valuer.require_loaded()
-
-    def clone_init(self, from_valuer):
-        super(AssignValuer, self).clone_init(from_valuer)
-        self.calculate_wait_loaded = from_valuer.calculate_wait_loaded
+    def __call__(self, data):
+        calculate_valuer = self.calculate_valuer.clone()
+        calculate_valuer.fill(data)
+        return calculate_valuer.get()
+
+
+class LambdaValuer(Valuer):
+    def __init__(self, calculate_valuer, inherit_valuers, *args, **kwargs):
+        self.calculate_valuer = calculate_valuer
+        self.inherit_valuers = inherit_valuers
+        super(LambdaValuer, self).__init__(*args, **kwargs)
 
     def add_inherit_valuer(self, valuer):
         self.inherit_valuers.append(valuer)
 
-    def clone(self):
-        calculate_valuer = self.calculate_valuer.clone() if self.calculate_valuer else None
-        return_valuer = self.return_valuer.clone() if self.return_valuer else None
-        inherit_valuers = [inherit_valuer.clone() for inherit_valuer in self.inherit_valuers] if self.inherit_valuers else None
-        return self.__class__(self.global_value, calculate_valuer, return_valuer, inherit_valuers,
-                              self.key, self.filter, from_valuer=self)
+    def clone(self, contexter=None):
+        calculate_valuer = self.calculate_valuer.clone(contexter) if self.calculate_valuer else None
+        inherit_valuers = [inherit_valuer.clone(contexter) for inherit_valuer in self.inherit_valuers] \
+            if self.inherit_valuers else None
+        if contexter is not None:
+            return ContextLambdaValuer(calculate_valuer, inherit_valuers, self.key, self.filter, from_valuer=self,
+                                       contexter=contexter)
+        if isinstance(self, ContextLambdaValuer):
+            return ContextLambdaValuer(calculate_valuer, inherit_valuers, self.key, self.filter, from_valuer=self,
+                                       contexter=self.contexter)
+        return self.__class__(calculate_valuer, inherit_valuers, self.key, self.filter, from_valuer=self)
 
     def fill(self, data):
         if self.inherit_valuers:
             for inherit_valuer in self.inherit_valuers:
                 inherit_valuer.fill(data)
-
-        if self.calculate_valuer:
-            self.calculate_valuer.fill(self.global_value)
-            if not self.calculate_wait_loaded:
-                self.do_filter(self.calculate_valuer.get())
-                self.global_value[self.key] = self.value
-                if self.return_valuer:
-                    self.return_valuer.fill(self.value)
-        elif self.return_valuer:
-            self.do_filter(self.global_value.get(self.key, None))
-            final_filter = self.return_valuer.get_final_filter()
-            if final_filter:
-                self.value = final_filter.filter(self.value)
-            self.return_valuer.fill(self.value)
-        else:
-            self.do_filter(self.global_value.get(self.key, None))
         return self
 
     def get(self):
-        if self.calculate_valuer:
-            if self.calculate_wait_loaded:
-                self.do_filter(self.calculate_valuer.get())
-                self.global_value[self.key] = self.value
-                if self.return_valuer:
-                    self.return_valuer.fill(self.value)
-
-        if self.return_valuer:
-            self.value = self.return_valuer.get()
-        return self.value
+        return LambdaFunction(self.calculate_valuer)
 
     def childs(self):
         childs = []
-        if self.calculate_valuer:
-            childs.append(self.calculate_valuer)
-        if self.return_valuer:
-            childs.append(self.return_valuer)
         if self.inherit_valuers:
             for inherit_valuer in self.inherit_valuers:
                 childs.append(inherit_valuer)
         return childs
 
     def get_fields(self):
         fields = []
         if self.inherit_valuers:
             for inherit_valuer in self.inherit_valuers:
                 for field in inherit_valuer.get_fields():
                     fields.append(field)
         return fields
 
     def get_final_filter(self):
-        if self.return_valuer:
-            return self.calculate_valuer.get_final_filter()
+        return None
 
-        if self.filter:
-            return self.filter
 
-        if self.calculate_valuer:
-            return self.calculate_valuer.get_final_filter()
-        return None
+class ContextLambdaValuer(LambdaValuer):
+    def __init__(self, *args, **kwargs):
+        self.contexter = kwargs.pop("contexter")
+        self.value_context_id = (id(self), "value")
+        super(ContextLambdaValuer, self).__init__(*args, **kwargs)
+
+    @property
+    def value(self):
+        try:
+            return self.contexter.values[self.value_context_id]
+        except KeyError:
+            return None
+
+    @value.setter
+    def value(self, v):
+        if v is None:
+            if self.value_context_id in self.contexter.values:
+                self.contexter.values.pop(self.value_context_id)
+            return
+        self.contexter.values[self.value_context_id] = v
```

### Comparing `syncany-0.2.6/syncany/valuers/cache.py` & `syncany-0.2.7/syncany/valuers/inherit.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,136 +1,169 @@
 # -*- coding: utf-8 -*-
-# 2021/11/7
+# 2020/6/28
 # create by: snower
 
+import weakref
 from .valuer import Valuer
 
-class CacheValuer(Valuer):
-    def __init__(self, cache_loader, key_valuer, calculate_valuer, return_valuer, inherit_valuers, *args, **kwargs):
-        self.cache_loader = cache_loader
-        self.key_valuer = key_valuer
-        self.calculate_valuer = calculate_valuer
-        self.return_valuer = return_valuer
-        self.inherit_valuers = inherit_valuers
-        super(CacheValuer, self).__init__(*args, **kwargs)
-
-        self.cache_key = ""
-
-    def new_init(self):
-        super(CacheValuer, self).new_init()
-        self.key_wait_loaded = self.key_valuer and self.key_valuer.require_loaded()
-        self.calculate_wait_loaded = self.calculate_valuer and self.calculate_valuer.require_loaded()
-
-    def clone_init(self, from_valuer):
-        super(CacheValuer, self).clone_init(from_valuer)
-        self.key_wait_loaded = from_valuer.key_wait_loaded
-        self.calculate_wait_loaded = from_valuer.calculate_wait_loaded
-
-    def add_inherit_valuer(self, valuer):
-        self.inherit_valuers.append(valuer)
-
-    def clone(self):
-        key_valuer = self.key_valuer.clone() if self.key_valuer else None
-        calculate_valuer = self.calculate_valuer.clone() if self.calculate_valuer else None
-        return_valuer = self.return_valuer.clone() if self.return_valuer else None
-        inherit_valuers = [inherit_valuer.clone() for inherit_valuer in self.inherit_valuers] if self.inherit_valuers else None
-        return self.__class__(self.cache_loader, key_valuer, calculate_valuer, return_valuer, inherit_valuers,
-                              self.key, self.filter, from_valuer=self)
 
-    def reinit(self):
-        self.cache_key = ""
-        return super(CacheValuer, self).reinit()
+class InheritValuer(Valuer):
+    filled = False
 
-    def fill(self, data):
-        if self.inherit_valuers:
-            for inherit_valuer in self.inherit_valuers:
-                inherit_valuer.fill(data)
-
-        self.key_valuer.fill(data)
-        if self.key_wait_loaded:
-            self.calculate_valuer.fill(data)
-            return self
-        self.cache_key = str(self.key_valuer.get())
-        self.value = self.cache_loader.get(self.cache_key)
-        if self.value is not None:
-            return self
+    def __init__(self, value_valuer, *args, **kwargs):
+        if isinstance(self, ContextInheritValuer):
+            self.child_valuer = ContextInheritChildValuer(self, value_valuer, *args, **kwargs, contexter=self.contexter)
+        else:
+            self.child_valuer = InheritChildValuer(self, value_valuer, *args, **kwargs)
+        self.value_valuer = value_valuer
+        self.cloned_child_valuer = None
+        super(InheritValuer, self).__init__(*args, **kwargs)
+
+    def get_inherit_child_valuer(self):
+        return self.child_valuer
 
-        self.calculate_valuer.fill(data)
-        if self.calculate_wait_loaded:
+    def clone(self, contexter=None):
+        if self.filled:
             return self
-        self.value = self.calculate_valuer.get()
-        if self.value is not None:
-            self.cache_loader.set(self.cache_key, self.value)
-
-        if self.return_valuer:
-            self.do_filter(self.value)
-            final_filter = self.return_valuer.get_final_filter()
-            if final_filter:
-                self.value = final_filter.filter(self.value)
-            self.return_valuer.fill(self.value)
+
+        if self.child_valuer.cloned_inherit_valuer:
+            inherit_valuer = self.child_valuer.cloned_inherit_valuer
+            self.child_valuer.cloned_inherit_valuer = None
+            return inherit_valuer
+
+        value_valuer = self.value_valuer.clone(contexter) if self.value_valuer else None
+        if contexter is not None:
+            inherit_valuer = ContextInheritValuer(value_valuer, self.key, self.filter, from_valuer=self,
+                                                  contexter=contexter)
+        elif isinstance(self, ContextInheritValuer):
+            inherit_valuer = ContextInheritValuer(value_valuer, self.key, self.filter, from_valuer=self,
+                                                  contexter=self.contexter)
         else:
-            self.do_filter(self.value)
+            inherit_valuer = self.__class__(value_valuer, self.key, self.filter, from_valuer=self)
+        self.cloned_child_valuer = inherit_valuer.get_inherit_child_valuer()
+        return inherit_valuer
+
+    def reinit(self):
+        self.filled = False
+        return super(InheritValuer, self).reinit()
+
+    def fill(self, data):
+        if self.value_valuer:
+            self.value_valuer.fill(self.do_filter(data))
+        else:
+            super(InheritValuer, self).fill(data)
+        self.filled = True
         return self
 
     def get(self):
-        if not self.key_wait_loaded:
-            if not self.calculate_wait_loaded:
-                if self.return_valuer:
-                    self.value = self.return_valuer.get()
-                return self.value
-        else:
-            self.cache_key = str(self.key_valuer.get())
-            self.value = self.cache_loader.get(self.cache_key)
+        return None
+
+    def childs(self):
+        if not self.value_valuer:
+            return []
+        return [self.value_valuer]
 
-        if self.value is None and self.calculate_wait_loaded:
-            self.value = self.calculate_valuer.get()
-            if self.value is not None:
-                self.cache_loader.set(self.cache_key, self.value)
-
-        if self.return_valuer:
-            self.do_filter(self.value)
-            final_filter = self.return_valuer.get_final_filter()
-            if final_filter:
-                self.value = final_filter.filter(self.value)
-            self.return_valuer.fill(self.value)
-            self.value = self.return_valuer.get()
+    def get_fields(self):
+        if not self.value_valuer:
+            return []
+        return self.value_valuer.get_fields()
+
+    def get_final_filter(self):
+        return None
+
+
+class ContextInheritValuer(InheritValuer):
+    def __init__(self, *args, **kwargs):
+        self.contexter = kwargs.pop("contexter")
+        self.value_context_id = (id(self), "value")
+        super(ContextInheritValuer, self).__init__(*args, **kwargs)
+
+    @property
+    def value(self):
+        try:
+            return self.contexter.values[self.value_context_id]
+        except KeyError:
+            return None
+
+    @value.setter
+    def value(self, v):
+        if v is None:
+            if self.value_context_id in self.contexter.values:
+                self.contexter.values.pop(self.value_context_id)
+            return
+        self.contexter.values[self.value_context_id] = v
+
+
+class InheritChildValuer(Valuer):
+    def __init__(self, inherit_valuer, value_valuer, *args, **kwargs):
+        self.inherit_valuer = weakref.proxy(inherit_valuer)
+        self.value_valuer = value_valuer
+        self.cloned_inherit_valuer = None
+        super(InheritChildValuer, self).__init__(*args, **kwargs)
+
+    def clone(self, contexter=None):
+        if self.inherit_valuer.filled:
+            return self
+
+        if self.inherit_valuer.cloned_child_valuer:
+            child_valuer = self.inherit_valuer.cloned_child_valuer
+            self.inherit_valuer.cloned_child_valuer = None
+            return child_valuer
+
+        value_valuer = self.value_valuer.clone(contexter) if self.value_valuer else None
+        if contexter is not None:
+            self.cloned_inherit_valuer = ContextInheritValuer(value_valuer, self.key, self.filter, from_valuer=self,
+                                                              contexter=contexter)
+        elif isinstance(self, ContextInheritChildValuer):
+            self.cloned_inherit_valuer = ContextInheritValuer(value_valuer, self.key, self.filter, from_valuer=self,
+                                                              contexter=self.contexter)
         else:
-            self.do_filter(self.value)
+            self.cloned_inherit_valuer = InheritValuer(value_valuer, self.key, self.filter, from_valuer=self)
+        return self.cloned_inherit_valuer.get_inherit_child_valuer()
+
+    def fill(self, data):
+        return self
+
+    def get(self):
+        if self.value_valuer:
+            return self.value_valuer.get()
         return self.value
 
     def childs(self):
-        childs = []
-        if self.key_valuer:
-            childs.append(self.key_valuer)
-        if self.calculate_valuer:
-            childs.append(self.calculate_valuer)
-        if self.return_valuer:
-            childs.append(self.return_valuer)
-        if self.inherit_valuers:
-            for inherit_valuer in self.inherit_valuers:
-                childs.append(inherit_valuer)
-        return childs
+        if not self.value_valuer:
+            return []
+        return [self.value_valuer]
 
     def get_fields(self):
-        fields = []
-        if self.key_valuer:
-            for field in self.key_valuer.get_fields():
-                fields.append(field)
-        if self.calculate_valuer:
-            for field in self.calculate_valuer.get_fields():
-                fields.append(field)
-        if self.inherit_valuers:
-            for inherit_valuer in self.inherit_valuers:
-                for field in inherit_valuer.get_fields():
-                    fields.append(field)
-        return fields
+        return []
 
     def get_final_filter(self):
-        if self.return_valuer:
-            return self.calculate_valuer.get_final_filter()
-
-        if self.filter:
-            return self.filter
-
-        if self.calculate_valuer:
-            return self.calculate_valuer.get_final_filter()
-        return None
+        if not self.value_valuer:
+            if self.filter:
+                return self.filter
+            return None
+        return self.value_valuer.get_final_filter()
+
+    def require_loaded(self):
+        return False
+
+
+class ContextInheritChildValuer(InheritChildValuer):
+    def __init__(self, *args, **kwargs):
+        self.contexter = kwargs.pop("contexter")
+        self.value_context_id = (id(self), "value")
+        super(ContextInheritChildValuer, self).__init__(*args, **kwargs)
+
+    @property
+    def value(self):
+        try:
+            return self.contexter.values[self.value_context_id]
+        except KeyError:
+            return None
+
+    @value.setter
+    def value(self, v):
+        if v is None:
+            if self.value_context_id in self.contexter.values:
+                self.contexter.values.pop(self.value_context_id)
+            return
+        self.contexter.values[self.value_context_id] = v
```

### Comparing `syncany-0.2.6/syncany/valuers/calculate.py` & `syncany-0.2.7/syncany/valuers/calculate.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*-
 # 18/8/15
 # create by: snower
 
 from .valuer import Valuer
 
+
 class CalculateValuer(Valuer):
     def __init__(self, calculater, args_valuers, return_valuer, inherit_valuers, *args, **kwargs):
         self.calculater = calculater
         self.args_valuers = args_valuers
         self.return_valuer = return_valuer
         self.inherit_valuers = inherit_valuers
         super(CalculateValuer, self).__init__(*args, **kwargs)
@@ -27,52 +28,54 @@
             if valuer.require_loaded():
                 self.wait_loaded = True
                 return
 
     def add_inherit_valuer(self, valuer):
         self.inherit_valuers.append(valuer)
 
-    def clone(self):
+    def clone(self, contexter=None):
         args_valuers = []
         for valuer in self.args_valuers:
-            args_valuers.append(valuer.clone())
-        return_valuer = self.return_valuer.clone() if self.return_valuer else None
-        inherit_valuers = [inherit_valuer.clone() for inherit_valuer in self.inherit_valuers] if self.inherit_valuers else None
+            args_valuers.append(valuer.clone(contexter))
+        return_valuer = self.return_valuer.clone(contexter) if self.return_valuer else None
+        inherit_valuers = [inherit_valuer.clone(contexter) for inherit_valuer in self.inherit_valuers] \
+            if self.inherit_valuers else None
+        if contexter is not None:
+            return ContextCalculateValuer(self.calculater, args_valuers, return_valuer, inherit_valuers,
+                                          self.key, self.filter, from_valuer=self, contexter=contexter)
+        if isinstance(self, ContextCalculateValuer):
+            return ContextCalculateValuer(self.calculater, args_valuers, return_valuer, inherit_valuers,
+                                          self.key, self.filter, from_valuer=self, contexter=self.contexter)
         return self.__class__(self.calculater, args_valuers, return_valuer, inherit_valuers,
                               self.key, self.filter, from_valuer=self)
 
     def fill(self, data):
         if self.inherit_valuers:
             for inherit_valuer in self.inherit_valuers:
                 inherit_valuer.fill(data)
 
         for valuer in self.args_valuers:
             valuer.fill(data)
 
         if not self.wait_loaded:
-            values = []
-            for valuer in self.args_valuers:
-                values.append(valuer.get())
-
-            self.do_filter(self.calculater.calculate(*values))
-            self.return_valuer.fill(self.value)
+            values = [valuer.get() for valuer in self.args_valuers]
+            if self.return_valuer:
+                self.return_valuer.fill(self.do_filter(self.calculater.calculate(*values)))
+            else:
+                self.value = self.do_filter(self.calculater.calculate(*values))
         return self
 
     def get(self):
         if self.wait_loaded:
-            values = []
-            for valuer in self.args_valuers:
-                values.append(valuer.get())
-
-            self.do_filter(self.calculater.calculate(*values))
+            values = [valuer.get() for valuer in self.args_valuers]
             if self.return_valuer:
-                self.return_valuer.fill(self.value)
-
+                return self.return_valuer.fill(self.do_filter(self.calculater.calculate(*values))).get()
+            return self.do_filter(self.calculater.calculate(*values))
         if self.return_valuer:
-            self.value = self.return_valuer.get()
+            return self.return_valuer.get()
         return self.value
 
     def childs(self):
         childs = []
         if self.args_valuers:
             for args_valuer in self.args_valuers:
                 childs.append(args_valuer)
@@ -106,11 +109,31 @@
         for valuer in self.args_valuers:
             filter = valuer.get_final_filter()
             if filter is None:
                 continue
 
             if final_filter is not None and final_filter.__class__ != filter.__class__:
                 return None
-
             final_filter = filter
+        return final_filter
+
 
-        return final_filter
+class ContextCalculateValuer(CalculateValuer):
+    def __init__(self, *args, **kwargs):
+        self.contexter = kwargs.pop("contexter")
+        self.value_context_id = (id(self), "value")
+        super(ContextCalculateValuer, self).__init__(*args, **kwargs)
+
+    @property
+    def value(self):
+        try:
+            return self.contexter.values[self.value_context_id]
+        except KeyError:
+            return None
+
+    @value.setter
+    def value(self, v):
+        if v is None:
+            if self.value_context_id in self.contexter.values:
+                self.contexter.values.pop(self.value_context_id)
+            return
+        self.contexter.values[self.value_context_id] = v
```

### Comparing `syncany-0.2.6/syncany/valuers/call.py` & `syncany-0.2.7/syncany/valuers/call.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*-
 # 2020/7/3
 # create by: snower
 
 from .valuer import Valuer, LoadAllFieldsException
 
+
 class CallReturnManager(object):
     def __init__(self):
         self.datas = {}
 
     def loaded(self, key):
         if not isinstance(key, (int, float, str, bytes)):
             key = "@id_%s" % id(key)
@@ -20,26 +21,27 @@
         if key not in self.datas:
             return None
         return self.datas[key]
 
     def set(self, key, value):
         self.datas[key] = value
 
+
 class CallValuer(Valuer):
+    calculated = False
+    calculated_key = None
+
     def __init__(self, value_valuer, calculate_valuer, return_valuer, inherit_valuers, return_manager, *args, **kwargs):
         self.value_valuer = value_valuer
         self.calculate_valuer = calculate_valuer
         self.return_valuer = return_valuer
         self.inherit_valuers = inherit_valuers
         self.return_manager = return_manager or CallReturnManager()
         super(CallValuer, self).__init__(*args, **kwargs)
 
-        self.calculated = False
-        self.calculated_key = None
-
     def new_init(self):
         super(CallValuer, self).new_init()
         self.value_wait_loaded = False if not self.value_valuer else self.value_valuer.require_loaded()
         self.calculate_wait_loaded = True if not self.value_wait_loaded or not self.return_valuer or \
                                              (self.calculate_valuer and
                                               self.calculate_valuer.require_loaded()) else False
 
@@ -50,19 +52,26 @@
 
     def get_manager(self):
         return self.return_manager
 
     def add_inherit_valuer(self, valuer):
         self.inherit_valuers.append(valuer)
 
-    def clone(self):
-        value_valuer = self.value_valuer.clone()
-        calculate_valuer = self.calculate_valuer.clone() if self.calculate_valuer else None
-        return_valuer = self.return_valuer.clone() if self.return_valuer else None
-        inherit_valuers = [inherit_valuer.clone() for inherit_valuer in self.inherit_valuers] if self.inherit_valuers else None
+    def clone(self, contexter=None):
+        value_valuer = self.value_valuer.clone(contexter)
+        calculate_valuer = self.calculate_valuer.clone(contexter) if self.calculate_valuer else None
+        return_valuer = self.return_valuer.clone(contexter) if self.return_valuer else None
+        inherit_valuers = [inherit_valuer.clone(contexter) for inherit_valuer in self.inherit_valuers] \
+            if self.inherit_valuers else None
+        if contexter is not None:
+            return ContextCallValuer(value_valuer, calculate_valuer, return_valuer, inherit_valuers,
+                                     self.return_manager, self.key, self.filter, from_valuer=self, contexter=contexter)
+        if isinstance(self, ContextCallValuer):
+            return ContextCallValuer(value_valuer, calculate_valuer, return_valuer, inherit_valuers,
+                                     self.return_manager, self.key, self.filter, from_valuer=self, contexter=self.contexter)
         return self.__class__(value_valuer, calculate_valuer, return_valuer, inherit_valuers,
                               self.return_manager, self.key, self.filter, from_valuer=self)
 
     def reinit(self):
         self.calculated = False
         self.calculated_key = None
         return super(CallValuer, self).reinit()
@@ -71,63 +80,67 @@
         if self.inherit_valuers:
             for inherit_valuer in self.inherit_valuers:
                 inherit_valuer.fill(data)
 
         if self.value_valuer:
             self.value_valuer.fill(data)
             if not self.value_wait_loaded:
-                self.value = self.value_valuer.get()
+                value = self.value_valuer.get()
+            else:
+                value = None
         else:
-            self.value = data
+            value = data
 
         if not self.value_wait_loaded:
-            self.calculated_key, self.calculated = self.return_manager.loaded(self.value)
+            self.calculated_key, self.calculated = self.return_manager.loaded(value)
             if not self.calculated:
-                self.calculate_valuer.fill(self.value)
+                self.calculate_valuer.fill(value)
                 if self.return_valuer and not self.calculate_wait_loaded:
-                    self.do_filter(self.calculate_valuer.get())
-                    self.return_manager.set(self.calculated_key, self.value)
-                    self.return_valuer.fill(self.value)
+                    value = self.do_filter(self.calculate_valuer.get())
+                    self.return_manager.set(self.calculated_key, value)
+                    self.return_valuer.fill(value)
             else:
-                self.value = self.return_manager.get(self.calculated_key)
+                value = self.return_manager.get(self.calculated_key)
                 if self.return_valuer:
-                    self.return_valuer.fill(self.value)
-
+                    self.return_valuer.fill(value)
+                else:
+                    self.value = value
         return self
 
     def get(self):
         if self.return_valuer and self.value_wait_loaded:
-            self.value = self.value_valuer.get()
+            value = self.value_valuer.get()
+        else:
+            value = self.value
 
         if self.value_wait_loaded:
-            self.calculated_key, self.calculated = self.return_manager.loaded(self.value)
+            self.calculated_key, self.calculated = self.return_manager.loaded(value)
             if not self.calculated:
-                self.calculate_valuer.fill(self.value)
+                self.calculate_valuer.fill(value)
                 if self.return_valuer and not self.calculate_wait_loaded:
-                    self.do_filter(self.calculate_valuer.get())
-                    self.return_manager.set(self.calculated_key, self.value)
-                    self.return_valuer.fill(self.value)
+                    value = self.do_filter(self.calculate_valuer.get())
+                    self.return_manager.set(self.calculated_key, value)
+                    self.return_valuer.fill(value)
             else:
-                self.value = self.return_manager.get(self.calculated_key)
+                value = self.return_manager.get(self.calculated_key)
                 if self.return_valuer:
-                    self.return_valuer.fill(self.value)
+                    self.return_valuer.fill(value)
 
         if self.calculated:
             if self.return_valuer:
                 return self.return_valuer.get()
-            return self.value
+            return value
 
         if self.calculate_wait_loaded:
-            self.do_filter(self.calculate_valuer.get())
-            self.return_manager.set(self.calculated_key, self.value)
+            value = self.do_filter(self.calculate_valuer.get())
+            self.return_manager.set(self.calculated_key, value)
             if self.return_valuer:
-                self.return_valuer.fill(self.value)
+                self.return_valuer.fill(value)
                 return self.return_valuer.get()
-
-        return self.value
+        return value
 
     def childs(self):
         childs = []
         if self.calculate_valuer:
             childs.append(self.calculate_valuer)
         if self.return_valuer:
             childs.append(self.return_valuer)
@@ -161,8 +174,62 @@
 
         if self.filter:
             return self.filter
 
         if self.calculate_valuer:
             return self.calculate_valuer.get_final_filter()
 
-        return None
+        return None
+
+
+class ContextCallValuer(CallValuer):
+    def __init__(self, *args, **kwargs):
+        self.contexter = kwargs.pop("contexter")
+        self.value_context_id = (id(self), "value")
+        self.calculated_context_id = (id(self), "calculated")
+        self.calculated_key_context_id = (id(self), "calculated_key")
+        super(ContextCallValuer, self).__init__(*args, **kwargs)
+
+    @property
+    def value(self):
+        try:
+            return self.contexter.values[self.value_context_id]
+        except KeyError:
+            return None
+
+    @value.setter
+    def value(self, v):
+        if v is None:
+            if self.value_context_id in self.contexter.values:
+                self.contexter.values.pop(self.value_context_id)
+            return
+        self.contexter.values[self.value_context_id] = v
+
+    @property
+    def calculated(self):
+        try:
+            return self.contexter.values[self.calculated_context_id]
+        except KeyError:
+            return False
+
+    @calculated.setter
+    def calculated(self, v):
+        if v is False:
+            if self.calculated_context_id in self.contexter.values:
+                self.contexter.values.pop(self.calculated_context_id)
+            return
+        self.contexter.values[self.calculated_context_id] = v
+
+    @property
+    def calculated_key(self):
+        try:
+            return self.contexter.values[self.calculated_key_context_id]
+        except KeyError:
+            return None
+
+    @calculated_key.setter
+    def calculated_key(self, v):
+        if v is None:
+            if self.calculated_context_id in self.contexter.values:
+                self.contexter.values.pop(self.calculated_context_id)
+            return
+        self.contexter.values[self.calculated_key_context_id] = v
```

### Comparing `syncany-0.2.6/syncany/valuers/case.py` & `syncany-0.2.7/syncany/valuers/state.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,139 +1,139 @@
 # -*- coding: utf-8 -*-
-# 18/8/8
+# 2021/11/7
 # create by: snower
 
 from .valuer import Valuer
 
-class CaseValuer(Valuer):
-    def __init__(self, case_valuers, default_case_valuer, value_valuer, return_valuer, inherit_valuers, *args, **kwargs):
-        self.case_valuers = case_valuers
-        self.default_case_valuer = default_case_valuer
-        self.value_valuer = value_valuer
+
+class StateValuer(Valuer):
+    def __init__(self, state_value, calculate_valuer, default_valuer, return_valuer, inherit_valuers, *args, **kwargs):
+        self.state_value = state_value
+        self.calculate_valuer = calculate_valuer
+        self.default_valuer = default_valuer
         self.return_valuer = return_valuer
         self.inherit_valuers = inherit_valuers
-        super(CaseValuer, self).__init__(*args, **kwargs)
+        super(StateValuer, self).__init__(*args, **kwargs)
 
     def new_init(self):
-        super(CaseValuer, self).new_init()
-        self.value_wait_loaded = True if self.value_valuer and self.value_valuer.require_loaded() else False
-        self.wait_loaded = True if self.return_valuer and self.return_valuer.require_loaded() else False
+        super(StateValuer, self).new_init()
+        self.calculate_wait_loaded = self.calculate_valuer and self.calculate_valuer.require_loaded()
 
     def clone_init(self, from_valuer):
-        super(CaseValuer, self).clone_init(from_valuer)
-        self.value_wait_loaded = from_valuer.value_wait_loaded
-        self.wait_loaded = from_valuer.wait_loaded
+        super(StateValuer, self).clone_init(from_valuer)
+        self.calculate_wait_loaded = from_valuer.calculate_wait_loaded
 
     def add_inherit_valuer(self, valuer):
         self.inherit_valuers.append(valuer)
 
-    def clone(self):
-        case_valuers = {}
-        for name, valuer in self.case_valuers.items():
-            case_valuers[name] = valuer.clone()
-        default_case_valuer = self.default_case_valuer.clone() if self.default_case_valuer else None
-        value_valuer = self.value_valuer.clone() if self.value_valuer else None
-        return_valuer = self.return_valuer.clone() if self.return_valuer else None
-        inherit_valuers = [inherit_valuer.clone() for inherit_valuer in self.inherit_valuers] if self.inherit_valuers else None
-        return self.__class__(case_valuers, default_case_valuer, value_valuer, return_valuer, inherit_valuers,
+    def clone(self, contexter=None):
+        calculate_valuer = self.calculate_valuer.clone(contexter) if self.calculate_valuer else None
+        default_valuer = self.default_valuer.clone(contexter) if self.default_valuer else None
+        return_valuer = self.return_valuer.clone(contexter) if self.return_valuer else None
+        inherit_valuers = [inherit_valuer.clone(contexter) for inherit_valuer in self.inherit_valuers] \
+            if self.inherit_valuers else None
+        if contexter is not None:
+            return ContextStateValuer(self.state_value, calculate_valuer, default_valuer, return_valuer, inherit_valuers,
+                                      self.key, self.filter, from_valuer=self, contexter=contexter)
+        if isinstance(self, ContextStateValuer):
+            return ContextStateValuer(self.state_value, calculate_valuer, default_valuer, return_valuer, inherit_valuers,
+                                      self.key, self.filter, from_valuer=self, contexter=self.contexter)
+        return self.__class__(self.state_value, calculate_valuer, default_valuer, return_valuer, inherit_valuers,
                               self.key, self.filter, from_valuer=self)
 
     def fill(self, data):
         if self.inherit_valuers:
             for inherit_valuer in self.inherit_valuers:
                 inherit_valuer.fill(data)
 
-        if self.value_valuer:
-            self.value_valuer.fill(data)
-            if self.value_wait_loaded:
-                for case_key, case_valuer in self.case_valuers.items():
-                    case_valuer.fill(data)
-                if self.default_case_valuer:
-                    self.default_case_valuer.fill(data)
-                return self
-            self.value = self.value_valuer.get()
+        if self.calculate_valuer:
+            self.calculate_valuer.fill(self.state_value)
+            if not self.calculate_wait_loaded:
+                value = self.calculate_valuer.get()
+                if not value and self.default_valuer:
+                    self.default_valuer.fill(self.state_value)
+                    value = self.default_valuer.get()
+                value = self.do_filter(value)
+                if self.return_valuer:
+                    self.return_valuer.fill(value)
+                else:
+                    self.value = value
+        elif self.return_valuer:
+            value = self.do_filter(self.state_value)
+            final_filter = self.return_valuer.get_final_filter()
+            if final_filter:
+                value = final_filter.filter(value)
+            self.return_valuer.fill(value)
         else:
-            self.value = data
-
-        if self.value in self.case_valuers:
-            self.case_valuers[self.value].fill(data)
-        elif self.default_case_valuer:
-            self.default_case_valuer.fill(data)
-
-        if self.wait_loaded:
-            if self.value in self.case_valuers:
-                self.do_filter(self.case_valuers[self.value].get())
-            elif self.default_case_valuer:
-                self.do_filter(self.default_case_valuer.get())
-            self.return_valuer.fill(self.value)
+            self.value = self.do_filter(self.state_value)
         return self
 
     def get(self):
-        if self.value_valuer and self.value_wait_loaded:
-            self.value = self.value_valuer.get()
-        elif self.wait_loaded:
-            return self.return_valuer.get()
-
-        if self.value in self.case_valuers:
-            self.do_filter(self.case_valuers[self.value].get())
-        elif self.default_case_valuer:
-            self.do_filter(self.default_case_valuer.get())
-
+        if self.calculate_valuer:
+            if self.calculate_wait_loaded:
+                value = self.calculate_valuer.get()
+                if not value and self.default_valuer:
+                    self.default_valuer.fill(self.state_value)
+                    value = self.default_valuer.get()
+                value = self.do_filter(value)
+                if self.return_valuer:
+                    return self.return_valuer.fill(value).get()
+                return value
         if self.return_valuer:
-            self.return_valuer.fill(self.value)
-            self.value = self.return_valuer.get()
+            return self.return_valuer.get()
         return self.value
 
     def childs(self):
-        childs = list(self.case_valuers.values())
-        if self.default_case_valuer:
-            childs.append(self.default_case_valuer)
-        if self.value_valuer:
-            childs.append(self.value_valuer)
+        childs = []
+        if self.calculate_valuer:
+            childs.append(self.calculate_valuer)
+        if self.default_valuer:
+            childs.append(self.default_valuer)
         if self.return_valuer:
             childs.append(self.return_valuer)
         if self.inherit_valuers:
             for inherit_valuer in self.inherit_valuers:
                 childs.append(inherit_valuer)
         return childs
 
     def get_fields(self):
-        fields = self.value_valuer.get_fields() if self.value_valuer else [self.key]
-        for _, valuer in self.case_valuers.items():
-            for field in valuer.get_fields():
-                fields.append(field)
-
-        if self.default_case_valuer:
-            for field in self.default_case_valuer.get_fields():
-                fields.append(field)
-
+        fields = []
         if self.inherit_valuers:
             for inherit_valuer in self.inherit_valuers:
                 for field in inherit_valuer.get_fields():
                     fields.append(field)
         return fields
 
     def get_final_filter(self):
         if self.return_valuer:
-            return self.return_valuer.get_final_filter()
+            return self.calculate_valuer.get_final_filter()
 
         if self.filter:
             return self.filter
 
-        final_filter = None
-        for _, valuer in self.case_valuers.items():
-            filter = valuer.get_final_filter()
-            if filter is None:
-                continue
-
-            if final_filter is not None and final_filter.__class__ != filter.__class__:
-                return None
-            final_filter = filter
-
-        if self.default_case_valuer:
-            filter = self.default_case_valuer.get_final_filter()
-            if filter is None:
-                return final_filter
-
-            if final_filter is not None and final_filter.__class__ != filter.__class__:
-                return None
-        return final_filter
+        if self.calculate_valuer:
+            return self.calculate_valuer.get_final_filter()
+        if self.default_valuer:
+            return self.default_valuer.get_final_filter()
+        return None
+
+
+class ContextStateValuer(StateValuer):
+    def __init__(self, *args, **kwargs):
+        self.contexter = kwargs.pop("contexter")
+        self.value_context_id = (id(self), "value")
+        super(ContextStateValuer, self).__init__(*args, **kwargs)
+
+    @property
+    def value(self):
+        try:
+            return self.contexter.values[self.value_context_id]
+        except KeyError:
+            return None
+
+    @value.setter
+    def value(self, v):
+        if v is None:
+            if self.value_context_id in self.contexter.values:
+                self.contexter.values.pop(self.value_context_id)
+            return
+        self.contexter.values[self.value_context_id] = v
```

### Comparing `syncany-0.2.6/syncany/valuers/condition.py` & `syncany-0.2.7/syncany/valuers/condition.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 # 2021/2/21
 # create by: snower
 
 
 from .valuer import Valuer
 
+
 class IfValuer(Valuer):
     def __init__(self, true_valuer, false_valuer, value_valuer, return_valuer, inherit_valuers, *args, **kwargs):
         self.true_valuer = true_valuer
         self.false_valuer = false_valuer
         self.value_valuer = value_valuer
         self.return_valuer = return_valuer
         self.inherit_valuers = inherit_valuers
@@ -23,20 +24,27 @@
         super(IfValuer, self).clone_init(from_valuer)
         self.value_wait_loaded = from_valuer.value_wait_loaded
         self.wait_loaded = from_valuer.wait_loaded
 
     def add_inherit_valuer(self, valuer):
         self.inherit_valuers.append(valuer)
 
-    def clone(self):
-        true_valuer = self.true_valuer.clone()
-        false_valuer = self.false_valuer.clone() if self.false_valuer else None
-        value_valuer = self.value_valuer.clone() if self.value_valuer else None
-        return_valuer = self.return_valuer.clone() if self.return_valuer else None
-        inherit_valuers = [inherit_valuer.clone() for inherit_valuer in self.inherit_valuers] if self.inherit_valuers else None
+    def clone(self, contexter=None):
+        true_valuer = self.true_valuer.clone(contexter)
+        false_valuer = self.false_valuer.clone(contexter) if self.false_valuer else None
+        value_valuer = self.value_valuer.clone(contexter) if self.value_valuer else None
+        return_valuer = self.return_valuer.clone(contexter) if self.return_valuer else None
+        inherit_valuers = [inherit_valuer.clone(contexter) for inherit_valuer in self.inherit_valuers] \
+            if self.inherit_valuers else None
+        if contexter is not None:
+            return ContextIfValuer(true_valuer, false_valuer, value_valuer, return_valuer, inherit_valuers,
+                                   self.key, self.filter, from_valuer=self, contexter=contexter)
+        if isinstance(self, ContextIfValuer):
+            return ContextIfValuer(true_valuer, false_valuer, value_valuer, return_valuer, inherit_valuers,
+                                   self.key, self.filter, from_valuer=self, contexter=self.contexter)
         return self.__class__(true_valuer, false_valuer, value_valuer, return_valuer, inherit_valuers,
                               self.key, self.filter, from_valuer=self)
 
     def fill(self, data):
         if self.inherit_valuers:
             for inherit_valuer in self.inherit_valuers:
                 inherit_valuer.fill(data)
@@ -44,45 +52,52 @@
         if self.value_valuer:
             self.value_valuer.fill(data)
             if self.value_wait_loaded:
                 self.true_valuer.fill(data)
                 if self.false_valuer:
                     self.false_valuer.fill(data)
                 return self
-            self.value = self.value_valuer.get()
+            value = self.value_valuer.get()
         else:
-            self.value = data
+            value = data
+
+        if self.wait_loaded:
+            if value:
+                value = self.do_filter(self.true_valuer.fill(data).get())
+            elif self.false_valuer:
+                value = self.do_filter(self.false_valuer.fill(data).get())
+            else:
+                value = self.do_filter(None)
+            self.return_valuer.fill(value)
+            return self
 
-        if self.value:
+        if value:
             self.true_valuer.fill(data)
         elif self.false_valuer:
             self.false_valuer.fill(data)
-
-        if self.wait_loaded:
-            if self.value:
-                self.do_filter(self.true_valuer.get())
-            elif self.false_valuer:
-                self.do_filter(self.false_valuer.get())
+        self.value = value
         return self
 
     def get(self):
         if self.value_valuer and self.value_wait_loaded:
-            self.value = self.value_valuer.get()
+            value = self.value_valuer.get()
         elif self.wait_loaded:
             return self.return_valuer.get()
+        else:
+            value = self.value
 
-        if self.value:
-            self.do_filter(self.true_valuer.get())
+        if value:
+            value = self.do_filter(self.true_valuer.get())
         elif self.false_valuer:
-            self.do_filter(self.false_valuer.get())
-
+            value = self.do_filter(self.false_valuer.get())
+        else:
+            value = self.do_filter(None)
         if self.return_valuer:
-            self.return_valuer.fill(self.value)
-            self.value = self.return_valuer.get()
-        return self.value
+            return self.return_valuer.fill(value).get()
+        return value
 
     def childs(self):
         childs = [self.true_valuer]
         if self.false_valuer:
             childs.append(self.false_valuer)
         if self.value_valuer:
             childs.append(self.value_valuer)
@@ -119,8 +134,30 @@
         if self.false_valuer:
             false_filter = self.false_valuer.get_final_filter()
             if false_filter is None:
                 return true_filter
 
             if false_filter is not None and true_filter.__class__ != false_filter.__class__:
                 return None
-        return true_filter
+        return true_filter
+
+
+class ContextIfValuer(IfValuer):
+    def __init__(self, *args, **kwargs):
+        self.contexter = kwargs.pop("contexter")
+        self.value_context_id = (id(self), "value")
+        super(ContextIfValuer, self).__init__(*args, **kwargs)
+
+    @property
+    def value(self):
+        try:
+            return self.contexter.values[self.value_context_id]
+        except KeyError:
+            return None
+
+    @value.setter
+    def value(self, v):
+        if v is None:
+            if self.value_context_id in self.contexter.values:
+                self.contexter.values.pop(self.value_context_id)
+            return
+        self.contexter.values[self.value_context_id] = v
```

### Comparing `syncany-0.2.6/syncany/valuers/db_join.py` & `syncany-0.2.7/syncany/valuers/let.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,130 +1,144 @@
 # -*- coding: utf-8 -*-
-# 18/8/6
+# 2020/7/1
 # create by: snower
 
-from .data import Valuer
+from .valuer import Valuer
 
 
-class DBJoinValuer(Valuer):
-    def __init__(self, loader, foreign_keys, foreign_filters, args_valuers, return_valuer, inherit_valuers, *args, **kwargs):
-        self.loader = loader
-        self.foreign_keys = foreign_keys
-        self.args_valuers = args_valuers
+class LetValuer(Valuer):
+    filled_data = None
+
+    def __init__(self, key_valuer, return_valuer, inherit_valuers, *args, **kwargs):
+        self.key_valuer = key_valuer
         self.return_valuer = return_valuer
         self.inherit_valuers = inherit_valuers
-        self.foreign_filters = foreign_filters
-        super(DBJoinValuer, self).__init__(*args, **kwargs)
+        super(LetValuer, self).__init__(*args, **kwargs)
+
+    def new_init(self):
+        super(LetValuer, self).new_init()
+        self.wait_loaded = True if not self.return_valuer else False
+        if self.return_valuer:
+            self.check_wait_loaded()
 
-        self.matcher = None
-        self.is_group_matcher = False
+    def clone_init(self, from_valuer):
+        super(LetValuer, self).clone_init(from_valuer)
+        self.wait_loaded = from_valuer.wait_loaded
+
+    def check_wait_loaded(self):
+        if self.key_valuer.require_loaded():
+            self.wait_loaded = True
 
     def add_inherit_valuer(self, valuer):
         self.inherit_valuers.append(valuer)
 
-    def clone(self):
-        args_valuers = [args_valuer.clone() for args_valuer in self.args_valuers] if self.args_valuers else None
-        return_valuer = self.return_valuer.clone()
-        inherit_valuers = [inherit_valuer.clone() for inherit_valuer in self.inherit_valuers] if self.inherit_valuers else None
-        return self.__class__(self.loader, self.foreign_keys, self.foreign_filters,
-                              args_valuers, return_valuer, inherit_valuers, self.key, self.filter, from_valuer=self)
+    def clone(self, contexter=None):
+        key_valuer = self.key_valuer.clone(contexter) if self.key_valuer else None
+        return_valuer = self.return_valuer.clone(contexter) if self.return_valuer else None
+        inherit_valuers = [inherit_valuer.clone(contexter) for inherit_valuer in self.inherit_valuers] \
+            if self.inherit_valuers else None
+        if contexter is not None:
+            return ContextLetValuer(key_valuer, return_valuer, inherit_valuers,
+                                    self.key, self.filter, from_valuer=self, contexter=contexter)
+        if isinstance(self, ContextLetValuer):
+            return ContextLetValuer(key_valuer, return_valuer, inherit_valuers,
+                                    self.key, self.filter, from_valuer=self, contexter=self.contexter)
+        return self.__class__(key_valuer, return_valuer, inherit_valuers,
+                              self.key, self.filter, from_valuer=self)
 
     def reinit(self):
-        self.matcher = None
-        self.is_group_matcher = False
-        return super(DBJoinValuer, self).reinit()
+        self.filled_data = None
+        return super(LetValuer, self).reinit()
 
     def fill(self, data):
         if self.inherit_valuers:
             for inherit_valuer in self.inherit_valuers:
                 inherit_valuer.fill(data)
 
-        if self.args_valuers:
-            join_values = []
-            for args_valuer in self.args_valuers:
-                args_valuer.fill(data)
-                join_values.append(args_valuer.get())
+        self.key_valuer.fill(data)
+
+        if not self.wait_loaded:
+            self.key = self.key_valuer.get()
+            super(LetValuer, self).fill(data)
+            if self.return_valuer:
+                self.return_valuer.fill(super(LetValuer, self).get())
         else:
-            if self.key:
-                super(DBJoinValuer, self).fill(data)
-            join_values = [self.value for _ in self.foreign_keys]
-
-        max_value_size = max([len(join_value) if isinstance(join_value, list) else 1 for join_value in join_values])
-        if max_value_size > 1:
-            self.matcher = self.loader.create_group_macther(self.return_valuer)
-            self.is_group_matcher = True
-            for i in range(max_value_size):
-                ds, has_value = [], False
-                for join_value in join_values:
-                    if not isinstance(join_value, list):
-                        ds.append(join_value)
-                        has_value = True if join_value is not None else has_value
-                    else:
-                        ds.append(join_value[i] if i < len(join_value) else None)
-                        has_value = True if i < len(join_value) else has_value
-                if not has_value:
-                    continue
-                matcher = self.loader.create_macther(self.foreign_keys, ds)
-                return_valuer = DBJoinGroupMatchValuer(self.matcher, "*")
-                matcher.add_valuer(return_valuer)
-                self.matcher.add_valuer(return_valuer)
-        elif join_values and any([join_value is not None for join_value in join_values]):
-            self.matcher = self.loader.create_macther(self.foreign_keys, join_values)
-            self.matcher.add_valuer(self.return_valuer)
-        self.loader.try_load()
+            self.filled_data = data
         return self
 
     def get(self):
-        self.loader.load()
-        if self.is_group_matcher:
-            self.matcher.get()
-        return self.return_valuer.get()
+        if self.wait_loaded:
+            self.key = self.key_valuer.get()
+            super(LetValuer, self).fill(self.filled_data)
+            self.filled_data = None
+            if self.return_valuer:
+                self.return_valuer.fill(super(LetValuer, self).get())
+                return self.return_valuer.get()
+        return super(LetValuer, self).get()
 
     def childs(self):
-        valuers = []
-        if self.args_valuers:
-            for args_valuer in self.args_valuers:
-                valuers.append(args_valuer)
+        childs = []
+        if self.key_valuer:
+            childs.append(self.key_valuer)
         if self.return_valuer:
-            valuers.append(self.return_valuer)
+            childs.append(self.return_valuer)
         if self.inherit_valuers:
             for inherit_valuer in self.inherit_valuers:
-                valuers.append(inherit_valuer)
-        return valuers
+                childs.append(inherit_valuer)
+        return childs
 
     def get_fields(self):
         fields = []
-
-        if self.args_valuers:
-            for args_valuer in self.args_valuers:
-                for field in args_valuer.get_fields():
-                    fields.append(field)
+        for field in self.key_valuer.get_fields():
+            fields.append(field)
 
         if self.inherit_valuers:
             for inherit_valuer in self.inherit_valuers:
                 for field in inherit_valuer.get_fields():
                     fields.append(field)
         return fields
 
     def get_final_filter(self):
         if self.return_valuer:
             return self.return_valuer.get_final_filter()
-        return None
-
-    def require_loaded(self):
-        return True
-
 
-class DBJoinGroupMatchValuer(Valuer):
-    def __init__(self, matcher, *args, **kwargs):
-        self.matcher = matcher
-        self.loaded = False
-        super(DBJoinGroupMatchValuer, self).__init__(*args, **kwargs)
+        if self.filter:
+            return self.filter
+        return None
 
-    def clone(self):
-        return self.__class__(self.matcher, self.key, self.filter)
 
-    def fill(self, data):
-        super(DBJoinGroupMatchValuer, self).fill(data)
-        self.loaded = None if data is None else True
-        self.matcher.fill(self, data)
-        return self
+class ContextLetValuer(LetValuer):
+    def __init__(self, *args, **kwargs):
+        self.contexter = kwargs.pop("contexter")
+        self.value_context_id = (id(self), "value")
+        self.filled_data_context_id = (id(self), "filled_data")
+        super(ContextLetValuer, self).__init__(*args, **kwargs)
+
+    @property
+    def value(self):
+        try:
+            return self.contexter.values[self.value_context_id]
+        except KeyError:
+            return None
+
+    @value.setter
+    def value(self, v):
+        if v is None:
+            if self.value_context_id in self.contexter.values:
+                self.contexter.values.pop(self.value_context_id)
+            return
+        self.contexter.values[self.value_context_id] = v
+
+    @property
+    def filled_data(self):
+        try:
+            return self.contexter.values[self.filled_data_context_id]
+        except KeyError:
+            return None
+
+    @filled_data.setter
+    def filled_data(self, v):
+        if v is None:
+            if self.filled_data_context_id in self.contexter.values:
+                self.contexter.values.pop(self.filled_data_context_id)
+            return
+        self.contexter.values[self.filled_data_context_id] = v
```

### Comparing `syncany-0.2.6/syncany/valuers/generator.py` & `syncany-0.2.7/syncany/valuers/assign.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,164 +1,127 @@
 # -*- coding: utf-8 -*-
-# 2020/7/2
+# 2020/7/3
 # create by: snower
 
-import types
-from .valuer import Valuer, LoadAllFieldsException
+from .valuer import Valuer
 
-class YieldValuer(Valuer):
-    def __init__(self, value_valuer, return_valuer, inherit_valuers, *args, **kwargs):
-        self.value_valuer = value_valuer
+
+class AssignValuer(Valuer):
+    def __init__(self, global_value, calculate_valuer, return_valuer, inherit_valuers, *args, **kwargs):
+        self.global_value = global_value
+        self.calculate_valuer = calculate_valuer
         self.return_valuer = return_valuer
         self.inherit_valuers = inherit_valuers
-        super(YieldValuer, self).__init__(*args, **kwargs)
-
-        self.iter_valuers = []
-        self.iter_datas = []
+        super(AssignValuer, self).__init__(*args, **kwargs)
 
     def new_init(self):
-        super(YieldValuer, self).new_init()
-        self.wait_loaded = True if not self.return_valuer else False
-        if self.return_valuer:
-            self.check_wait_loaded()
+        super(AssignValuer, self).new_init()
+        self.calculate_wait_loaded = self.calculate_valuer and self.calculate_valuer.require_loaded()
 
     def clone_init(self, from_valuer):
-        super(YieldValuer, self).clone_init(from_valuer)
-        self.wait_loaded = from_valuer.wait_loaded
-
-    def check_wait_loaded(self):
-        if self.value_valuer and self.value_valuer.require_loaded():
-            self.wait_loaded = True
+        super(AssignValuer, self).clone_init(from_valuer)
+        self.calculate_wait_loaded = from_valuer.calculate_wait_loaded
 
     def add_inherit_valuer(self, valuer):
         self.inherit_valuers.append(valuer)
 
-    def clone(self):
-        value_valuer = self.value_valuer.clone() if self.value_valuer else None
-        return_valuer = self.return_valuer.clone() if self.return_valuer else None
-        inherit_valuers = [inherit_valuer.clone() for inherit_valuer in self.inherit_valuers] if self.inherit_valuers else None
-        return self.__class__(value_valuer, return_valuer, inherit_valuers,
+    def clone(self, contexter=None):
+        calculate_valuer = self.calculate_valuer.clone(contexter) if self.calculate_valuer else None
+        return_valuer = self.return_valuer.clone(contexter) if self.return_valuer else None
+        inherit_valuers = [inherit_valuer.clone(contexter) for inherit_valuer in self.inherit_valuers] \
+            if self.inherit_valuers else None
+        if contexter is not None:
+            return ContextAssignValuer(self.global_value, calculate_valuer, return_valuer, inherit_valuers,
+                                       self.key, self.filter, from_valuer=self, contexter=contexter)
+        if isinstance(self, ContextAssignValuer):
+            return ContextAssignValuer(self.global_value, calculate_valuer, return_valuer, inherit_valuers,
+                                       self.key, self.filter, from_valuer=self, contexter=self.contexter)
+        return self.__class__(self.global_value, calculate_valuer, return_valuer, inherit_valuers,
                               self.key, self.filter, from_valuer=self)
 
-    def reinit(self):
-        self.iter_valuers = []
-        self.iter_datas = []
-        return super(YieldValuer, self).reinit()
-
     def fill(self, data):
         if self.inherit_valuers:
             for inherit_valuer in self.inherit_valuers:
                 inherit_valuer.fill(data)
 
-        if self.value_valuer:
-            self.value_valuer.fill(data)
-
-        if self.return_valuer and not self.wait_loaded:
-            if self.value_valuer:
-                data = self.value_valuer.get()
-
-            if isinstance(data, list):
-                for d in data:
-                    return_valuer = self.return_valuer.clone()
-                    return_valuer.fill(self.do_filter(d))
-                    self.iter_valuers.append(return_valuer)
-            else:
-                return_valuer = self.return_valuer.clone()
-                return_valuer.fill(self.do_filter(data))
-                self.iter_valuers.append(return_valuer)
-            return self
-
-        if not self.value_valuer:
-            if isinstance(data, list):
-                self.iter_datas = [self.do_filter(d) for d in data]
-            else:
-                self.iter_datas = [self.do_filter(data)]
+        if self.calculate_valuer:
+            self.calculate_valuer.fill(self.global_value)
+            if not self.calculate_wait_loaded:
+                value = self.do_filter(self.calculate_valuer.get())
+                self.global_value[self.key] = value
+                if self.return_valuer:
+                    self.return_valuer.fill(value)
+                else:
+                    self.value = value
+        elif self.return_valuer:
+            value = self.do_filter(self.global_value.get(self.key, None))
+            final_filter = self.return_valuer.get_final_filter()
+            if final_filter:
+                value = final_filter.filter(value)
+            self.return_valuer.fill(value)
+        else:
+            self.value = self.do_filter(self.global_value.get(self.key, None))
         return self
 
     def get(self):
+        if self.calculate_valuer:
+            if self.calculate_wait_loaded:
+                value = self.do_filter(self.calculate_valuer.get())
+                self.global_value[self.key] = value
+                if self.return_valuer:
+                    return self.return_valuer.fill(value).get()
+                return value
         if self.return_valuer:
-            if self.wait_loaded:
-                if self.value_valuer:
-                    data = self.value_valuer.get()
-                else:
-                    data = self.iter_datas
-
-                if isinstance(data, list):
-                    for d in data:
-                        return_valuer = self.return_valuer.clone()
-                        return_valuer.fill(self.do_filter(d))
-                        self.iter_valuers.append(return_valuer)
-                else:
-                    return_valuer = self.return_valuer.clone()
-                    return_valuer.fill(self.do_filter(data))
-                    self.iter_valuers.append(return_valuer)
-
-            self.iter_datas = []
-            for valuer in self.iter_valuers:
-                self.iter_datas.append(valuer.get())
-        else:
-            if self.value_valuer:
-                data = self.value_valuer.get()
-                if isinstance(data, list):
-                    self.iter_datas = [self.do_filter(d) for d in data]
-                else:
-                    self.iter_datas = [self.do_filter(data)]
-
-        def gen_iter():
-            gdata = yield None
-            for data in self.iter_datas:
-                if isinstance(data, types.FunctionType):
-                    try:
-                        child_data = data(gdata)
-                        gdata = yield child_data
-                    except StopIteration:
-                        pass
-                elif isinstance(data, types.GeneratorType):
-                    while True:
-                        try:
-                            child_data = data.send(gdata)
-                            gdata = yield child_data
-                        except StopIteration:
-                            break
-                else:
-                    gdata = yield data
-        g = gen_iter()
-        g.send(None)
-        return g
+            return self.return_valuer.get()
+        return self.value
 
     def childs(self):
         childs = []
-        if self.value_valuer:
-            childs.append(self.value_valuer)
+        if self.calculate_valuer:
+            childs.append(self.calculate_valuer)
         if self.return_valuer:
             childs.append(self.return_valuer)
         if self.inherit_valuers:
             for inherit_valuer in self.inherit_valuers:
                 childs.append(inherit_valuer)
         return childs
 
     def get_fields(self):
-        is_pass, fields = False, []
-        try:
-            if self.value_valuer:
-                for field in self.value_valuer.get_fields():
-                    fields.append(field)
-        except LoadAllFieldsException:
-            is_pass = True
-
-        if (not self.value_valuer or is_pass) and self.return_valuer:
-            for field in self.return_valuer.get_fields():
-                fields.append(field)
-
+        fields = []
         if self.inherit_valuers:
             for inherit_valuer in self.inherit_valuers:
                 for field in inherit_valuer.get_fields():
                     fields.append(field)
         return fields
 
     def get_final_filter(self):
         if self.return_valuer:
-            return self.return_valuer.get_final_filter()
+            return self.calculate_valuer.get_final_filter()
 
         if self.filter:
             return self.filter
-        return None
+
+        if self.calculate_valuer:
+            return self.calculate_valuer.get_final_filter()
+        return None
+
+
+class ContextAssignValuer(AssignValuer):
+    def __init__(self, *args, **kwargs):
+        self.contexter = kwargs.pop("contexter")
+        self.value_context_id = (id(self), "value")
+        super(ContextAssignValuer, self).__init__(*args, **kwargs)
+
+    @property
+    def value(self):
+        try:
+            return self.contexter.values[self.value_context_id]
+        except KeyError:
+            return None
+
+    @value.setter
+    def value(self, v):
+        if v is None:
+            if self.value_context_id in self.contexter.values:
+                self.contexter.values.pop(self.value_context_id)
+            return
+        self.contexter.values[self.value_context_id] = v
```

### Comparing `syncany-0.2.6/syncany/valuers/inherit.py` & `syncany-0.2.7/syncany/valuers/db_load.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,113 +1,91 @@
 # -*- coding: utf-8 -*-
-# 2020/6/28
+# 18/8/6
 # create by: snower
 
-import weakref
-from .valuer import Valuer
+from .data import Valuer
 
-class InheritValuer(Valuer):
-    def __init__(self, value_valuer, *args, **kwargs):
-        self.child_valuer = InheritChildValuer(self, value_valuer, *args, **kwargs)
-        self.value_valuer = value_valuer
-        super(InheritValuer, self).__init__(*args, **kwargs)
-
-        self.filled = False
-        self.cloned_child_valuer = None
-
-    def get_inherit_child_valuer(self):
-        return self.child_valuer
-
-    def clone(self):
-        if self.filled:
-            return self
-
-        if self.child_valuer.cloned_inherit_valuer:
-            inherit_valuer = self.child_valuer.cloned_inherit_valuer
-            self.child_valuer.cloned_inherit_valuer = None
-            return inherit_valuer
-
-        value_valuer = self.value_valuer.clone() if self.value_valuer else None
-        inherit_valuer = self.__class__(value_valuer, self.key, self.filter, from_valuer=self)
-        self.cloned_child_valuer = inherit_valuer.get_inherit_child_valuer()
-        return inherit_valuer
-
-    def reinit(self):
-        self.filled = False
-        self.cloned_child_valuer = None
-        return super(InheritValuer, self).reinit()
+
+class DBLoadValuer(Valuer):
+    def __init__(self, loader, foreign_keys, foreign_filters, return_valuer, inherit_valuers, *args, **kwargs):
+        self.loader = loader
+        self.foreign_keys = foreign_keys
+        self.return_valuer = return_valuer
+        self.inherit_valuers = inherit_valuers
+        self.foreign_filters = foreign_filters
+        super(DBLoadValuer, self).__init__(*args, **kwargs)
+
+    def add_inherit_valuer(self, valuer):
+        self.inherit_valuers.append(valuer)
+
+    def clone(self, contexter=None):
+        return_valuer = self.return_valuer.clone(contexter)
+        inherit_valuers = [inherit_valuer.clone(contexter) for inherit_valuer in self.inherit_valuers] \
+            if self.inherit_valuers else None
+        if contexter is not None:
+            return ContextDBLoadValuer(self.loader, self.foreign_keys, self.foreign_filters,
+                                       return_valuer, inherit_valuers, self.key, self.filter, from_valuer=self,
+                                       contexter=contexter)
+        if isinstance(self, ContextDBLoadValuer):
+            return ContextDBLoadValuer(self.loader, self.foreign_keys, self.foreign_filters,
+                                       return_valuer, inherit_valuers, self.key, self.filter, from_valuer=self,
+                                       contexter=self.contexter)
+        return self.__class__(self.loader, self.foreign_keys, self.foreign_filters,
+                              return_valuer, inherit_valuers, self.key, self.filter, from_valuer=self)
 
     def fill(self, data):
-        if self.value_valuer:
-            self.value_valuer.fill(self.do_filter(data))
-        else:
-            super(InheritValuer, self).fill(data)
-        self.filled = True
+        if self.inherit_valuers:
+            for inherit_valuer in self.inherit_valuers:
+                inherit_valuer.fill(data)
+
+        self.return_valuer.fill(self.loader.get())
         return self
 
     def get(self):
-        return None
+        return self.return_valuer.get()
 
     def childs(self):
-        if not self.value_valuer:
-            return []
-        return [self.value_valuer]
+        valuers = []
+        if self.return_valuer:
+            valuers.append(self.return_valuer)
+        if self.inherit_valuers:
+            for inherit_valuer in self.inherit_valuers:
+                valuers.append(inherit_valuer)
+        return valuers
 
     def get_fields(self):
-        if not self.value_valuer:
-            return []
-        return self.value_valuer.get_fields()
+        fields = []
+        if self.inherit_valuers:
+            for inherit_valuer in self.inherit_valuers:
+                for field in inherit_valuer.get_fields():
+                    fields.append(field)
+        return fields
 
     def get_final_filter(self):
+        if self.return_valuer:
+            return self.return_valuer.get_final_filter()
         return None
 
+    def require_loaded(self):
+        return True
 
-class InheritChildValuer(Valuer):
-    def __init__(self, inherit_valuer, value_valuer, *args, **kwargs):
-        self.inherit_valuer = weakref.proxy(inherit_valuer)
-        self.value_valuer = value_valuer
-        super(InheritChildValuer, self).__init__(*args, **kwargs)
-
-        self.cloned_inherit_valuer = None
-
-    def clone(self):
-        if self.inherit_valuer.filled:
-            return self
-
-        if self.inherit_valuer.cloned_child_valuer:
-            child_valuer = self.inherit_valuer.cloned_child_valuer
-            self.inherit_valuer.cloned_child_valuer = None
-            return child_valuer
-
-        value_valuer = self.value_valuer.clone() if self.value_valuer else None
-        self.cloned_inherit_valuer = InheritValuer(value_valuer, self.key, self.filter, from_valuer=self)
-        return self.cloned_inherit_valuer.get_inherit_child_valuer()
-
-    def reinit(self):
-        self.cloned_inherit_valuer = None
-        return super(InheritChildValuer, self).reinit()
-
-    def fill(self, data):
-        return self
-
-    def get(self):
-        if self.value_valuer:
-            return self.value_valuer.get()
-        return self.value
-
-    def childs(self):
-        if not self.value_valuer:
-            return []
-        return [self.value_valuer]
 
-    def get_fields(self):
-        return []
-
-    def get_final_filter(self):
-        if not self.value_valuer:
-            if self.filter:
-                return self.filter
+class ContextDBLoadValuer(DBLoadValuer):
+    def __init__(self, *args, **kwargs):
+        self.contexter = kwargs.pop("contexter")
+        self.value_context_id = (id(self), "value")
+        super(ContextDBLoadValuer, self).__init__(*args, **kwargs)
+
+    @property
+    def value(self):
+        try:
+            return self.contexter.values[self.value_context_id]
+        except KeyError:
             return None
-        return self.value_valuer.get_final_filter()
 
-    def require_loaded(self):
-        return False
+    @value.setter
+    def value(self, v):
+        if v is None:
+            if self.value_context_id in self.contexter.values:
+                self.contexter.values.pop(self.value_context_id)
+            return
+        self.contexter.values[self.value_context_id] = v
```

### Comparing `syncany-0.2.6/syncany/valuers/loop.py` & `syncany-0.2.7/syncany/valuers/loop.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 # 2021/2/5
 # create by: snower
 
 import types
 from .valuer import Valuer, LoadAllFieldsException
 from ..filters import ArrayFilter
 
+
 range_type = type(range(1))
 
+
 class BreakReturn(Exception):
     NULL = object()
 
     def __init__(self, value=NULL, *args, **kwargs):
         super(BreakReturn, self).__init__(*args, **kwargs)
         self.value = value
 
@@ -27,14 +29,16 @@
         self.value = value
 
     def get(self):
         return self.value
 
 
 class ForeachValuer(Valuer):
+    calculated_values = None
+
     def __init__(self, value_valuer, calculate_valuer, return_valuer, inherit_valuers, *args, **kwargs):
         self.value_valuer = value_valuer
         self.calculate_valuer = calculate_valuer
         self.return_valuer = return_valuer
         self.inherit_valuers = inherit_valuers
         super(ForeachValuer, self).__init__(*args, **kwargs)
 
@@ -51,19 +55,26 @@
         super(ForeachValuer, self).clone_init(from_valuer)
         self.value_wait_loaded = from_valuer.value_wait_loaded
         self.calculate_wait_loaded = from_valuer.calculate_wait_loaded
 
     def add_inherit_valuer(self, valuer):
         self.inherit_valuers.append(valuer)
 
-    def clone(self):
-        value_valuer = self.value_valuer.clone() if self.value_valuer else None
-        calculate_valuer = self.calculate_valuer.clone() if self.calculate_valuer else None
-        return_valuer = self.return_valuer.clone() if self.return_valuer else None
-        inherit_valuers = [inherit_valuer.clone() for inherit_valuer in self.inherit_valuers] if self.inherit_valuers else None
+    def clone(self, contexter=None):
+        value_valuer = self.value_valuer.clone(contexter) if self.value_valuer else None
+        calculate_valuer = self.calculate_valuer.clone(contexter) if self.calculate_valuer else None
+        return_valuer = self.return_valuer.clone(contexter) if self.return_valuer else None
+        inherit_valuers = [inherit_valuer.clone(contexter) for inherit_valuer in self.inherit_valuers] \
+            if self.inherit_valuers else None
+        if contexter is not None:
+            return ContextForeachValuer(value_valuer, calculate_valuer, return_valuer, inherit_valuers,
+                              self.key, self.filter, from_valuer=self, contexter=contexter)
+        if isinstance(self, ContextForeachValuer):
+            return ContextForeachValuer(value_valuer, calculate_valuer, return_valuer, inherit_valuers,
+                                        self.key, self.filter, from_valuer=self, contexter=self.contexter)
         return self.__class__(value_valuer, calculate_valuer, return_valuer, inherit_valuers,
                               self.key, self.filter, from_valuer=self)
     
     def reinit(self):
         self.calculated_values = []
         return super(ForeachValuer, self).reinit()
 
@@ -71,102 +82,111 @@
         if self.inherit_valuers:
             for inherit_valuer in self.inherit_valuers:
                 inherit_valuer.fill(data)
 
         if self.value_valuer:
             self.value_valuer.fill(data)
             if not self.value_wait_loaded:
-                self.value = self.value_valuer.get()
+                value = self.value_valuer.get()
+            else:
+                value = data
         else:
-            self.value = data
+            value = data
 
         if not self.value_wait_loaded:
-            if isinstance(self.value, dict):
-                for k, v in self.value.items():
+            calculated_values = []
+            if isinstance(value, dict):
+                for k, v in value.items():
                     calculate_valuer = self.calculate_valuer.clone()
                     if isinstance(v, dict):
                         calculate_valuer.fill(dict(_index_=k, **v))
                     else:
                         calculate_valuer.fill(dict(_index_=k, _value_=v))
-                    self.calculated_values.append(calculate_valuer)
-            elif isinstance(self.value, (list, types.GeneratorType)):
-                for i in range(len(self.value)):
+                    calculated_values.append(calculate_valuer)
+            elif isinstance(value, (list, types.GeneratorType)):
+                for i in range(len(value)):
                     calculate_valuer = self.calculate_valuer.clone()
-                    if isinstance(self.value[i], dict):
-                        calculate_valuer.fill(dict(_index_=i, **self.value[i]))
+                    if isinstance(value[i], dict):
+                        calculate_valuer.fill(dict(_index_=i, **value[i]))
                     else:
-                        calculate_valuer.fill(dict(_index_=i, _value_=self.value[i]))
-                    self.calculated_values.append(calculate_valuer)
-            elif isinstance(self.value, range_type):
-                for i in self.value:
+                        calculate_valuer.fill(dict(_index_=i, _value_=value[i]))
+                    calculated_values.append(calculate_valuer)
+            elif isinstance(value, range_type):
+                for i in value:
                     calculate_valuer = self.calculate_valuer.clone()
                     calculate_valuer.fill(dict(_index_=i))
-                    self.calculated_values.append(calculate_valuer)
+                    calculated_values.append(calculate_valuer)
 
             if not self.calculate_wait_loaded:
                 values = []
-                for valuer in self.calculated_values:
+                for valuer in calculated_values:
                     try:
                         values.append(self.do_filter(valuer.get()))
                     except ContinueReturn as e:
                         if e.value != ContinueReturn.NULL:
                             values.append(e.value)
                         continue
                     except BreakReturn as e:
                         if e.value != BreakReturn.NULL:
                             values.append(e.value)
                         break
-                self.value = values
                 if self.return_valuer:
-                    self.return_valuer.fill(self.value)
+                    self.return_valuer.fill(values)
+                else:
+                    self.value = values
+            else:
+                self.calculated_values = calculated_values
         return self
 
     def get(self):
         if self.value_valuer and self.value_wait_loaded:
-            self.value = self.value_valuer.get()
+            value = self.value_valuer.get()
+        else:
+            value = self.value
 
         if self.value_wait_loaded:
-            if isinstance(self.value, dict):
-                for k, v in self.value.items():
+            calculated_values = self.calculated_values
+            if isinstance(value, dict):
+                for k, v in value.items():
                     calculate_valuer = self.calculate_valuer.clone()
                     if isinstance(v, dict):
                         calculate_valuer.fill(dict(_index_=k, **v))
                     else:
                         calculate_valuer.fill(dict(_index_=k, _value_=v))
-                    self.calculated_values.append(calculate_valuer)
-            elif isinstance(self.value, (list, types.GeneratorType)):
-                for i in range(len(self.value)):
+                    calculated_values.append(calculate_valuer)
+            elif isinstance(value, (list, types.GeneratorType)):
+                for i in range(len(value)):
                     calculate_valuer = self.calculate_valuer.clone()
-                    if isinstance(self.value[i], dict):
-                        calculate_valuer.fill(dict(_index_=i, **self.value[i]))
+                    if isinstance(value[i], dict):
+                        calculate_valuer.fill(dict(_index_=i, **value[i]))
                     else:
-                        calculate_valuer.fill(dict(_index_=i, _value_=self.value[i]))
-                    self.calculated_values.append(calculate_valuer)
-            elif isinstance(self.value, range_type):
-                for i in self.value:
+                        calculate_valuer.fill(dict(_index_=i, _value_=value[i]))
+                    calculated_values.append(calculate_valuer)
+            elif isinstance(value, range_type):
+                for i in value:
                     calculate_valuer = self.calculate_valuer.clone()
                     calculate_valuer.fill(dict(_index_=i))
-                    self.calculated_values.append(calculate_valuer)
+                    calculated_values.append(calculate_valuer)
 
         if self.calculate_wait_loaded:
-            values = []
-            for valuer in self.calculated_values:
+            calculated_values, values = self.calculated_values, []
+            for valuer in calculated_values:
                 try:
                     values.append(self.do_filter(valuer.get()))
                 except ContinueReturn as e:
                     if e.value != ContinueReturn.NULL:
                         values.append(e.value)
                     continue
                 except BreakReturn as e:
                     if e.value != BreakReturn.NULL:
                         values.append(e.value)
                     break
-            self.value = values
             if self.return_valuer:
-                self.return_valuer.fill(self.value)
+                return self.return_valuer.fill(values).get()
+            return values
 
         if self.return_valuer:
             return self.return_valuer.get()
         return self.value
 
     def childs(self):
         childs = []
@@ -202,27 +222,72 @@
 
     def get_final_filter(self):
         if self.return_valuer:
             return self.return_valuer.get_final_filter()
         return ArrayFilter()
 
 
+class ContextForeachValuer(ForeachValuer):
+    def __init__(self, *args, **kwargs):
+        self.contexter = kwargs.pop("contexter")
+        self.value_context_id = (id(self), "value")
+        self.calculated_values_context_id = (id(self), "calculated_values")
+        super(ContextForeachValuer, self).__init__(*args, **kwargs)
+
+    @property
+    def value(self):
+        try:
+            return self.contexter.values[self.value_context_id]
+        except KeyError:
+            return None
+
+    @value.setter
+    def value(self, v):
+        if v is None:
+            if self.value_context_id in self.contexter.values:
+                self.contexter.values.pop(self.value_context_id)
+            return
+        self.contexter.values[self.value_context_id] = v
+
+    @property
+    def calculated_values(self):
+        try:
+            return self.contexter.values[self.calculated_values_context_id]
+        except KeyError:
+            return []
+
+    @calculated_values.setter
+    def calculated_values(self, v):
+        if not v:
+            if self.calculated_values_context_id in self.contexter.values:
+                self.contexter.values.pop(self.calculated_values_context_id)
+            return
+        self.contexter.values[self.calculated_values_context_id] = v
+
+
 class BreakValuer(Valuer):
     def __init__(self, return_valuer, inherit_valuers, *args, **kwargs):
         self.return_valuer = return_valuer
         self.inherit_valuers = inherit_valuers
         super(BreakValuer, self).__init__(*args, **kwargs)
 
     def add_inherit_valuer(self, valuer):
         self.inherit_valuers.append(valuer)
 
-    def clone(self):
-        return_valuer = self.return_valuer.clone() if self.return_valuer else None
-        inherit_valuers = [inherit_valuer.clone() for inherit_valuer in self.inherit_valuers] if self.inherit_valuers else None
-        return self.__class__(return_valuer, inherit_valuers, self.key, self.filter)
+    def clone(self, contexter=None):
+        return_valuer = self.return_valuer.clone(contexter) if self.return_valuer else None
+        inherit_valuers = [inherit_valuer.clone(contexter) for inherit_valuer in self.inherit_valuers] \
+            if self.inherit_valuers else None
+        if contexter is not None:
+            return ContextBreakValuer(return_valuer, inherit_valuers, self.key, self.filter, from_valuer=self,
+                                      contexter=contexter)
+        if isinstance(self, ContextBreakValuer):
+            return ContextBreakValuer(return_valuer, inherit_valuers, self.key, self.filter, from_valuer=self,
+                                      contexter=self.contexter)
+        return self.__class__(return_valuer, inherit_valuers, self.key, self.filter, from_valuer=self)
 
     def fill(self, data):
         if self.inherit_valuers:
             for inherit_valuer in self.inherit_valuers:
                 inherit_valuer.fill(data)
 
         if self.return_valuer:
@@ -256,27 +321,56 @@
 
     def get_final_filter(self):
         if self.return_valuer:
             return self.return_valuer.get_final_filter()
         return None
 
 
+class ContextBreakValuer(BreakValuer):
+    def __init__(self, *args, **kwargs):
+        self.contexter = kwargs.pop("contexter")
+        self.value_context_id = (id(self), "value")
+        super(ContextBreakValuer, self).__init__(*args, **kwargs)
+
+    @property
+    def value(self):
+        try:
+            return self.contexter.values[self.value_context_id]
+        except KeyError:
+            return None
+
+    @value.setter
+    def value(self, v):
+        if v is None:
+            if self.value_context_id in self.contexter.values:
+                self.contexter.values.pop(self.value_context_id)
+            return
+        self.contexter.values[self.value_context_id] = v
+
+
 class ContinueValuer(Valuer):
     def __init__(self, return_valuer, inherit_valuers, *args, **kwargs):
         self.return_valuer = return_valuer
         self.inherit_valuers = inherit_valuers
         super(ContinueValuer, self).__init__(*args, **kwargs)
 
     def add_inherit_valuer(self, valuer):
         self.inherit_valuers.append(valuer)
 
-    def clone(self):
-        return_valuer = self.return_valuer.clone() if self.return_valuer else None
-        inherit_valuers = [inherit_valuer.clone() for inherit_valuer in self.inherit_valuers] if self.inherit_valuers else None
-        return self.__class__(return_valuer, inherit_valuers, self.key, self.filter)
+    def clone(self, contexter=None):
+        return_valuer = self.return_valuer.clone(contexter) if self.return_valuer else None
+        inherit_valuers = [inherit_valuer.clone(contexter) for inherit_valuer in self.inherit_valuers] \
+            if self.inherit_valuers else None
+        if contexter is not None:
+            return ContextContinueValuer(return_valuer, inherit_valuers, self.key, self.filter, from_valuer=self,
+                                         contexter=contexter)
+        if isinstance(self, ContextContinueValuer):
+            return ContextContinueValuer(return_valuer, inherit_valuers, self.key, self.filter, from_valuer=self,
+                                         contexter=self.contexter)
+        return self.__class__(return_valuer, inherit_valuers, self.key, self.filter, from_valuer=self)
 
     def fill(self, data):
         if self.inherit_valuers:
             for inherit_valuer in self.inherit_valuers:
                 inherit_valuer.fill(data)
 
         if self.return_valuer:
@@ -307,8 +401,30 @@
                 for field in inherit_valuer.get_fields():
                     fields.append(field)
         return fields
 
     def get_final_filter(self):
         if self.return_valuer:
             return self.return_valuer.get_final_filter()
-        return None
+        return None
+
+
+class ContextContinueValuer(ContinueValuer):
+    def __init__(self, *args, **kwargs):
+        self.contexter = kwargs.pop("contexter")
+        self.value_context_id = (id(self), "value")
+        super(ContextContinueValuer, self).__init__(*args, **kwargs)
+
+    @property
+    def value(self):
+        try:
+            return self.contexter.values[self.value_context_id]
+        except KeyError:
+            return None
+
+    @value.setter
+    def value(self, v):
+        if v is None:
+            if self.value_context_id in self.contexter.values:
+                self.contexter.values.pop(self.value_context_id)
+            return
+        self.contexter.values[self.value_context_id] = v
```

### Comparing `syncany-0.2.6/syncany/valuers/make.py` & `syncany-0.2.7/syncany/valuers/make.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     def clone_init(self, from_valuer):
         super(MakeValuer, self).clone_init(from_valuer)
         self.wait_loaded = from_valuer.wait_loaded
 
     def check_wait_loaded(self):
         if isinstance(self.value_valuer, dict):
             for _, (key_valuer, value_valuer) in self.value_valuer.items():
-                if key_valuer and key_valuer.require_loaded():
+                if key_valuer.require_loaded():
                     self.wait_loaded = True
                     return
                 if value_valuer.require_loaded():
                     self.wait_loaded = True
                     return
         elif isinstance(self.value_valuer, list):
             for value_valuer in self.value_valuer:
@@ -40,89 +40,86 @@
             if self.value_valuer.require_loaded():
                 self.wait_loaded = True
                 return
 
     def add_inherit_valuer(self, valuer):
         self.inherit_valuers.append(valuer)
 
-    def clone(self):
+    def clone(self, contexter=None):
         if isinstance(self.value_valuer, dict):
-            value_valuer = {key: (key_valuer.clone(), value_valuer.clone())
+            value_valuer = {key: (key_valuer.clone(contexter), value_valuer.clone(contexter))
                             for key, (key_valuer, value_valuer) in self.value_valuer.items()}
         elif isinstance(self.value_valuer, list):
-            value_valuer = [valuer.clone() for valuer in self.value_valuer]
+            value_valuer = [valuer.clone(contexter) for valuer in self.value_valuer]
         elif isinstance(self.value_valuer, Valuer):
-            value_valuer = self.value_valuer.clone()
+            value_valuer = self.value_valuer.clone(contexter)
         else:
             value_valuer = None
-        return_valuer = self.return_valuer.clone() if self.return_valuer else None
-        inherit_valuers = [inherit_valuer.clone() for inherit_valuer in self.inherit_valuers] if self.inherit_valuers else None
+        return_valuer = self.return_valuer.clone(contexter) if self.return_valuer else None
+        inherit_valuers = [inherit_valuer.clone(contexter) for inherit_valuer in self.inherit_valuers] \
+            if self.inherit_valuers else None
+        if contexter is not None:
+            return ContextMakeValuer(value_valuer, return_valuer, inherit_valuers,
+                                     self.key, self.filter, from_valuer=self, contexter=contexter)
+        if isinstance(self, ContextMakeValuer):
+            return ContextMakeValuer(value_valuer, return_valuer, inherit_valuers,
+                                     self.key, self.filter, from_valuer=self, contexter=self.contexter)
         return self.__class__(value_valuer, return_valuer, inherit_valuers,
                               self.key, self.filter, from_valuer=self)
 
     def fill(self, data):
         if self.inherit_valuers:
             for inherit_valuer in self.inherit_valuers:
                 inherit_valuer.fill(data)
 
+        if not self.wait_loaded:
+            if isinstance(self.value_valuer, dict):
+                value = {key_valuer.fill(data).get(): value_valuer.fill(data).get()
+                         for key, (key_valuer, value_valuer) in self.value_valuer.items()}
+            elif isinstance(self.value_valuer, list):
+                value = [value_valuer.fill(data).get() for value_valuer in self.value_valuer]
+                if len(value) == 1 and isinstance(value[0], list):
+                    value = value[0]
+            elif isinstance(self.value_valuer, Valuer):
+                value = self.do_filter(self.value_valuer.fill(data).get())
+            else:
+                value = self.do_filter(None)
+            if self.return_valuer:
+                self.return_valuer.fill(value)
+            else:
+                self.value = value
+            return self
+
         if isinstance(self.value_valuer, dict):
             for _, (key_valuer, value_valuer) in self.value_valuer.items():
-                if key_valuer:
-                    key_valuer.fill(data)
+                key_valuer.fill(data)
                 value_valuer.fill(data)
         elif isinstance(self.value_valuer, list):
             for value_valuer in self.value_valuer:
                 value_valuer.fill(data)
         elif isinstance(self.value_valuer, Valuer):
             self.value_valuer.fill(data)
-
-        if self.return_valuer and not self.wait_loaded:
-            if isinstance(self.value_valuer, dict):
-                result = {}
-                for key, (key_valuer, value_valuer) in self.value_valuer.items():
-                    kv = key_valuer.get()
-                    vv = value_valuer.get()
-                    if isinstance(kv, list):
-                        for ki in range(len(kv)):
-                            result[kv[ki]] = vv[ki] if isinstance(vv, list) and len(vv) > ki else None
-                    else:
-                        result[kv] = vv
-            elif isinstance(self.value_valuer, list):
-                result = [value_valuer.get() for value_valuer in self.value_valuer]
-                if len(self.value) == 1 and isinstance(self.value[0], list):
-                    self.value = self.value[0]
-            elif isinstance(self.value_valuer, Valuer):
-                result = self.do_filter(self.value_valuer.get())
-            else:
-                result = None
-            self.return_valuer.fill(result)
         return self
 
     def get(self):
-        if not self.return_valuer or self.wait_loaded:
+        if self.wait_loaded:
             if isinstance(self.value_valuer, dict):
-                self.value = {}
-                for key, (key_valuer, value_valuer) in self.value_valuer.items():
-                    kv = key_valuer.get()
-                    vv = value_valuer.get()
-                    if isinstance(kv, list):
-                        for ki in range(len(kv)):
-                            self.value[kv[ki]] = vv[ki] if isinstance(vv, list) and len(vv) > ki else None
-                    else:
-                        self.value[kv] = vv
+                value = {key_valuer.get(): value_valuer.get()
+                         for key, (key_valuer, value_valuer) in self.value_valuer.items()}
             elif isinstance(self.value_valuer, list):
-                self.value = [value_valuer.get() for value_valuer in self.value_valuer]
-                if len(self.value) == 1 and isinstance(self.value[0], list):
-                    self.value = self.value[0]
+                value = [value_valuer.get() for value_valuer in self.value_valuer]
+                if len(value) == 1 and isinstance(value[0], list):
+                    value = value[0]
             elif isinstance(self.value_valuer, Valuer):
-                self.do_filter(self.value_valuer.get())
+                value = self.do_filter(self.value_valuer.get())
             else:
-                self.value = None
+                value = self.do_filter(None)
             if self.return_valuer:
-                self.return_valuer.fill(self.value)
+                return self.return_valuer.fill(value).get()
+            return value
         if self.return_valuer:
             return self.return_valuer.get()
         return self.value
 
     def childs(self):
         childs = []
         if isinstance(self.value_valuer, dict):
@@ -168,8 +165,30 @@
 
         if self.filter:
             return self.filter
 
         if isinstance(self.value_valuer, Valuer):
             return self.value_valuer.get_final_filter()
 
-        return None
+        return None
+
+
+class ContextMakeValuer(MakeValuer):
+    def __init__(self, *args, **kwargs):
+        self.contexter = kwargs.pop("contexter")
+        self.value_context_id = (id(self), "value")
+        super(ContextMakeValuer, self).__init__(*args, **kwargs)
+
+    @property
+    def value(self):
+        try:
+            return self.contexter.values[self.value_context_id]
+        except KeyError:
+            return None
+
+    @value.setter
+    def value(self, v):
+        if v is None:
+            if self.value_context_id in self.contexter.values:
+                self.contexter.values.pop(self.value_context_id)
+            return
+        self.contexter.values[self.value_context_id] = v
```

### Comparing `syncany-0.2.6/syncany/valuers/match.py` & `syncany-0.2.7/syncany/valuers/match.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # 2021/3/15
 # create by: snower
 
 import re
 import json
 from .valuer import Valuer
 
+
 class Matcher(object):
     ARRAY_SEPS = {"{": "}", "[": "]", "(": ")"}
 
     def __init__(self, matcher, valuer):
         self.matcher = matcher
         self.valuer = valuer
 
@@ -28,14 +29,15 @@
         elif matcher[:1] in (">", "<") or matcher[:2] in ("<=", ">="):
             return CmpMatcher(matcher, valuer)
         return None
 
     def match(self, value):
         return None
 
+
 class ReMatcher(Matcher):
     RE_FLAGS = {"a": re.A, "i": re.I, "l": re.L, "u": re.U, "m": re.M, "s": re.S, "x": re.X}
 
     def __init__(self, *args, **kwargs):
         super(ReMatcher, self).__init__(*args, **kwargs)
 
         index = self.matcher.rindex("/")
@@ -50,14 +52,15 @@
             m = self.r.match(value if isinstance(value, str) else str(value))
             if not m:
                 return None
             return {"match_groups": list(m.groups()), "match": self.matcher, "value": value}
         except:
             return None
 
+
 class InMatcher(Matcher):
     def __init__(self, *args, **kwargs):
         super(InMatcher, self).__init__(*args, **kwargs)
 
         try:
             if self.matcher[:1] == "(" and self.matcher[-1:] == ")":
                 self.values = json.loads("[" + self.matcher[1:-1] + "]")
@@ -82,14 +85,15 @@
                 if match is None:
                     continue
                 return match
             if self.values[i] == value:
                 return {"match_key": i, "match_value": self.values[i], "match": self.matcher, "value": value}
         return None
 
+
 class CmpMatcher(Matcher):
     def __init__(self, *args, **kwargs):
         super(CmpMatcher, self).__init__(*args, **kwargs)
 
         self.cmpers = []
         for cmper in self.matcher.split(","):
             if cmper[:2] == ">=":
@@ -110,22 +114,24 @@
 
     def match(self, value):
         for cmper in self.cmpers:
             if not cmper(value):
                 return None
         return {"match": self.matcher, "value": value}
 
+
 class MatchValuer(Valuer):
+    matched_value = None
+
     def __init__(self, match_valuers, default_match_valuer, value_valuer, return_valuer, inherit_valuers, *args, **kwargs):
         self.match_valuers = match_valuers
         self.default_match_valuer = default_match_valuer
         self.value_valuer = value_valuer
         self.return_valuer = return_valuer
         self.inherit_valuers = inherit_valuers
-        self.matched_value = None
         super(MatchValuer, self).__init__(*args, **kwargs)
 
     def new_init(self):
         super(MatchValuer, self).new_init()
         self.value_wait_loaded = True if self.value_valuer and self.value_valuer.require_loaded() else False
         self.wait_loaded = True if self.return_valuer and self.return_valuer.require_loaded() else False
         self.matchers = []
@@ -141,22 +147,29 @@
         self.value_wait_loaded = from_valuer.value_wait_loaded
         self.wait_loaded = from_valuer.wait_loaded
         self.matchers = from_valuer.matchers
 
     def add_inherit_valuer(self, valuer):
         self.inherit_valuers.append(valuer)
 
-    def clone(self):
+    def clone(self, contexter=None):
         match_valuers = {}
         for name, valuer in self.match_valuers.items():
-            match_valuers[name] = valuer.clone()
-        default_match_valuer = self.default_match_valuer.clone() if self.default_match_valuer else None
-        value_valuer = self.value_valuer.clone() if self.value_valuer else None
-        return_valuer = self.return_valuer.clone() if self.return_valuer else None
-        inherit_valuers = [inherit_valuer.clone() for inherit_valuer in self.inherit_valuers] if self.inherit_valuers else None
+            match_valuers[name] = valuer.clone(contexter)
+        default_match_valuer = self.default_match_valuer.clone(contexter) if self.default_match_valuer else None
+        value_valuer = self.value_valuer.clone(contexter) if self.value_valuer else None
+        return_valuer = self.return_valuer.clone(contexter) if self.return_valuer else None
+        inherit_valuers = [inherit_valuer.clone(contexter) for inherit_valuer in self.inherit_valuers] \
+            if self.inherit_valuers else None
+        if contexter is not None:
+            return ContextMatchValuer(match_valuers, default_match_valuer, value_valuer, return_valuer, inherit_valuers,
+                                      self.key, self.filter, from_valuer=self, contexter=contexter)
+        if isinstance(self, ContextMatchValuer):
+            return ContextMatchValuer(match_valuers, default_match_valuer, value_valuer, return_valuer, inherit_valuers,
+                                      self.key, self.filter, from_valuer=self, contexter=self.contexter)
         return self.__class__(match_valuers, default_match_valuer, value_valuer, return_valuer, inherit_valuers,
                               self.key, self.filter, from_valuer=self)
     
     def reinit(self):
         self.matched_value = None
         return super(MatchValuer, self).reinit()
 
@@ -167,54 +180,64 @@
 
         if self.value_valuer:
             self.value_valuer.fill(data)
             if self.value_wait_loaded:
                 if self.default_match_valuer:
                     self.default_match_valuer.fill(data)
                 return self
-            self.value = self.value_valuer.get()
+            value = self.value_valuer.get()
         else:
-            self.value = data
+            value = data
 
+        matched_value = None
         for matcher in self.matchers:
-            self.matched_value = matcher.match(self.value)
-            if self.matched_value is not None:
-                self.match_valuers[matcher.matcher].fill(self.matched_value)
+            matched_value = matcher.match(value)
+            if matched_value is not None:
+                self.match_valuers[matcher.matcher].fill(matched_value)
                 break
-        if self.matched_value is None and self.default_match_valuer:
+        if matched_value is None and self.default_match_valuer:
             self.default_match_valuer.fill(data)
 
         if self.wait_loaded:
-            if self.matched_value is not None:
-                self.do_filter(self.match_valuers[self.matched_value["match"]].get())
+            if matched_value is not None:
+                value = self.do_filter(self.match_valuers[matched_value["match"]].get())
             elif self.default_match_valuer:
-                self.do_filter(self.default_match_valuer.get())
-            self.return_valuer.fill(self.value)
+                value = self.do_filter(self.default_match_valuer.get())
+            else:
+                value = self.do_filter(None)
+            if self.return_valuer:
+                self.return_valuer.fill(value)
+            else:
+                self.value = value
+        self.matched_value = matched_value
         return self
 
     def get(self):
         if self.value_valuer and self.value_wait_loaded:
-            self.value = self.value_valuer.get()
+            value, matched_value = self.value_valuer.get(), None
             for matcher in self.matchers:
-                self.matched_value = matcher.match(self.value)
-                if self.matched_value is not None:
-                    self.match_valuers[matcher.matcher].fill(self.matched_value)
+                matched_value = matcher.match(value)
+                if matched_value is not None:
+                    self.match_valuers[matcher.matcher].fill(matched_value)
                     break
         elif self.wait_loaded:
             return self.return_valuer.get()
+        else:
+            value, matched_value = self.value, self.matched_value
 
-        if self.matched_value is not None:
-            self.do_filter(self.match_valuers[self.matched_value["match"]].get())
+        if matched_value is not None:
+            value = self.do_filter(self.match_valuers[matched_value["match"]].get())
         elif self.default_match_valuer:
-            self.do_filter(self.default_match_valuer.get())
+            value = self.do_filter(self.default_match_valuer.get())
+        else:
+            value = self.do_filter(None)
 
         if self.return_valuer:
-            self.return_valuer.fill(self.value)
-            self.value = self.return_valuer.get()
-        return self.value
+            return self.return_valuer.fill(value).get()
+        return value
 
     def childs(self):
         childs = list(self.match_valuers.values())
         if self.default_match_valuer:
             childs.append(self.default_match_valuer)
         if self.value_valuer:
             childs.append(self.value_valuer)
@@ -258,8 +281,46 @@
         if self.default_match_valuer:
             filter = self.default_match_valuer.get_final_filter()
             if filter is None:
                 return final_filter
 
             if final_filter is not None and final_filter.__class__ != filter.__class__:
                 return None
-        return final_filter
+        return final_filter
+
+
+class ContextMatchValuer(MatchValuer):
+    def __init__(self, *args, **kwargs):
+        self.contexter = kwargs.pop("contexter")
+        self.value_context_id = (id(self), "value")
+        self.matched_value_context_id = (id(self), "matched_value")
+        super(ContextMatchValuer, self).__init__(*args, **kwargs)
+
+    @property
+    def value(self):
+        try:
+            return self.contexter.values[self.value_context_id]
+        except KeyError:
+            return None
+
+    @value.setter
+    def value(self, v):
+        if v is None:
+            if self.value_context_id in self.contexter.values:
+                self.contexter.values.pop(self.value_context_id)
+            return
+        self.contexter.values[self.value_context_id] = v
+
+    @property
+    def matched_value(self):
+        try:
+            return self.contexter.values[self.matched_value_context_id]
+        except KeyError:
+            return None
+
+    @matched_value.setter
+    def matched_value(self, v):
+        if v is None:
+            if self.matched_value_context_id in self.contexter.values:
+                self.contexter.values.pop(self.matched_value_context_id)
+            return
+        self.contexter.values[self.matched_value_context_id] = v
```

### Comparing `syncany-0.2.6/syncany/valuers/schema.py` & `syncany-0.2.7/syncany/valuers/schema.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 # -*- coding: utf-8 -*-
 # 18/8/15
 # create by: snower
 
 from .valuer import Valuer
 
+
 class SchemaValuer(Valuer):
     def __init__(self, schema_valuers, *args, **kwargs):
         self.schema_valuers = schema_valuers
         super(SchemaValuer, self).__init__(*args, **kwargs)
 
-    def clone(self):
+    def clone(self, contexter=None):
         schema_valuers = {}
         for name, valuer in self.schema_valuers.items():
-            schema_valuers[name] = valuer.clone()
+            schema_valuers[name] = valuer.clone(contexter)
+        if contexter is not None:
+            return ContextSchemaValuer(schema_valuers, self.key, self.filter, from_valuer=self, contexter=contexter)
+        if isinstance(self, ContextSchemaValuer):
+            return ContextSchemaValuer(schema_valuers, self.key, self.filter, from_valuer=self, contexter=self.contexter)
         return self.__class__(schema_valuers, self.key, self.filter, from_valuer=self)
 
     def fill(self, data):
         super(SchemaValuer, self).fill(data)
 
         for name, valuer in self.schema_valuers.items():
             valuer.fill(data)
@@ -37,8 +42,30 @@
         for name, valuer in self.schema_valuers.items():
             for field in valuer.get_fields():
                 fields.append(field)
 
         return fields
 
     def get_final_filter(self):
-        return None
+        return None
+
+
+class ContextSchemaValuer(SchemaValuer):
+    def __init__(self, *args, **kwargs):
+        self.contexter = kwargs.pop("contexter")
+        self.value_context_id = (id(self), "value")
+        super(ContextSchemaValuer, self).__init__(*args, **kwargs)
+
+    @property
+    def value(self):
+        try:
+            return self.contexter.values[self.value_context_id]
+        except KeyError:
+            return None
+
+    @value.setter
+    def value(self, v):
+        if v is None:
+            if self.value_context_id in self.contexter.values:
+                self.contexter.values.pop(self.value_context_id)
+            return
+        self.contexter.values[self.value_context_id] = v
```

### Comparing `syncany-0.2.6/syncany/valuers/valuer.py` & `syncany-0.2.7/syncany/valuers/valuer.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # 18/8/6
 # create by: snower
 
 import datetime
 from ..errors import SyncanyException
 from ..utils import ensure_timezone
 
+
 class LoadAllFieldsException(SyncanyException):
     pass
 
 
 def get_key(data, key, dot_keys):
     if key in data:
         return data[key], 1
@@ -19,69 +20,99 @@
         dot_key = ".".join(dot_keys[:i + 1])
         if dot_key in data:
             return data[dot_key], i + 1
     return None, 1
 
 def dict_key(key, dot_keys=None):
     def _(data):
+        if isinstance(data, dict):
+            return get_key(data, key, dot_keys)
         if isinstance(data, list):
             rdata, rindex = [], len(dot_keys)
             for value in data:
                 if not isinstance(value, dict):
-                    continue
-                value, vindex = get_key(value, key, dot_keys)
+                    if not hasattr(value, key):
+                        continue
+                    value, vindex = getattr(value, key), 1
+                else:
+                    value, vindex = get_key(value, key, dot_keys)
                 if value is None:
                     continue
                 rdata.append(value)
                 rindex = min(rindex, vindex)
             return rdata, rindex
-        if isinstance(data, dict):
-            return get_key(data, key, dot_keys)
+        if hasattr(data, key):
+            return getattr(data, key), 1
         return None, 1
     return _
 
 def list_key(key):
     def _(data):
+        if isinstance(data, list) and key < len(data):
+            return data[key], 1
         if isinstance(data, dict):
             colon_key = ":%d" % key
             if colon_key in data:
                 return data[colon_key], 1
             if key == 0:
                 return data, 1
             return None, 1
-        if isinstance(data, list) and key < len(data):
-            return data[key], 1
         return None, 1
     return _
 
 def slice_key(key):
     def _(data):
+        if isinstance(data, list):
+            if len(key) == 1:
+                return data[key[0]:], 1
+            if len(key) == 2:
+                return data[key[0]: key[1]], 1
+            return data[key[0]: key[1]: key[2]], 1
         if isinstance(data, dict):
             colon_key = ":" + ":".join([str(k) for k in key])
             if colon_key in data:
                 return data[colon_key], 1
             if key and key[0] == 0:
                 return data, 1
             return None, 1
-        if isinstance(data, list):
-            if len(key) == 1:
-                return data[key[0]:], 1
-            if len(key) == 2:
-                return data[key[0]: key[1]], 1
-            return data[key[0]: key[1]: key[2]], 1
         return None, 1
     return _
 
+
+class ContextRunner(object):
+    def __init__(self, contexter, valuer, values=None):
+        self.contexter = contexter
+        self.valuer = valuer
+        self.values = {} if values is None else values
+
+    def fill(self, data):
+        self.contexter.values = self.values
+        self.valuer.fill(data)
+        return self
+
+    def get(self):
+        self.contexter.values = self.values
+        return self.valuer.get()
+
+
+class Contexter(object):
+    def __init__(self):
+        self.values = {}
+
+    def create_runner(self, valuer, values=None):
+        return ContextRunner(self, valuer, values)
+
+
 class Valuer(object):
     KEY_GETTER_CACHES = {}
+    value = None
 
     def __init__(self, key, filter=None, from_valuer=None):
         self.key = key
         self.filter = filter
-        self.value = None
         if from_valuer is None:
             self.new_init()
         else:
             self.clone_init(from_valuer)
 
     def new_init(self):
         self.key_getters = []
@@ -118,79 +149,98 @@
                 self.key_getters.append(dict_key(key, keys[i:]))
         if len(self.KEY_GETTER_CACHES) > 1024:
             cache_keys = list(self.KEY_GETTER_CACHES.keys())
             for cache_key in cache_keys[:len(cache_keys) - 512]:
                 self.KEY_GETTER_CACHES.pop(cache_key, None)
         self.KEY_GETTER_CACHES[self.key] = self.key_getters
 
-    def clone(self):
+    def clone(self, contexter=None):
+        if contexter is not None:
+            return ContextValuer(self.key, self.filter, from_valuer=self, contexter=contexter)
+        if isinstance(self, ContextValuer):
+            return ContextValuer(self.key, self.filter, from_valuer=self, contexter=self.contexter)
         return self.__class__(self.key, self.filter, from_valuer=self)
 
     def reinit(self):
         self.value = None
         for valuer in self.child_valuers:
             valuer.reinit()
         return self
 
     def fill(self, data):
-        if data is None or not self.key:
-            self.do_filter(None)
+        if isinstance(data, dict) and self.key in data:
+            self.value = self.do_filter(data[self.key])
             return self
-
-        if self.key == "*" or not isinstance(data, (dict, list)):
-            self.do_filter(data)
+        if data is None or not self.key:
+            self.value = self.do_filter(None)
             return self
-
-        if self.key in data:
-            self.do_filter(data[self.key])
+        if self.key == "*":
+            self.value = self.do_filter(data)
             return self
 
         if not self.key_getters:
             if self.key in self.KEY_GETTER_CACHES:
                 self.key_getters = self.KEY_GETTER_CACHES[self.key]
             else:
                 self.parse_key()
         try:
             key_getter_index, key_getter_len = 0, len(self.key_getters)
             while key_getter_index < key_getter_len:
                 data, index = self.key_getters[key_getter_index](data)
                 if data is None:
                     break
                 key_getter_index += index
-            self.value = data
+            self.value = self.do_filter(data)
         except:
-            self.value = None
-        self.do_filter(self.value)
+            self.value = self.do_filter(None)
         return self
 
     def get(self):
         return self.value
 
     def reset(self):
         for valuer in self.child_valuers:
             valuer.reset()
 
     def do_filter(self, value):
         if not self.filter:
             if isinstance(value, datetime.datetime):
-                self.value = ensure_timezone(value)
-            else:
-                self.value = value
-            return self.value
-
-        self.value = self.filter.filter(value)
-        return self.value
+                value = ensure_timezone(value)
+            return value
+        return self.filter.filter(value)
 
     def childs(self):
         return []
 
     def get_fields(self):
         return []
 
     def get_final_filter(self):
         return self.filter
 
     def require_loaded(self):
         for child in self.child_valuers:
             if child.require_loaded():
                 return True
-        return False
+        return False
+
+
+class ContextValuer(Valuer):
+    def __init__(self, *args, **kwargs):
+        self.contexter = kwargs.pop("contexter")
+        self.value_context_id = (id(self), "value")
+        super(ContextValuer, self).__init__(*args, **kwargs)
+
+    @property
+    def value(self):
+        try:
+            return self.contexter.values[self.value_context_id]
+        except KeyError:
+            return None
+
+    @value.setter
+    def value(self, v):
+        if v is None:
+            if self.value_context_id in self.contexter.values:
+                self.contexter.values.pop(self.value_context_id)
+            return
+        self.contexter.values[self.value_context_id] = v
```

### Comparing `syncany-0.2.6/syncany.egg-info/PKG-INFO` & `syncany-0.2.7/syncany.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncany
-Version: 0.2.6
+Version: 0.2.7
 Summary: 简单易用的数据同步转换导出框架
 Home-page: https://github.com/snower/syncany
 Author: snower
 Author-email: sujian199@gmail.com
 License: MIT
 Description: # syncany
```

### Comparing `syncany-0.2.6/syncany.egg-info/SOURCES.txt` & `syncany-0.2.7/syncany.egg-info/SOURCES.txt`

 * *Files identical despite different names*

