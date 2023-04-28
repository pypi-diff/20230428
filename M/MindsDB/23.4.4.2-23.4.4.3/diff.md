# Comparing `tmp/MindsDB-23.4.4.2.tar.gz` & `tmp/MindsDB-23.4.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/MindsDB-23.4.4.2.tar", last modified: Thu Apr 27 09:37:45 2023, max compression
+gzip compressed data, was "dist/MindsDB-23.4.4.3.tar", last modified: Fri Apr 28 09:30:45 2023, max compression
```

## Comparing `MindsDB-23.4.4.2.tar` & `MindsDB-23.4.4.3.tar`

### file list

```diff
@@ -1,1169 +1,1167 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-27 09:37:24.000000 MindsDB-23.4.4.2/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/MindsDB.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23921 2023-04-27 09:37:44.000000 MindsDB-23.4.4.2/MindsDB.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    54678 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/MindsDB.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 09:37:44.000000 MindsDB-23.4.4.2/MindsDB.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-27 09:37:44.000000 MindsDB-23.4.4.2/MindsDB.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-27 09:37:44.000000 MindsDB-23.4.4.2/MindsDB.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    23921 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21883 2023-04-27 09:37:24.000000 MindsDB-23.4.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13090 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/api/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/common/check_auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/api/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/http/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/http/gunicorn_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    12801 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/http/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/api/http/namespaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/http/namespaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/http/namespaces/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/http/namespaces/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/http/namespaces/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/api/http/namespaces/configs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/http/namespaces/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/http/namespaces/configs/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/http/namespaces/configs/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/http/namespaces/configs/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/http/namespaces/configs/databases.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/http/namespaces/configs/default.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/http/namespaces/configs/files.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/http/namespaces/configs/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/http/namespaces/configs/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/http/namespaces/configs/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/http/namespaces/configs/streams.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/http/namespaces/configs/tabs.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/http/namespaces/configs/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/http/namespaces/configs/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/http/namespaces/databases.py
--rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/http/namespaces/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/http/namespaces/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/http/namespaces/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/http/namespaces/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/http/namespaces/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/http/namespaces/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/http/namespaces/tab.py
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/http/namespaces/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/http/namespaces/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/http/start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/http/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/api/mongo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mongo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/api/mongo/classes/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mongo/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mongo/classes/query_sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mongo/classes/responder.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mongo/classes/responder_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mongo/classes/scram.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mongo/classes/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/api/mongo/functions/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mongo/functions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/api/mongo/responders/
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mongo/responders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mongo/responders/add_shard.py
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mongo/responders/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mongo/responders/buildinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mongo/responders/coll_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mongo/responders/company_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mongo/responders/connection_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mongo/responders/count.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mongo/responders/db_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mongo/responders/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mongo/responders/end_sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5487 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mongo/responders/find.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mongo/responders/get_cmd_line_opts.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mongo/responders/get_free_monitoring_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mongo/responders/get_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mongo/responders/getlog.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mongo/responders/host_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     9041 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mongo/responders/insert.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mongo/responders/is_master.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mongo/responders/is_master_lower.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mongo/responders/list_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mongo/responders/list_databases.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mongo/responders/list_indexes.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mongo/responders/ping.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mongo/responders/recv_chunk_start.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mongo/responders/replsetgetstatus.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mongo/responders/sasl_continue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mongo/responders/sasl_start.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mongo/responders/update_range_deletions.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mongo/responders/whatsmyuri.py
--rw-r--r--   0 runner    (1001) docker     (123)    14041 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mongo/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mongo/start.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/api/mongo/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mongo/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mongo/utilities/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mongo/utilities/mongodb_ast.py
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mongo/utilities/mongodb_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mongo/utilities/mongodb_query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/classes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/classes/client_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/classes/com_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/fake_mysql_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/classes/server_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    56478 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/classes/sql_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/classes/sql_statement_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/controllers/session_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/data_types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/data_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/data_types/mysql_datum.py
--rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/binary_resultset_row_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_count_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_definition_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/command_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/eof_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/err_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/fast_auth_fail_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_response_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/ok_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/password_answer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/resultset_row_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/stmt_prepare_header.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_response_packet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/datahub/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/datahub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/datahub/classes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/datahub/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/datahub/classes/tables_row.py
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/datahub/datahub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/datanode.py
--rw-r--r--   0 runner    (1001) docker     (123)    23115 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/information_schema_datanode.py
--rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/integration_datanode.py
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/project_datanode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/executor/
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/executor/data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/executor/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/executor/executor_client_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    67024 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/executor/executor_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/executor/executor_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/external_libs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/external_libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/external_libs/mysql_scramble.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/libs/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/libs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/libs/constants/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/libs/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35316 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/libs/constants/mysql.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/libs/constants/response_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    31908 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/mysql_proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/utilities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/utilities/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/utilities/lightwood_dtype.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/utilities/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/utilities/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/mysql/start.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/api/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/nlp/nlp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/api/postgres/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/postgres/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/api/postgres/postgres_proxy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/postgres/postgres_proxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/api/postgres/postgres_proxy/executor/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/postgres/postgres_proxy/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6543 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/postgres/postgres_proxy/executor/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/api/postgres/postgres_proxy/postgres_packets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/postgres/postgres_proxy/postgres_packets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12729 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/postgres/postgres_proxy/postgres_packets/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message.py
--rw-r--r--   0 runner    (1001) docker     (123)    40804 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_formats.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_identifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_packets.py
--rw-r--r--   0 runner    (1001) docker     (123)    19291 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/postgres/postgres_proxy/postgres_proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/api/postgres/postgres_proxy/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/postgres/postgres_proxy/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/api/postgres/start.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/access_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/access_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/access_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/access_handler/access_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    32145 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/access_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/access_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/access_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/access_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/access_handler/tests/test_access_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/airtable_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/airtable_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/airtable_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/airtable_handler/airtable_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/airtable_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/airtable_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/airtable_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/airtable_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/airtable_handler/tests/test_airtable_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/altibase_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/altibase_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/altibase_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/altibase_handler/altibase_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)   342129 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/altibase_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/altibase_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/altibase_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/altibase_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/altibase_handler/tests/test_altibase_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/aurora_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/aurora_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/aurora_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6404 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/aurora_handler/aurora_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11767 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/aurora_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/aurora_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/aurora_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/aurora_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_mysql_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_postgres_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/autokeras_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/autokeras_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/autokeras_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/autokeras_handler/autokeras_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/autokeras_handler/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/autokeras_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/autosklearn_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/autosklearn_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/autosklearn_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/autosklearn_handler/autosklearn_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/autosklearn_handler/config.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/autosklearn_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/autosklearn_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/bigquery_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/bigquery_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/bigquery_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/bigquery_handler/bigquery_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/bigquery_handler/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/bigquery_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/bigquery_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/bigquery_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/bigquery_handler/tests/test_bigquery_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/binance_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/binance_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/binance_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/binance_handler/binance_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/binance_handler/binance_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/binance_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/binance_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/byom_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/byom_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/byom_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6590 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/byom_handler/byom_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/byom_handler/proc_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/cassandra_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/cassandra_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/cassandra_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/cassandra_handler/cassandra_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)   176707 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/cassandra_handler/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/cassandra_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/cassandra_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/cassandra_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/cassandra_handler/tests/test_cassandra_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/ckan_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/ckan_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/ckan_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/ckan_handler/ckan_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    17688 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/ckan_handler/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/ckan_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/ckan_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/ckan_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/ckan_handler/tests/test_ckan_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/clickhouse_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/clickhouse_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/clickhouse_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/clickhouse_handler/clickhouse_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/clickhouse_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/clickhouse_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/clickhouse_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/clickhouse_handler/tests/test_clickhouse_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/cloud_spanner_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/cloud_spanner_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/cloud_spanner_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/cloud_spanner_handler/cloud_spanner_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/cloud_spanner_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/cloud_spanner_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/cloud_spanner_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/cloud_spanner_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/cloud_spanner_handler/tests/test_cloud_spanner_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/cloud_sql_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/cloud_sql_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/cloud_sql_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/cloud_sql_handler/cloud_sql_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    37571 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/cloud_sql_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/cloud_sql_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/cloud_sql_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/cloud_sql_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mssql_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mysql_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/cockroach_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/cockroach_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/cockroach_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/cockroach_handler/cockroach_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/cockroach_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/cockroach_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/cockroach_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/cockroach_handler/tests/test_cockroachdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/confluence_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/confluence_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/confluence_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/confluence_handler/confluence_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/confluence_handler/confluence_table.py
--rw-r--r--   0 runner    (1001) docker     (123)    76194 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/confluence_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/confluence_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/couchbase_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/couchbase_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/couchbase_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/couchbase_handler/couchbase_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/couchbase_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/couchbase_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/couchbase_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/couchbase_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/couchbase_handler/tests/test_couchbase_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/crate_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/crate_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/crate_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7157 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/crate_handler/crate_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/crate_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/crate_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/crate_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/crate_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/crate_handler/tests/test_crate_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/d0lt_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/d0lt_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/d0lt_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/d0lt_handler/d0lt_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/d0lt_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/d0lt_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/d0lt_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/d0lt_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/d0lt_handler/tests/test_d0lt_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/databend_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/databend_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/databend_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/databend_handler/databend_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6443 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/databend_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/databend_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/databend_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/databend_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/databend_handler/tests/test_databend_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/databricks_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/databricks_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/databricks_handler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/databricks_handler/databricks/
--rw-r--r--   0 runner    (1001) docker     (123)    86110 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/databricks_handler/databricks/createdb.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    58645 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/databricks_handler/databricks/createpred.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    35986 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/databricks_handler/databricks/hivmetastore.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    21694 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/databricks_handler/databricks/mindsdbdatabricks.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    62078 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/databricks_handler/databricks/selectfrom.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     7952 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/databricks_handler/databricks_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12097 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/databricks_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/databricks_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/databricks_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/databricks_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/databricks_handler/tests/test_databricks_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/datastax_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/datastax_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/datastax_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/datastax_handler/datastax_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    26175 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/datastax_handler/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/datastax_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/datastax_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/datastax_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/datastax_handler/tests/test_cassandra_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/db2_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/db2_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/db2_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/db2_handler/db2_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    19117 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/db2_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/db2_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/db2_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/db2_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/db2_handler/tests/test_db2_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/derby_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/derby_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/derby_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8751 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/derby_handler/derby_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/derby_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/derby_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/derby_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/derby_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/derby_handler/tests/test_derby_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/dremio_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/dremio_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/dremio_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/dremio_handler/dremio_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    52734 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/dremio_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/dremio_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/dremio_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/dremio_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/dremio_handler/tests/test_dremio_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/druid_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/druid_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/druid_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7324 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/druid_handler/druid_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    29112 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/druid_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/druid_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/druid_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/druid_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/druid_handler/tests/test_druid_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/duckdb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/duckdb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/duckdb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/duckdb_handler/duckdb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    19548 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/duckdb_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/duckdb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/duckdb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/duckdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/duckdb_handler/tests/test_duckdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/dynamodb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/dynamodb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/dynamodb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/dynamodb_handler/dynamodb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    55623 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/dynamodb_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/dynamodb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/dynamodb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/dynamodb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/dynamodb_handler/tests/test_dynamodb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/edgelessdb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/edgelessdb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/edgelessdb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/edgelessdb_handler/edgelessdb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/edgelessdb_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/edgelessdb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/edgelessdb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/edgelessdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/edgelessdb_handler/tests/test_edgelessdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/elasticsearch_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/elasticsearch_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/elasticsearch_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/elasticsearch_handler/elasticsearch_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/elasticsearch_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/elasticsearch_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/elasticsearch_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/elasticsearch_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/elasticsearch_handler/tests/test_elasticsearch_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/empress_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/empress_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/empress_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/empress_handler/empress_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11249 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/empress_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/empress_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/empress_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/empress_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/empress_handler/tests/test_empress_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/eventstoredb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/eventstoredb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/eventstoredb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9062 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/eventstoredb_handler/eventstoredb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/eventstoredb_handler/icon.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/file_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/file_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/file_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10837 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/file_handler/file_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/firebird_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/firebird_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/firebird_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/firebird_handler/firebird_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    54033 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/firebird_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/firebird_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/firebird_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/firebird_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/firebird_handler/tests/test_firebird_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/github_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/github_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/github_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/github_handler/github_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11793 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/github_handler/github_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/github_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/github_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/google_calendar_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/google_calendar_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/google_calendar_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/google_calendar_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/google_calendar_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/google_calendar_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/google_calendar_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/google_calendar_handler/tests/test_google_calendar_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/hana_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/hana_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/hana_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11104 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/hana_handler/hana_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/hana_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/hana_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/hive_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/hive_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/hive_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/hive_handler/hive_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    14000 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/hive_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/hive_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/hive_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/hive_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/hive_handler/tests/test_hive_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/hsqldb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/hsqldb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/hsqldb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7491 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/hsqldb_handler/hsqldb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/hsqldb_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/hsqldb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/huggingface_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/huggingface_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/huggingface_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11247 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/huggingface_handler/huggingface_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/huggingface_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/huggingface_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/ignite_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/ignite_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/ignite_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45779 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/ignite_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/ignite_handler/ignite_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/ignite_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/ignite_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/ignite_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/ignite_handler/tests/test_ignite_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/impala_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/impala_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/impala_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/impala_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/impala_handler/impala_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/impala_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/impala_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/impala_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/impala_handler/tests/test_impala_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/influxdb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/influxdb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/influxdb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    63375 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/influxdb_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/influxdb_handler/influxdb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/influxdb_handler/influxdb_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/influxdb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/informix_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/informix_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/informix_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6694 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/informix_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     9618 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/informix_handler/informix_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/informix_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/informix_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/informix_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/informix_handler/tests/test_informix_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/ingres_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/ingres_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/ingres_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/ingres_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/ingres_handler/ingres_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/ingres_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/ingres_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/ingres_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/ingres_handler/tests/test_ingres_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/jira_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/jira_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/jira_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16812 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/jira_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/jira_handler/jira_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/jira_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/jira_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/jira_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/jira_handler/tests/test_jira_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/langchain_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/langchain_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/langchain_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10109 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/langchain_handler/langchain_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/langchain_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/langchain_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/lightwood_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/lightwood_handler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8825 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    20696 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/lightwood_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/lightwood_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/lightwood_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/lightwood_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/lightwood_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10985 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/lightwood_handler/tests/test_lightwood_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/ludwig_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/ludwig_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/ludwig_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/ludwig_handler/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/ludwig_handler/ludwig_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/ludwig_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/ludwig_handler/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/ludwig_handler/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/mariadb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/mariadb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/mariadb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    99045 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/mariadb_handler/create-db.png
--rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/mariadb_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/mariadb_handler/mariadb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    98530 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/mariadb_handler/predict-db.png
--rw-r--r--   0 runner    (1001) docker     (123)   100718 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/mariadb_handler/predictor.png
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/mariadb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/materialize_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/materialize_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/materialize_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47935 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/materialize_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/materialize_handler/materialize_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/materialize_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/materialize_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/materialize_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/materialize_handler/tests/test_materialize_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/matrixone_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/matrixone_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/matrixone_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    57976 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/matrixone_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/matrixone_handler/matrixone_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/matrixone_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/matrixone_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/matrixone_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/matrixone_handler/tests/test_matrixone_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/merlion_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/merlion_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/merlion_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8498 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/merlion_handler/adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8217 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/merlion_handler/merlion_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/merlion_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/merlion_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/mlflow_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/mlflow_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/mlflow_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/mlflow_handler/mlflow_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/mlflow_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/mlflow_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/monetdb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/monetdb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/monetdb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    64685 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/monetdb_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     8113 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/monetdb_handler/monetdb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/monetdb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/monetdb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/monetdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/monetdb_handler/tests/test_monetdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/monetdb_handler/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/monetdb_handler/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/monetdb_handler/utils/monet_get_id.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/mongodb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/mongodb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/mongodb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15045 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/mongodb_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/mongodb_handler/mongodb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/mongodb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/mongodb_handler/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/mongodb_handler/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/mongodb_handler/utils/mongodb_render.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/mssql_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/mssql_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/mssql_handler/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14543 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/mssql_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/mssql_handler/mssql_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/mssql_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/mssql_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/mssql_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/mssql_handler/tests/test_mssql_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/mysql_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/mysql_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/mysql_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/mysql_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6812 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/mysql_handler/mysql_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/mysql_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/neuralforecast_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/neuralforecast_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/neuralforecast_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/neuralforecast_handler/neuralforecast_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/neuralforecast_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/neuralforecast_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/nuo_jdbc_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/nuo_jdbc_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/nuo_jdbc_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    95071 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/nuo_jdbc_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     9833 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/nuo_jdbc_handler/nuo_jdbc_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/nuo_jdbc_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/test_nuo_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/oceanbase_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/oceanbase_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/oceanbase_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37289 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/oceanbase_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/oceanbase_handler/oceanbase_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/oceanbase_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/oceanbase_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/oceanbase_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/oceanbase_handler/tests/test_oceanbase_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/openai_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/openai_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/openai_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/openai_handler/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    27870 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/openai_handler/openai_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/openai_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/openai_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/opengauss_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/opengauss_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/opengauss_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/opengauss_handler/opengauss_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/opengauss_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/opengauss_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/opengauss_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/opengauss_handler/tests/test_opengauss_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/oracle_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/oracle_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/oracle_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/oracle_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/oracle_handler/oracle_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/oracle_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/oracle_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/oracle_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/oracle_handler/tests/test_oracle_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/orioledb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/orioledb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/orioledb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/orioledb_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/orioledb_handler/orioledb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/orioledb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/orioledb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/orioledb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/orioledb_handler/tests/test_orioledb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/phoenix_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/phoenix_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/phoenix_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/phoenix_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     8767 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/phoenix_handler/phoenix_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/phoenix_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/phoenix_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/phoenix_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/phoenix_handler/tests/test_phoenix_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/pinot_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/pinot_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/pinot_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18645 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/pinot_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     8577 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/pinot_handler/pinot_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/pinot_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/pinot_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/pinot_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/pinot_handler/tests/test_pinot_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/plaid_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/plaid_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/plaid_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/plaid_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8076 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/plaid_handler/plaid_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/plaid_handler/plaid_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/plaid_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/plaid_handler/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/planetscale_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/planetscale_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/planetscale_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/planetscale_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/planetscale_handler/planetscale_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/planetscale_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/postgres_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/postgres_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/postgres_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15261 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/postgres_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5725 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/postgres_handler/postgres_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/postgres_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/questdb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/questdb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/questdb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/questdb_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/questdb_handler/questdb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/questdb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/questdb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/questdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/questdb_handler/tests/test_questdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/ray_serve_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/ray_serve_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/ray_serve_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/ray_serve_handler/ray_serve_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/ray_serve_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/ray_serve_handler/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/reddit_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/reddit_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/reddit_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/reddit_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/reddit_handler/reddit_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6558 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/reddit_handler/reddit_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/reddit_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/redshift_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/redshift_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/redshift_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17615 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/redshift_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     7319 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/redshift_handler/redshift_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/redshift_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/redshift_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/redshift_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/redshift_handler/tests/test_redshift_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/rockset_handler/
--rw-r--r--   0 runner    (1001) docker     (123)    22361 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/rockset_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/rockset_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/rockset_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)   194064 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/rockset_handler/tests/test.png
--rw-r--r--   0 runner    (1001) docker     (123)   108141 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/rockset_handler/tests/test2.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/s3_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/s3_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/s3_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24332 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/s3_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/s3_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/s3_handler/s3_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/s3_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/s3_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/s3_handler/tests/test_s3_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/scylla_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/scylla_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/scylla_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40148 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/scylla_handler/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/scylla_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/scylla_handler/scylla_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/scylla_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/scylla_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/scylla_handler/tests/test_scylla_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/sheets_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/sheets_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/sheets_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27211 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/sheets_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/sheets_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/sheets_handler/sheets_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/sheets_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/sheets_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/sheets_handler/tests/test_sheets_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/singlestore_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/singlestore_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/singlestore_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/singlestore_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/singlestore_handler/singlestore_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/singlestore_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/singlestore_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/singlestore_handler/tests/test_singlestore_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/snowflake_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/snowflake_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/snowflake_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/snowflake_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/snowflake_handler/snowflake_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/snowflake_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/snowflake_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/snowflake_handler/tests/test_snowflake_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/solr_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/solr_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/solr_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/solr_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/solr_handler/solr.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/solr_handler/solr_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/solr_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/solr_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/solr_handler/tests/test_solr_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/sqlany_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/sqlany_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/sqlany_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/sqlany_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/sqlany_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/sqlany_handler/sqlany_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/sqlite_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/sqlite_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/sqlite_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   521282 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/sqlite_handler/db_connection.png
--rw-r--r--   0 runner    (1001) docker     (123)   369371 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/sqlite_handler/error.png
--rw-r--r--   0 runner    (1001) docker     (123)    11559 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/sqlite_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)   479779 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/sqlite_handler/model_drop.png
--rw-r--r--   0 runner    (1001) docker     (123)   477242 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/sqlite_handler/prediction_result.png
--rw-r--r--   0 runner    (1001) docker     (123)   552154 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/sqlite_handler/predictor_model.png
--rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/sqlite_handler/sqlite_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/sqlite_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/sqlite_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/sqlite_handler/tests/test_sqlite_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/sqreamdb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/sqreamdb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/sqreamdb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/sqreamdb_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/sqreamdb_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/sqreamdb_handler/sqreamdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/sqreamdb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/sqreamdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/sqreamdb_handler/tests/test_sqreamdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/starrocks_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/starrocks_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/starrocks_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    72778 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/starrocks_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/starrocks_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/starrocks_handler/starrocks_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/starrocks_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/starrocks_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/starrocks_handler/tests/test_starrocks_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/statsforecast_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/statsforecast_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/statsforecast_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/statsforecast_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/statsforecast_handler/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     7584 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/statsforecast_handler/statsforecast_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/supabase_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/supabase_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/supabase_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/supabase_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/supabase_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/supabase_handler/supabase_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/supabase_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/supabase_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/supabase_handler/tests/test_supabase_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/surrealdb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/surrealdb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/surrealdb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25475 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/surrealdb_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/surrealdb_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7116 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/surrealdb_handler/surrealdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/surrealdb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/surrealdb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/surrealdb_handler/tests/test_surrealdb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/surrealdb_handler/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/surrealdb_handler/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/surrealdb_handler/utils/surreal_get_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/tdengine_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/tdengine_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/tdengine_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/tdengine_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/tdengine_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/tdengine_handler/tdengine_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/tdengine_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/tdengine_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/tdengine_handler/tests/test_tdengine_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/teradata_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/teradata_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/teradata_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/teradata_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/teradata_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/teradata_handler/teradata_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/tidb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/tidb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/tidb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/tidb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/tidb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/tidb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/tidb_handler/tests/test_tidb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/tidb_handler/tidb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/timescaledb_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/timescaledb_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/timescaledb_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11184 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/timescaledb_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/timescaledb_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/timescaledb_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/timescaledb_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/timescaledb_handler/tests/test_timescaledb_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/timescaledb_handler/timescaledb_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/tpot_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/tpot_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/tpot_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/tpot_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/tpot_handler/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/tpot_handler/tpot_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/trino_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/trino_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/trino_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13752 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/trino_handler/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/trino_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/trino_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/trino_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/trino_handler/tests/test_trino_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/trino_handler/trino_config_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/trino_handler/trino_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/twitter_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/twitter_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/twitter_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/twitter_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/twitter_handler/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16126 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/twitter_handler/twitter_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/vertica_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/vertica_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/vertica_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/vertica_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/vertica_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/vertica_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/vertica_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/vertica_handler/tests/test_vertica_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/vertica_handler/vertica_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/vitess_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/vitess_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/vitess_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/vitess_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/vitess_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/vitess_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/vitess_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/vitess_handler/tests/test_vitess_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/vitess_handler/vitess_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/yugabyte_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/yugabyte_handler/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/yugabyte_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16563 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/yugabyte_handler/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/yugabyte_handler/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/yugabyte_handler/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/yugabyte_handler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/yugabyte_handler/tests/test_yugabyte_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers/yugabyte_handler/yugabyte_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers_client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers_client/db_client_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers_client/db_grpc_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers_client/ml_client_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers_client/ml_grpc_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers_wrapper/db_grpc_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers_wrapper/db_handler_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers_wrapper/ml_grpc_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/handlers_wrapper/ml_handler_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/libs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/libs/api_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7147 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/libs/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/libs/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/libs/handler_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    17360 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/libs/ml_exec_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/libs/ml_handler_proc.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/libs/net_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/libs/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/libs/storage_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/integrations/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/utilities/date_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/utilities/install.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/utilities/processes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/utilities/sql_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/utilities/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/utilities/time_series_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/integrations/utilities/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/interfaces/database/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/interfaces/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/interfaces/database/database.py
--rw-r--r--   0 runner    (1001) docker     (123)    18638 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/interfaces/database/integrations.py
--rw-r--r--   0 runner    (1001) docker     (123)     9095 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/interfaces/database/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/interfaces/database/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/interfaces/file/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/interfaces/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/interfaces/file/file_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/interfaces/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/interfaces/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13068 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/interfaces/jobs/jobs_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/interfaces/jobs/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/interfaces/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/interfaces/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/interfaces/model/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    21478 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/interfaces/model/model_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/interfaces/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/interfaces/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9337 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/interfaces/storage/db.py
--rw-r--r--   0 runner    (1001) docker     (123)    10434 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/interfaces/storage/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/interfaces/storage/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/interfaces/storage/model_fs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/interfaces/stream/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/interfaces/stream/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/interfaces/stream/base/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/interfaces/stream/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/interfaces/stream/base/integration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/interfaces/stream/kafka/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/interfaces/stream/kafka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/interfaces/stream/kafka/kafkadb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/interfaces/stream/redis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/interfaces/stream/redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/interfaces/stream/redis/redisdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/interfaces/stream/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/interfaces/stream/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/microservices_grpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/microservices_grpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/microservices_grpc/db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/microservices_grpc/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/microservices_grpc/db/common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/microservices_grpc/db/common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/microservices_grpc/db/db_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12845 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/microservices_grpc/db/db_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/microservices_grpc/executor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/microservices_grpc/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/microservices_grpc/executor/executor_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    14810 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/microservices_grpc/executor/executor_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/microservices_grpc/ml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/microservices_grpc/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/microservices_grpc/ml/common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/microservices_grpc/ml/common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/microservices_grpc/ml/ml_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/microservices_grpc/ml/ml_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/migrations/alembic.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/migrations/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/migrations/migrate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/migrations/versions/
--rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/migrations/versions/2021-11-30_17c3d2384711_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/migrations/versions/2022-01-26_47f97b83cee4_views.py
--rw-r--r--   0 runner    (1001) docker     (123)    10808 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/migrations/versions/2022-02-09_27c5aca9e47e_db_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/migrations/versions/2022-05-25_d74c189b87e6_predictor_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/migrations/versions/2022-07-08_999bceb904df_integration_args.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/migrations/versions/2022-07-15_b5b53e0ea7f8_training_data_rows_columns_count.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/migrations/versions/2022-07-22_6e834843e7e9_training_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/migrations/versions/2022-08-19_976f15a37e6a_predictors_versioning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/migrations/versions/2022-08-25_6a54ba55872e_view_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/migrations/versions/2022-08-29_473e8f239481_straighten.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/migrations/versions/2022-09-06_96d5fef10caa_data_integration_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/migrations/versions/2022-09-08_87b2df2b83e1_predictor_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/migrations/versions/2022-09-19_3d5e70105df7_content_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/migrations/versions/2022-09-29_cada7d2be947_json_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/migrations/versions/2022-10-14_43c52d23845a_projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/migrations/versions/2022-11-07_1e60096fc817_predictor_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/migrations/versions/2022-11-11_d429095b570f_data_integration_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/migrations/versions/2022-12-26_459218b0844c_fix_unique_constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/migrations/versions/2023-02-02_b6d0a47294ac_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/migrations/versions/2023-02-17_ee63d868fa84_predictor_integration_null.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/migrations/versions/2023-02-25_3154382dab17_training_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/migrations/versions/2023-02-27_ef04cdbe51ed_jobs_user_class.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/migrations/versions/2023-04-11_b8be148dbc85_jobs_history_query.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/migrations/versions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/utilities/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/utilities/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/utilities/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/utilities/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/utilities/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/utilities/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/utilities/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/utilities/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/utilities/hooks/profiling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/utilities/json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/utilities/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/utilities/log_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/mindsdb/utilities/profiler/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/utilities/profiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/utilities/profiler/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/utilities/ps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/utilities/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/mindsdb/utilities/wizards.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 09:37:45.000000 MindsDB-23.4.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-04-27 09:37:25.000000 MindsDB-23.4.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/MindsDB.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23862 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/MindsDB.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    54604 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/MindsDB.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/MindsDB.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/MindsDB.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/MindsDB.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    23862 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21824 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13090 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/api/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/common/check_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/api/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/http/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/http/gunicorn_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12801 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/http/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/api/http/namespaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/http/namespaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/http/namespaces/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/http/namespaces/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/http/namespaces/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/api/http/namespaces/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/http/namespaces/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/http/namespaces/configs/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/http/namespaces/configs/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/http/namespaces/configs/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/http/namespaces/configs/databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/http/namespaces/configs/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/http/namespaces/configs/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/http/namespaces/configs/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/http/namespaces/configs/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/http/namespaces/configs/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/http/namespaces/configs/streams.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/http/namespaces/configs/tabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/http/namespaces/configs/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/http/namespaces/configs/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10355 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/http/namespaces/databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/http/namespaces/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/http/namespaces/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/http/namespaces/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/http/namespaces/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/http/namespaces/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/http/namespaces/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/http/namespaces/tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/http/namespaces/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/http/namespaces/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/http/start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/http/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/api/mongo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mongo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/api/mongo/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mongo/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mongo/classes/query_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mongo/classes/responder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mongo/classes/responder_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mongo/classes/scram.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mongo/classes/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/api/mongo/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mongo/functions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/api/mongo/responders/
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mongo/responders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mongo/responders/add_shard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mongo/responders/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mongo/responders/buildinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mongo/responders/coll_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mongo/responders/company_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mongo/responders/connection_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mongo/responders/count.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mongo/responders/db_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mongo/responders/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mongo/responders/end_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5487 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mongo/responders/find.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mongo/responders/get_cmd_line_opts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mongo/responders/get_free_monitoring_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mongo/responders/get_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mongo/responders/getlog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mongo/responders/host_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9041 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mongo/responders/insert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mongo/responders/is_master.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mongo/responders/is_master_lower.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mongo/responders/list_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mongo/responders/list_databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mongo/responders/list_indexes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mongo/responders/ping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mongo/responders/recv_chunk_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mongo/responders/replsetgetstatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mongo/responders/sasl_continue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mongo/responders/sasl_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mongo/responders/update_range_deletions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mongo/responders/whatsmyuri.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14041 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mongo/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mongo/start.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/api/mongo/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mongo/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mongo/utilities/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mongo/utilities/mongodb_ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mongo/utilities/mongodb_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mongo/utilities/mongodb_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/classes/client_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/classes/com_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/fake_mysql_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/classes/server_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56478 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/classes/sql_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/classes/sql_statement_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/controllers/session_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/data_types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/data_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/data_types/mysql_datum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/binary_resultset_row_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_count_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_definition_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/command_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/eof_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/err_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/fast_auth_fail_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_response_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/ok_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/password_answer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/resultset_row_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/stmt_prepare_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_response_packet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/datahub/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/datahub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/datahub/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/datahub/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/datahub/classes/tables_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/datahub/datahub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/datanode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23115 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/information_schema_datanode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/integration_datanode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/project_datanode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/executor/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/executor/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/executor/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/executor/executor_client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67024 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/executor/executor_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/executor/executor_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/external_libs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/external_libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/external_libs/mysql_scramble.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/libs/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/libs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/libs/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/libs/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35316 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/libs/constants/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/libs/constants/response_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31908 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/mysql_proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/utilities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/utilities/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/utilities/lightwood_dtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/utilities/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/utilities/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/mysql/start.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/api/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/nlp/nlp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/api/postgres/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/postgres/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/api/postgres/postgres_proxy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/postgres/postgres_proxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/api/postgres/postgres_proxy/executor/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/postgres/postgres_proxy/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6543 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/postgres/postgres_proxy/executor/executor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/api/postgres/postgres_proxy/postgres_packets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/postgres/postgres_proxy/postgres_packets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12729 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/postgres/postgres_proxy/postgres_packets/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40804 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_identifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_packets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19291 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/postgres/postgres_proxy/postgres_proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/api/postgres/postgres_proxy/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/postgres/postgres_proxy/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/api/postgres/start.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/access_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/access_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/access_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/access_handler/access_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32145 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/access_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/access_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/access_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/access_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/access_handler/tests/test_access_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/airtable_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/airtable_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/airtable_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/airtable_handler/airtable_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/airtable_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/airtable_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/airtable_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/airtable_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/airtable_handler/tests/test_airtable_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/altibase_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/altibase_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/altibase_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/altibase_handler/altibase_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)   342129 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/altibase_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/altibase_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/altibase_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/altibase_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/altibase_handler/tests/test_altibase_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/aurora_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/aurora_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/aurora_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6404 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/aurora_handler/aurora_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11767 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/aurora_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/aurora_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/aurora_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/aurora_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_mysql_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_postgres_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/autokeras_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/autokeras_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/autokeras_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/autokeras_handler/autokeras_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/autokeras_handler/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/autokeras_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/autosklearn_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/autosklearn_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/autosklearn_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/autosklearn_handler/autosklearn_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/autosklearn_handler/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/autosklearn_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/autosklearn_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/bigquery_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/bigquery_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/bigquery_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/bigquery_handler/bigquery_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/bigquery_handler/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/bigquery_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/bigquery_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/bigquery_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/bigquery_handler/tests/test_bigquery_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/binance_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/binance_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/binance_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/binance_handler/binance_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/binance_handler/binance_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/binance_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/binance_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/byom_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/byom_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/byom_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6590 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/byom_handler/byom_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/byom_handler/proc_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/cassandra_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/cassandra_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/cassandra_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/cassandra_handler/cassandra_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)   176707 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/cassandra_handler/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/cassandra_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/cassandra_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/cassandra_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/cassandra_handler/tests/test_cassandra_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/ckan_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/ckan_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/ckan_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/ckan_handler/ckan_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17688 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/ckan_handler/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/ckan_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/ckan_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/ckan_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/ckan_handler/tests/test_ckan_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/clickhouse_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/clickhouse_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/clickhouse_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/clickhouse_handler/clickhouse_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/clickhouse_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/clickhouse_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/clickhouse_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/clickhouse_handler/tests/test_clickhouse_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/cloud_spanner_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/cloud_spanner_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/cloud_spanner_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/cloud_spanner_handler/cloud_spanner_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6419 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/cloud_spanner_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/cloud_spanner_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/cloud_spanner_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/cloud_spanner_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/cloud_spanner_handler/tests/test_cloud_spanner_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/cloud_sql_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/cloud_sql_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/cloud_sql_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/cloud_sql_handler/cloud_sql_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37571 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/cloud_sql_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/cloud_sql_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/cloud_sql_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/cloud_sql_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mssql_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mysql_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/cockroach_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/cockroach_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/cockroach_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/cockroach_handler/cockroach_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/cockroach_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/cockroach_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/cockroach_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/cockroach_handler/tests/test_cockroachdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/confluence_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/confluence_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/confluence_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/confluence_handler/confluence_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/confluence_handler/confluence_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76194 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/confluence_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/confluence_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/couchbase_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/couchbase_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/couchbase_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/couchbase_handler/couchbase_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/couchbase_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/couchbase_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/couchbase_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/couchbase_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/couchbase_handler/tests/test_couchbase_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/crate_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/crate_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/crate_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7157 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/crate_handler/crate_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/crate_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/crate_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/crate_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/crate_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/crate_handler/tests/test_crate_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/d0lt_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/d0lt_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/d0lt_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/d0lt_handler/d0lt_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/d0lt_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/d0lt_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/d0lt_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/d0lt_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/d0lt_handler/tests/test_d0lt_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/databend_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/databend_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/databend_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/databend_handler/databend_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6443 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/databend_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/databend_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/databend_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/databend_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/databend_handler/tests/test_databend_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/databricks_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/databricks_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/databricks_handler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/databricks_handler/databricks/
+-rw-r--r--   0 runner    (1001) docker     (123)    86110 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/databricks_handler/databricks/createdb.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    58645 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/databricks_handler/databricks/createpred.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    35986 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/databricks_handler/databricks/hivmetastore.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    21694 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/databricks_handler/databricks/mindsdbdatabricks.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    62078 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/databricks_handler/databricks/selectfrom.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     7952 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/databricks_handler/databricks_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12097 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/databricks_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/databricks_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/databricks_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/databricks_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/databricks_handler/tests/test_databricks_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/datastax_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/datastax_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/datastax_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/datastax_handler/datastax_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26175 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/datastax_handler/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/datastax_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/datastax_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/datastax_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/datastax_handler/tests/test_cassandra_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/db2_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/db2_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/db2_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9099 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/db2_handler/db2_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19117 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/db2_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/db2_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/db2_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/db2_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/db2_handler/tests/test_db2_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/derby_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/derby_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/derby_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8751 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/derby_handler/derby_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7305 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/derby_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/derby_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/derby_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/derby_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/derby_handler/tests/test_derby_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/dremio_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/dremio_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/dremio_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/dremio_handler/dremio_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52734 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/dremio_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/dremio_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/dremio_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/dremio_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/dremio_handler/tests/test_dremio_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/druid_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/druid_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/druid_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7324 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/druid_handler/druid_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29112 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/druid_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/druid_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/druid_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/druid_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/druid_handler/tests/test_druid_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/duckdb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/duckdb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/duckdb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/duckdb_handler/duckdb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19548 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/duckdb_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/duckdb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/duckdb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/duckdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/duckdb_handler/tests/test_duckdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/dynamodb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/dynamodb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/dynamodb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/dynamodb_handler/dynamodb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55623 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/dynamodb_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/dynamodb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/dynamodb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/dynamodb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/dynamodb_handler/tests/test_dynamodb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/edgelessdb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/edgelessdb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/edgelessdb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/edgelessdb_handler/edgelessdb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/edgelessdb_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/edgelessdb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/edgelessdb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/edgelessdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/edgelessdb_handler/tests/test_edgelessdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/elasticsearch_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/elasticsearch_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/elasticsearch_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/elasticsearch_handler/elasticsearch_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/elasticsearch_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/elasticsearch_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/elasticsearch_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/elasticsearch_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/elasticsearch_handler/tests/test_elasticsearch_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/empress_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/empress_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/empress_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/empress_handler/empress_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11249 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/empress_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/empress_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/empress_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/empress_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/empress_handler/tests/test_empress_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/eventstoredb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/eventstoredb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/eventstoredb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9062 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/eventstoredb_handler/eventstoredb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/eventstoredb_handler/icon.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/file_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/file_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/file_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10837 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/file_handler/file_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/firebird_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/firebird_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/firebird_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/firebird_handler/firebird_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54033 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/firebird_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/firebird_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/firebird_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/firebird_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/firebird_handler/tests/test_firebird_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/github_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/github_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/github_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/github_handler/github_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11793 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/github_handler/github_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/github_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/github_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/google_calendar_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/google_calendar_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/google_calendar_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/google_calendar_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/google_calendar_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/google_calendar_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/google_calendar_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/google_calendar_handler/tests/test_google_calendar_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/hana_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/hana_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/hana_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11104 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/hana_handler/hana_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/hana_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/hana_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/hive_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/hive_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/hive_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/hive_handler/hive_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14000 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/hive_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/hive_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/hive_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/hive_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/hive_handler/tests/test_hive_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/hsqldb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/hsqldb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/hsqldb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7491 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/hsqldb_handler/hsqldb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/hsqldb_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/hsqldb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/huggingface_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/huggingface_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/huggingface_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11247 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/huggingface_handler/huggingface_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/huggingface_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/huggingface_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/ignite_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/ignite_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/ignite_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45779 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/ignite_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/ignite_handler/ignite_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/ignite_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/ignite_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/ignite_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/ignite_handler/tests/test_ignite_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/impala_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/impala_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/impala_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/impala_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/impala_handler/impala_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/impala_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/impala_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/impala_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/impala_handler/tests/test_impala_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/influxdb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/influxdb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/influxdb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63375 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/influxdb_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/influxdb_handler/influxdb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/influxdb_handler/influxdb_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/influxdb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/informix_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/informix_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/informix_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6694 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/informix_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9618 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/informix_handler/informix_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/informix_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/informix_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/informix_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/informix_handler/tests/test_informix_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/ingres_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/ingres_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/ingres_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/ingres_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/ingres_handler/ingres_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/ingres_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/ingres_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/ingres_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/ingres_handler/tests/test_ingres_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/jira_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/jira_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/jira_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16812 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/jira_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/jira_handler/jira_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5493 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/jira_handler/jira_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/jira_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/langchain_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/langchain_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/langchain_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10109 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/langchain_handler/langchain_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/langchain_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/langchain_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/lightwood_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/lightwood_handler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8825 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20696 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/lightwood_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/lightwood_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/lightwood_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/lightwood_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/lightwood_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10985 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/lightwood_handler/tests/test_lightwood_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/ludwig_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/ludwig_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/ludwig_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/ludwig_handler/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/ludwig_handler/ludwig_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/ludwig_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/ludwig_handler/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/ludwig_handler/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/mariadb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/mariadb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/mariadb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99045 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/mariadb_handler/create-db.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/mariadb_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/mariadb_handler/mariadb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98530 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/mariadb_handler/predict-db.png
+-rw-r--r--   0 runner    (1001) docker     (123)   100718 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/mariadb_handler/predictor.png
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/mariadb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/materialize_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/materialize_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/materialize_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47935 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/materialize_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/materialize_handler/materialize_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/materialize_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/materialize_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/materialize_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/materialize_handler/tests/test_materialize_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/matrixone_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/matrixone_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/matrixone_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57976 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/matrixone_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/matrixone_handler/matrixone_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/matrixone_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/matrixone_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/matrixone_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/matrixone_handler/tests/test_matrixone_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/merlion_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/merlion_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/merlion_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8498 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/merlion_handler/adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8217 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/merlion_handler/merlion_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/merlion_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/merlion_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/mlflow_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/mlflow_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/mlflow_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/mlflow_handler/mlflow_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/mlflow_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/mlflow_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/monetdb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/monetdb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/monetdb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64685 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/monetdb_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8113 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/monetdb_handler/monetdb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/monetdb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/monetdb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/monetdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/monetdb_handler/tests/test_monetdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/monetdb_handler/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/monetdb_handler/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/monetdb_handler/utils/monet_get_id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/mongodb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/mongodb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/mongodb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15045 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/mongodb_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/mongodb_handler/mongodb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/mongodb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/mongodb_handler/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/mongodb_handler/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6410 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/mongodb_handler/utils/mongodb_render.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/mssql_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/mssql_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/mssql_handler/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14543 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/mssql_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/mssql_handler/mssql_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/mssql_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/mssql_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/mssql_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/mssql_handler/tests/test_mssql_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/mysql_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/mysql_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/mysql_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/mysql_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6812 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/mysql_handler/mysql_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/mysql_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/neuralforecast_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/neuralforecast_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/neuralforecast_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/neuralforecast_handler/neuralforecast_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/neuralforecast_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/neuralforecast_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/nuo_jdbc_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/nuo_jdbc_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/nuo_jdbc_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    95071 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/nuo_jdbc_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9833 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/nuo_jdbc_handler/nuo_jdbc_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/nuo_jdbc_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/test_nuo_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/oceanbase_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/oceanbase_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/oceanbase_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37289 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/oceanbase_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/oceanbase_handler/oceanbase_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/oceanbase_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/oceanbase_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/oceanbase_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/oceanbase_handler/tests/test_oceanbase_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/openai_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/openai_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/openai_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/openai_handler/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27870 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/openai_handler/openai_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/openai_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/openai_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/opengauss_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/opengauss_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/opengauss_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/opengauss_handler/opengauss_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/opengauss_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/opengauss_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/opengauss_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/opengauss_handler/tests/test_opengauss_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/oracle_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/oracle_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/oracle_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/oracle_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/oracle_handler/oracle_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/oracle_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/oracle_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/oracle_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/oracle_handler/tests/test_oracle_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/orioledb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/orioledb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/orioledb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/orioledb_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/orioledb_handler/orioledb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/orioledb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/orioledb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/orioledb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/orioledb_handler/tests/test_orioledb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/phoenix_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/phoenix_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/phoenix_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/phoenix_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8767 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/phoenix_handler/phoenix_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/phoenix_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/phoenix_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/phoenix_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/phoenix_handler/tests/test_phoenix_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/pinot_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/pinot_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/pinot_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18645 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/pinot_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8577 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/pinot_handler/pinot_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/pinot_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/pinot_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/pinot_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/pinot_handler/tests/test_pinot_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/plaid_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/plaid_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/plaid_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/plaid_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8076 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/plaid_handler/plaid_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/plaid_handler/plaid_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/plaid_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/plaid_handler/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/planetscale_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/planetscale_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/planetscale_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/planetscale_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/planetscale_handler/planetscale_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/planetscale_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/postgres_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/postgres_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/postgres_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15261 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/postgres_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5725 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/postgres_handler/postgres_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/postgres_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/questdb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/questdb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/questdb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/questdb_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/questdb_handler/questdb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/questdb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/questdb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/questdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/questdb_handler/tests/test_questdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/ray_serve_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/ray_serve_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/ray_serve_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/ray_serve_handler/ray_serve_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/ray_serve_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/ray_serve_handler/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/reddit_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/reddit_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/reddit_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/reddit_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/reddit_handler/reddit_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6558 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/reddit_handler/reddit_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/reddit_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/redshift_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/redshift_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/redshift_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17615 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/redshift_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7319 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/redshift_handler/redshift_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/redshift_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/redshift_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/redshift_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/redshift_handler/tests/test_redshift_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/rockset_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)    22361 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/rockset_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/rockset_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/rockset_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)   194064 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/rockset_handler/tests/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)   108141 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/rockset_handler/tests/test2.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/s3_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/s3_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/s3_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24332 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/s3_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/s3_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/s3_handler/s3_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/s3_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/s3_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/s3_handler/tests/test_s3_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/scylla_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/scylla_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/scylla_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40148 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/scylla_handler/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/scylla_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/scylla_handler/scylla_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/scylla_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/scylla_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/scylla_handler/tests/test_scylla_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/sheets_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/sheets_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/sheets_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27211 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/sheets_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/sheets_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/sheets_handler/sheets_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/sheets_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/sheets_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/sheets_handler/tests/test_sheets_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/singlestore_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/singlestore_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/singlestore_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/singlestore_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/singlestore_handler/singlestore_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/singlestore_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/singlestore_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/singlestore_handler/tests/test_singlestore_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/snowflake_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/snowflake_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/snowflake_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/snowflake_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/snowflake_handler/snowflake_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/snowflake_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/snowflake_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/snowflake_handler/tests/test_snowflake_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/solr_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/solr_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/solr_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/solr_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/solr_handler/solr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/solr_handler/solr_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/solr_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/solr_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/solr_handler/tests/test_solr_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/sqlany_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/sqlany_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/sqlany_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/sqlany_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/sqlany_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/sqlany_handler/sqlany_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/sqlite_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/sqlite_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/sqlite_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   521282 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/sqlite_handler/db_connection.png
+-rw-r--r--   0 runner    (1001) docker     (123)   369371 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/sqlite_handler/error.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11559 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/sqlite_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)   479779 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/sqlite_handler/model_drop.png
+-rw-r--r--   0 runner    (1001) docker     (123)   477242 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/sqlite_handler/prediction_result.png
+-rw-r--r--   0 runner    (1001) docker     (123)   552154 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/sqlite_handler/predictor_model.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/sqlite_handler/sqlite_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/sqlite_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/sqlite_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/sqlite_handler/tests/test_sqlite_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/sqreamdb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/sqreamdb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/sqreamdb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/sqreamdb_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/sqreamdb_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/sqreamdb_handler/sqreamdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/sqreamdb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/sqreamdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/sqreamdb_handler/tests/test_sqreamdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/starrocks_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/starrocks_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/starrocks_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72778 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/starrocks_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/starrocks_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/starrocks_handler/starrocks_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/starrocks_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/starrocks_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/starrocks_handler/tests/test_starrocks_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/statsforecast_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/statsforecast_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/statsforecast_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/statsforecast_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/statsforecast_handler/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7584 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/statsforecast_handler/statsforecast_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/supabase_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/supabase_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/supabase_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/supabase_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/supabase_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/supabase_handler/supabase_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/supabase_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/supabase_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/supabase_handler/tests/test_supabase_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/surrealdb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/surrealdb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/surrealdb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25475 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/surrealdb_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/surrealdb_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7116 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/surrealdb_handler/surrealdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/surrealdb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/surrealdb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/surrealdb_handler/tests/test_surrealdb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/surrealdb_handler/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/surrealdb_handler/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/surrealdb_handler/utils/surreal_get_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/tdengine_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/tdengine_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/tdengine_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/tdengine_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/tdengine_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/tdengine_handler/tdengine_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/tdengine_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/tdengine_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/tdengine_handler/tests/test_tdengine_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/teradata_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/teradata_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/teradata_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/teradata_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/teradata_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/teradata_handler/teradata_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/tidb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/tidb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/tidb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/tidb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/tidb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/tidb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/tidb_handler/tests/test_tidb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/tidb_handler/tidb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/timescaledb_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/timescaledb_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/timescaledb_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11184 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/timescaledb_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/timescaledb_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/timescaledb_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/timescaledb_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/timescaledb_handler/tests/test_timescaledb_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/timescaledb_handler/timescaledb_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/tpot_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/tpot_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/tpot_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/tpot_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/tpot_handler/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/tpot_handler/tpot_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/trino_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/trino_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/trino_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13752 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/trino_handler/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/trino_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/trino_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/trino_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/trino_handler/tests/test_trino_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/trino_handler/trino_config_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/trino_handler/trino_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/twitter_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/twitter_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/twitter_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/twitter_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/twitter_handler/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16126 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/twitter_handler/twitter_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/vertica_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/vertica_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/vertica_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/vertica_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/vertica_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/vertica_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/vertica_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/vertica_handler/tests/test_vertica_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/vertica_handler/vertica_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/vitess_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/vitess_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/vitess_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/vitess_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/vitess_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/vitess_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/vitess_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/vitess_handler/tests/test_vitess_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/vitess_handler/vitess_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/yugabyte_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/yugabyte_handler/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/yugabyte_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16563 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/yugabyte_handler/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/yugabyte_handler/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/yugabyte_handler/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/yugabyte_handler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/yugabyte_handler/tests/test_yugabyte_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers/yugabyte_handler/yugabyte_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers_client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers_client/db_client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers_client/db_grpc_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers_client/ml_client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers_client/ml_grpc_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers_wrapper/db_grpc_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers_wrapper/db_handler_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers_wrapper/ml_grpc_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/handlers_wrapper/ml_handler_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/libs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/libs/api_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7147 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/libs/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/libs/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/libs/handler_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17360 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/libs/ml_exec_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/libs/ml_handler_proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/libs/net_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/libs/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/libs/storage_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/integrations/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/utilities/date_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/utilities/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/utilities/processes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/utilities/sql_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/utilities/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/utilities/time_series_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/integrations/utilities/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/interfaces/database/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/interfaces/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/interfaces/database/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18638 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/interfaces/database/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9095 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/interfaces/database/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/interfaces/database/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/interfaces/file/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/interfaces/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/interfaces/file/file_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/interfaces/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/interfaces/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13068 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/interfaces/jobs/jobs_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/interfaces/jobs/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/interfaces/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/interfaces/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/interfaces/model/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21478 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/interfaces/model/model_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/interfaces/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/interfaces/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9337 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/interfaces/storage/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10434 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/interfaces/storage/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/interfaces/storage/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/interfaces/storage/model_fs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/interfaces/stream/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/interfaces/stream/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/interfaces/stream/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/interfaces/stream/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/interfaces/stream/base/integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/interfaces/stream/kafka/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/interfaces/stream/kafka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/interfaces/stream/kafka/kafkadb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/interfaces/stream/redis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/interfaces/stream/redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/interfaces/stream/redis/redisdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/interfaces/stream/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/interfaces/stream/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/microservices_grpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/microservices_grpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/microservices_grpc/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/microservices_grpc/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/microservices_grpc/db/common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/microservices_grpc/db/common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/microservices_grpc/db/db_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12845 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/microservices_grpc/db/db_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/microservices_grpc/executor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/microservices_grpc/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/microservices_grpc/executor/executor_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14810 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/microservices_grpc/executor/executor_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/microservices_grpc/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/microservices_grpc/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/microservices_grpc/ml/common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/microservices_grpc/ml/common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/microservices_grpc/ml/ml_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/microservices_grpc/ml/ml_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/migrations/alembic.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/migrations/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/migrations/migrate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/migrations/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/migrations/versions/2021-11-30_17c3d2384711_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/migrations/versions/2022-01-26_47f97b83cee4_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10808 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/migrations/versions/2022-02-09_27c5aca9e47e_db_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/migrations/versions/2022-05-25_d74c189b87e6_predictor_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/migrations/versions/2022-07-08_999bceb904df_integration_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/migrations/versions/2022-07-15_b5b53e0ea7f8_training_data_rows_columns_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/migrations/versions/2022-07-22_6e834843e7e9_training_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/migrations/versions/2022-08-19_976f15a37e6a_predictors_versioning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/migrations/versions/2022-08-25_6a54ba55872e_view_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/migrations/versions/2022-08-29_473e8f239481_straighten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/migrations/versions/2022-09-06_96d5fef10caa_data_integration_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/migrations/versions/2022-09-08_87b2df2b83e1_predictor_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/migrations/versions/2022-09-19_3d5e70105df7_content_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/migrations/versions/2022-09-29_cada7d2be947_json_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/migrations/versions/2022-10-14_43c52d23845a_projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/migrations/versions/2022-11-07_1e60096fc817_predictor_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/migrations/versions/2022-11-11_d429095b570f_data_integration_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/migrations/versions/2022-12-26_459218b0844c_fix_unique_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/migrations/versions/2023-02-02_b6d0a47294ac_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/migrations/versions/2023-02-17_ee63d868fa84_predictor_integration_null.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/migrations/versions/2023-02-25_3154382dab17_training_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/migrations/versions/2023-02-27_ef04cdbe51ed_jobs_user_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/migrations/versions/2023-04-11_b8be148dbc85_jobs_history_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/migrations/versions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/utilities/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/utilities/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/utilities/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/utilities/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/utilities/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/utilities/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/utilities/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/utilities/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/utilities/hooks/profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/utilities/json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/utilities/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/utilities/log_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/mindsdb/utilities/profiler/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/utilities/profiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/utilities/profiler/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/utilities/ps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/utilities/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/mindsdb/utilities/wizards.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 09:30:45.000000 MindsDB-23.4.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-04-28 09:30:31.000000 MindsDB-23.4.4.3/setup.py
```

### Comparing `MindsDB-23.4.4.2/MindsDB.egg-info/PKG-INFO` & `MindsDB-23.4.4.3/MindsDB.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MindsDB
-Version: 23.4.4.2
+Version: 23.4.4.3
 Summary: MindsDB server, provides server capabilities to mindsdb native python library
 Home-page: https://github.com/mindsdb/mindsdb
 Author: MindsDB Inc
 Author-email: jorge@mindsdb.com
 License: GPL-3.0
 Download-URL: https://pypi.org/project/mindsdb/
 Description: <h1 align="center">
@@ -125,23 +125,23 @@
         
         MindsDB works with most of the SQL and NoSQL databases, data lakes, data Streams and popular applications.
         
         | Connect your Data | Connect your Data | Connect your Data
         |-|-|-|
         | <a href="https://docs.mindsdb.com/connect/kafka"><img src="https://img.shields.io/badge/Apache Kafka-808080?style=for-the-badge&logo=apache-kafka&logoColor=white" alt="Connect Apache Kafka"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#microsoft-access"><img src="https://img.shields.io/badge/Microsoft%20Access-A4373A?logo=microsoftaccess&logoColor=fff&style=for-the-badge" alt="Connect Microsoft Access"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#oracle"><img src="https://img.shields.io/badge/Oracle-F80000?logo=oracle&logoColor=fff&style=for-the-badge" alt="Oracle Badge"></a> |
         | <a href=" https://docs.mindsdb.com/data-integrations/all-data-integrations#amazon-redshift"><img src="https://img.shields.io/badge/Amazon%20Redshift-0466C8?style=for-the-badge&logo=amazon-aws&logoColor=white" alt="Connect Amazon Redshift"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#airtable"><img src="https://img.shields.io/badge/Airtable-18BFFF?logo=airtable&logoColor=fff&style=for-the-badge" alt="Airtable Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/Apache-Pinot"><img src="https://img.shields.io/badge/Pinot-000?logo=pinot&logoColor=fff&style=for-the-badge" alt="Pinot Badge"></a> |
-        | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#cassandra"><img src="https://img.shields.io/badge/Cassandra-1287B1?style=for-the-badge&logo=apache%20cassandra&logoColor=white" alt="Connect Cassandra"></a> | <a href=" https://docs.mindsdb.com/data-integrations/all-data-integrations#datastax"><img src="https://img.shields.io/badge/DataStax-3A3A42?logo=datastax&logoColor=fff&style=for-the-badge" alt="DataStax Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#s3"><img src="https://img.shields.io/badge/Amazon%20S3-569A31?logo=amazons3&logoColor=fff&style=for-the-badge" alt="Amazon S3 Badge"></a> |
+        | <a href="https://docs.mindsdb.com/data-integrations/apache-cassandra"><img src="https://img.shields.io/badge/Cassandra-1287B1?style=for-the-badge&logo=apache%20cassandra&logoColor=white" alt="Connect Cassandra"></a> | <a href=" https://docs.mindsdb.com/data-integrations/all-data-integrations#datastax"><img src="https://img.shields.io/badge/DataStax-3A3A42?logo=datastax&logoColor=fff&style=for-the-badge" alt="DataStax Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#s3"><img src="https://img.shields.io/badge/Amazon%20S3-569A31?logo=amazons3&logoColor=fff&style=for-the-badge" alt="Amazon S3 Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/cockroachdb"><img src="https://img.shields.io/badge/CockroachDB-426EDF?style=for-the-badge&logo=cockroach-labs&logoColor=white" alt="Connect CockroachDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/ckan"><img src="https://img.shields.io/badge/ckan-7D929E?logo=ckan&logoColor=fff&style=for-the-badge" alt="ckan Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#supabase"><img src="https://img.shields.io/badge/Supabase-3ECF8E?logo=supabase&logoColor=fff&style=for-the-badge" alt="Supabase Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#clickhouse"><img src="https://img.shields.io/badge/Clickhouse-e6e600?style=for-the-badge&logo=clickhouse&logoColor=white" alt="Connect Clickhouse"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#google-bigquery"><img src="https://img.shields.io/badge/Google Big Query-0466C8?logo=Big Query&logoColor=fff&style=for-the-badge" alt="Google Big Query Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#sqlite"><img src="https://img.shields.io/badge/SQLite-003B57?logo=sqlite&logoColor=fff&style=for-the-badge" alt="SQLite Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#mariadb"><img src="https://img.shields.io/badge/MariaDB-003545?style=for-the-badge&logo=mariadb&logoColor=white" alt="Connect MariaDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#couchbase"><img src="https://img.shields.io/badge/Couchbase-EA2328?logo=couchbase&logoColor=fff&style=for-the-badge" alt="Couchbase Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/TiDB#tidb-handler"><img src="https://img.shields.io/badge/TiDB-DD0031?logo=tidb&logoColor=fff&style=for-the-badge" alt="TiDB Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#microsoft-sql-server"><img src="https://img.shields.io/badge/Microsoft%20SQL%20Sever-CC2927?style=for-the-badge&logo=microsoft%20sql%20server&logoColor=white" alt="Connect SQL Server"></a> | <a href="https://docs.mindsdb.com/data-integrations/cratedb"><img src="https://img.shields.io/badge/CrateDB-009DC7?logo=cratedb&logoColor=fff&style=for-the-badge" alt="CrateDB Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#timescaledb"><img src="https://img.shields.io/badge/Timescale-FDB515?logo=timescale&logoColor=fff&style=for-the-badge" alt="Timescale Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#mongodb"><img src="https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white" alt="Connect MongoDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#d0lt"><img src="https://img.shields.io/badge/DoIt-00B388?logo=DoIt&logoColor=fff&style=for-the-badge" alt="DoIt Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#aws-dynamodb"><img src="https://img.shields.io/badge/Amazon%20DynamoDB-4053D6?logo=amazondynamodb&logoColor=fff&style=for-the-badge" alt="Amazon DynamoDB Badge"></a> |
-        | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#postgresql"><img src="https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white" alt="Connect PostgreSQL"></a> | <a href="https://docs.mindsdb.com/data-integrations/db2"><img src="https://img.shields.io/badge/IBMDB2-008000?logo=IBMDB2&logoColor=fff&style=for-the-badge" alt="IBMDB2 Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#opengauss"><img src="https://img.shields.io/badge/openGauss-02458D?logo=opengauss&logoColor=fff&style=for-the-badge" alt="openGauss Badge"></a> |
+        | <a href="https://docs.mindsdb.com/data-integrations/postgresql"><img src="https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white" alt="Connect PostgreSQL"></a> | <a href="https://docs.mindsdb.com/data-integrations/db2"><img src="https://img.shields.io/badge/IBMDB2-008000?logo=IBMDB2&logoColor=fff&style=for-the-badge" alt="IBMDB2 Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#opengauss"><img src="https://img.shields.io/badge/openGauss-02458D?logo=opengauss&logoColor=fff&style=for-the-badge" alt="openGauss Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#mysql"><img src="https://img.shields.io/badge/MySQL-00758F?style=for-the-badge&logo=mysql&logoColor=white" alt="Connect MySQL"></a> | <a href=" https://docs.mindsdb.com/data-integrations/all-data-integrations#databricks"><img src="https://img.shields.io/badge/Databricks-FF3621?logo=databricks&logoColor=fff&style=for-the-badge" alt="Databricks Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#yugabyte"><img src="https://img.shields.io/badge/YugabyteDB-02458D?logo=yugabytedb&logoColor=fff&style=for-the-badge" alt="YugabyteDB Badge"></a>
-        | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#questdb"><img src="https://img.shields.io/badge/QuestDB-d14671?style=for-the-badge&logo=questdb&logoColor=white" alt="Connect QuestDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#druid"><img src="https://img.shields.io/badge/Apache%20Druid-29F1FB?logo=apachedruid&logoColor=000&style=for-the-badge" alt="Apache Druid Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#starrocks"><img src="https://img.shields.io/badge/starrocks-000000?style=for-the-badge&logo=starrocks&logoColor=white" alt="StarRocks Badge"></a> |
+        | <a href="https://docs.mindsdb.com/data-integrations/questdb"><img src="https://img.shields.io/badge/QuestDB-d14671?style=for-the-badge&logo=questdb&logoColor=white" alt="Connect QuestDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#druid"><img src="https://img.shields.io/badge/Apache%20Druid-29F1FB?logo=apachedruid&logoColor=000&style=for-the-badge" alt="Apache Druid Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#starrocks"><img src="https://img.shields.io/badge/starrocks-000000?style=for-the-badge&logo=starrocks&logoColor=white" alt="StarRocks Badge"></a> |
         | <a href="https://docs.mindsdb.com/"><img src="https://img.shields.io/badge/redis-%23DD0031.svg?&style=for-the-badge&logo=redis&logoColor=white" alt="Connect Redis"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#vertica"><img src="https://img.shields.io/badge/Vertica-000?logo=vertica&logoColor=fff&style=for-the-badge" alt="Vertica Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#duckdb"><img src="https://img.shields.io/badge/duckdb-fff?logo=duckdb&logoColor=000&style=for-the-badge" alt="DuckDB Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#sap-hana"><img src="https://img.shields.io/badge/SAP%20HANA-1661BE?style=for-the-badge&logo=sap&logoColor=white" alt="Connect SAP HANA"></a> | <a href=" https://docs.mindsdb.com/data-integrations/all-data-integrations#elastic-search"><img src="https://img.shields.io/badge/Elastic-005571?logo=elastic&logoColor=fff&style=for-the-badge" alt="Elastic Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#cloud-spanner"><img src="https://img.shields.io/badge/Cloud%20Spanner-4285F4?style=for-the-badge" alt="Cloud Spanner Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#scylla"><img src="https://img.shields.io/badge/ScyllaDB-53CADD?style=for-the-badge&logo=scylladbb&logoColor=white" alt="Connect ScyllaDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#firebird"><img src="https://img.shields.io/badge/Firebird-F40D12?logo=Firebird&logoColor=fff&style=for-the-badge" alt="Firebird Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#singlestore"><img src="https://img.shields.io/badge/Singlestore-5f07b4?style=for-the-badge&logo=singlestore&logoColor=white" alt="Connect Singlestore"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#hive"><img src="https://img.shields.io/badge/Apache%20Hive-FDEE21?logo=apachehive&logoColor=000&style=for-the-badge" alt="Apache Hive Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#teradata"><img src="https://img.shields.io/badge/Teradata-e36c42?style=for-the-badge&logo=teradata&logoColor=white" alt="Connect Teradata"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#matrix-one"><img src="https://img.shields.io/badge/Matrixone-02458D?logo=Matrixone&logoColor=fff&style=for-the-badge" alt="Matrixone Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#snowflake"><img src="https://img.shields.io/badge/Snowflake-35aedd?style=for-the-badge&logo=snowflake&logoColor=blue" alt="Connect Snowflake"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#informix"><img src="https://img.shields.io/badge/Informix-191A1B?logo=informix&logoColor=fff&style=for-the-badge" alt="Informix Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#trino"><img src="https://img.shields.io/badge/Trino-dd00a1?style=for-the-badge&logo=trino&logoColor=white" alt="Connect Trino"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#monetdb"><img src="https://img.shields.io/badge/Monetdb-0099E5?logo=Monetdb&logoColor=fff&style=for-the-badge" alt="Monetdb Badge"></a> |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: MindsDB Version: 23.4.4.2 Summary: MindsDB server,
+Metadata-Version: 2.1 Name: MindsDB Version: 23.4.4.3 Summary: MindsDB server,
 provides server capabilities to mindsdb native python library Home-page: https:
 //github.com/mindsdb/mindsdb Author: MindsDB Inc Author-email:
 jorge@mindsdb.com License: GPL-3.0 Download-URL: https://pypi.org/project/
 mindsdb/ Description:
                                ****** [MindsDB]
                                      ******
       [ROSS_Index_-_Fastest_Growing_Open-Source_Startups_|_Runa_Capital]
```

### Comparing `MindsDB-23.4.4.2/MindsDB.egg-info/SOURCES.txt` & `MindsDB-23.4.4.3/MindsDB.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -471,17 +471,16 @@
 mindsdb/integrations/handlers/ingres_handler/requirements.txt
 mindsdb/integrations/handlers/ingres_handler/tests/__init__.py
 mindsdb/integrations/handlers/ingres_handler/tests/test_ingres_handler.py
 mindsdb/integrations/handlers/jira_handler/__about__.py
 mindsdb/integrations/handlers/jira_handler/__init__.py
 mindsdb/integrations/handlers/jira_handler/icon.png
 mindsdb/integrations/handlers/jira_handler/jira_handler.py
+mindsdb/integrations/handlers/jira_handler/jira_table.py
 mindsdb/integrations/handlers/jira_handler/requirements.txt
-mindsdb/integrations/handlers/jira_handler/tests/__init__.py
-mindsdb/integrations/handlers/jira_handler/tests/test_jira_handler.py
 mindsdb/integrations/handlers/langchain_handler/__about__.py
 mindsdb/integrations/handlers/langchain_handler/__init__.py
 mindsdb/integrations/handlers/langchain_handler/langchain_handler.py
 mindsdb/integrations/handlers/langchain_handler/requirements.txt
 mindsdb/integrations/handlers/langchain_handler/setup.py
 mindsdb/integrations/handlers/lightwood_handler/__init__.py
 mindsdb/integrations/handlers/lightwood_handler/requirements.txt
```

### Comparing `MindsDB-23.4.4.2/MindsDB.egg-info/requires.txt` & `MindsDB-23.4.4.3/MindsDB.egg-info/requires.txt`

 * *Files 15% similar despite different names*

```diff
@@ -28,12 +28,12 @@
 mysql-connector-python
 clickhouse-driver
 clickhouse-sqlalchemy
 charset-normalizer
 dill>=0.3.4
 pyOpenSSL>=22.0.0
 pydateinfer==0.3.0
-pyarrow<10.0.0,>=9.0.0
+pyarrow<10.1.0,>=10.0.1
 dataprep_ml
 grpcio-tools
 python-magic>=0.4.27
 openpyxl>=3.1.1
```

### Comparing `MindsDB-23.4.4.2/PKG-INFO` & `MindsDB-23.4.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MindsDB
-Version: 23.4.4.2
+Version: 23.4.4.3
 Summary: MindsDB server, provides server capabilities to mindsdb native python library
 Home-page: https://github.com/mindsdb/mindsdb
 Author: MindsDB Inc
 Author-email: jorge@mindsdb.com
 License: GPL-3.0
 Download-URL: https://pypi.org/project/mindsdb/
 Description: <h1 align="center">
@@ -125,23 +125,23 @@
         
         MindsDB works with most of the SQL and NoSQL databases, data lakes, data Streams and popular applications.
         
         | Connect your Data | Connect your Data | Connect your Data
         |-|-|-|
         | <a href="https://docs.mindsdb.com/connect/kafka"><img src="https://img.shields.io/badge/Apache Kafka-808080?style=for-the-badge&logo=apache-kafka&logoColor=white" alt="Connect Apache Kafka"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#microsoft-access"><img src="https://img.shields.io/badge/Microsoft%20Access-A4373A?logo=microsoftaccess&logoColor=fff&style=for-the-badge" alt="Connect Microsoft Access"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#oracle"><img src="https://img.shields.io/badge/Oracle-F80000?logo=oracle&logoColor=fff&style=for-the-badge" alt="Oracle Badge"></a> |
         | <a href=" https://docs.mindsdb.com/data-integrations/all-data-integrations#amazon-redshift"><img src="https://img.shields.io/badge/Amazon%20Redshift-0466C8?style=for-the-badge&logo=amazon-aws&logoColor=white" alt="Connect Amazon Redshift"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#airtable"><img src="https://img.shields.io/badge/Airtable-18BFFF?logo=airtable&logoColor=fff&style=for-the-badge" alt="Airtable Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/Apache-Pinot"><img src="https://img.shields.io/badge/Pinot-000?logo=pinot&logoColor=fff&style=for-the-badge" alt="Pinot Badge"></a> |
-        | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#cassandra"><img src="https://img.shields.io/badge/Cassandra-1287B1?style=for-the-badge&logo=apache%20cassandra&logoColor=white" alt="Connect Cassandra"></a> | <a href=" https://docs.mindsdb.com/data-integrations/all-data-integrations#datastax"><img src="https://img.shields.io/badge/DataStax-3A3A42?logo=datastax&logoColor=fff&style=for-the-badge" alt="DataStax Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#s3"><img src="https://img.shields.io/badge/Amazon%20S3-569A31?logo=amazons3&logoColor=fff&style=for-the-badge" alt="Amazon S3 Badge"></a> |
+        | <a href="https://docs.mindsdb.com/data-integrations/apache-cassandra"><img src="https://img.shields.io/badge/Cassandra-1287B1?style=for-the-badge&logo=apache%20cassandra&logoColor=white" alt="Connect Cassandra"></a> | <a href=" https://docs.mindsdb.com/data-integrations/all-data-integrations#datastax"><img src="https://img.shields.io/badge/DataStax-3A3A42?logo=datastax&logoColor=fff&style=for-the-badge" alt="DataStax Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#s3"><img src="https://img.shields.io/badge/Amazon%20S3-569A31?logo=amazons3&logoColor=fff&style=for-the-badge" alt="Amazon S3 Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/cockroachdb"><img src="https://img.shields.io/badge/CockroachDB-426EDF?style=for-the-badge&logo=cockroach-labs&logoColor=white" alt="Connect CockroachDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/ckan"><img src="https://img.shields.io/badge/ckan-7D929E?logo=ckan&logoColor=fff&style=for-the-badge" alt="ckan Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#supabase"><img src="https://img.shields.io/badge/Supabase-3ECF8E?logo=supabase&logoColor=fff&style=for-the-badge" alt="Supabase Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#clickhouse"><img src="https://img.shields.io/badge/Clickhouse-e6e600?style=for-the-badge&logo=clickhouse&logoColor=white" alt="Connect Clickhouse"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#google-bigquery"><img src="https://img.shields.io/badge/Google Big Query-0466C8?logo=Big Query&logoColor=fff&style=for-the-badge" alt="Google Big Query Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#sqlite"><img src="https://img.shields.io/badge/SQLite-003B57?logo=sqlite&logoColor=fff&style=for-the-badge" alt="SQLite Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#mariadb"><img src="https://img.shields.io/badge/MariaDB-003545?style=for-the-badge&logo=mariadb&logoColor=white" alt="Connect MariaDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#couchbase"><img src="https://img.shields.io/badge/Couchbase-EA2328?logo=couchbase&logoColor=fff&style=for-the-badge" alt="Couchbase Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/TiDB#tidb-handler"><img src="https://img.shields.io/badge/TiDB-DD0031?logo=tidb&logoColor=fff&style=for-the-badge" alt="TiDB Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#microsoft-sql-server"><img src="https://img.shields.io/badge/Microsoft%20SQL%20Sever-CC2927?style=for-the-badge&logo=microsoft%20sql%20server&logoColor=white" alt="Connect SQL Server"></a> | <a href="https://docs.mindsdb.com/data-integrations/cratedb"><img src="https://img.shields.io/badge/CrateDB-009DC7?logo=cratedb&logoColor=fff&style=for-the-badge" alt="CrateDB Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#timescaledb"><img src="https://img.shields.io/badge/Timescale-FDB515?logo=timescale&logoColor=fff&style=for-the-badge" alt="Timescale Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#mongodb"><img src="https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white" alt="Connect MongoDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#d0lt"><img src="https://img.shields.io/badge/DoIt-00B388?logo=DoIt&logoColor=fff&style=for-the-badge" alt="DoIt Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#aws-dynamodb"><img src="https://img.shields.io/badge/Amazon%20DynamoDB-4053D6?logo=amazondynamodb&logoColor=fff&style=for-the-badge" alt="Amazon DynamoDB Badge"></a> |
-        | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#postgresql"><img src="https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white" alt="Connect PostgreSQL"></a> | <a href="https://docs.mindsdb.com/data-integrations/db2"><img src="https://img.shields.io/badge/IBMDB2-008000?logo=IBMDB2&logoColor=fff&style=for-the-badge" alt="IBMDB2 Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#opengauss"><img src="https://img.shields.io/badge/openGauss-02458D?logo=opengauss&logoColor=fff&style=for-the-badge" alt="openGauss Badge"></a> |
+        | <a href="https://docs.mindsdb.com/data-integrations/postgresql"><img src="https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white" alt="Connect PostgreSQL"></a> | <a href="https://docs.mindsdb.com/data-integrations/db2"><img src="https://img.shields.io/badge/IBMDB2-008000?logo=IBMDB2&logoColor=fff&style=for-the-badge" alt="IBMDB2 Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#opengauss"><img src="https://img.shields.io/badge/openGauss-02458D?logo=opengauss&logoColor=fff&style=for-the-badge" alt="openGauss Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#mysql"><img src="https://img.shields.io/badge/MySQL-00758F?style=for-the-badge&logo=mysql&logoColor=white" alt="Connect MySQL"></a> | <a href=" https://docs.mindsdb.com/data-integrations/all-data-integrations#databricks"><img src="https://img.shields.io/badge/Databricks-FF3621?logo=databricks&logoColor=fff&style=for-the-badge" alt="Databricks Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#yugabyte"><img src="https://img.shields.io/badge/YugabyteDB-02458D?logo=yugabytedb&logoColor=fff&style=for-the-badge" alt="YugabyteDB Badge"></a>
-        | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#questdb"><img src="https://img.shields.io/badge/QuestDB-d14671?style=for-the-badge&logo=questdb&logoColor=white" alt="Connect QuestDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#druid"><img src="https://img.shields.io/badge/Apache%20Druid-29F1FB?logo=apachedruid&logoColor=000&style=for-the-badge" alt="Apache Druid Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#starrocks"><img src="https://img.shields.io/badge/starrocks-000000?style=for-the-badge&logo=starrocks&logoColor=white" alt="StarRocks Badge"></a> |
+        | <a href="https://docs.mindsdb.com/data-integrations/questdb"><img src="https://img.shields.io/badge/QuestDB-d14671?style=for-the-badge&logo=questdb&logoColor=white" alt="Connect QuestDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#druid"><img src="https://img.shields.io/badge/Apache%20Druid-29F1FB?logo=apachedruid&logoColor=000&style=for-the-badge" alt="Apache Druid Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#starrocks"><img src="https://img.shields.io/badge/starrocks-000000?style=for-the-badge&logo=starrocks&logoColor=white" alt="StarRocks Badge"></a> |
         | <a href="https://docs.mindsdb.com/"><img src="https://img.shields.io/badge/redis-%23DD0031.svg?&style=for-the-badge&logo=redis&logoColor=white" alt="Connect Redis"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#vertica"><img src="https://img.shields.io/badge/Vertica-000?logo=vertica&logoColor=fff&style=for-the-badge" alt="Vertica Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#duckdb"><img src="https://img.shields.io/badge/duckdb-fff?logo=duckdb&logoColor=000&style=for-the-badge" alt="DuckDB Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#sap-hana"><img src="https://img.shields.io/badge/SAP%20HANA-1661BE?style=for-the-badge&logo=sap&logoColor=white" alt="Connect SAP HANA"></a> | <a href=" https://docs.mindsdb.com/data-integrations/all-data-integrations#elastic-search"><img src="https://img.shields.io/badge/Elastic-005571?logo=elastic&logoColor=fff&style=for-the-badge" alt="Elastic Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#cloud-spanner"><img src="https://img.shields.io/badge/Cloud%20Spanner-4285F4?style=for-the-badge" alt="Cloud Spanner Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#scylla"><img src="https://img.shields.io/badge/ScyllaDB-53CADD?style=for-the-badge&logo=scylladbb&logoColor=white" alt="Connect ScyllaDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#firebird"><img src="https://img.shields.io/badge/Firebird-F40D12?logo=Firebird&logoColor=fff&style=for-the-badge" alt="Firebird Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#singlestore"><img src="https://img.shields.io/badge/Singlestore-5f07b4?style=for-the-badge&logo=singlestore&logoColor=white" alt="Connect Singlestore"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#hive"><img src="https://img.shields.io/badge/Apache%20Hive-FDEE21?logo=apachehive&logoColor=000&style=for-the-badge" alt="Apache Hive Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#teradata"><img src="https://img.shields.io/badge/Teradata-e36c42?style=for-the-badge&logo=teradata&logoColor=white" alt="Connect Teradata"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#matrix-one"><img src="https://img.shields.io/badge/Matrixone-02458D?logo=Matrixone&logoColor=fff&style=for-the-badge" alt="Matrixone Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#snowflake"><img src="https://img.shields.io/badge/Snowflake-35aedd?style=for-the-badge&logo=snowflake&logoColor=blue" alt="Connect Snowflake"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#informix"><img src="https://img.shields.io/badge/Informix-191A1B?logo=informix&logoColor=fff&style=for-the-badge" alt="Informix Badge"></a> |
         | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#trino"><img src="https://img.shields.io/badge/Trino-dd00a1?style=for-the-badge&logo=trino&logoColor=white" alt="Connect Trino"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#monetdb"><img src="https://img.shields.io/badge/Monetdb-0099E5?logo=Monetdb&logoColor=fff&style=for-the-badge" alt="Monetdb Badge"></a> |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: MindsDB Version: 23.4.4.2 Summary: MindsDB server,
+Metadata-Version: 2.1 Name: MindsDB Version: 23.4.4.3 Summary: MindsDB server,
 provides server capabilities to mindsdb native python library Home-page: https:
 //github.com/mindsdb/mindsdb Author: MindsDB Inc Author-email:
 jorge@mindsdb.com License: GPL-3.0 Download-URL: https://pypi.org/project/
 mindsdb/ Description:
                                ****** [MindsDB]
                                      ******
       [ROSS_Index_-_Fastest_Growing_Open-Source_Startups_|_Runa_Capital]
```

### Comparing `MindsDB-23.4.4.2/README.md` & `MindsDB-23.4.4.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -116,23 +116,23 @@
 
 MindsDB works with most of the SQL and NoSQL databases, data lakes, data Streams and popular applications.
 
 | Connect your Data | Connect your Data | Connect your Data
 |-|-|-|
 | <a href="https://docs.mindsdb.com/connect/kafka"><img src="https://img.shields.io/badge/Apache Kafka-808080?style=for-the-badge&logo=apache-kafka&logoColor=white" alt="Connect Apache Kafka"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#microsoft-access"><img src="https://img.shields.io/badge/Microsoft%20Access-A4373A?logo=microsoftaccess&logoColor=fff&style=for-the-badge" alt="Connect Microsoft Access"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#oracle"><img src="https://img.shields.io/badge/Oracle-F80000?logo=oracle&logoColor=fff&style=for-the-badge" alt="Oracle Badge"></a> |
 | <a href=" https://docs.mindsdb.com/data-integrations/all-data-integrations#amazon-redshift"><img src="https://img.shields.io/badge/Amazon%20Redshift-0466C8?style=for-the-badge&logo=amazon-aws&logoColor=white" alt="Connect Amazon Redshift"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#airtable"><img src="https://img.shields.io/badge/Airtable-18BFFF?logo=airtable&logoColor=fff&style=for-the-badge" alt="Airtable Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/Apache-Pinot"><img src="https://img.shields.io/badge/Pinot-000?logo=pinot&logoColor=fff&style=for-the-badge" alt="Pinot Badge"></a> |
-| <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#cassandra"><img src="https://img.shields.io/badge/Cassandra-1287B1?style=for-the-badge&logo=apache%20cassandra&logoColor=white" alt="Connect Cassandra"></a> | <a href=" https://docs.mindsdb.com/data-integrations/all-data-integrations#datastax"><img src="https://img.shields.io/badge/DataStax-3A3A42?logo=datastax&logoColor=fff&style=for-the-badge" alt="DataStax Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#s3"><img src="https://img.shields.io/badge/Amazon%20S3-569A31?logo=amazons3&logoColor=fff&style=for-the-badge" alt="Amazon S3 Badge"></a> |
+| <a href="https://docs.mindsdb.com/data-integrations/apache-cassandra"><img src="https://img.shields.io/badge/Cassandra-1287B1?style=for-the-badge&logo=apache%20cassandra&logoColor=white" alt="Connect Cassandra"></a> | <a href=" https://docs.mindsdb.com/data-integrations/all-data-integrations#datastax"><img src="https://img.shields.io/badge/DataStax-3A3A42?logo=datastax&logoColor=fff&style=for-the-badge" alt="DataStax Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#s3"><img src="https://img.shields.io/badge/Amazon%20S3-569A31?logo=amazons3&logoColor=fff&style=for-the-badge" alt="Amazon S3 Badge"></a> |
 | <a href="https://docs.mindsdb.com/data-integrations/cockroachdb"><img src="https://img.shields.io/badge/CockroachDB-426EDF?style=for-the-badge&logo=cockroach-labs&logoColor=white" alt="Connect CockroachDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/ckan"><img src="https://img.shields.io/badge/ckan-7D929E?logo=ckan&logoColor=fff&style=for-the-badge" alt="ckan Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#supabase"><img src="https://img.shields.io/badge/Supabase-3ECF8E?logo=supabase&logoColor=fff&style=for-the-badge" alt="Supabase Badge"></a> |
 | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#clickhouse"><img src="https://img.shields.io/badge/Clickhouse-e6e600?style=for-the-badge&logo=clickhouse&logoColor=white" alt="Connect Clickhouse"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#google-bigquery"><img src="https://img.shields.io/badge/Google Big Query-0466C8?logo=Big Query&logoColor=fff&style=for-the-badge" alt="Google Big Query Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#sqlite"><img src="https://img.shields.io/badge/SQLite-003B57?logo=sqlite&logoColor=fff&style=for-the-badge" alt="SQLite Badge"></a> |
 | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#mariadb"><img src="https://img.shields.io/badge/MariaDB-003545?style=for-the-badge&logo=mariadb&logoColor=white" alt="Connect MariaDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#couchbase"><img src="https://img.shields.io/badge/Couchbase-EA2328?logo=couchbase&logoColor=fff&style=for-the-badge" alt="Couchbase Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/TiDB#tidb-handler"><img src="https://img.shields.io/badge/TiDB-DD0031?logo=tidb&logoColor=fff&style=for-the-badge" alt="TiDB Badge"></a> |
 | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#microsoft-sql-server"><img src="https://img.shields.io/badge/Microsoft%20SQL%20Sever-CC2927?style=for-the-badge&logo=microsoft%20sql%20server&logoColor=white" alt="Connect SQL Server"></a> | <a href="https://docs.mindsdb.com/data-integrations/cratedb"><img src="https://img.shields.io/badge/CrateDB-009DC7?logo=cratedb&logoColor=fff&style=for-the-badge" alt="CrateDB Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#timescaledb"><img src="https://img.shields.io/badge/Timescale-FDB515?logo=timescale&logoColor=fff&style=for-the-badge" alt="Timescale Badge"></a> |
 | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#mongodb"><img src="https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge&logo=mongodb&logoColor=white" alt="Connect MongoDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#d0lt"><img src="https://img.shields.io/badge/DoIt-00B388?logo=DoIt&logoColor=fff&style=for-the-badge" alt="DoIt Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#aws-dynamodb"><img src="https://img.shields.io/badge/Amazon%20DynamoDB-4053D6?logo=amazondynamodb&logoColor=fff&style=for-the-badge" alt="Amazon DynamoDB Badge"></a> |
-| <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#postgresql"><img src="https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white" alt="Connect PostgreSQL"></a> | <a href="https://docs.mindsdb.com/data-integrations/db2"><img src="https://img.shields.io/badge/IBMDB2-008000?logo=IBMDB2&logoColor=fff&style=for-the-badge" alt="IBMDB2 Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#opengauss"><img src="https://img.shields.io/badge/openGauss-02458D?logo=opengauss&logoColor=fff&style=for-the-badge" alt="openGauss Badge"></a> |
+| <a href="https://docs.mindsdb.com/data-integrations/postgresql"><img src="https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white" alt="Connect PostgreSQL"></a> | <a href="https://docs.mindsdb.com/data-integrations/db2"><img src="https://img.shields.io/badge/IBMDB2-008000?logo=IBMDB2&logoColor=fff&style=for-the-badge" alt="IBMDB2 Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#opengauss"><img src="https://img.shields.io/badge/openGauss-02458D?logo=opengauss&logoColor=fff&style=for-the-badge" alt="openGauss Badge"></a> |
 | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#mysql"><img src="https://img.shields.io/badge/MySQL-00758F?style=for-the-badge&logo=mysql&logoColor=white" alt="Connect MySQL"></a> | <a href=" https://docs.mindsdb.com/data-integrations/all-data-integrations#databricks"><img src="https://img.shields.io/badge/Databricks-FF3621?logo=databricks&logoColor=fff&style=for-the-badge" alt="Databricks Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#yugabyte"><img src="https://img.shields.io/badge/YugabyteDB-02458D?logo=yugabytedb&logoColor=fff&style=for-the-badge" alt="YugabyteDB Badge"></a>
-| <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#questdb"><img src="https://img.shields.io/badge/QuestDB-d14671?style=for-the-badge&logo=questdb&logoColor=white" alt="Connect QuestDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#druid"><img src="https://img.shields.io/badge/Apache%20Druid-29F1FB?logo=apachedruid&logoColor=000&style=for-the-badge" alt="Apache Druid Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#starrocks"><img src="https://img.shields.io/badge/starrocks-000000?style=for-the-badge&logo=starrocks&logoColor=white" alt="StarRocks Badge"></a> |
+| <a href="https://docs.mindsdb.com/data-integrations/questdb"><img src="https://img.shields.io/badge/QuestDB-d14671?style=for-the-badge&logo=questdb&logoColor=white" alt="Connect QuestDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#druid"><img src="https://img.shields.io/badge/Apache%20Druid-29F1FB?logo=apachedruid&logoColor=000&style=for-the-badge" alt="Apache Druid Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#starrocks"><img src="https://img.shields.io/badge/starrocks-000000?style=for-the-badge&logo=starrocks&logoColor=white" alt="StarRocks Badge"></a> |
 | <a href="https://docs.mindsdb.com/"><img src="https://img.shields.io/badge/redis-%23DD0031.svg?&style=for-the-badge&logo=redis&logoColor=white" alt="Connect Redis"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#vertica"><img src="https://img.shields.io/badge/Vertica-000?logo=vertica&logoColor=fff&style=for-the-badge" alt="Vertica Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#duckdb"><img src="https://img.shields.io/badge/duckdb-fff?logo=duckdb&logoColor=000&style=for-the-badge" alt="DuckDB Badge"></a> |
 | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#sap-hana"><img src="https://img.shields.io/badge/SAP%20HANA-1661BE?style=for-the-badge&logo=sap&logoColor=white" alt="Connect SAP HANA"></a> | <a href=" https://docs.mindsdb.com/data-integrations/all-data-integrations#elastic-search"><img src="https://img.shields.io/badge/Elastic-005571?logo=elastic&logoColor=fff&style=for-the-badge" alt="Elastic Badge"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#cloud-spanner"><img src="https://img.shields.io/badge/Cloud%20Spanner-4285F4?style=for-the-badge" alt="Cloud Spanner Badge"></a> |
 | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#scylla"><img src="https://img.shields.io/badge/ScyllaDB-53CADD?style=for-the-badge&logo=scylladbb&logoColor=white" alt="Connect ScyllaDB"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#firebird"><img src="https://img.shields.io/badge/Firebird-F40D12?logo=Firebird&logoColor=fff&style=for-the-badge" alt="Firebird Badge"></a> |
 | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#singlestore"><img src="https://img.shields.io/badge/Singlestore-5f07b4?style=for-the-badge&logo=singlestore&logoColor=white" alt="Connect Singlestore"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#hive"><img src="https://img.shields.io/badge/Apache%20Hive-FDEE21?logo=apachehive&logoColor=000&style=for-the-badge" alt="Apache Hive Badge"></a> |
 | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#teradata"><img src="https://img.shields.io/badge/Teradata-e36c42?style=for-the-badge&logo=teradata&logoColor=white" alt="Connect Teradata"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#matrix-one"><img src="https://img.shields.io/badge/Matrixone-02458D?logo=Matrixone&logoColor=fff&style=for-the-badge" alt="Matrixone Badge"></a> |
 | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#snowflake"><img src="https://img.shields.io/badge/Snowflake-35aedd?style=for-the-badge&logo=snowflake&logoColor=blue" alt="Connect Snowflake"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#informix"><img src="https://img.shields.io/badge/Informix-191A1B?logo=informix&logoColor=fff&style=for-the-badge" alt="Informix Badge"></a> |
 | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#trino"><img src="https://img.shields.io/badge/Trino-dd00a1?style=for-the-badge&logo=trino&logoColor=white" alt="Connect Trino"></a> | <a href="https://docs.mindsdb.com/data-integrations/all-data-integrations#monetdb"><img src="https://img.shields.io/badge/Monetdb-0099E5?logo=Monetdb&logoColor=fff&style=for-the-badge" alt="Monetdb Badge"></a> |
```

### Comparing `MindsDB-23.4.4.2/mindsdb/__main__.py` & `MindsDB-23.4.4.3/mindsdb/__main__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/common/check_auth.py` & `MindsDB-23.4.4.3/mindsdb/api/common/check_auth.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/http/gui.py` & `MindsDB-23.4.4.3/mindsdb/api/http/gui.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/http/gunicorn_wrapper.py` & `MindsDB-23.4.4.3/mindsdb/api/http/gunicorn_wrapper.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/http/initialize.py` & `MindsDB-23.4.4.3/mindsdb/api/http/initialize.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/http/namespaces/analysis.py` & `MindsDB-23.4.4.3/mindsdb/api/http/namespaces/analysis.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/http/namespaces/auth.py` & `MindsDB-23.4.4.3/mindsdb/api/http/namespaces/auth.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/http/namespaces/config.py` & `MindsDB-23.4.4.3/mindsdb/api/http/namespaces/config.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/http/namespaces/default.py` & `MindsDB-23.4.4.3/mindsdb/api/http/namespaces/default.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/http/namespaces/file.py` & `MindsDB-23.4.4.3/mindsdb/api/http/namespaces/file.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/http/namespaces/handlers.py` & `MindsDB-23.4.4.3/mindsdb/api/http/namespaces/handlers.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/http/namespaces/projects.py` & `MindsDB-23.4.4.3/mindsdb/api/http/namespaces/projects.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/http/namespaces/sql.py` & `MindsDB-23.4.4.3/mindsdb/api/http/namespaces/sql.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/http/namespaces/stream.py` & `MindsDB-23.4.4.3/mindsdb/api/http/namespaces/stream.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/http/namespaces/tab.py` & `MindsDB-23.4.4.3/mindsdb/api/http/namespaces/tab.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/http/namespaces/tree.py` & `MindsDB-23.4.4.3/mindsdb/api/http/namespaces/tree.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/http/namespaces/util.py` & `MindsDB-23.4.4.3/mindsdb/api/http/namespaces/util.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/http/start.py` & `MindsDB-23.4.4.3/mindsdb/api/http/start.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/http/utils.py` & `MindsDB-23.4.4.3/mindsdb/api/http/utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/mongo/classes/query_sql.py` & `MindsDB-23.4.4.3/mindsdb/api/mongo/classes/query_sql.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/mongo/classes/responder.py` & `MindsDB-23.4.4.3/mindsdb/api/mongo/classes/responder.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/mongo/classes/responder_collection.py` & `MindsDB-23.4.4.3/mindsdb/api/mongo/classes/responder_collection.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/mongo/classes/scram.py` & `MindsDB-23.4.4.3/mindsdb/api/mongo/classes/scram.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/mongo/classes/session.py` & `MindsDB-23.4.4.3/mindsdb/api/mongo/classes/session.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/mongo/responders/__init__.py` & `MindsDB-23.4.4.3/mindsdb/api/mongo/responders/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/mongo/responders/aggregate.py` & `MindsDB-23.4.4.3/mindsdb/api/mongo/responders/aggregate.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/mongo/responders/coll_stats.py` & `MindsDB-23.4.4.3/mindsdb/api/mongo/responders/coll_stats.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/mongo/responders/company_id.py` & `MindsDB-23.4.4.3/mindsdb/api/mongo/responders/company_id.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/mongo/responders/connection_status.py` & `MindsDB-23.4.4.3/mindsdb/api/mongo/responders/connection_status.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/mongo/responders/db_stats.py` & `MindsDB-23.4.4.3/mindsdb/api/mongo/responders/db_stats.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/mongo/responders/delete.py` & `MindsDB-23.4.4.3/mindsdb/api/mongo/responders/delete.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/mongo/responders/find.py` & `MindsDB-23.4.4.3/mindsdb/api/mongo/responders/find.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/mongo/responders/get_parameter.py` & `MindsDB-23.4.4.3/mindsdb/api/mongo/responders/get_parameter.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/mongo/responders/host_info.py` & `MindsDB-23.4.4.3/mindsdb/api/mongo/responders/host_info.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/mongo/responders/insert.py` & `MindsDB-23.4.4.3/mindsdb/api/mongo/responders/insert.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/mongo/responders/list_collections.py` & `MindsDB-23.4.4.3/mindsdb/api/mongo/responders/list_collections.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/mongo/responders/list_databases.py` & `MindsDB-23.4.4.3/mindsdb/api/mongo/responders/list_databases.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/mongo/responders/list_indexes.py` & `MindsDB-23.4.4.3/mindsdb/api/mongo/responders/list_indexes.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/mongo/responders/sasl_continue.py` & `MindsDB-23.4.4.3/mindsdb/api/mongo/responders/sasl_continue.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/mongo/responders/sasl_start.py` & `MindsDB-23.4.4.3/mindsdb/api/mongo/responders/sasl_start.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/mongo/server.py` & `MindsDB-23.4.4.3/mindsdb/api/mongo/server.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/mongo/utilities/mongodb_ast.py` & `MindsDB-23.4.4.3/mindsdb/api/mongo/utilities/mongodb_ast.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/mongo/utilities/mongodb_parser.py` & `MindsDB-23.4.4.3/mindsdb/api/mongo/utilities/mongodb_parser.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/mongo/utilities/mongodb_query.py` & `MindsDB-23.4.4.3/mindsdb/api/mongo/utilities/mongodb_query.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/classes/client_capabilities.py` & `MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/classes/client_capabilities.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/classes/com_operators.py` & `MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/classes/com_operators.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/fake_mysql_proxy.py` & `MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/classes/fake_mysql_proxy/fake_mysql_proxy.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/classes/server_capabilities.py` & `MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/classes/server_capabilities.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/classes/sql_query.py` & `MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/classes/sql_query.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/classes/sql_statement_parser.py` & `MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/classes/sql_statement_parser.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/controllers/session_controller.py` & `MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/controllers/session_controller.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/data_types/mysql_datum.py` & `MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/data_types/mysql_datum.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packet.py` & `MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/__init__.py` & `MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/binary_resultset_row_package.py` & `MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/binary_resultset_row_package.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_count_packet.py` & `MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_count_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_definition_packet.py` & `MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/column_definition_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/command_packet.py` & `MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/command_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/eof_packet.py` & `MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/eof_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/err_packet.py` & `MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/err_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_packet.py` & `MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_response_packet.py` & `MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/handshake_response_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/ok_packet.py` & `MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/ok_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/resultset_row_package.py` & `MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/resultset_row_package.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/stmt_prepare_header.py` & `MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/stmt_prepare_header.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_packet.py` & `MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_response_packet.py` & `MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/data_types/mysql_packets/switch_auth_response_packet.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/datahub/classes/tables_row.py` & `MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/datahub/classes/tables_row.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/information_schema_datanode.py` & `MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/information_schema_datanode.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/integration_datanode.py` & `MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/integration_datanode.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/project_datanode.py` & `MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/datahub/datanodes/project_datanode.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/executor/data_types.py` & `MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/executor/data_types.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/executor/executor.py` & `MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/executor/executor.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/executor/executor_client_factory.py` & `MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/executor/executor_client_factory.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/executor/executor_commands.py` & `MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/executor/executor_commands.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_client.py` & `MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_client.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_wrapper.py` & `MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/executor/executor_grpc_wrapper.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/executor/executor_service.py` & `MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/executor/executor_service.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/external_libs/mysql_scramble.py` & `MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/external_libs/mysql_scramble.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/libs/constants/mysql.py` & `MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/libs/constants/mysql.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/mysql_proxy.py` & `MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/mysql_proxy.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/utilities/exceptions.py` & `MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/utilities/functions.py` & `MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/utilities/functions.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/utilities/lightwood_dtype.py` & `MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/utilities/lightwood_dtype.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/mysql/mysql_proxy/utilities/sql.py` & `MindsDB-23.4.4.3/mindsdb/api/mysql/mysql_proxy/utilities/sql.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/nlp/nlp.py` & `MindsDB-23.4.4.3/mindsdb/api/nlp/nlp.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/postgres/postgres_proxy/executor/executor.py` & `MindsDB-23.4.4.3/mindsdb/api/postgres/postgres_proxy/executor/executor.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/postgres/postgres_proxy/postgres_packets/errors.py` & `MindsDB-23.4.4.3/mindsdb/api/postgres/postgres_proxy/postgres_packets/errors.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_fields.py` & `MindsDB-23.4.4.3/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_fields.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message.py` & `MindsDB-23.4.4.3/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_formats.py` & `MindsDB-23.4.4.3/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_formats.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_identifiers.py` & `MindsDB-23.4.4.3/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_message_identifiers.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_packets.py` & `MindsDB-23.4.4.3/mindsdb/api/postgres/postgres_proxy/postgres_packets/postgres_packets.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/api/postgres/postgres_proxy/postgres_proxy.py` & `MindsDB-23.4.4.3/mindsdb/api/postgres/postgres_proxy/postgres_proxy.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/access_handler/__init__.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/access_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/access_handler/access_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/access_handler/access_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/access_handler/icon.png` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/access_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/access_handler/tests/test_access_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/access_handler/tests/test_access_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/airtable_handler/__init__.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/airtable_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/airtable_handler/airtable_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/airtable_handler/airtable_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/airtable_handler/icon.png` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/airtable_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/airtable_handler/tests/test_airtable_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/airtable_handler/tests/test_airtable_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/altibase_handler/__init__.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/altibase_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/altibase_handler/altibase_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/altibase_handler/altibase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/altibase_handler/icon.png` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/altibase_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/altibase_handler/tests/test_altibase_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/altibase_handler/tests/test_altibase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/aurora_handler/__init__.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/aurora_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/aurora_handler/aurora_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/aurora_handler/aurora_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/aurora_handler/icon.png` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/aurora_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_mysql_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_mysql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_postgres_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/aurora_handler/tests/test_aurora_postgres_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/autokeras_handler/__init__.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/autokeras_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/autokeras_handler/autokeras_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/autokeras_handler/autokeras_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/autokeras_handler/setup.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/autokeras_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/autosklearn_handler/__init__.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/autosklearn_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/autosklearn_handler/autosklearn_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/autosklearn_handler/autosklearn_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/autosklearn_handler/config.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/autosklearn_handler/config.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/autosklearn_handler/setup.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/autosklearn_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/bigquery_handler/__init__.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/bigquery_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/bigquery_handler/bigquery_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/bigquery_handler/bigquery_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/bigquery_handler/logo.svg` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/bigquery_handler/logo.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/bigquery_handler/tests/test_bigquery_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/bigquery_handler/tests/test_bigquery_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/binance_handler/binance_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/binance_handler/binance_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/binance_handler/binance_tables.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/binance_handler/binance_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/binance_handler/icon.svg` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/binance_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/byom_handler/byom_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/byom_handler/byom_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/byom_handler/proc_wrapper.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/byom_handler/proc_wrapper.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/cassandra_handler/__init__.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/cassandra_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/cassandra_handler/cassandra_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/cassandra_handler/cassandra_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/cassandra_handler/logo.png` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/cassandra_handler/logo.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/cassandra_handler/tests/test_cassandra_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/cassandra_handler/tests/test_cassandra_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/ckan_handler/ckan_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/ckan_handler/ckan_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/ckan_handler/logo.png` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/ckan_handler/logo.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/ckan_handler/tests/test_ckan_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/ckan_handler/tests/test_ckan_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/clickhouse_handler/__init__.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/clickhouse_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/clickhouse_handler/clickhouse_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/clickhouse_handler/clickhouse_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/clickhouse_handler/tests/test_clickhouse_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/clickhouse_handler/tests/test_clickhouse_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/cloud_spanner_handler/__init__.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/cloud_spanner_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/cloud_spanner_handler/cloud_spanner_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/cloud_spanner_handler/cloud_spanner_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/cloud_spanner_handler/icon.png` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/cloud_spanner_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/cloud_spanner_handler/tests/test_cloud_spanner_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/cloud_spanner_handler/tests/test_cloud_spanner_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/cloud_sql_handler/__init__.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/cloud_sql_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/cloud_sql_handler/cloud_sql_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/cloud_sql_handler/cloud_sql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/cloud_sql_handler/icon.png` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/cloud_sql_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mssql_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mssql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mysql_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/cloud_sql_handler/tests/test_cloud_sql_mysql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/cockroach_handler/tests/test_cockroachdb_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/cockroach_handler/tests/test_cockroachdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/confluence_handler/__init__.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/confluence_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/confluence_handler/confluence_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/confluence_handler/confluence_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/confluence_handler/confluence_table.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/confluence_handler/confluence_table.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/confluence_handler/icon.png` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/confluence_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/couchbase_handler/__init__.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/couchbase_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/couchbase_handler/couchbase_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/couchbase_handler/couchbase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/couchbase_handler/icon.svg` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/couchbase_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/couchbase_handler/tests/test_couchbase_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/couchbase_handler/tests/test_couchbase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/crate_handler/crate_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/crate_handler/crate_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/crate_handler/icon.svg` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/crate_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/crate_handler/tests/test_crate_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/crate_handler/tests/test_crate_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/d0lt_handler/icon.svg` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/d0lt_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/d0lt_handler/tests/test_d0lt_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/d0lt_handler/tests/test_d0lt_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/databend_handler/__init__.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/databend_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/databend_handler/databend_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/databend_handler/databend_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/databend_handler/icon.png` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/databend_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/databend_handler/tests/test_databend_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/databend_handler/tests/test_databend_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/databricks_handler/__init__.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/databricks_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/databricks_handler/databricks/createdb.jpg` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/databricks_handler/databricks/createdb.jpg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/databricks_handler/databricks/createpred.jpg` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/databricks_handler/databricks/createpred.jpg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/databricks_handler/databricks/hivmetastore.jpg` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/databricks_handler/databricks/hivmetastore.jpg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/databricks_handler/databricks/mindsdbdatabricks.jpg` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/databricks_handler/databricks/mindsdbdatabricks.jpg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/databricks_handler/databricks/selectfrom.jpg` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/databricks_handler/databricks/selectfrom.jpg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/databricks_handler/databricks_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/databricks_handler/databricks_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/databricks_handler/icon.png` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/databricks_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/databricks_handler/tests/test_databricks_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/databricks_handler/tests/test_databricks_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/datastax_handler/__init__.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/datastax_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/datastax_handler/logo.png` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/datastax_handler/logo.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/datastax_handler/tests/test_cassandra_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/datastax_handler/tests/test_cassandra_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/db2_handler/__init__.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/db2_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/db2_handler/db2_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/db2_handler/db2_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/db2_handler/icon.png` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/db2_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/db2_handler/tests/test_db2_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/db2_handler/tests/test_db2_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/derby_handler/__init__.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/derby_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/derby_handler/derby_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/derby_handler/derby_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/derby_handler/icon.png` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/derby_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/derby_handler/tests/test_derby_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/derby_handler/tests/test_derby_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/dremio_handler/__init__.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/dremio_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/dremio_handler/dremio_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/dremio_handler/dremio_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/dremio_handler/icon.png` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/dremio_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/dremio_handler/tests/test_dremio_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/dremio_handler/tests/test_dremio_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/druid_handler/__init__.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/druid_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/druid_handler/druid_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/druid_handler/druid_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/druid_handler/icon.png` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/druid_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/druid_handler/tests/test_druid_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/druid_handler/tests/test_druid_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/duckdb_handler/__init__.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/duckdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/duckdb_handler/duckdb_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/duckdb_handler/duckdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/duckdb_handler/icon.png` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/duckdb_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/duckdb_handler/tests/test_duckdb_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/duckdb_handler/tests/test_duckdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/dynamodb_handler/__init__.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/dynamodb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/dynamodb_handler/dynamodb_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/dynamodb_handler/dynamodb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/dynamodb_handler/icon.png` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/dynamodb_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/dynamodb_handler/tests/test_dynamodb_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/dynamodb_handler/tests/test_dynamodb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/edgelessdb_handler/__init__.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/edgelessdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/edgelessdb_handler/edgelessdb_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/edgelessdb_handler/edgelessdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/edgelessdb_handler/icon.svg` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/edgelessdb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/edgelessdb_handler/tests/test_edgelessdb_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/edgelessdb_handler/tests/test_edgelessdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/elasticsearch_handler/__init__.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/elasticsearch_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/elasticsearch_handler/elasticsearch_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/elasticsearch_handler/elasticsearch_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/elasticsearch_handler/icon.png` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/elasticsearch_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/elasticsearch_handler/tests/test_elasticsearch_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/elasticsearch_handler/tests/test_elasticsearch_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/empress_handler/__init__.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/empress_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/empress_handler/empress_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/empress_handler/empress_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/empress_handler/icon.svg` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/empress_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/empress_handler/tests/test_empress_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/empress_handler/tests/test_empress_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/eventstoredb_handler/eventstoredb_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/eventstoredb_handler/eventstoredb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/eventstoredb_handler/icon.svg` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/eventstoredb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/file_handler/file_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/file_handler/file_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/firebird_handler/__init__.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/firebird_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/firebird_handler/firebird_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/firebird_handler/firebird_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/firebird_handler/icon.png` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/firebird_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/firebird_handler/tests/test_firebird_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/firebird_handler/tests/test_firebird_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/github_handler/github_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/github_handler/github_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/github_handler/github_tables.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/github_handler/github_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/github_handler/icon.svg` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/github_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/google_calendar_handler/__init__.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/google_calendar_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_tables.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/google_calendar_handler/google_calendar_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/google_calendar_handler/icon.svg` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/google_calendar_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/google_calendar_handler/tests/test_google_calendar_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/google_calendar_handler/tests/test_google_calendar_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/hana_handler/__init__.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/hana_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/hana_handler/hana_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/hana_handler/hana_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/hana_handler/icon.svg` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/hana_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/hive_handler/__init__.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/hive_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/hive_handler/hive_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/hive_handler/hive_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/hive_handler/icon.svg` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/hive_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/hive_handler/tests/test_hive_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/hive_handler/tests/test_hive_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/hsqldb_handler/__init__.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/hsqldb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/hsqldb_handler/hsqldb_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/hsqldb_handler/hsqldb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/hsqldb_handler/icon.png` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/hsqldb_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/huggingface_handler/__init__.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/huggingface_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/huggingface_handler/huggingface_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/huggingface_handler/huggingface_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/huggingface_handler/setup.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/huggingface_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/ignite_handler/__init__.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/ignite_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/ignite_handler/icon.png` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/ignite_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/ignite_handler/ignite_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/ignite_handler/ignite_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/ignite_handler/tests/test_ignite_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/ignite_handler/tests/test_ignite_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/impala_handler/__init__.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/impala_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/impala_handler/icon.svg` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/impala_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/impala_handler/impala_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/impala_handler/impala_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/impala_handler/tests/test_impala_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/impala_handler/tests/test_impala_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/influxdb_handler/__init__.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/influxdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/influxdb_handler/icon.png` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/influxdb_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/influxdb_handler/influxdb_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/influxdb_handler/influxdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/influxdb_handler/influxdb_tables.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/influxdb_handler/influxdb_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/informix_handler/icon.png` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/informix_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/informix_handler/informix_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/informix_handler/informix_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/informix_handler/tests/test_informix_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/informix_handler/tests/test_informix_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/ingres_handler/__init__.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/ingres_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/ingres_handler/icon.svg` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/ingres_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/ingres_handler/ingres_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/ingres_handler/ingres_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/ingres_handler/tests/test_ingres_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/ingres_handler/tests/test_ingres_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/jira_handler/__init__.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/matrixone_handler/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 from mindsdb.integrations.libs.const import HANDLER_TYPE
+
 from .__about__ import __version__ as version, __description__ as description
-from mindsdb.utilities.log import get_log
-log = get_log()
 try:
-    from .jira_handler import (
-        JiraHandler as Handler,
+    from .matrixone_handler import (
+        MatrixOneHandler as Handler,
         connection_args_example,
         connection_args
     )
     import_error = None
 except Exception as e:
     Handler = None
     import_error = e
 
-
-title = 'Atlassian Jira'
-name = 'jira'
+title = 'MatrixOne'
+name = 'matrixone'
 type = HANDLER_TYPE.DATA
 icon_path = 'icon.png'
 
-
 __all__ = [
     'Handler', 'version', 'name', 'type', 'title', 'description',
     'connection_args', 'connection_args_example', 'import_error', 'icon_path'
 ]
```

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/jira_handler/icon.png` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/jira_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/jira_handler/jira_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/oracle_handler/oracle_handler.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,225 +1,196 @@
 from typing import Optional
 from collections import OrderedDict
 
 import pandas as pd
-import duckdb
-import json
-from atlassian import Jira
+import oracledb
+from oracledb import connect, Connection, makedsn
 
-from mindsdb_sql import parse_sql
-from mindsdb.integrations.libs.base import DatabaseHandler
-from mindsdb.utilities.log import get_log
+from mindsdb_sql.render.sqlalchemy_render import SqlalchemyRender
 from mindsdb_sql.parser.ast.base import ASTNode
 
+from mindsdb.utilities import log
+from mindsdb.integrations.libs.base import DatabaseHandler
 from mindsdb.integrations.libs.response import (
     HandlerStatusResponse as StatusResponse,
     HandlerResponse as Response,
-    RESPONSE_TYPE
+    RESPONSE_TYPE,
 )
 from mindsdb.integrations.libs.const import HANDLER_CONNECTION_ARG_TYPE as ARG_TYPE
 
-log = get_log()
+oracledb.defaults.fetch_lobs = False  # return LOBs directly as strings or bytes
 
 
-class JiraHandler(DatabaseHandler):
+class OracleHandler(DatabaseHandler):
     """
-    This handler handles connection and execution of the Airtable statements.
+    This handler handles connection and execution of the Microsoft SQL Server statements.
     """
 
-    name = 'jira'
+    name = "oracle"
+
     def __init__(self, name: str, connection_data: Optional[dict], **kwargs):
-        """
-        Initialize the handler.
-        Args:
-            name (str): name of particular handler instance
-            connection_data (dict): parameters for connecting to the database
-            **kwargs: arbitrary keyword arguments.
-        """
         super().__init__(name)
-        self.parser = parse_sql
-        self.dialect = 'jira'
-        self.connection_data = connection_data
-        self.kwargs = kwargs
+        self.host = connection_data.get("host")
+        self.port = int(connection_data.get("port") or 1521)
+        self.sid = connection_data.get("sid")
+        self.service_name = connection_data.get("service_name")
+        self.user = connection_data.get("user")
+        self.password = connection_data.get("password")
+
+        if self.sid is None and self.service_name is None:
+            raise ValueError("Either 'sid' or 'service_name' must be given")
+        if self.sid and self.service_name:
+            raise ValueError("Only one of 'sid' or 'service_name' must be given")
+
+        if self.sid:
+            self.dsn = makedsn(host=self.host, port=self.port, sid=self.sid)
+        else:
+            self.dsn = makedsn(host=self.host, port=self.port, service_name=self.service_name)
 
         self.connection = None
         self.is_connected = False
 
-    def __del__(self):
+    def connect(self) -> Connection:
         if self.is_connected is True:
-            self.disconnect()
+            return self.connection
 
-    def connect(self) -> StatusResponse:
-        """
-        Set up the connection required by the handler.
-        Returns:
-            HandlerStatusResponse
-        """
+        connection = connect(user=self.user, password=self.password, dsn=self.dsn)
 
-        if self.is_connected is True:
-            return self.connection
-        
-        self.connection = Jira(
-            url=self.connection_data['jira_url'],
-            username=self.connection_data['user_id'],
-            password=self.connection_data['api_key'],
-            cloud=True)
-        
         self.is_connected = True
-
+        self.connection = connection
         return self.connection
 
     def disconnect(self):
-        """
-        Close any existing connections.
-        """
-
-        if self.is_connected is False:
-            return
-
-        self.connection.close()
+        if self.is_connected:
+            self.connection.close()
         self.is_connected = False
-        return self.is_connected
+        return
 
     def check_connection(self) -> StatusResponse:
         """
-        Check connection to the handler.
-        Returns:
-            HandlerStatusResponse
+        Check the connection of the database
+        :return: success status and error message if error occurs
         """
 
         response = StatusResponse(False)
         need_to_close = self.is_connected is False
 
         try:
-            self.connect()
+            con = self.connect()
+            con.ping()
             response.success = True
         except Exception as e:
-            log.error(f'Error connecting to Jira portal {self.connection_data["jira_url"]}, {e}!')
+            log.logger.error(f"Error connecting to Oracle DB {self.dsn}, {e}!")
             response.error_message = str(e)
         finally:
             if response.success is True and need_to_close:
                 self.disconnect()
             if response.success is False and self.is_connected is True:
                 self.is_connected = False
-
         return response
 
-    def native_query(self, query: str) -> StatusResponse:
+    def native_query(self, query: str) -> Response:
         """
-        Receive raw query and act upon it somehow.
-        Args:
-            query (str): query in native format
-        Returns:
-            HandlerResponse
+        Receive SQL query and runs it
+        :param query: The SQL query to run
+        :return: returns the records from the current recordset
         """
-
         need_to_close = self.is_connected is False
 
         connection = self.connect()
-        results = connection.jql(self.connection_data['jira_query'])
-        df = pd.json_normalize(results["issues"])
-        fields_name= ["key", "fields.summary","fields.status.name", "fields.reporter.name","fields.assignee.name","fields.priority.name"]
-        locals()[self.connection_data['table_name']] = df[fields_name]
-        try:            
-            result = duckdb.query(query)
-            if result:
-                response = Response(RESPONSE_TYPE.TABLE,data_frame=result.df())                   
-            else:
-                response = Response(RESPONSE_TYPE.OK)
+        with connection.cursor() as cur:
+            try:
+                cur.execute(query)
+                result = cur.fetchall()
+                if result:
+                    response = Response(
+                        RESPONSE_TYPE.TABLE,
+                        data_frame=pd.DataFrame(
+                            result,
+                            columns=[row[0] for row in cur.description],
+                        ),
+                    )
+                else:
+                    response = Response(RESPONSE_TYPE.OK)
+
+                connection.commit()
+            except Exception as e:
+                log.logger.error(f"Error running query: {query} on {self.dsn}!")
+                response = Response(
+                    RESPONSE_TYPE.ERROR,
+                    error_message=str(e),
+                )
+                connection.rollback()
 
-        except Exception as e:
-            log.error(f'Error running query  {query} on jira handler')
-            response = Response(
-                RESPONSE_TYPE.ERROR,
-                error_message=str(e)
-            )
-        
         if need_to_close is True:
             self.disconnect()
 
         return response
 
-    def query(self, query: ASTNode) -> StatusResponse:
+    def query(self, query: ASTNode) -> Response:
         """
-        Receive query as AST (abstract syntax tree) and act upon it somehow.
-        Args:
-            query (ASTNode): sql query represented as AST. May be any kind
-                of query: SELECT, INTSERT, DELETE, etc
-        Returns:
-            HandlerResponse
+        Retrieve the data from the SQL statement.
         """
+        renderer = SqlalchemyRender("oracle")
+        query_str = renderer.get_string(query, with_failback=True)
+        return self.native_query(query_str)
 
-        return self.native_query(query.to_string())
-
-    def get_tables(self) -> StatusResponse:
+    def get_tables(self) -> Response:
         """
-        Return list of entities that will be accessible as tables.
-        Returns:
-            HandlerResponse
+        List all tables in Oracle DB owned by the current user.
         """
+        query = """
+            SELECT table_name
+            FROM user_tables
+            ORDER BY 1;
+        """
+        return self.native_query(query)
 
-        response = Response(
-            RESPONSE_TYPE.TABLE,
-            data_frame=pd.DataFrame(
-                [self.connection_data['table_name']],
-                columns=['table_name']
-            )
-        )
-
-        return response
-
-    def get_columns(self) -> StatusResponse:
+    def get_columns(self, table_name: str) -> Response:
         """
-        Returns a list of entity columns.
-        Args:
-            table_name (str): name of one of tables returned by self.get_tables()
-        Returns:
-            HandlerResponse
+        Show details about the table.
+        """
+        query = f"""
+            SELECT 
+                column_name,
+                data_type
+            FROM USER_TAB_COLUMNS
+            WHERE table_name = '{table_name}'
         """
-        query = 'SELECT * FROM '+ str(self.connection_data['table_name'])+ ' LIMIT 10'
         result = self.native_query(query)
-
-        response = Response(
-            RESPONSE_TYPE.TABLE,
-            data_frame=pd.DataFrame(
-                {
-                    'column_name': result.data_frame.columns,
-                    'data_type': result.data_frame.dtypes
-                }
-            )
-        )
-
-        return response
+        return result
 
 
 connection_args = OrderedDict(
-    table_name={
-        'type': ARG_TYPE.STR,
-        'description': 'Sample Jira table name.'
-    },
-    jira_url={
-        'type': ARG_TYPE.STR,
-        'description': 'Jira  url'
-    },
-    user_id={
-        'type': ARG_TYPE.STR,
-        'description': 'Jira User ID.'
-    },
-    api_key={
-        'type': ARG_TYPE.STR,
-        'description': 'API key for the Jira API.'
-    },
-    jira_query={
-        'type': ARG_TYPE.STR,
-        'description': 'Jira Search Query '
-    }
-   
+    host={
+        "type": ARG_TYPE.STR,
+        "description": "The host name or IP address of the Oracle DB.",
+    },
+    port={
+        "type": ARG_TYPE.INT,
+        "description": "The TCP/IP port of the Oracle DB. Must be an integer. Default 1521.",
+    },
+    sid={
+        "type": ARG_TYPE.STR,
+        "description": "The site identifier of the Oracle DB. Either sid or service_name should be provided.",
+    },
+    service_name={
+        "type": ARG_TYPE.STR,
+        "description": "The name of the Oracle DB service. Either sid or service_name should be provided.",
+    },
+    user={
+        "type": ARG_TYPE.STR,
+        "description": "The user name used to authenticate against the Oracle DB.",
+    },
+    password={
+        "type": ARG_TYPE.STR,
+        "description": "The password to authenticate the user against Oracle DB.",
+    },
 )
 
 connection_args_example = OrderedDict(
-    table_name ='project',
-    jira_url ='https://jira.linuxfoundation.org/',
-    user_id='balaceg',
-    api_key='4Rhq&Ehd#KV4an!',
-    jira_query = 'project = RELENG and status = In Progress'
+    host="127.0.0.1",
+    port=1521,
+    user="admin",
+    password="password",
+    sid="ORCL",
 )
```

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/jira_handler/tests/test_jira_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/test_nuo_handler.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,36 +1,50 @@
 import unittest
-from mindsdb.integrations.handlers.jira_handler.jira_handler import JiraHandler
+from mindsdb.integrations.handlers.nuo_jdbc_handler.nuo_jdbc_handler import NuoHandler
 from mindsdb.api.mysql.mysql_proxy.libs.constants.response_type import RESPONSE_TYPE
 
-
-class JiraHandlerTest(unittest.TestCase):
+class NuoHandlerTest(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
         cls.kwargs = {
-            "table_name": "project",
-            "jira_url": "https://jira.linuxfoundation.org/",
-            "user_id": "balaceg",
-            "api_key": "4Rhq&Ehd#KV4an!",
-            "jira_query": "project = RELENG and status = 'In Progress'"
+            "connection_data": {
+                "host": "localhost",
+                "port": 48006,
+                "database": "test",
+                "schema": "hockey",
+                "user": "dba",
+                "password": "goalie",
+                "is_direct": "true",
+            }
         }
-        cls.handler = JiraHandler('test_jira_handler', cls.kwargs)
-
-    def test_0_check_connection(self):
-        assert self.handler.check_connection()
-
-    def test_1_native_query_select(self):
-        query = "SELECT * FROM project LIMIT 10"
-        result = self.handler.native_query(query)
-        assert result.type is RESPONSE_TYPE.TABLE
-
-    def test_2_get_tables(self):
-        tables = self.handler.get_tables()
-        assert tables.type is not RESPONSE_TYPE.ERROR
-
-    def test_3_get_columns(self):
-        columns = self.handler.get_columns()
-        assert columns.type is not RESPONSE_TYPE.ERROR
+        cls.handler = NuoHandler('test_nuo_handler', **cls.kwargs)
 
+    def test_0_connect(self):
+        self.handler.connect()
+    
+    def test_1_check_connection(self):
+        self.handler.check_connection()
+
+    def test_2_create(self):
+        res = self.handler.query('CREATE TABLE TESTTABLEX3 (ID INT PRIMARY KEY, NAME VARCHAR(14))')
+        assert res.type is RESPONSE_TYPE.OK
+
+    def test_3_insert(self):
+        res = self.handler.query("INSERT INTO TESTTABLEX3 VALUES (100,'ONE HUNDRED'),(200,'TWO HUNDRED'),(300,'THREE HUNDRED')")
+        assert res.type is RESPONSE_TYPE.OK
+
+    def test_4_select(self):
+        res = self.handler.query('SELECT * FROM HOCKEY')
+        assert res.type is RESPONSE_TYPE.TABLE
+    
+    def test_5_get_tables(self):
+        res = self.handler.get_tables()
+        assert res.type is RESPONSE_TYPE.TABLE
+
+    def test_6_get_columns(self):
+        res = self.handler.get_columns("HOCKEY")
+        assert res.type is RESPONSE_TYPE.TABLE
+    
 
+        
 if __name__ == '__main__':
-    unittest.main()
+    unittest.main()
```

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/langchain_handler/langchain_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/langchain_handler/langchain_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/langchain_handler/setup.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/langchain_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/functions.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/functions.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/lightwood_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/lightwood_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/utils.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/lightwood_handler/lightwood_handler/utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/lightwood_handler/setup.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/lightwood_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/lightwood_handler/tests/test_lightwood_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/lightwood_handler/tests/test_lightwood_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/ludwig_handler/ludwig_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/ludwig_handler/ludwig_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/ludwig_handler/setup.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/ludwig_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/mariadb_handler/create-db.png` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/mariadb_handler/create-db.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/mariadb_handler/icon.svg` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/mariadb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/mariadb_handler/predict-db.png` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/mariadb_handler/predict-db.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/mariadb_handler/predictor.png` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/mariadb_handler/predictor.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/materialize_handler/icon.png` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/materialize_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/materialize_handler/materialize_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/materialize_handler/materialize_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/materialize_handler/tests/test_materialize_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/materialize_handler/tests/test_materialize_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/matrixone_handler/__init__.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/sheets_handler/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from mindsdb.integrations.libs.const import HANDLER_TYPE
 
 from .__about__ import __version__ as version, __description__ as description
 try:
-    from .matrixone_handler import (
-        MatrixOneHandler as Handler,
+    from .sheets_handler import (
+        SheetsHandler as Handler,
         connection_args_example,
         connection_args
     )
     import_error = None
 except Exception as e:
     Handler = None
     import_error = e
 
-title = 'MatrixOne'
-name = 'matrixone'
+title = 'Google Sheets'
+name = 'sheets'
 type = HANDLER_TYPE.DATA
 icon_path = 'icon.png'
 
 __all__ = [
     'Handler', 'version', 'name', 'type', 'title', 'description',
     'connection_args', 'connection_args_example', 'import_error', 'icon_path'
 ]
```

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/matrixone_handler/icon.png` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/matrixone_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/matrixone_handler/matrixone_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/matrixone_handler/matrixone_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/matrixone_handler/tests/test_matrixone_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/matrixone_handler/tests/test_matrixone_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/merlion_handler/adapters.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/merlion_handler/adapters.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/merlion_handler/merlion_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/merlion_handler/merlion_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/merlion_handler/setup.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/merlion_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/mlflow_handler/__init__.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/mlflow_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/mlflow_handler/mlflow_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/mlflow_handler/mlflow_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/mlflow_handler/setup.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/mlflow_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/monetdb_handler/__init__.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/monetdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/monetdb_handler/icon.png` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/monetdb_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/monetdb_handler/monetdb_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/monetdb_handler/monetdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/monetdb_handler/tests/test_monetdb_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/monetdb_handler/tests/test_monetdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/monetdb_handler/utils/monet_get_id.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/monetdb_handler/utils/monet_get_id.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/mongodb_handler/icon.svg` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/mongodb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/mongodb_handler/mongodb_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/mongodb_handler/mongodb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/mongodb_handler/utils/mongodb_render.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/mongodb_handler/utils/mongodb_render.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/mssql_handler/icon.png` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/mssql_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/mssql_handler/mssql_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/mssql_handler/mssql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/mssql_handler/tests/test_mssql_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/mssql_handler/tests/test_mssql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/mysql_handler/__init__.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/mysql_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/mysql_handler/icon.svg` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/mysql_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/mysql_handler/mysql_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/mysql_handler/mysql_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/neuralforecast_handler/neuralforecast_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/neuralforecast_handler/neuralforecast_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/neuralforecast_handler/setup.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/neuralforecast_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/nuo_jdbc_handler/__init__.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/nuo_jdbc_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/nuo_jdbc_handler/icon.png` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/nuo_jdbc_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/nuo_jdbc_handler/nuo_jdbc_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/nuo_jdbc_handler/nuo_jdbc_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/nuo_jdbc_handler/tests/test_nuo_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/yugabyte_handler/tests/test_yugabyte_handler.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,49 @@
 import unittest
-from mindsdb.integrations.handlers.nuo_jdbc_handler.nuo_jdbc_handler import NuoHandler
+from mindsdb.integrations.handlers.yugabyte_handler.yugabyte_handler import YugabyteHandler
 from mindsdb.api.mysql.mysql_proxy.libs.constants.response_type import RESPONSE_TYPE
 
-class NuoHandlerTest(unittest.TestCase):
+
+class YugabyteHandlerTest(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
         cls.kwargs = {
             "connection_data": {
                 "host": "localhost",
-                "port": 48006,
-                "database": "test",
-                "schema": "hockey",
-                "user": "dba",
-                "password": "goalie",
-                "is_direct": "true",
+                "port": 5433,
+                "user": "admin",
+                "password": "",
+                "database": "yugabyte"
             }
         }
-        cls.handler = NuoHandler('test_nuo_handler', **cls.kwargs)
+        cls.handler = YugabyteHandler('test_yugabyte_handler', cls.kwargs)
 
     def test_0_connect(self):
         self.handler.connect()
-    
-    def test_1_check_connection(self):
-        self.handler.check_connection()
 
-    def test_2_create(self):
-        res = self.handler.query('CREATE TABLE TESTTABLEX3 (ID INT PRIMARY KEY, NAME VARCHAR(14))')
-        assert res.type is RESPONSE_TYPE.OK
-
-    def test_3_insert(self):
-        res = self.handler.query("INSERT INTO TESTTABLEX3 VALUES (100,'ONE HUNDRED'),(200,'TWO HUNDRED'),(300,'THREE HUNDRED')")
-        assert res.type is RESPONSE_TYPE.OK
-
-    def test_4_select(self):
-        res = self.handler.query('SELECT * FROM HOCKEY')
-        assert res.type is RESPONSE_TYPE.TABLE
-    
-    def test_5_get_tables(self):
-        res = self.handler.get_tables()
-        assert res.type is RESPONSE_TYPE.TABLE
-
-    def test_6_get_columns(self):
-        res = self.handler.get_columns("HOCKEY")
-        assert res.type is RESPONSE_TYPE.TABLE
-    
+    def test_1_drop_table(self):
+        res = self.handler.query("DROP TABLE IF EXISTS PREM;")
+        assert res.type is not RESPONSE_TYPE.ERROR
+
+    def test_2_create_table(self):
+        res = self.handler.query("CREATE TABLE IF NOT EXISTS PREM (Premi varchar(50));")
+        assert res.type is not RESPONSE_TYPE.ERROR
+
+    def test_3_insert_table(self):
+        res = self.handler.query("INSERT INTO PREM VALUES('Radha <3 Krishna');")
+        assert res.type is not RESPONSE_TYPE.ERROR
+
+    def test_4_get_tables(self):
+        tables = self.handler.get_tables()
+        assert tables.type is not RESPONSE_TYPE.ERROR
+ 
+    def test_5_select_query(self):
+        query = "SELECT * FROM PREM;"
+        result = self.handler.native_query(query)
+        assert result.type is RESPONSE_TYPE.TABLE or RESPONSE_TYPE.OK
+
+    def test_6_check_connection(self):
+        self.handler.check_connection()
 
         
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/oceanbase_handler/icon.png` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/oceanbase_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/oceanbase_handler/oceanbase_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/oceanbase_handler/oceanbase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/oceanbase_handler/tests/test_oceanbase_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/oceanbase_handler/tests/test_oceanbase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/openai_handler/helpers.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/openai_handler/helpers.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/openai_handler/openai_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/openai_handler/openai_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/openai_handler/setup.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/openai_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/opengauss_handler/__init__.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/opengauss_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/opengauss_handler/opengauss_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/opengauss_handler/opengauss_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/opengauss_handler/tests/test_opengauss_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/opengauss_handler/tests/test_opengauss_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/oracle_handler/__init__.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/oracle_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/oracle_handler/icon.svg` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/oracle_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/oracle_handler/oracle_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/postgres_handler/postgres_handler.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,196 +1,173 @@
-from typing import Optional
-from collections import OrderedDict
-
-import pandas as pd
-import oracledb
-from oracledb import connect, Connection, makedsn
+import psycopg
+from psycopg.pq import ExecStatus
+from pandas import DataFrame
 
+from mindsdb_sql import parse_sql
 from mindsdb_sql.render.sqlalchemy_render import SqlalchemyRender
 from mindsdb_sql.parser.ast.base import ASTNode
 
-from mindsdb.utilities import log
 from mindsdb.integrations.libs.base import DatabaseHandler
+from mindsdb.utilities import log
 from mindsdb.integrations.libs.response import (
     HandlerStatusResponse as StatusResponse,
     HandlerResponse as Response,
-    RESPONSE_TYPE,
+    RESPONSE_TYPE
 )
-from mindsdb.integrations.libs.const import HANDLER_CONNECTION_ARG_TYPE as ARG_TYPE
-
-oracledb.defaults.fetch_lobs = False  # return LOBs directly as strings or bytes
+import mindsdb.utilities.profiler as profiler
 
 
-class OracleHandler(DatabaseHandler):
+class PostgresHandler(DatabaseHandler):
     """
-    This handler handles connection and execution of the Microsoft SQL Server statements.
+    This handler handles connection and execution of the PostgreSQL statements.
     """
+    name = 'postgres'
 
-    name = "oracle"
-
-    def __init__(self, name: str, connection_data: Optional[dict], **kwargs):
+    @profiler.profile('init_pg_handler')
+    def __init__(self, name=None, **kwargs):
         super().__init__(name)
-        self.host = connection_data.get("host")
-        self.port = int(connection_data.get("port") or 1521)
-        self.sid = connection_data.get("sid")
-        self.service_name = connection_data.get("service_name")
-        self.user = connection_data.get("user")
-        self.password = connection_data.get("password")
-
-        if self.sid is None and self.service_name is None:
-            raise ValueError("Either 'sid' or 'service_name' must be given")
-        if self.sid and self.service_name:
-            raise ValueError("Only one of 'sid' or 'service_name' must be given")
-
-        if self.sid:
-            self.dsn = makedsn(host=self.host, port=self.port, sid=self.sid)
-        else:
-            self.dsn = makedsn(host=self.host, port=self.port, service_name=self.service_name)
+        self.parser = parse_sql
+        self.connection_args = kwargs.get('connection_data')
+        self.dialect = 'postgresql'
+        self.database = self.connection_args.get('database')
+        self.renderer = SqlalchemyRender('postgres')
 
         self.connection = None
         self.is_connected = False
 
-    def connect(self) -> Connection:
+    def __del__(self):
+        if self.is_connected is True:
+            self.disconnect()
+
+    @profiler.profile()
+    def connect(self):
+        """
+        Handles the connection to a PostgreSQL database instance.
+        """
         if self.is_connected is True:
             return self.connection
 
-        connection = connect(user=self.user, password=self.password, dsn=self.dsn)
+        config = {
+            'host': self.connection_args.get('host'),
+            'port': self.connection_args.get('port'),
+            'user': self.connection_args.get('user'),
+            'password': self.connection_args.get('password'),
+            'dbname': self.connection_args.get('database')
+        }
+
+        if self.connection_args.get('sslmode'):
+            config['sslmode'] = self.connection_args.get('sslmode')
+
+        if self.connection_args.get('schema'):
+            config['options'] = f'-c search_path={self.connection_args.get("schema")},public'
+
+        connection = psycopg.connect(**config, connect_timeout=10)
 
         self.is_connected = True
         self.connection = connection
         return self.connection
 
     def disconnect(self):
-        if self.is_connected:
-            self.connection.close()
+        if self.is_connected is False:
+            return
+        self.connection.close()
         self.is_connected = False
-        return
 
     def check_connection(self) -> StatusResponse:
         """
-        Check the connection of the database
+        Check the connection of the PostgreSQL database
         :return: success status and error message if error occurs
         """
-
         response = StatusResponse(False)
         need_to_close = self.is_connected is False
 
         try:
-            con = self.connect()
-            con.ping()
+            connection = self.connect()
+            with connection.cursor() as cur:
+                cur.execute('select 1;')
             response.success = True
-        except Exception as e:
-            log.logger.error(f"Error connecting to Oracle DB {self.dsn}, {e}!")
-            response.error_message = str(e)
-        finally:
-            if response.success is True and need_to_close:
-                self.disconnect()
-            if response.success is False and self.is_connected is True:
-                self.is_connected = False
+        except psycopg.Error as e:
+            log.logger.error(f'Error connecting to PostgreSQL {self.database}, {e}!')
+            response.error_message = e
+
+        if response.success is True and need_to_close:
+            self.disconnect()
+        if response.success is False and self.is_connected is True:
+            self.is_connected = False
+
         return response
 
+    @profiler.profile()
     def native_query(self, query: str) -> Response:
         """
         Receive SQL query and runs it
-        :param query: The SQL query to run
+        :param query: The SQL query to run in PostgreSQL
         :return: returns the records from the current recordset
         """
         need_to_close = self.is_connected is False
 
         connection = self.connect()
         with connection.cursor() as cur:
             try:
                 cur.execute(query)
-                result = cur.fetchall()
-                if result:
+                if ExecStatus(cur.pgresult.status) == ExecStatus.COMMAND_OK:
+                    response = Response(RESPONSE_TYPE.OK)
+                else:
+                    result = cur.fetchall()
                     response = Response(
                         RESPONSE_TYPE.TABLE,
-                        data_frame=pd.DataFrame(
+                        DataFrame(
                             result,
-                            columns=[row[0] for row in cur.description],
-                        ),
+                            columns=[x.name for x in cur.description]
+                        )
                     )
-                else:
-                    response = Response(RESPONSE_TYPE.OK)
-
                 connection.commit()
             except Exception as e:
-                log.logger.error(f"Error running query: {query} on {self.dsn}!")
+                log.logger.error(f'Error running query: {query} on {self.database}!')
                 response = Response(
                     RESPONSE_TYPE.ERROR,
-                    error_message=str(e),
+                    error_code=0,
+                    error_message=str(e)
                 )
                 connection.rollback()
 
         if need_to_close is True:
             self.disconnect()
 
         return response
 
+    @profiler.profile()
     def query(self, query: ASTNode) -> Response:
         """
-        Retrieve the data from the SQL statement.
+        Retrieve the data from the SQL statement with eliminated rows that dont satisfy the WHERE condition
         """
-        renderer = SqlalchemyRender("oracle")
-        query_str = renderer.get_string(query, with_failback=True)
+        query_str = self.renderer.get_string(query, with_failback=True)
         return self.native_query(query_str)
 
     def get_tables(self) -> Response:
         """
-        List all tables in Oracle DB owned by the current user.
+        List all tables in PostgreSQL without the system tables information_schema and pg_catalog
         """
         query = """
-            SELECT table_name
-            FROM user_tables
-            ORDER BY 1;
+            SELECT
+                table_schema,
+                table_name,
+                table_type
+            FROM
+                information_schema.tables
+            WHERE
+                table_schema NOT IN ('information_schema', 'pg_catalog')
+                and table_type in ('BASE TABLE', 'VIEW')
         """
         return self.native_query(query)
 
     def get_columns(self, table_name: str) -> Response:
-        """
-        Show details about the table.
-        """
         query = f"""
-            SELECT 
-                column_name,
-                data_type
-            FROM USER_TAB_COLUMNS
-            WHERE table_name = '{table_name}'
-        """
-        result = self.native_query(query)
-        return result
-
-
-connection_args = OrderedDict(
-    host={
-        "type": ARG_TYPE.STR,
-        "description": "The host name or IP address of the Oracle DB.",
-    },
-    port={
-        "type": ARG_TYPE.INT,
-        "description": "The TCP/IP port of the Oracle DB. Must be an integer. Default 1521.",
-    },
-    sid={
-        "type": ARG_TYPE.STR,
-        "description": "The site identifier of the Oracle DB. Either sid or service_name should be provided.",
-    },
-    service_name={
-        "type": ARG_TYPE.STR,
-        "description": "The name of the Oracle DB service. Either sid or service_name should be provided.",
-    },
-    user={
-        "type": ARG_TYPE.STR,
-        "description": "The user name used to authenticate against the Oracle DB.",
-    },
-    password={
-        "type": ARG_TYPE.STR,
-        "description": "The password to authenticate the user against Oracle DB.",
-    },
-)
-
-connection_args_example = OrderedDict(
-    host="127.0.0.1",
-    port=1521,
-    user="admin",
-    password="password",
-    sid="ORCL",
-)
+            SELECT
+                column_name as "Field",
+                data_type as "Type"
+            FROM
+                information_schema.columns
+            WHERE
+                table_name = '{table_name}'
+        """
+        return self.native_query(query)
```

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/oracle_handler/tests/test_oracle_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/oracle_handler/tests/test_oracle_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/orioledb_handler/icon.svg` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/orioledb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/orioledb_handler/orioledb_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/orioledb_handler/orioledb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/orioledb_handler/tests/test_orioledb_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/orioledb_handler/tests/test_orioledb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/phoenix_handler/__init__.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/phoenix_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/phoenix_handler/icon.png` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/phoenix_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/phoenix_handler/phoenix_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/phoenix_handler/phoenix_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/phoenix_handler/tests/test_phoenix_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/phoenix_handler/tests/test_phoenix_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/pinot_handler/__init__.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/pinot_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/pinot_handler/icon.png` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/pinot_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/pinot_handler/pinot_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/pinot_handler/pinot_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/pinot_handler/tests/test_pinot_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/pinot_handler/tests/test_pinot_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/plaid_handler/icon.svg` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/plaid_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/plaid_handler/plaid_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/plaid_handler/plaid_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/plaid_handler/plaid_tables.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/plaid_handler/plaid_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/planetscale_handler/__init__.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/planetscale_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/planetscale_handler/icon.svg` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/planetscale_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/postgres_handler/icon.svg` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/postgres_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/postgres_handler/postgres_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/tdengine_handler/tdengine_handler.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,173 +1,183 @@
-import psycopg
-from psycopg.pq import ExecStatus
-from pandas import DataFrame
+from collections import OrderedDict
+from typing import Optional
+import pandas as pd
+import taosrest as td
+from taosrest import sqlalchemy as SA
 
 from mindsdb_sql import parse_sql
 from mindsdb_sql.render.sqlalchemy_render import SqlalchemyRender
 from mindsdb_sql.parser.ast.base import ASTNode
 
+from mindsdb.utilities.log import get_log
 from mindsdb.integrations.libs.base import DatabaseHandler
-from mindsdb.utilities import log
 from mindsdb.integrations.libs.response import (
     HandlerStatusResponse as StatusResponse,
     HandlerResponse as Response,
     RESPONSE_TYPE
 )
-import mindsdb.utilities.profiler as profiler
+from mindsdb.integrations.libs.const import HANDLER_CONNECTION_ARG_TYPE as ARG_TYPE
 
 
-class PostgresHandler(DatabaseHandler):
+log = get_log()
+
+
+class TDEngineHandler(DatabaseHandler):
     """
-    This handler handles connection and execution of the PostgreSQL statements.
+    This handler handles connection and execution of the TDEngine statements.
     """
-    name = 'postgres'
 
-    @profiler.profile('init_pg_handler')
-    def __init__(self, name=None, **kwargs):
+    name = 'tdengine'
+
+    def __init__(self, name, connection_data: Optional[dict], **kwargs):
         super().__init__(name)
+        
         self.parser = parse_sql
-        self.connection_args = kwargs.get('connection_data')
-        self.dialect = 'postgresql'
-        self.database = self.connection_args.get('database')
-        self.renderer = SqlalchemyRender('postgres')
+        self.dialect = 'tdengine'
+        self.kwargs = kwargs
+        self.connection_data = connection_data
 
         self.connection = None
         self.is_connected = False
 
-    def __del__(self):
-        if self.is_connected is True:
-            self.disconnect()
 
-    @profiler.profile()
     def connect(self):
-        """
-        Handles the connection to a PostgreSQL database instance.
-        """
         if self.is_connected is True:
             return self.connection
 
         config = {
-            'host': self.connection_args.get('host'),
-            'port': self.connection_args.get('port'),
-            'user': self.connection_args.get('user'),
-            'password': self.connection_args.get('password'),
-            'dbname': self.connection_args.get('database')
+            'url': self.connection_data.get('url', "http://localhost:6041"),
+            'token': self.connection_data.get('token'),
+            'user': self.connection_data.get('user','root'),
+            'password': self.connection_data.get('password','taosdata'),
+            'database': self.connection_data.get('database')
         }
 
-        if self.connection_args.get('sslmode'):
-            config['sslmode'] = self.connection_args.get('sslmode')
-
-        if self.connection_args.get('schema'):
-            config['options'] = f'-c search_path={self.connection_args.get("schema")},public'
-
-        connection = psycopg.connect(**config, connect_timeout=10)
-
+        connection = td.connect(**config)
         self.is_connected = True
         self.connection = connection
         return self.connection
 
     def disconnect(self):
         if self.is_connected is False:
             return
         self.connection.close()
         self.is_connected = False
+        return
 
     def check_connection(self) -> StatusResponse:
-        """
-        Check the connection of the PostgreSQL database
-        :return: success status and error message if error occurs
-        """
-        response = StatusResponse(False)
+       
+        result = StatusResponse(False)
         need_to_close = self.is_connected is False
 
         try:
             connection = self.connect()
-            with connection.cursor() as cur:
-                cur.execute('select 1;')
-            response.success = True
-        except psycopg.Error as e:
-            log.logger.error(f'Error connecting to PostgreSQL {self.database}, {e}!')
-            response.error_message = e
+            result.success = connection is not None
+        except Exception as e:
+            log.error(f'Error connecting to TDEngine {self.connection_data["database"]}, {e}!')
+            result.error_message = str(e)
 
-        if response.success is True and need_to_close:
+        if result.success is True and need_to_close:
             self.disconnect()
-        if response.success is False and self.is_connected is True:
+        if result.success is False and self.is_connected is True:
             self.is_connected = False
 
-        return response
+        return result
 
-    @profiler.profile()
     def native_query(self, query: str) -> Response:
         """
         Receive SQL query and runs it
-        :param query: The SQL query to run in PostgreSQL
+        :param query: The SQL query to run in TDEngine
         :return: returns the records from the current recordset
         """
+
         need_to_close = self.is_connected is False
 
         connection = self.connect()
-        with connection.cursor() as cur:
-            try:
+        cur = connection.cursor() 
+        try:
                 cur.execute(query)
-                if ExecStatus(cur.pgresult.status) == ExecStatus.COMMAND_OK:
-                    response = Response(RESPONSE_TYPE.OK)
-                else:
+                
+                if cur.rowcount != 0:
                     result = cur.fetchall()
                     response = Response(
                         RESPONSE_TYPE.TABLE,
-                        DataFrame(
+                        pd.DataFrame(
                             result,
-                            columns=[x.name for x in cur.description]
+                            columns=[x[0] for x in cur.description]
                         )
                     )
+                else:
+                    response = Response(RESPONSE_TYPE.OK)
                 connection.commit()
-            except Exception as e:
-                log.logger.error(f'Error running query: {query} on {self.database}!')
+        except Exception as e:
+                log.error(f'Error running query: {query} on {self.connection_data["database"]}!')
                 response = Response(
                     RESPONSE_TYPE.ERROR,
-                    error_code=0,
                     error_message=str(e)
                 )
-                connection.rollback()
-
+                # connection.rollback()
+        cur.close()
         if need_to_close is True:
             self.disconnect()
 
         return response
 
-    @profiler.profile()
     def query(self, query: ASTNode) -> Response:
         """
-        Retrieve the data from the SQL statement with eliminated rows that dont satisfy the WHERE condition
+        Retrieve the data from the SQL statement.
         """
-        query_str = self.renderer.get_string(query, with_failback=True)
+        renderer = SqlalchemyRender(SA.TaosRestDialect)
+        query_str = renderer.get_string(query, with_failback=True)
         return self.native_query(query_str)
 
     def get_tables(self) -> Response:
         """
-        List all tables in PostgreSQL without the system tables information_schema and pg_catalog
+        Get a list with all of the tabels in TDEngine
         """
-        query = """
-            SELECT
-                table_schema,
-                table_name,
-                table_type
-            FROM
-                information_schema.tables
-            WHERE
-                table_schema NOT IN ('information_schema', 'pg_catalog')
-                and table_type in ('BASE TABLE', 'VIEW')
-        """
-        return self.native_query(query)
-
-    def get_columns(self, table_name: str) -> Response:
-        query = f"""
-            SELECT
-                column_name as "Field",
-                data_type as "Type"
-            FROM
-                information_schema.columns
-            WHERE
-                table_name = '{table_name}'
+        q = 'SHOW TABLES;'
+
+         
+        return self.native_query(q)
+
+    def get_columns(self, table_name) -> Response:
         """
-        return self.native_query(query)
+        Show details about the table
+        """
+        q = f'DESCRIBE {table_name};'
+
+        
+        return self.native_query(q)
+
+
+connection_args = OrderedDict(
+    user={
+        'type': ARG_TYPE.STR,
+        'description': 'The user name used to authenticate with the TDEngine server.'
+    },
+    password={
+        'type': ARG_TYPE.STR,
+        'description': 'The password to authenticate the user with the TDEngine server.'
+    },
+    database={
+        'type': ARG_TYPE.STR,
+        'description': 'The database name to use when connecting with the TDEngine server.'
+    },
+    url={
+        'type': ARG_TYPE.STR,
+        'description': 'The url of the TDEngine server Instance. '
+    },
+    token={
+        'type': ARG_TYPE.INT,
+        'description': 'Unique Token to COnnect TDEngine'
+    },
+
+
+)
+
+connection_args_example = OrderedDict(
+    url='127.0.0.1:6041',
+    token='<token comes here>',
+    user='root',
+    password='taosdata',
+    database='test'
+)
```

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/questdb_handler/icon.svg` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/questdb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/questdb_handler/questdb_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/questdb_handler/questdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/questdb_handler/tests/test_questdb_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/questdb_handler/tests/test_questdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/ray_serve_handler/__init__.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/ray_serve_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/ray_serve_handler/ray_serve_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/ray_serve_handler/ray_serve_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/ray_serve_handler/setup.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/ray_serve_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/reddit_handler/icon.svg` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/reddit_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/reddit_handler/reddit_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/reddit_handler/reddit_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/reddit_handler/reddit_tables.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/reddit_handler/reddit_tables.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/redshift_handler/__init__.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/redshift_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/redshift_handler/icon.png` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/redshift_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/redshift_handler/redshift_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/redshift_handler/redshift_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/redshift_handler/tests/test_redshift_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/redshift_handler/tests/test_redshift_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/rockset_handler/icon.png` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/rockset_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/rockset_handler/tests/test.png` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/rockset_handler/tests/test.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/rockset_handler/tests/test2.png` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/rockset_handler/tests/test2.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/s3_handler/__init__.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/s3_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/s3_handler/icon.png` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/s3_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/s3_handler/s3_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/s3_handler/s3_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/s3_handler/tests/test_s3_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/s3_handler/tests/test_s3_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/scylla_handler/__init__.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/scylla_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/scylla_handler/logo.png` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/scylla_handler/logo.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/scylla_handler/scylla_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/scylla_handler/scylla_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/scylla_handler/tests/test_scylla_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/scylla_handler/tests/test_scylla_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/sheets_handler/__init__.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/surrealdb_handler/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from mindsdb.integrations.libs.const import HANDLER_TYPE
-
 from .__about__ import __version__ as version, __description__ as description
+
 try:
-    from .sheets_handler import (
-        SheetsHandler as Handler,
+    from .surrealdb_handler import (
+        SurrealDBHandler as Handler,
         connection_args_example,
-        connection_args
-    )
+        connection_args)
     import_error = None
 except Exception as e:
     Handler = None
     import_error = e
 
-title = 'Google Sheets'
-name = 'sheets'
+title = 'SurrealDB'
+name = 'surrealdb'
 type = HANDLER_TYPE.DATA
 icon_path = 'icon.png'
 
 __all__ = [
     'Handler', 'version', 'name', 'type', 'title', 'description',
     'connection_args', 'connection_args_example', 'import_error', 'icon_path'
 ]
```

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/sheets_handler/icon.png` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/sheets_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/sheets_handler/sheets_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/sheets_handler/sheets_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/sheets_handler/tests/test_sheets_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/sheets_handler/tests/test_sheets_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/singlestore_handler/tests/test_singlestore_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/singlestore_handler/tests/test_singlestore_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/snowflake_handler/snowflake_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/snowflake_handler/snowflake_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/snowflake_handler/tests/test_snowflake_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/snowflake_handler/tests/test_snowflake_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/solr_handler/__init__.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/solr_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/solr_handler/solr.svg` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/solr_handler/solr.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/solr_handler/solr_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/solr_handler/solr_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/solr_handler/tests/test_solr_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/solr_handler/tests/test_solr_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/sqlany_handler/__init__.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/sqlany_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/sqlany_handler/icon.svg` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/sqlany_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/sqlany_handler/sqlany_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/sqlany_handler/sqlany_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/sqlite_handler/__init__.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/sqlite_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/sqlite_handler/db_connection.png` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/sqlite_handler/db_connection.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/sqlite_handler/error.png` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/sqlite_handler/error.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/sqlite_handler/icon.png` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/sqlite_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/sqlite_handler/model_drop.png` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/sqlite_handler/model_drop.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/sqlite_handler/prediction_result.png` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/sqlite_handler/prediction_result.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/sqlite_handler/predictor_model.png` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/sqlite_handler/predictor_model.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/sqlite_handler/sqlite_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/sqlite_handler/sqlite_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/sqlite_handler/tests/test_sqlite_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/sqlite_handler/tests/test_sqlite_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/sqreamdb_handler/__init__.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/sqreamdb_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/sqreamdb_handler/icon.png` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/sqreamdb_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/sqreamdb_handler/sqreamdb_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/sqreamdb_handler/sqreamdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/sqreamdb_handler/tests/test_sqreamdb_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/sqreamdb_handler/tests/test_sqreamdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/starrocks_handler/icon.png` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/starrocks_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/starrocks_handler/starrocks_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/starrocks_handler/starrocks_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/starrocks_handler/tests/test_starrocks_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/starrocks_handler/tests/test_starrocks_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/statsforecast_handler/setup.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/statsforecast_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/statsforecast_handler/statsforecast_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/statsforecast_handler/statsforecast_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/supabase_handler/icon.svg` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/supabase_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/supabase_handler/tests/test_supabase_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/supabase_handler/tests/test_supabase_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/surrealdb_handler/__init__.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/tidb_handler/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from mindsdb.integrations.libs.const import HANDLER_TYPE
-from .__about__ import __version__ as version, __description__ as description
 
 try:
-    from .surrealdb_handler import (
-        SurrealDBHandler as Handler,
+    from .tidb_handler import (
+        TiDBHandler as Handler,
         connection_args_example,
-        connection_args)
+        connection_args
+    )
     import_error = None
 except Exception as e:
     Handler = None
     import_error = e
+from .__about__ import __version__ as version, __description__ as description
+
 
-title = 'SurrealDB'
-name = 'surrealdb'
+title = 'TiDB'
+name = 'tidb'
 type = HANDLER_TYPE.DATA
-icon_path = 'icon.png'
 
 __all__ = [
     'Handler', 'version', 'name', 'type', 'title', 'description',
     'connection_args', 'connection_args_example', 'import_error', 'icon_path'
 ]
```

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/surrealdb_handler/icon.png` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/surrealdb_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/surrealdb_handler/surrealdb_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/surrealdb_handler/surrealdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/surrealdb_handler/tests/test_surrealdb_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/surrealdb_handler/tests/test_surrealdb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/surrealdb_handler/utils/surreal_get_info.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/surrealdb_handler/utils/surreal_get_info.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/tdengine_handler/__init__.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/tdengine_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/tdengine_handler/icon.svg` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/tdengine_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/tdengine_handler/tdengine_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/vertica_handler/vertica_handler.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,62 +1,65 @@
 from collections import OrderedDict
 from typing import Optional
 import pandas as pd
-import taosrest as td
-from taosrest import sqlalchemy as SA
+import vertica_python as vp
+
 
 from mindsdb_sql import parse_sql
 from mindsdb_sql.render.sqlalchemy_render import SqlalchemyRender
 from mindsdb_sql.parser.ast.base import ASTNode
 
-from mindsdb.utilities.log import get_log
+from mindsdb.utilities import log
 from mindsdb.integrations.libs.base import DatabaseHandler
 from mindsdb.integrations.libs.response import (
     HandlerStatusResponse as StatusResponse,
     HandlerResponse as Response,
     RESPONSE_TYPE
 )
 from mindsdb.integrations.libs.const import HANDLER_CONNECTION_ARG_TYPE as ARG_TYPE
 
+# from sqlalchemy_vertica.dialect_pyodbc  import VerticaDialect
+from sqla_vertica_python.vertica_python import VerticaDialect
+
 
-log = get_log()
 
 
-class TDEngineHandler(DatabaseHandler):
+class VerticaHandler(DatabaseHandler):
     """
-    This handler handles connection and execution of the TDEngine statements.
+    This handler handles connection and execution of the Vertica statements.
     """
 
-    name = 'tdengine'
+    name = 'vertica'
 
     def __init__(self, name, connection_data: Optional[dict], **kwargs):
         super().__init__(name)
         
         self.parser = parse_sql
-        self.dialect = 'tdengine'
+        self.dialect = 'vertica'
         self.kwargs = kwargs
         self.connection_data = connection_data
+        self.schema_name = connection_data['schema_name'] if 'schema_name' in connection_data else "public"
 
         self.connection = None
         self.is_connected = False
 
 
     def connect(self):
         if self.is_connected is True:
             return self.connection
 
         config = {
-            'url': self.connection_data.get('url', "http://localhost:6041"),
-            'token': self.connection_data.get('token'),
-            'user': self.connection_data.get('user','root'),
-            'password': self.connection_data.get('password','taosdata'),
-            'database': self.connection_data.get('database')
+            'host': self.connection_data['host'],
+            'port': self.connection_data['port'],
+            'user': self.connection_data['user'],
+            'password': self.connection_data['password'],
+            'database': self.connection_data['database']
         }
 
-        connection = td.connect(**config)
+        connection = vp.connect(**config)
         self.is_connected = True
         self.connection = connection
         return self.connection
 
     def disconnect(self):
         if self.is_connected is False:
             return
@@ -67,117 +70,131 @@
     def check_connection(self) -> StatusResponse:
        
         result = StatusResponse(False)
         need_to_close = self.is_connected is False
 
         try:
             connection = self.connect()
-            result.success = connection is not None
+            result.success = connection.opened()
         except Exception as e:
-            log.error(f'Error connecting to TDEngine {self.connection_data["database"]}, {e}!')
+            log.logger.error(f'Error connecting to Vertica {self.connection_data["database"]}, {e}!')
             result.error_message = str(e)
 
         if result.success is True and need_to_close:
             self.disconnect()
         if result.success is False and self.is_connected is True:
             self.is_connected = False
 
         return result
 
     def native_query(self, query: str) -> Response:
         """
         Receive SQL query and runs it
-        :param query: The SQL query to run in TDEngine
+        :param query: The SQL query to run in VERTICA
         :return: returns the records from the current recordset
         """
 
         need_to_close = self.is_connected is False
 
         connection = self.connect()
-        cur = connection.cursor() 
-        try:
-                cur.execute(query)
-                
-                if cur.rowcount != 0:
-                    result = cur.fetchall()
+        with connection.cursor() as cur:
+            try:
+                e=cur.execute(query)
+                result = e.fetchall()
+                if e.rowcount != -1:
+                    
                     response = Response(
                         RESPONSE_TYPE.TABLE,
                         pd.DataFrame(
                             result,
-                            columns=[x[0] for x in cur.description]
+                            columns=[x.name for x in cur.description]
                         )
                     )
                 else:
                     response = Response(RESPONSE_TYPE.OK)
                 connection.commit()
-        except Exception as e:
-                log.error(f'Error running query: {query} on {self.connection_data["database"]}!')
+            except Exception as e:
+                log.logger.error(f'Error running query: {query} on {self.connection_data["database"]}!')
                 response = Response(
                     RESPONSE_TYPE.ERROR,
                     error_message=str(e)
                 )
-                # connection.rollback()
-        cur.close()
+                connection.rollback()
+
         if need_to_close is True:
             self.disconnect()
 
         return response
 
     def query(self, query: ASTNode) -> Response:
         """
         Retrieve the data from the SQL statement.
         """
-        renderer = SqlalchemyRender(SA.TaosRestDialect)
+        renderer = SqlalchemyRender(VerticaDialect)
         query_str = renderer.get_string(query, with_failback=True)
         return self.native_query(query_str)
 
     def get_tables(self) -> Response:
         """
-        Get a list with all of the tabels in TDEngine
+        Get a list with all of the tabels in VERTICA
         """
-        q = 'SHOW TABLES;'
+        q = f'''SELECT 
+        TABLE_NAME,
+        TABLE_SCHEMA
+        from v_catalog.tables 
+        WHERE table_schema='{self.schema_name}' 
+        order by
+        table_name;'''
 
          
         return self.native_query(q)
 
     def get_columns(self, table_name) -> Response:
         """
         Show details about the table
         """
-        q = f'DESCRIBE {table_name};'
+        q = f'''SELECT 
+        column_name , 
+        data_type 
+        FROM v_catalog.columns 
+        WHERE table_name='{table_name}';'''
 
         
         return self.native_query(q)
 
 
 connection_args = OrderedDict(
     user={
         'type': ARG_TYPE.STR,
-        'description': 'The user name used to authenticate with the TDEngine server.'
+        'description': 'The user name used to authenticate with the Vertica server.'
     },
     password={
         'type': ARG_TYPE.STR,
-        'description': 'The password to authenticate the user with the TDEngine server.'
+        'description': 'The password to authenticate the user with the VERTICA server.'
     },
     database={
         'type': ARG_TYPE.STR,
-        'description': 'The database name to use when connecting with the TDEngine server.'
+        'description': 'The database name to use when connecting with the VERTICA server.'
     },
-    url={
+    host={
         'type': ARG_TYPE.STR,
-        'description': 'The url of the TDEngine server Instance. '
+        'description': 'The host name or IP address of the VERTICA server. NOTE: use \'127.0.0.1\' instead of \'localhost\' to connect to local server.'
     },
-    token={
+    port={
         'type': ARG_TYPE.INT,
-        'description': 'Unique Token to COnnect TDEngine'
+        'description': 'The TCP/IP port of the VERTICA server. Must be an integer.'
     },
-
+    schema_name={
+        'type': ARG_TYPE.STR,
+        'description': 'Table are listed according to schema name (it is optional). Note: Default value is "public"'
+    }
 
 )
 
 connection_args_example = OrderedDict(
-    url='127.0.0.1:6041',
-    token='<token comes here>',
+    host='127.0.0.1',
+    port=5433,
     user='root',
-    password='taosdata',
-    database='test'
+    password='password',
+    database='database',
+    schema_name='xyz'
 )
```

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/tdengine_handler/tests/test_tdengine_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/tdengine_handler/tests/test_tdengine_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/teradata_handler/__init__.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/teradata_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/teradata_handler/icon.svg` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/teradata_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/teradata_handler/teradata_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/teradata_handler/teradata_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/tidb_handler/tests/test_tidb_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/tidb_handler/tests/test_tidb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/tidb_handler/tidb_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/tidb_handler/tidb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/timescaledb_handler/icon.svg` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/timescaledb_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/timescaledb_handler/tests/test_timescaledb_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/timescaledb_handler/tests/test_timescaledb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/timescaledb_handler/timescaledb_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/timescaledb_handler/timescaledb_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/tpot_handler/setup.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/tpot_handler/setup.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/tpot_handler/tpot_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/tpot_handler/tpot_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/trino_handler/icon.png` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/trino_handler/icon.png`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/trino_handler/tests/test_trino_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/trino_handler/tests/test_trino_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/trino_handler/trino_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/trino_handler/trino_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/twitter_handler/icon.svg` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/twitter_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/twitter_handler/twitter_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/twitter_handler/twitter_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/vertica_handler/__init__.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/vertica_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/vertica_handler/icon.svg` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/vertica_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/vertica_handler/tests/test_vertica_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/vertica_handler/tests/test_vertica_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/vertica_handler/vertica_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/yugabyte_handler/yugabyte_handler.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,200 +1,177 @@
-from collections import OrderedDict
+import psycopg2
+from pandas import DataFrame
 from typing import Optional
-import pandas as pd
-import vertica_python as vp
-
-
+from collections import OrderedDict
+from mindsdb.integrations.libs.const import HANDLER_CONNECTION_ARG_TYPE as ARG_TYPE
 from mindsdb_sql import parse_sql
 from mindsdb_sql.render.sqlalchemy_render import SqlalchemyRender
 from mindsdb_sql.parser.ast.base import ASTNode
 
-from mindsdb.utilities import log
 from mindsdb.integrations.libs.base import DatabaseHandler
+from mindsdb.utilities import log
 from mindsdb.integrations.libs.response import (
     HandlerStatusResponse as StatusResponse,
     HandlerResponse as Response,
     RESPONSE_TYPE
 )
-from mindsdb.integrations.libs.const import HANDLER_CONNECTION_ARG_TYPE as ARG_TYPE
-
-# from sqlalchemy_vertica.dialect_pyodbc  import VerticaDialect
-from sqla_vertica_python.vertica_python import VerticaDialect
 
 
-
-
-class VerticaHandler(DatabaseHandler):
+class YugabyteHandler(DatabaseHandler):
     """
-    This handler handles connection and execution of the Vertica statements.
+    This handler handles connection and execution of the YugabyteSQL statements.
     """
+    name = 'yugabyte'
 
-    name = 'vertica'
-
-    def __init__(self, name, connection_data: Optional[dict], **kwargs):
+    def __init__(self, name: str, connection_data: Optional[dict], **kwargs):
         super().__init__(name)
-        
         self.parser = parse_sql
-        self.dialect = 'vertica'
-        self.kwargs = kwargs
         self.connection_data = connection_data
-        self.schema_name = connection_data['schema_name'] if 'schema_name' in connection_data else "public"
+        self.dialect = 'postgresql'
+        self.database = connection_data['database']
+        self.renderer = SqlalchemyRender('postgres')
 
         self.connection = None
         self.is_connected = False
 
 
     def connect(self):
+        """
+        Handles the connection to a YugabyteSQL database insance.
+        """
         if self.is_connected is True:
             return self.connection
-
-        config = {
-            'host': self.connection_data['host'],
-            'port': self.connection_data['port'],
-            'user': self.connection_data['user'],
-            'password': self.connection_data['password'],
-            'database': self.connection_data['database']
+        
+        args={
+            "dbname": self.database,
+            "host": self.connection_data['host'],
+            "port": self.connection_data['port'],
+            "user": self.connection_data['user'],
+            "password": self.connection_data['password'],
         }
 
-        connection = vp.connect(**config)
+
+
+        connection = psycopg2.connect(**args, connect_timeout=10)
+
         self.is_connected = True
         self.connection = connection
         return self.connection
 
-    def disconnect(self):
-        if self.is_connected is False:
-            return
-        self.connection.close()
-        self.is_connected = False
-        return
-
     def check_connection(self) -> StatusResponse:
-       
-        result = StatusResponse(False)
+        """
+        Check the connection of the PostgreSQL database
+        :return: success status and error message if error occurs
+        """
+        response = StatusResponse(False)
         need_to_close = self.is_connected is False
 
         try:
             connection = self.connect()
-            result.success = connection.opened()
-        except Exception as e:
-            log.logger.error(f'Error connecting to Vertica {self.connection_data["database"]}, {e}!')
-            result.error_message = str(e)
+            with connection.cursor() as cur:
+                cur.execute('select 1;')
+            response.success = True
+        except psycopg2.Error as e:
+            log.logger.error(f'Error connecting to PostgreSQL {self.database}, {e}!')
+            response.error_message = e
 
-        if result.success is True and need_to_close:
+        if response.success is True and need_to_close:
             self.disconnect()
-        if result.success is False and self.is_connected is True:
+        if response.success is False and self.is_connected is True:
             self.is_connected = False
 
-        return result
+        return response
 
-    def native_query(self, query: str) -> Response:
-        """
-        Receive SQL query and runs it
-        :param query: The SQL query to run in VERTICA
-        :return: returns the records from the current recordset
+    def native_query(self, query: str) -> StatusResponse:
+        """Receive raw query and act upon it somehow.
+        Args:
+            query (Any): query in native format (str for sql databases,
+                dict for mongo, etc)
+        Returns:
+            HandlerResponse
         """
-
         need_to_close = self.is_connected is False
-
-        connection = self.connect()
-        with connection.cursor() as cur:
+        conn = self.connect()
+        with conn.cursor() as cur:
             try:
-                e=cur.execute(query)
-                result = e.fetchall()
-                if e.rowcount != -1:
-                    
+                cur.execute(query)
+                   
+                if cur.rowcount >0 and query.upper().startswith('SELECT') :
+                    result = cur.fetchall() 
                     response = Response(
                         RESPONSE_TYPE.TABLE,
-                        pd.DataFrame(
+                        data_frame=DataFrame(
                             result,
-                            columns=[x.name for x in cur.description]
+                            columns=[x[0] for x in cur.description]
                         )
                     )
                 else:
                     response = Response(RESPONSE_TYPE.OK)
-                connection.commit()
+                self.connection.commit()
             except Exception as e:
-                log.logger.error(f'Error running query: {query} on {self.connection_data["database"]}!')
+                log.logger.error(f'Error running query: {query} on {self.database}!')
                 response = Response(
                     RESPONSE_TYPE.ERROR,
                     error_message=str(e)
                 )
-                connection.rollback()
+                self.connection.rollback()
 
         if need_to_close is True:
             self.disconnect()
 
         return response
 
     def query(self, query: ASTNode) -> Response:
         """
-        Retrieve the data from the SQL statement.
+        Retrieve the data from the SQL statement with eliminated rows that dont satisfy the WHERE condition
         """
-        renderer = SqlalchemyRender(VerticaDialect)
-        query_str = renderer.get_string(query, with_failback=True)
+        query_str = self.renderer.get_string(query, with_failback=True)
         return self.native_query(query_str)
 
     def get_tables(self) -> Response:
         """
-        Get a list with all of the tabels in VERTICA
+        List all tabels in PostgreSQL without the system tables information_schema and pg_catalog
         """
-        q = f'''SELECT 
-        TABLE_NAME,
-        TABLE_SCHEMA
-        from v_catalog.tables 
-        WHERE table_schema='{self.schema_name}' 
-        order by
-        table_name;'''
-
-         
-        return self.native_query(q)
-
-    def get_columns(self, table_name) -> Response:
-        """
-        Show details about the table
-        """
-        q = f'''SELECT 
-        column_name , 
-        data_type 
-        FROM v_catalog.columns 
-        WHERE table_name='{table_name}';'''
 
-        
-        return self.native_query(q)
+        query = """SELECT table_schema,table_name,table_type FROM information_schema.tables WHERE table_schema NOT IN ('information_schema', 'pg_catalog') and table_type in ('BASE TABLE', 'VIEW')"""
+        return self.query(query)
+
+    def get_columns(self, table_name):
+        query = f"""SELECT column_name as "Field", data_type as "Type" FROM information_schema.columns WHERE table_name = '{table_name}'"""
+        return self.query(query)
+
 
 
 connection_args = OrderedDict(
-    user={
-        'type': ARG_TYPE.STR,
-        'description': 'The user name used to authenticate with the Vertica server.'
-    },
-    password={
+    host={
         'type': ARG_TYPE.STR,
-        'description': 'The password to authenticate the user with the VERTICA server.'
+        'description': 'The host name or IP address of the YugabyteDB server/database.'
     },
-    database={
+    user={
         'type': ARG_TYPE.STR,
-        'description': 'The database name to use when connecting with the VERTICA server.'
+        'description': 'The user name used to authenticate with the YugabyteDB server.'
     },
-    host={
+    password={
         'type': ARG_TYPE.STR,
-        'description': 'The host name or IP address of the VERTICA server. NOTE: use \'127.0.0.1\' instead of \'localhost\' to connect to local server.'
+        'description': 'The password to authenticate the user with the YugabyteDB server.'
     },
     port={
         'type': ARG_TYPE.INT,
-        'description': 'The TCP/IP port of the VERTICA server. Must be an integer.'
-    },
-    schema_name={
+        'description': 'Specify port to connect YugabyteDB server'
+    }, 
+    database={
         'type': ARG_TYPE.STR,
-        'description': 'Table are listed according to schema name (it is optional). Note: Default value is "public"'
-    }
+        'description': 'Specify database name  to connect YugabyteDB server'
+    },
+
 
 )
 
 connection_args_example = OrderedDict(
     host='127.0.0.1',
     port=5433,
-    user='root',
-    password='password',
-    database='database',
-    schema_name='xyz'
+    password='',
+    user='admin',
+    database='yugabyte'
+    
+
 )
```

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/vitess_handler/icon.svg` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/vitess_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/vitess_handler/tests/test_vitess_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/vitess_handler/tests/test_vitess_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/vitess_handler/vitess_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/vitess_handler/vitess_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers/yugabyte_handler/icon.svg` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers/yugabyte_handler/icon.svg`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers_client/db_client_factory.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers_client/db_client_factory.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers_client/db_grpc_client.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers_client/db_grpc_client.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers_client/ml_client_factory.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers_client/ml_client_factory.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers_client/ml_grpc_client.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers_client/ml_grpc_client.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers_wrapper/db_grpc_wrapper.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers_wrapper/db_grpc_wrapper.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers_wrapper/db_handler_service.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers_wrapper/db_handler_service.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers_wrapper/ml_grpc_wrapper.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers_wrapper/ml_grpc_wrapper.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/handlers_wrapper/ml_handler_service.py` & `MindsDB-23.4.4.3/mindsdb/integrations/handlers_wrapper/ml_handler_service.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/libs/api_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/libs/api_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/libs/base.py` & `MindsDB-23.4.4.3/mindsdb/integrations/libs/base.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/libs/handler_helpers.py` & `MindsDB-23.4.4.3/mindsdb/integrations/libs/handler_helpers.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/libs/ml_exec_base.py` & `MindsDB-23.4.4.3/mindsdb/integrations/libs/ml_exec_base.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/libs/ml_handler_proc.py` & `MindsDB-23.4.4.3/mindsdb/integrations/libs/ml_handler_proc.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/libs/net_helpers.py` & `MindsDB-23.4.4.3/mindsdb/integrations/libs/net_helpers.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/libs/response.py` & `MindsDB-23.4.4.3/mindsdb/integrations/libs/response.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/libs/storage_handler.py` & `MindsDB-23.4.4.3/mindsdb/integrations/libs/storage_handler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/utilities/date_utils.py` & `MindsDB-23.4.4.3/mindsdb/integrations/utilities/date_utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/utilities/install.py` & `MindsDB-23.4.4.3/mindsdb/integrations/utilities/install.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/utilities/sql_utils.py` & `MindsDB-23.4.4.3/mindsdb/integrations/utilities/sql_utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/utilities/test_utils.py` & `MindsDB-23.4.4.3/mindsdb/integrations/utilities/test_utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/integrations/utilities/time_series_utils.py` & `MindsDB-23.4.4.3/mindsdb/integrations/utilities/time_series_utils.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/interfaces/database/database.py` & `MindsDB-23.4.4.3/mindsdb/interfaces/database/database.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/interfaces/database/integrations.py` & `MindsDB-23.4.4.3/mindsdb/interfaces/database/integrations.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/interfaces/database/projects.py` & `MindsDB-23.4.4.3/mindsdb/interfaces/database/projects.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/interfaces/database/views.py` & `MindsDB-23.4.4.3/mindsdb/interfaces/database/views.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/interfaces/file/file_controller.py` & `MindsDB-23.4.4.3/mindsdb/interfaces/file/file_controller.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/interfaces/jobs/jobs_controller.py` & `MindsDB-23.4.4.3/mindsdb/interfaces/jobs/jobs_controller.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/interfaces/jobs/scheduler.py` & `MindsDB-23.4.4.3/mindsdb/interfaces/jobs/scheduler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/interfaces/model/functions.py` & `MindsDB-23.4.4.3/mindsdb/interfaces/model/functions.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/interfaces/model/model_controller.py` & `MindsDB-23.4.4.3/mindsdb/interfaces/model/model_controller.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/interfaces/storage/db.py` & `MindsDB-23.4.4.3/mindsdb/interfaces/storage/db.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/interfaces/storage/fs.py` & `MindsDB-23.4.4.3/mindsdb/interfaces/storage/fs.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/interfaces/storage/json.py` & `MindsDB-23.4.4.3/mindsdb/interfaces/storage/json.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/interfaces/storage/model_fs.py` & `MindsDB-23.4.4.3/mindsdb/interfaces/storage/model_fs.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/interfaces/stream/base/integration.py` & `MindsDB-23.4.4.3/mindsdb/interfaces/stream/base/integration.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/interfaces/stream/kafka/kafkadb.py` & `MindsDB-23.4.4.3/mindsdb/interfaces/stream/kafka/kafkadb.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/interfaces/stream/redis/redisdb.py` & `MindsDB-23.4.4.3/mindsdb/interfaces/stream/redis/redisdb.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/interfaces/stream/stream.py` & `MindsDB-23.4.4.3/mindsdb/interfaces/stream/stream.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/microservices_grpc/db/common_pb2.py` & `MindsDB-23.4.4.3/mindsdb/microservices_grpc/db/common_pb2.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/microservices_grpc/db/db_pb2.py` & `MindsDB-23.4.4.3/mindsdb/microservices_grpc/db/db_pb2.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/microservices_grpc/db/db_pb2_grpc.py` & `MindsDB-23.4.4.3/mindsdb/microservices_grpc/db/db_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/microservices_grpc/executor/executor_pb2.py` & `MindsDB-23.4.4.3/mindsdb/microservices_grpc/executor/executor_pb2.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/microservices_grpc/executor/executor_pb2_grpc.py` & `MindsDB-23.4.4.3/mindsdb/microservices_grpc/executor/executor_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/microservices_grpc/ml/common_pb2.py` & `MindsDB-23.4.4.3/mindsdb/microservices_grpc/ml/common_pb2.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/microservices_grpc/ml/ml_pb2.py` & `MindsDB-23.4.4.3/mindsdb/microservices_grpc/ml/ml_pb2.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/microservices_grpc/ml/ml_pb2_grpc.py` & `MindsDB-23.4.4.3/mindsdb/microservices_grpc/ml/ml_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/migrations/alembic.ini` & `MindsDB-23.4.4.3/mindsdb/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/migrations/env.py` & `MindsDB-23.4.4.3/mindsdb/migrations/env.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/migrations/migrate.py` & `MindsDB-23.4.4.3/mindsdb/migrations/migrate.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/migrations/versions/2021-11-30_17c3d2384711_init.py` & `MindsDB-23.4.4.3/mindsdb/migrations/versions/2021-11-30_17c3d2384711_init.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/migrations/versions/2022-01-26_47f97b83cee4_views.py` & `MindsDB-23.4.4.3/mindsdb/migrations/versions/2022-01-26_47f97b83cee4_views.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/migrations/versions/2022-02-09_27c5aca9e47e_db_files.py` & `MindsDB-23.4.4.3/mindsdb/migrations/versions/2022-02-09_27c5aca9e47e_db_files.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/migrations/versions/2022-05-25_d74c189b87e6_predictor_integration.py` & `MindsDB-23.4.4.3/mindsdb/migrations/versions/2022-05-25_d74c189b87e6_predictor_integration.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/migrations/versions/2022-07-08_999bceb904df_integration_args.py` & `MindsDB-23.4.4.3/mindsdb/migrations/versions/2022-07-08_999bceb904df_integration_args.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/migrations/versions/2022-07-15_b5b53e0ea7f8_training_data_rows_columns_count.py` & `MindsDB-23.4.4.3/mindsdb/migrations/versions/2022-07-15_b5b53e0ea7f8_training_data_rows_columns_count.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/migrations/versions/2022-07-22_6e834843e7e9_training_time.py` & `MindsDB-23.4.4.3/mindsdb/migrations/versions/2022-07-22_6e834843e7e9_training_time.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/migrations/versions/2022-08-19_976f15a37e6a_predictors_versioning.py` & `MindsDB-23.4.4.3/mindsdb/migrations/versions/2022-08-19_976f15a37e6a_predictors_versioning.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/migrations/versions/2022-08-25_6a54ba55872e_view_integration.py` & `MindsDB-23.4.4.3/mindsdb/migrations/versions/2022-08-25_6a54ba55872e_view_integration.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/migrations/versions/2022-08-29_473e8f239481_straighten.py` & `MindsDB-23.4.4.3/mindsdb/migrations/versions/2022-08-29_473e8f239481_straighten.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/migrations/versions/2022-09-06_96d5fef10caa_data_integration_id.py` & `MindsDB-23.4.4.3/mindsdb/migrations/versions/2022-09-06_96d5fef10caa_data_integration_id.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/migrations/versions/2022-09-08_87b2df2b83e1_predictor_status.py` & `MindsDB-23.4.4.3/mindsdb/migrations/versions/2022-09-08_87b2df2b83e1_predictor_status.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/migrations/versions/2022-09-19_3d5e70105df7_content_storage.py` & `MindsDB-23.4.4.3/mindsdb/migrations/versions/2022-09-19_3d5e70105df7_content_storage.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/migrations/versions/2022-09-29_cada7d2be947_json_storage.py` & `MindsDB-23.4.4.3/mindsdb/migrations/versions/2022-09-29_cada7d2be947_json_storage.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/migrations/versions/2022-10-14_43c52d23845a_projects.py` & `MindsDB-23.4.4.3/mindsdb/migrations/versions/2022-10-14_43c52d23845a_projects.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/migrations/versions/2022-11-07_1e60096fc817_predictor_version.py` & `MindsDB-23.4.4.3/mindsdb/migrations/versions/2022-11-07_1e60096fc817_predictor_version.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/migrations/versions/2022-11-11_d429095b570f_data_integration_id.py` & `MindsDB-23.4.4.3/mindsdb/migrations/versions/2022-11-11_d429095b570f_data_integration_id.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/migrations/versions/2022-12-26_459218b0844c_fix_unique_constraint.py` & `MindsDB-23.4.4.3/mindsdb/migrations/versions/2022-12-26_459218b0844c_fix_unique_constraint.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/migrations/versions/2023-02-02_b6d0a47294ac_jobs.py` & `MindsDB-23.4.4.3/mindsdb/migrations/versions/2023-02-02_b6d0a47294ac_jobs.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/migrations/versions/2023-02-17_ee63d868fa84_predictor_integration_null.py` & `MindsDB-23.4.4.3/mindsdb/migrations/versions/2023-02-17_ee63d868fa84_predictor_integration_null.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/migrations/versions/2023-02-25_3154382dab17_training_progress.py` & `MindsDB-23.4.4.3/mindsdb/migrations/versions/2023-02-25_3154382dab17_training_progress.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/migrations/versions/2023-02-27_ef04cdbe51ed_jobs_user_class.py` & `MindsDB-23.4.4.3/mindsdb/migrations/versions/2023-02-27_ef04cdbe51ed_jobs_user_class.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/migrations/versions/2023-04-11_b8be148dbc85_jobs_history_query.py` & `MindsDB-23.4.4.3/mindsdb/migrations/versions/2023-04-11_b8be148dbc85_jobs_history_query.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/utilities/auth.py` & `MindsDB-23.4.4.3/mindsdb/utilities/auth.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/utilities/cache.py` & `MindsDB-23.4.4.3/mindsdb/utilities/cache.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/utilities/config.py` & `MindsDB-23.4.4.3/mindsdb/utilities/config.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/utilities/context.py` & `MindsDB-23.4.4.3/mindsdb/utilities/context.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/utilities/fs.py` & `MindsDB-23.4.4.3/mindsdb/utilities/fs.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/utilities/functions.py` & `MindsDB-23.4.4.3/mindsdb/utilities/functions.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/utilities/hooks/profiling.py` & `MindsDB-23.4.4.3/mindsdb/utilities/hooks/profiling.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/utilities/json_encoder.py` & `MindsDB-23.4.4.3/mindsdb/utilities/json_encoder.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/utilities/log.py` & `MindsDB-23.4.4.3/mindsdb/utilities/log.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/utilities/log_controller.py` & `MindsDB-23.4.4.3/mindsdb/utilities/log_controller.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/utilities/profiler/profiler.py` & `MindsDB-23.4.4.3/mindsdb/utilities/profiler/profiler.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/utilities/ps.py` & `MindsDB-23.4.4.3/mindsdb/utilities/ps.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/utilities/telemetry.py` & `MindsDB-23.4.4.3/mindsdb/utilities/telemetry.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/mindsdb/utilities/wizards.py` & `MindsDB-23.4.4.3/mindsdb/utilities/wizards.py`

 * *Files identical despite different names*

### Comparing `MindsDB-23.4.4.2/requirements.txt` & `MindsDB-23.4.4.3/requirements.txt`

 * *Files 17% similar despite different names*

```diff
@@ -28,12 +28,12 @@
 mysql-connector-python
 clickhouse-driver
 clickhouse-sqlalchemy
 charset-normalizer
 dill >= 0.3.4
 pyOpenSSL >= 22.0.0
 pydateinfer==0.3.0
-pyarrow >= 9.0.0, < 10.0.0
+pyarrow >= 10.0.1, < 10.1.0
 dataprep_ml
 grpcio-tools
 python-magic >= 0.4.27
 openpyxl >= 3.1.1
```

### Comparing `MindsDB-23.4.4.2/setup.py` & `MindsDB-23.4.4.3/setup.py`

 * *Files identical despite different names*

