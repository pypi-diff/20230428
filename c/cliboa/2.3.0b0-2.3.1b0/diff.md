# Comparing `tmp/cliboa-2.3.0b0.tar.gz` & `tmp/cliboa-2.3.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cliboa-2.3.0b0.tar", last modified: Fri Sep 30 14:58:11 2022, max compression
+gzip compressed data, was "cliboa-2.3.1b0.tar", last modified: Fri Apr 28 09:16:51 2023, max compression
```

## Comparing `cliboa-2.3.0b0.tar` & `cliboa-2.3.1b0.tar`

### file list

```diff
@@ -1,117 +1,117 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-30 14:58:11.881029 cliboa-2.3.0b0/
--rw-r--r--   0 root         (0) root         (0)     6397 2022-09-30 14:58:11.885029 cliboa-2.3.0b0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4669 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-30 14:58:11.877029 cliboa-2.3.0b0/cliboa/
--rw-r--r--   0 root         (0) root         (0)        0 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-30 14:58:11.877029 cliboa-2.3.0b0/cliboa/adapter/
--rw-r--r--   0 root         (0) root         (0)        0 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/adapter/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2106 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/adapter/aws.py
--rw-r--r--   0 root         (0) root         (0)     1011 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/adapter/azure.py
--rw-r--r--   0 root         (0) root         (0)     3145 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/adapter/ftp.py
--rw-r--r--   0 root         (0) root         (0)     2372 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/adapter/gcp.py
--rw-r--r--   0 root         (0) root         (0)      562 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/adapter/mysql.py
--rw-r--r--   0 root         (0) root         (0)     1028 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/adapter/postgres.py
--rw-r--r--   0 root         (0) root         (0)     3649 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/adapter/rdbms.py
--rw-r--r--   0 root         (0) root         (0)     4011 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/adapter/sftp.py
--rw-r--r--   0 root         (0) root         (0)     8565 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/adapter/sqlite.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-30 14:58:11.877029 cliboa-2.3.0b0/cliboa/cli/
--rw-r--r--   0 root         (0) root         (0)        0 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6292 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/cli/cliboadmin.py
--rw-r--r--   0 root         (0) root         (0)     3031 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-30 14:58:11.877029 cliboa-2.3.0b0/cliboa/common/
--rw-r--r--   0 root         (0) root         (0)     1482 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/common/environment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-30 14:58:11.877029 cliboa-2.3.0b0/cliboa/conf/
--rw-r--r--   0 root         (0) root         (0)     1333 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/conf/__init__.py
--rw-r--r--   0 root         (0) root         (0)       58 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/conf/cliboa.ini
--rw-r--r--   0 root         (0) root         (0)     1429 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/conf/default_environment.py
--rw-r--r--   0 root         (0) root         (0)      360 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/conf/logging.conf
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-30 14:58:11.877029 cliboa-2.3.0b0/cliboa/core/
--rw-r--r--   0 root         (0) root         (0)        0 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2537 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/core/factory.py
--rw-r--r--   0 root         (0) root         (0)     7381 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/core/file_parser.py
--rw-r--r--   0 root         (0) root         (0)     3152 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/core/listener.py
--rw-r--r--   0 root         (0) root         (0)    12236 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/core/manager.py
--rw-r--r--   0 root         (0) root         (0)     1001 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/core/scenario_queue.py
--rw-r--r--   0 root         (0) root         (0)     1848 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/core/step_queue.py
--rw-r--r--   0 root         (0) root         (0)     4406 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/core/strategy.py
--rw-r--r--   0 root         (0) root         (0)     6369 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/core/validator.py
--rw-r--r--   0 root         (0) root         (0)     2955 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/core/worker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-30 14:58:11.877029 cliboa-2.3.0b0/cliboa/scenario/
--rw-r--r--   0 root         (0) root         (0)     2212 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/scenario/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1732 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/scenario/aws.py
--rw-r--r--   0 root         (0) root         (0)     1718 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/scenario/azure.py
--rw-r--r--   0 root         (0) root         (0)     4554 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/scenario/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-30 14:58:11.881029 cliboa-2.3.0b0/cliboa/scenario/extract/
--rw-r--r--   0 root         (0) root         (0)     6230 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/scenario/extract/aws.py
--rw-r--r--   0 root         (0) root         (0)     2312 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/scenario/extract/azure.py
--rw-r--r--   0 root         (0) root         (0)     1470 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/scenario/extract/file.py
--rw-r--r--   0 root         (0) root         (0)     3143 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/scenario/extract/ftp.py
--rw-r--r--   0 root         (0) root         (0)    10021 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/scenario/extract/gcp.py
--rw-r--r--   0 root         (0) root         (0)     3729 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/scenario/extract/http.py
--rw-r--r--   0 root         (0) root         (0)      932 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/scenario/extract/mysql.py
--rw-r--r--   0 root         (0) root         (0)      950 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/scenario/extract/postgres.py
--rw-r--r--   0 root         (0) root         (0)     5575 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/scenario/extract/sftp.py
--rw-r--r--   0 root         (0) root         (0)     1839 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/scenario/extract/sqlite.py
--rw-r--r--   0 root         (0) root         (0)      308 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/scenario/extras.py
--rw-r--r--   0 root         (0) root         (0)     2004 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/scenario/ftp.py
--rw-r--r--   0 root         (0) root         (0)     3090 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/scenario/gcp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-30 14:58:11.881029 cliboa-2.3.0b0/cliboa/scenario/load/
--rw-r--r--   0 root         (0) root         (0)     2442 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/scenario/load/aws.py
--rw-r--r--   0 root         (0) root         (0)     2516 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/scenario/load/azure.py
--rw-r--r--   0 root         (0) root         (0)     1291 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/scenario/load/file.py
--rw-r--r--   0 root         (0) root         (0)     9340 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/scenario/load/gcp.py
--rw-r--r--   0 root         (0) root         (0)      935 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/scenario/load/mysql.py
--rw-r--r--   0 root         (0) root         (0)      953 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/scenario/load/postgres.py
--rw-r--r--   0 root         (0) root         (0)     2518 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/scenario/load/sftp.py
--rw-r--r--   0 root         (0) root         (0)     4178 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/scenario/load/sqlite.py
--rw-r--r--   0 root         (0) root         (0)     6186 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/scenario/rdbms.py
--rw-r--r--   0 root         (0) root         (0)     2144 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/scenario/sample_step.py
--rw-r--r--   0 root         (0) root         (0)     2846 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/scenario/sftp.py
--rw-r--r--   0 root         (0) root         (0)     3313 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/scenario/sqlite.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-30 14:58:11.881029 cliboa-2.3.0b0/cliboa/scenario/transform/
--rw-r--r--   0 root         (0) root         (0)    22952 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/scenario/transform/csv.py
--rw-r--r--   0 root         (0) root         (0)    21122 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/scenario/transform/file.py
--rw-r--r--   0 root         (0) root         (0)     4972 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/scenario/transform/gpg.py
--rw-r--r--   0 root         (0) root         (0)     3814 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/scenario/transform/json.py
--rw-r--r--   0 root         (0) root         (0)     1890 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/scenario/transform/system.py
--rw-r--r--   0 root         (0) root         (0)     2498 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/scenario/validator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-30 14:58:11.881029 cliboa-2.3.0b0/cliboa/template/
--rw-r--r--   0 root         (0) root         (0)     1214 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/template/Pipfile.above36
--rw-r--r--   0 root         (0) root         (0)     1238 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/template/Pipfile.above37
--rw-r--r--   0 root         (0) root         (0)     1237 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/template/Pipfile.above38
--rw-r--r--   0 root         (0) root         (0)     1237 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/template/Pipfile.above39
--rw-r--r--   0 root         (0) root         (0)        0 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/template/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-30 14:58:11.881029 cliboa-2.3.0b0/cliboa/template/bin/
--rw-r--r--   0 root         (0) root         (0)        0 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/template/bin/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1002 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/template/bin/clibomanager.py
--rw-r--r--   0 root         (0) root         (0)     1283 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/template/pyproject.above37.toml
--rw-r--r--   0 root         (0) root         (0)     1282 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/template/pyproject.above38.toml
--rw-r--r--   0 root         (0) root         (0)     1282 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/template/pyproject.above39.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-30 14:58:11.881029 cliboa-2.3.0b0/cliboa/util/
--rw-r--r--   0 root         (0) root         (0)        0 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2444 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/util/cache.py
--rw-r--r--   0 root         (0) root         (0)     1285 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/util/class_util.py
--rw-r--r--   0 root         (0) root         (0)       78 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/util/constant.py
--rw-r--r--   0 root         (0) root         (0)     4240 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/util/csv.py
--rw-r--r--   0 root         (0) root         (0)     1353 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/util/date.py
--rw-r--r--   0 root         (0) root         (0)     1723 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/util/exception.py
--rw-r--r--   0 root         (0) root         (0)     2975 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/util/file.py
--rw-r--r--   0 root         (0) root         (0)     4240 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/util/ftp_util.py
--rw-r--r--   0 root         (0) root         (0)     1561 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/util/gcp.py
--rw-r--r--   0 root         (0) root         (0)     2598 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/util/gpg.py
--rw-r--r--   0 root         (0) root         (0)     1255 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/util/helper.py
--rw-r--r--   0 root         (0) root         (0)     3621 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/util/http.py
--rw-r--r--   0 root         (0) root         (0)      318 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/util/lisboa_log.py
--rw-r--r--   0 root         (0) root         (0)      747 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/util/parallel_with_config.py
--rw-r--r--   0 root         (0) root         (0)     1942 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/util/rdbms_util.py
--rw-r--r--   0 root         (0) root         (0)     9191 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/util/sftp.py
--rw-r--r--   0 root         (0) root         (0)     1130 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/cliboa/util/string.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-30 14:58:11.877029 cliboa-2.3.0b0/cliboa.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6397 2022-09-30 14:58:11.000000 cliboa-2.3.0b0/cliboa.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2698 2022-09-30 14:58:11.000000 cliboa-2.3.0b0/cliboa.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-09-30 14:58:11.000000 cliboa-2.3.0b0/cliboa.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       59 2022-09-30 14:58:11.000000 cliboa-2.3.0b0/cliboa.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        7 2022-09-30 14:58:11.000000 cliboa-2.3.0b0/cliboa.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1275 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      344 2022-09-30 14:58:11.885029 cliboa-2.3.0b0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2640 2022-09-30 14:58:06.000000 cliboa-2.3.0b0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 09:16:51.738918 cliboa-2.3.1b0/
+-rw-r--r--   0 root         (0) root         (0)     1082 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5408 2023-04-28 09:16:51.738918 cliboa-2.3.1b0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4669 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 09:16:51.730918 cliboa-2.3.1b0/cliboa/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 09:16:51.730918 cliboa-2.3.1b0/cliboa/adapter/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/adapter/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2106 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/adapter/aws.py
+-rw-r--r--   0 root         (0) root         (0)     1011 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/adapter/azure.py
+-rw-r--r--   0 root         (0) root         (0)     3145 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/adapter/ftp.py
+-rw-r--r--   0 root         (0) root         (0)     3243 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/adapter/gcp.py
+-rw-r--r--   0 root         (0) root         (0)      562 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/adapter/mysql.py
+-rw-r--r--   0 root         (0) root         (0)     1028 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/adapter/postgres.py
+-rw-r--r--   0 root         (0) root         (0)     3649 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/adapter/rdbms.py
+-rw-r--r--   0 root         (0) root         (0)     4011 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/adapter/sftp.py
+-rw-r--r--   0 root         (0) root         (0)     8565 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/adapter/sqlite.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 09:16:51.730918 cliboa-2.3.1b0/cliboa/cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6292 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/cli/cliboadmin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 09:16:51.730918 cliboa-2.3.1b0/cliboa/common/
+-rw-r--r--   0 root         (0) root         (0)     1482 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/common/environment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 09:16:51.730918 cliboa-2.3.1b0/cliboa/conf/
+-rw-r--r--   0 root         (0) root         (0)     1333 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/conf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       58 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/conf/cliboa.ini
+-rw-r--r--   0 root         (0) root         (0)     1429 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/conf/default_environment.py
+-rw-r--r--   0 root         (0) root         (0)      360 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/conf/logging.conf
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 09:16:51.730918 cliboa-2.3.1b0/cliboa/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2537 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/core/factory.py
+-rw-r--r--   0 root         (0) root         (0)     7381 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/core/file_parser.py
+-rw-r--r--   0 root         (0) root         (0)     3152 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/core/listener.py
+-rw-r--r--   0 root         (0) root         (0)    12553 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/core/manager.py
+-rw-r--r--   0 root         (0) root         (0)     1001 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/core/scenario_queue.py
+-rw-r--r--   0 root         (0) root         (0)     1848 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/core/step_queue.py
+-rw-r--r--   0 root         (0) root         (0)     4406 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/core/strategy.py
+-rw-r--r--   0 root         (0) root         (0)     6369 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/core/validator.py
+-rw-r--r--   0 root         (0) root         (0)     2955 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/core/worker.py
+-rw-r--r--   0 root         (0) root         (0)     3031 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/interface.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 09:16:51.734918 cliboa-2.3.1b0/cliboa/scenario/
+-rw-r--r--   0 root         (0) root         (0)     2253 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1732 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/aws.py
+-rw-r--r--   0 root         (0) root         (0)     1718 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/azure.py
+-rw-r--r--   0 root         (0) root         (0)     4554 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 09:16:51.734918 cliboa-2.3.1b0/cliboa/scenario/extract/
+-rw-r--r--   0 root         (0) root         (0)     6328 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/extract/aws.py
+-rw-r--r--   0 root         (0) root         (0)     2402 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/extract/azure.py
+-rw-r--r--   0 root         (0) root         (0)     1470 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/extract/file.py
+-rw-r--r--   0 root         (0) root         (0)     3143 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/extract/ftp.py
+-rw-r--r--   0 root         (0) root         (0)    10166 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/extract/gcp.py
+-rw-r--r--   0 root         (0) root         (0)     3729 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/extract/http.py
+-rw-r--r--   0 root         (0) root         (0)      932 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/extract/mysql.py
+-rw-r--r--   0 root         (0) root         (0)      950 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/extract/postgres.py
+-rw-r--r--   0 root         (0) root         (0)     5575 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/extract/sftp.py
+-rw-r--r--   0 root         (0) root         (0)     1973 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/extract/sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      308 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/extras.py
+-rw-r--r--   0 root         (0) root         (0)     2004 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/ftp.py
+-rw-r--r--   0 root         (0) root         (0)     3090 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/gcp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 09:16:51.734918 cliboa-2.3.1b0/cliboa/scenario/load/
+-rw-r--r--   0 root         (0) root         (0)     2442 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/load/aws.py
+-rw-r--r--   0 root         (0) root         (0)     2516 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/load/azure.py
+-rw-r--r--   0 root         (0) root         (0)     1291 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/load/file.py
+-rw-r--r--   0 root         (0) root         (0)     9340 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/load/gcp.py
+-rw-r--r--   0 root         (0) root         (0)      935 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/load/mysql.py
+-rw-r--r--   0 root         (0) root         (0)      953 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/load/postgres.py
+-rw-r--r--   0 root         (0) root         (0)     2518 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/load/sftp.py
+-rw-r--r--   0 root         (0) root         (0)     4178 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/load/sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     6319 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/rdbms.py
+-rw-r--r--   0 root         (0) root         (0)     2144 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/sample_step.py
+-rw-r--r--   0 root         (0) root         (0)     2846 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/sftp.py
+-rw-r--r--   0 root         (0) root         (0)     3313 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/sqlite.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 09:16:51.734918 cliboa-2.3.1b0/cliboa/scenario/transform/
+-rw-r--r--   0 root         (0) root         (0)     3267 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/transform/aes.py
+-rw-r--r--   0 root         (0) root         (0)    30540 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/transform/csv.py
+-rw-r--r--   0 root         (0) root         (0)    21683 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/transform/file.py
+-rw-r--r--   0 root         (0) root         (0)     5130 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/transform/gpg.py
+-rw-r--r--   0 root         (0) root         (0)     3721 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/transform/json.py
+-rw-r--r--   0 root         (0) root         (0)     1894 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/transform/system.py
+-rw-r--r--   0 root         (0) root         (0)     2498 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/scenario/validator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 09:16:51.734918 cliboa-2.3.1b0/cliboa/template/
+-rw-r--r--   0 root         (0) root         (0)     1214 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/template/Pipfile.above36
+-rw-r--r--   0 root         (0) root         (0)     1238 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/template/Pipfile.above37
+-rw-r--r--   0 root         (0) root         (0)     1237 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/template/Pipfile.above38
+-rw-r--r--   0 root         (0) root         (0)     1237 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/template/Pipfile.above39
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/template/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 09:16:51.734918 cliboa-2.3.1b0/cliboa/template/bin/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/template/bin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1005 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/template/bin/clibomanager.py
+-rw-r--r--   0 root         (0) root         (0)     1283 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/template/pyproject.above37.toml
+-rw-r--r--   0 root         (0) root         (0)     1282 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/template/pyproject.above38.toml
+-rw-r--r--   0 root         (0) root         (0)     1282 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/template/pyproject.above39.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 09:16:51.738918 cliboa-2.3.1b0/cliboa/util/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2444 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/util/cache.py
+-rw-r--r--   0 root         (0) root         (0)     1285 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/util/class_util.py
+-rw-r--r--   0 root         (0) root         (0)       78 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/util/constant.py
+-rw-r--r--   0 root         (0) root         (0)     4240 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/util/csv.py
+-rw-r--r--   0 root         (0) root         (0)     1353 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/util/date.py
+-rw-r--r--   0 root         (0) root         (0)     1723 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/util/exception.py
+-rw-r--r--   0 root         (0) root         (0)     2975 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/util/file.py
+-rw-r--r--   0 root         (0) root         (0)     4240 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/util/ftp_util.py
+-rw-r--r--   0 root         (0) root         (0)     2598 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/util/gpg.py
+-rw-r--r--   0 root         (0) root         (0)     1255 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/util/helper.py
+-rw-r--r--   0 root         (0) root         (0)     3621 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/util/http.py
+-rw-r--r--   0 root         (0) root         (0)      318 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/util/lisboa_log.py
+-rw-r--r--   0 root         (0) root         (0)      747 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/util/parallel_with_config.py
+-rw-r--r--   0 root         (0) root         (0)     1942 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/util/rdbms_util.py
+-rw-r--r--   0 root         (0) root         (0)     9191 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/util/sftp.py
+-rw-r--r--   0 root         (0) root         (0)     1130 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/cliboa/util/string.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 09:16:51.730918 cliboa-2.3.1b0/cliboa.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5408 2023-04-28 09:16:51.000000 cliboa-2.3.1b0/cliboa.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2708 2023-04-28 09:16:51.000000 cliboa-2.3.1b0/cliboa.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 09:16:51.000000 cliboa-2.3.1b0/cliboa.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2023-04-28 09:16:51.000000 cliboa-2.3.1b0/cliboa.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-28 09:16:51.000000 cliboa-2.3.1b0/cliboa.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      344 2023-04-28 09:16:51.738918 cliboa-2.3.1b0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2640 2023-04-28 09:16:45.000000 cliboa-2.3.1b0/setup.py
```

### Comparing `cliboa-2.3.0b0/README.md` & `cliboa-2.3.1b0/README.md`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.0b0/cliboa/adapter/aws.py` & `cliboa-2.3.1b0/cliboa/adapter/aws.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.0b0/cliboa/adapter/azure.py` & `cliboa-2.3.1b0/cliboa/adapter/azure.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.0b0/cliboa/adapter/ftp.py` & `cliboa-2.3.1b0/cliboa/adapter/ftp.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.0b0/cliboa/adapter/mysql.py` & `cliboa-2.3.1b0/cliboa/adapter/mysql.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.0b0/cliboa/adapter/postgres.py` & `cliboa-2.3.1b0/cliboa/adapter/postgres.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.0b0/cliboa/adapter/rdbms.py` & `cliboa-2.3.1b0/cliboa/adapter/rdbms.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.0b0/cliboa/adapter/sftp.py` & `cliboa-2.3.1b0/cliboa/adapter/sftp.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.0b0/cliboa/adapter/sqlite.py` & `cliboa-2.3.1b0/cliboa/adapter/sqlite.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.0b0/cliboa/cli/cliboadmin.py` & `cliboa-2.3.1b0/cliboa/cli/cliboadmin.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.0b0/cliboa/client.py` & `cliboa-2.3.1b0/cliboa/interface.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.0b0/cliboa/common/environment.py` & `cliboa-2.3.1b0/cliboa/common/environment.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.0b0/cliboa/conf/__init__.py` & `cliboa-2.3.1b0/cliboa/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.0b0/cliboa/conf/default_environment.py` & `cliboa-2.3.1b0/cliboa/conf/default_environment.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.0b0/cliboa/core/factory.py` & `cliboa-2.3.1b0/cliboa/core/factory.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.0b0/cliboa/core/file_parser.py` & `cliboa-2.3.1b0/cliboa/core/file_parser.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.0b0/cliboa/core/listener.py` & `cliboa-2.3.1b0/cliboa/core/listener.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.0b0/cliboa/core/manager.py` & `cliboa-2.3.1b0/cliboa/core/manager.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
 #
 # The above copyright notice and this permission notice shall be included in
 # all copies or substantial portions of the Software.
 #
-import json
 import os
 import re
 import subprocess
 from abc import abstractmethod
 
 from cliboa.conf import env
 from cliboa.core.file_parser import JsonScenarioParser, YamlScenarioParser
@@ -60,14 +59,15 @@
                 os.path.join(env.PROJECT_DIR, cmd_args.project_name, env.SCENARIO_FILE_NAME)
                 + "."
                 + cmd_args.format
             )
             self._cmn_scenario_file = (
                 os.path.join(env.COMMON_DIR, env.SCENARIO_FILE_NAME) + "." + cmd_args.format
             )
+        self._replace_vars_pattern = re.compile(r"{{(.*?)}}")
 
     def create_scenario_queue(self):
         # validation
         self._valid_essential_dir()
         self._valid_essential_files()
 
         scenario_list = self.parse_file()
@@ -164,15 +164,17 @@
         cls_attrs_dict = {}
         if "arguments" in s_dict.keys():
             cls_attrs_dict = s_dict["arguments"]
 
         values = {}
         if cls_attrs_dict:
             cls_attrs_dict, with_vars = self._split_class_vars(cls_attrs_dict)
-            ret = self._set_values(instance, cls_attrs_dict, with_vars)
+            ret = self._replace_arguments(cls_attrs_dict, with_vars)
+            for dict_k, dict_v in ret.items():
+                Helper.set_property(instance, dict_k, dict_v)
             values.update(ret)
 
         base_args = ["step", "symbol", "parallel", "listeners"]
         for arg in base_args:
             if arg == "listeners":
                 self._append_listeners(instance, s_dict.get(arg), values)
             else:
@@ -202,49 +204,51 @@
         if exists_with_vars:
             variables = arguments["with_vars"]
             for yaml_k, yaml_v in variables.items():
                 with_vars[yaml_k] = yaml_v
             del arguments["with_vars"]
         return arguments, with_vars
 
-    def _set_values(self, instance, arguments, with_vars):
+    def _replace_arguments(self, arguments, with_vars):
         """
-        Set parameters to the instance.
+        Nested replacement of argments.
 
-        Args:
-            instance (class): instance
+        First args:
             arguments (dict): Arguments of steps
             with_vars (dict): with_vars parameter
 
         Returns:
-            dict: Dictionary of arguments which was set
+            dict: Dictionary of arguments which was replaced.
         """
-        pattern = re.compile(r"{{(.*?)}}")
-        values = {}
-        for yaml_k, yaml_v in arguments.items():
-            js = json.dumps(yaml_v)
-            matches = pattern.findall(js)
+        if isinstance(arguments, dict):
+            return {
+                dict_k: self._replace_arguments(dict_v, with_vars)
+                for dict_k, dict_v in arguments.items()
+            }
+        elif isinstance(arguments, list):
+            return [self._replace_arguments(list_v, with_vars) for list_v in arguments]
+        elif isinstance(arguments, str):
+            matches = self._replace_vars_pattern.findall(arguments)
             for match in matches:
                 var_name = match.strip()
                 if not var_name:
                     raise InvalidParameter("Alternative argument was empty.")
                 if var_name.startswith("env."):
-                    js = self._replace_envs(js, var_name)
+                    arguments = self._replace_envs(arguments, var_name)
                 else:
                     cmd = with_vars[var_name]
                     if not cmd:
                         raise ScenarioFileInvalid(
                             "scenario file is invalid. 'with_vars' definition against %s does not exist."  # noqa
                             % var_name
                         )
-                    js = self._replace_vars(js, var_name, cmd)
-                yaml_v = json.loads(js)
-            Helper.set_property(instance, yaml_k, yaml_v)
-            values[yaml_k] = yaml_v
-        return values
+                    arguments = self._replace_vars(arguments, var_name, cmd)
+            return arguments
+        else:
+            return arguments
 
     def _replace_vars(self, yaml_v, var_name, cmd):
         """
         This method replaces the value of {{ xxx }} based on the result of the shell script.
 
         Ex.
           -- IN --
```

### Comparing `cliboa-2.3.0b0/cliboa/core/scenario_queue.py` & `cliboa-2.3.1b0/cliboa/core/scenario_queue.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.0b0/cliboa/core/step_queue.py` & `cliboa-2.3.1b0/cliboa/core/step_queue.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.0b0/cliboa/core/strategy.py` & `cliboa-2.3.1b0/cliboa/core/strategy.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.0b0/cliboa/core/validator.py` & `cliboa-2.3.1b0/cliboa/core/validator.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.0b0/cliboa/core/worker.py` & `cliboa-2.3.1b0/cliboa/core/worker.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.0b0/cliboa/scenario/__init__.py` & `cliboa-2.3.1b0/cliboa/scenario/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,17 +34,19 @@
 from .load.postgres import PostgresqlWrite
 from .load.sftp import SftpUpload
 from .load.sqlite import SqliteImport
 from .sqlite import SqliteQueryExecute
 from .transform.csv import (
     ColumnLengthAdjust,
     CsvColumnConcat,
+    CsvColumnCopy,
     CsvColumnDelete,
     CsvColumnExtract,
     CsvColumnHash,
+    CsvColumnReplace,
     CsvConcat,
     CsvConvert,
     CsvMerge,
     CsvSort,
     CsvToJsonl,
     CsvValueExtract,
 )
```

### Comparing `cliboa-2.3.0b0/cliboa/scenario/aws.py` & `cliboa-2.3.1b0/cliboa/scenario/aws.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.0b0/cliboa/scenario/azure.py` & `cliboa-2.3.1b0/cliboa/scenario/azure.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.0b0/cliboa/scenario/base.py` & `cliboa-2.3.1b0/cliboa/scenario/base.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.0b0/cliboa/scenario/extract/aws.py` & `cliboa-2.3.1b0/cliboa/scenario/extract/aws.py`

 * *Files 5% similar despite different names*

```diff
@@ -59,14 +59,16 @@
         for page in p.paginate(Bucket=self._bucket, Delimiter=self._delimiter, Prefix=self._prefix):
             for c in page.get("Contents", []):
                 path = c.get("Key")
                 filename = os.path.basename(path)
                 rec = re.compile(self._src_pattern)
                 if not rec.fullmatch(filename):
                     continue
+                if self._dest_dir:
+                    os.makedirs(self._dest_dir, exist_ok=True)
                 dest_path = os.path.join(self._dest_dir, filename)
                 client.download_file(self._bucket, path, dest_path)
                 keys.append(path)
 
         # cache
         ObjectStore.put(self._step, {"bucket": self._bucket, "keys": keys})
```

### Comparing `cliboa-2.3.0b0/cliboa/scenario/extract/azure.py` & `cliboa-2.3.1b0/cliboa/scenario/extract/azure.py`

 * *Files 7% similar despite different names*

```diff
@@ -53,13 +53,15 @@
         container_client = service.get_container_client(self._container_name)
         blobs = container_client.list_blobs(name_starts_with=self._prefix)
         for blob in blobs:
             filename = blob.name
             rec = re.compile(self._src_pattern)
             if not rec.fullmatch(filename):
                 continue
+            if self._dest_dir:
+                os.makedirs(self._dest_dir, exist_ok=True)
             dest_path = os.path.join(self._dest_dir, os.path.basename(filename))
             blob_client = service.get_blob_client(container=self._container_name, blob=filename)
 
             with open(dest_path, "wb") as local_blob:
                 blob_data = blob_client.download_blob()
                 blob_data.readinto(local_blob)
```

### Comparing `cliboa-2.3.0b0/cliboa/scenario/extract/file.py` & `cliboa-2.3.1b0/cliboa/scenario/extract/file.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.0b0/cliboa/scenario/extract/ftp.py` & `cliboa-2.3.1b0/cliboa/scenario/extract/ftp.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.0b0/cliboa/scenario/extract/gcp.py` & `cliboa-2.3.1b0/cliboa/scenario/extract/gcp.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 
 from cliboa.adapter.gcp import BigQueryAdapter, FireStoreAdapter, GcsAdapter
 from cliboa.scenario.gcp import BaseBigQuery, BaseFirestore, BaseGcs
 from cliboa.scenario.validator import EssentialParameters
 from cliboa.util.cache import ObjectStore
 from cliboa.util.constant import StepStatus
 from cliboa.util.exception import InvalidParameter
-from cliboa.util.gcp import BigQuery
 from cliboa.util.string import StringUtil
 
 
 class BigQueryRead(BaseBigQuery):
     """
     Read data from BigQuery and put them into on-memory or export to a file via GCS.
     """
@@ -107,41 +106,41 @@
             tmp_tbl = "tmp_" + StringUtil().random_str(self._RANDOM_STR_LENGTH) + "_" + ymd_hms
             table_ref = gbq_client.dataset(self._dataset).table(tmp_tbl)
 
         gcs_client = GcsAdapter().get_client(credentials=self.get_credentials())
         gcs_bucket = gcs_client.bucket(self._bucket)
 
         # extract job config settings
-        ext_job_config = BigQuery.get_extract_job_config()
-        ext_job_config.compression = BigQuery.get_compression_type()
+        ext_job_config = BigQueryAdapter.get_extract_job_config()
+        ext_job_config.compression = BigQueryAdapter.get_compression_type()
         ext = ".csv"
         if self._filename:
             _, ext = os.path.splitext(self._filename)
             support_ext = [".csv", ".json"]
             if ext not in support_ext:
                 raise InvalidParameter("%s is not supported as filename." % ext)
-        ext_job_config.destination_format = BigQuery.get_destination_format(ext)
+        ext_job_config.destination_format = BigQueryAdapter.get_destination_format(ext)
 
         comp_format_and_ext = {"GZIP": ".gz"}
-        comp_ext = comp_format_and_ext.get(str(BigQuery.get_compression_type()))
+        comp_ext = comp_format_and_ext.get(str(BigQueryAdapter.get_compression_type()))
         if self._filename:
             dest_gcs = "gs://%s/%s/%s%s" % (
                 self._bucket,
                 prefix,
                 self._filename,
                 comp_ext,
             )
         else:
             dest_gcs = "gs://%s/%s/*%s%s" % (self._bucket, prefix, ext, comp_ext)
 
         # Execute query.
         if self._query:
-            query_job_config = BigQuery.get_query_job_config()
+            query_job_config = BigQueryAdapter.get_query_job_config()
             query_job_config.destination = table_ref
-            query_job_config.write_disposition = BigQuery.get_write_disposition()
+            query_job_config.write_disposition = BigQueryAdapter.get_write_disposition()
             query_job = gbq_client.query(
                 self._query, location=self._location, job_config=query_job_config
             )
             query_job.result()
 
         # Extract to GCS
         extract_job = gbq_client.extract_table(
@@ -189,20 +188,22 @@
 
     def execute(self, *args):
         super().execute()
 
         valid = EssentialParameters(self.__class__.__name__, [self._src_pattern])
         valid()
 
+        os.makedirs(self._dest_dir, exist_ok=True)
+
         client = GcsAdapter().get_client(credentials=self.get_credentials())
         bucket = client.bucket(self._bucket)
         dl_files = []
         for blob in client.list_blobs(bucket, prefix=self._prefix, delimiter=self._delimiter):
             r = re.compile(self._src_pattern)
-            if not r.fullmatch(blob.name):
+            if not r.fullmatch(os.path.basename(blob.name)):
                 continue
             dl_files.append(blob.name)
             blob.download_to_filename(os.path.join(self._dest_dir, os.path.basename(blob.name)))
 
         ObjectStore.put(self._step, dl_files)
 
 
@@ -250,14 +251,16 @@
         super().execute()
 
         valid = EssentialParameters(
             self.__class__.__name__, [self._collection, self._document, self._dest_dir]
         )
         valid()
 
+        os.makedirs(self._dest_dir, exist_ok=True)
+
         client = FireStoreAdapter().get_client(self.get_credentials())
         ref = client.document(self._collection, self._document)
         doc = ref.get()
 
         with open(os.path.join(self._dest_dir, doc.id), mode="wt") as f:
             f.write(json.dumps(doc.to_dict()))
 
@@ -290,15 +293,15 @@
 
         client = GcsAdapter().get_client(credentials=self.get_credentials())
         dl_files = []
         bucket = client.bucket(super().get_step_argument("bucket"))
 
         for blob in client.list_blobs(bucket, prefix=self._prefix, delimiter=self._delimiter):
             r = re.compile(self._src_pattern)
-            if not r.fullmatch(blob.name):
+            if not r.fullmatch(os.path.basename(blob.name)):
                 continue
             dl_files.append(blob.name)
 
         if len(dl_files) == 0:
             self._logger.info("File not found in GCS. After process will not be processed")
             return StepStatus.SUCCESSFUL_TERMINATION
```

### Comparing `cliboa-2.3.0b0/cliboa/scenario/extract/http.py` & `cliboa-2.3.1b0/cliboa/scenario/extract/http.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.0b0/cliboa/scenario/extract/mysql.py` & `cliboa-2.3.1b0/cliboa/scenario/extract/mysql.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.0b0/cliboa/scenario/extract/postgres.py` & `cliboa-2.3.1b0/cliboa/scenario/extract/postgres.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.0b0/cliboa/scenario/extract/sftp.py` & `cliboa-2.3.1b0/cliboa/scenario/extract/sftp.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.0b0/cliboa/scenario/extract/sqlite.py` & `cliboa-2.3.1b0/cliboa/scenario/extract/sqlite.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
 #
 # The above copyright notice and this permission notice shall be included in
 # all copies or substantial portions of the Software.
 #
+import os
+
 from cliboa.scenario.sqlite import BaseSqlite
 from cliboa.scenario.validator import EssentialParameters
 
 
 class SqliteExport(BaseSqlite):
     def __init__(self):
         super().__init__()
@@ -41,14 +43,18 @@
 
     def execute(self, *args):
         super().execute()
 
         valid = EssentialParameters(self.__class__.__name__, [self._dest_path])
         valid()
 
+        dest_dir = os.path.dirname(self._dest_path)
+        if dest_dir:
+            os.makedirs(dest_dir, exist_ok=True)
+
         self._sqlite_adptr.connect(self._dbname)
         try:
             self._sqlite_adptr.export_table(
                 self._tblname,
                 self._dest_path,
                 encoding=self._encoding,
                 order=self._order,
```

### Comparing `cliboa-2.3.0b0/cliboa/scenario/ftp.py` & `cliboa-2.3.1b0/cliboa/scenario/ftp.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.0b0/cliboa/scenario/gcp.py` & `cliboa-2.3.1b0/cliboa/scenario/gcp.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.0b0/cliboa/scenario/load/aws.py` & `cliboa-2.3.1b0/cliboa/scenario/load/aws.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.0b0/cliboa/scenario/load/azure.py` & `cliboa-2.3.1b0/cliboa/scenario/load/azure.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.0b0/cliboa/scenario/load/file.py` & `cliboa-2.3.1b0/cliboa/scenario/load/file.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.0b0/cliboa/scenario/load/gcp.py` & `cliboa-2.3.1b0/cliboa/scenario/load/gcp.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.0b0/cliboa/scenario/load/mysql.py` & `cliboa-2.3.1b0/cliboa/scenario/load/mysql.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.0b0/cliboa/scenario/load/postgres.py` & `cliboa-2.3.1b0/cliboa/scenario/load/postgres.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.0b0/cliboa/scenario/load/sftp.py` & `cliboa-2.3.1b0/cliboa/scenario/load/sftp.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.0b0/cliboa/scenario/load/sqlite.py` & `cliboa-2.3.1b0/cliboa/scenario/load/sqlite.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.0b0/cliboa/scenario/rdbms.py` & `cliboa-2.3.1b0/cliboa/scenario/rdbms.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
 #
 # The above copyright notice and this permission notice shall be included in
 # all copies or substantial portions of the Software.
 #
 import csv
+import os
 
 from cliboa.core.validator import EssentialParameters
 from cliboa.scenario.base import BaseStep
 from cliboa.util.exception import FileNotFound, InvalidParameter
 from cliboa.util.rdbms_util import Rdbms_Util
 
 
@@ -84,14 +85,18 @@
 
         valid = EssentialParameters(self.__class__.__name__, [self._dest_path])
         valid()
 
         if (self._query and self._tblname) or (not self._query and not self._tblname):
             raise InvalidParameter("Either query or tblname is required.")
 
+        dest_dir = os.path.dirname(self._dest_path)
+        if dest_dir:
+            os.makedirs(dest_dir, exist_ok=True)
+
         with self.get_adaptor() as adaptor:
             with open(self._dest_path, mode="w", encoding=self._encoding, newline="") as f:
                 if self._tblname:
                     query = Rdbms_Util().select_sql(self._tblname)
                 elif isinstance(self._query, str):
                     self._logger.warning(
                         (
```

### Comparing `cliboa-2.3.0b0/cliboa/scenario/sample_step.py` & `cliboa-2.3.1b0/cliboa/scenario/sample_step.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.0b0/cliboa/scenario/sftp.py` & `cliboa-2.3.1b0/cliboa/scenario/sftp.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.0b0/cliboa/scenario/sqlite.py` & `cliboa-2.3.1b0/cliboa/scenario/sqlite.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.0b0/cliboa/scenario/transform/csv.py` & `cliboa-2.3.1b0/cliboa/scenario/transform/csv.py`

 * *Files 26% similar despite different names*

```diff
@@ -48,36 +48,42 @@
     def execute(self, *args):
         valid = EssentialParameters(
             self.__class__.__name__,
             [self._src_dir, self._src_pattern, self._columns],
         )
         valid()
 
-        if self._dest_dir:
-            os.makedirs(self._dest_dir, exist_ok=True)
-
         files = super().get_target_files(self._src_dir, self._src_pattern)
         self.check_file_existence(files)
 
         super().io_files(files, func=self.convert)
 
     def convert(self, fi, fo):
-        df = pandas.read_csv(
+        chunk_size_handling(self._read_csv_func, fi, fo)
+
+    def _read_csv_func(self, chunksize, fi, fo):
+        # Used in chunk_size_handling
+        first_write = True
+        tfr = pandas.read_csv(
             fi,
             dtype=str,
             encoding=self._encoding,
+            chunksize=chunksize,
         )
-        for c in self._columns:
-            df[c] = df[c].apply(self._stringToHash)
-
-        df.to_csv(
-            fo,
-            encoding=self._encoding,
-            index=False,
-        )
+        for df in tfr:
+            for c in self._columns:
+                df[c] = df[c].apply(self._stringToHash)
+            df.to_csv(
+                fo,
+                encoding=self._encoding,
+                header=True if first_write else False,
+                index=False,
+                mode="w" if first_write else "a",
+            )
+            first_write = False
 
 
 class CsvColumnExtract(FileBaseTransform):
     """
     Remove specific columns from csv file.
     """
 
@@ -92,17 +98,14 @@
     def column_numbers(self, column_numbers):
         self._column_numbers = column_numbers
 
     def execute(self, *args):
         valid = EssentialParameters(self.__class__.__name__, [self._src_dir, self._src_pattern])
         valid()
 
-        if self._dest_dir:
-            os.makedirs(self._dest_dir, exist_ok=True)
-
         if not self._columns and not self._column_numbers:
             raise InvalidParameter("Specifying either 'column' or 'column_numbers' is essential.")
         if self._columns and self._column_numbers:
             raise InvalidParameter("Cannot specify both 'column' and 'column_numbers'.")
 
         files = super().get_target_files(self._src_dir, self._src_pattern)
         self.check_file_existence(files)
@@ -142,33 +145,41 @@
 
         files = super().get_target_files(self._src_dir, self._src_pattern)
         self.check_file_existence(files)
 
         super().io_files(files, func=self.convert)
 
     def convert(self, fi, fo):
-        df = pandas.read_csv(
+        chunk_size_handling(self._read_csv_func, fi, fo)
+
+    def _read_csv_func(self, chunksize, fi, fo):
+        # Used in chunk_size_handling
+        first_write = True
+        tfr = pandas.read_csv(
             fi,
             dtype=str,
             encoding=self._encoding,
+            chunksize=chunksize,
         )
         pattern = re.compile(self._regex_pattern)
-        for column in df.columns.values:
-            if pattern.fullmatch(column):
-                df = df.drop(column, axis=1)
-
-        # output an empty file when all columns are deleted
-        if df.empty:
-            df = df.dropna(how="all")
-
-        df.to_csv(
-            fo,
-            encoding=self._encoding,
-            index=False,
-        )
+        for df in tfr:
+            for column in df.columns.values:
+                if pattern.fullmatch(column):
+                    df = df.drop(column, axis=1)
+                # output an empty file when all columns are deleted
+                if df.empty:
+                    df = df.dropna(how="all")
+            df.to_csv(
+                fo,
+                encoding=self._encoding,
+                header=True if first_write else False,
+                index=False,
+                mode="w" if first_write else "a",
+            )
+            first_write = False
 
 
 class CsvValueExtract(FileBaseTransform):
     """
     Extract a specific column from a CSV file and then replace it with a regular expression.
     """
 
@@ -177,21 +188,19 @@
         self._column_regex_pattern = None
 
     def column_regex_pattern(self, column_regex_pattern):
         self._column_regex_pattern = column_regex_pattern
 
     def execute(self, *args):
         valid = EssentialParameters(
-            self.__class__.__name__, [self._src_dir, self._src_pattern, self._column_regex_pattern]
+            self.__class__.__name__,
+            [self._src_dir, self._src_pattern, self._column_regex_pattern],
         )
         valid()
 
-        if self._dest_dir:
-            os.makedirs(self._dest_dir, exist_ok=True)
-
         files = super().get_target_files(self._src_dir, self._src_pattern)
         self.check_file_existence(files)
         super().io_files(files, func=self.convert)
 
     def convert(self, fi, fo):
         with open(fi, mode="rt") as i:
             reader = csv.DictReader(i)
@@ -230,46 +239,51 @@
     def execute(self, *args):
         valid = EssentialParameters(
             self.__class__.__name__,
             [self._src_dir, self._src_pattern, self._dest_column_name],
         )
         valid()
 
-        if self._dest_dir:
-            os.makedirs(self._dest_dir, exist_ok=True)
-
         if len(self._columns) < 2 or type(self._columns) is not list:
             raise InvalidParameter("'columns' must 2 or more lengths")
 
         files = super().get_target_files(self._src_dir, self._src_pattern)
         self.check_file_existence(files)
 
         super().io_files(files, func=self.convert)
 
     def convert(self, fi, fo):
-        df = pandas.read_csv(
+        chunk_size_handling(self._read_csv_func, fi, fo)
+
+    def _read_csv_func(self, chunksize, fi, fo):
+        # Used in chunk_size_handling
+        first_write = True
+        tfr = pandas.read_csv(
             fi,
             dtype=str,
             encoding=self._encoding,
+            chunksize=chunksize,
         )
-
         dest_str = None
-        for c in self._columns:
-            if dest_str is None:
-                dest_str = df[c].astype(str)
-            else:
-                dest_str = dest_str + self._sep + df[c].astype(str)
-            df = df.drop(columns=[c])
-        df[self._dest_column_name] = dest_str
-
-        df.to_csv(
-            fo,
-            encoding=self._encoding,
-            index=False,
-        )
+        for df in tfr:
+            for c in self._columns:
+                if dest_str is None:
+                    dest_str = df[c].astype(str)
+                else:
+                    dest_str = dest_str + self._sep + df[c].astype(str)
+                df = df.drop(columns=[c])
+            df[self._dest_column_name] = dest_str
+            df.to_csv(
+                fo,
+                encoding=self._encoding,
+                header=True if first_write else False,
+                index=False,
+                mode="w" if first_write else "a",
+            )
+            first_write = False
 
 
 class CsvMergeExclusive(FileBaseTransform):
     """
     Compare specific columns each file.
     If matched, exclude rows.
     """
@@ -298,49 +312,57 @@
                 self._src_column,
                 self._target_compare_path,
                 self._target_column,
             ],
         )
         valid()
 
-        if self._dest_dir:
-            os.makedirs(self._dest_dir, exist_ok=True)
-
         files = super().get_target_files(self._src_dir, self._src_pattern)
         self.check_file_existence(files)
 
         target = super().get_target_files(
-            os.path.dirname(self._target_compare_path), os.path.basename(self._target_compare_path)
+            os.path.dirname(self._target_compare_path),
+            os.path.basename(self._target_compare_path),
         )
         self.check_file_existence(target)
 
-        self.df_target = pandas.read_csv(self._target_compare_path)
-        if self._target_column not in self.df_target:
+        header = pandas.read_csv(self._target_compare_path, nrows=0)
+        if self._target_column not in header:
             raise KeyError(
                 "Target Compare file does not exist target column [%s]." % self._target_column
             )
 
-        self.df_target_list = self.df_target[self._target_column].values.tolist()
+        df_target = pandas.read_csv(self._target_compare_path, usecols=[self._target_column])
+        self.df_target_list = df_target[self._target_column].values.tolist()
 
         super().io_files(files, func=self.convert)
 
     def convert(self, fi, fo):
-        df = pandas.read_csv(fi)
+        header = pandas.read_csv(fi, dtype=str, encoding=self._encoding, nrows=0)
         try:
-            df[self._src_column].values.tolist()
+            header[self._src_column].values.tolist()
         except KeyError:
             raise KeyError("Src file does not exist target column [%s]." % self._target_column)
 
-        df = df[~df[self._src_column].isin(self.df_target_list)]
+        chunk_size_handling(self._read_csv_func, fi, fo)
 
-        df.to_csv(
-            fo,
-            encoding=self._encoding,
-            index=False,
-        )
+    def _read_csv_func(self, chunksize, fi, fo):
+        # Used in chunk_size_handling
+        first_write = True
+        tfr = pandas.read_csv(fi, chunksize=chunksize)
+        for df in tfr:
+            df = df[~df[self._src_column].isin(self.df_target_list)]
+            df.to_csv(
+                fo,
+                encoding=self._encoding,
+                header=True if first_write else False,
+                index=False,
+                mode="w" if first_write else "a",
+            )
+            first_write = False
 
 
 class ColumnLengthAdjust(FileBaseTransform):
     """
     Adjust csv (tsv) column to maximum length
     """
 
@@ -354,17 +376,14 @@
     def execute(self, *args):
         valid = EssentialParameters(
             self.__class__.__name__,
             [self._src_dir, self._src_pattern, self._adjust],
         )
         valid()
 
-        if self._dest_dir:
-            os.makedirs(self._dest_dir, exist_ok=True)
-
         files = super().get_target_files(self._src_dir, self._src_pattern)
         self.check_file_existence(files)
 
         super().io_writers(files, encoding=self._encoding)
 
         for fi, fo in super().io_writers(files, encoding=self._encoding):
             reader = csv.DictReader(fi)
@@ -406,16 +425,15 @@
                 self._src2_pattern,
                 self._dest_dir,
                 self._dest_name,
             ],
         )
         valid()
 
-        if self._dest_dir:
-            os.makedirs(self._dest_dir, exist_ok=True)
+        os.makedirs(self._dest_dir, exist_ok=True)
 
         target1_files = File().get_target_files(self._src_dir, self._src1_pattern)
         target2_files = File().get_target_files(self._src_dir, self._src2_pattern)
         if len(target1_files) == 0:
             raise InvalidCount(
                 "An input file %s does not exist." % os.path.join(self._src_dir, self._src1_pattern)
             )
@@ -427,35 +445,49 @@
             self._logger.error("Hit target files %s" % target1_files)
             raise InvalidCount("Input files must be only one.")
         elif len(target2_files) > 1:
             self._logger.error("Hit target files %s" % target2_files)
             raise InvalidCount("Input files must be only one.")
 
         self._logger.info("Merge %s and %s." % (target1_files[0], target2_files[0]))
-        df1 = pandas.read_csv(
+
+        chunk_size_handling(self._read_csv_func, target1_files, target2_files)
+
+    def _read_csv_func(self, chunksize, target1_files, target2_files):
+        # Used in chunk_size_handling
+        first_write = True
+        tfr1 = pandas.read_csv(
             os.path.join(self._src_dir, target1_files[0]),
             dtype=str,
             encoding=self._encoding,
+            chunksize=chunksize,
         )
-        df2 = pandas.read_csv(
+        for df in tfr1:
+            df.to_csv(
+                os.path.join(self._dest_dir, self._dest_name),
+                encoding=self._encoding,
+                header=True if first_write else False,
+                index=False,
+                mode="w" if first_write else "a",
+            )
+            first_write = False
+        tfr2 = pandas.read_csv(
             os.path.join(self._src_dir, target2_files[0]),
             dtype=str,
             encoding=self._encoding,
+            chunksize=chunksize,
         )
-        df = pandas.merge(df1, df2)
-        if "Unnamed: 0" in df.index:
-            del df["Unnamed: 0"]
-
-        dest_name = self._dest_name
-
-        df.to_csv(
-            os.path.join(self._dest_dir, dest_name),
-            encoding=self._encoding,
-            index=False,
-        )
+        for df in tfr2:
+            df.to_csv(
+                os.path.join(self._dest_dir, self._dest_name),
+                encoding=self._encoding,
+                header=False,
+                index=False,
+                mode="a",
+            )
 
 
 class CsvColumnSelect(FileBaseTransform):
     """
     Select columns in Csv file in specified order
     """
 
@@ -465,41 +497,53 @@
 
     def column_order(self, column_order):
         self._column_order = column_order
 
     def execute(self, *args):
         # essential parameters check
         valid = EssentialParameters(
-            self.__class__.__name__, [self._src_dir, self._src_pattern, self._column_order]
+            self.__class__.__name__,
+            [self._src_dir, self._src_pattern, self._column_order],
         )
         valid()
 
-        if self._dest_dir:
-            os.makedirs(self._dest_dir, exist_ok=True)
-
         files = File().get_target_files(self._src_dir, self._src_pattern)
         if len(files) == 0:
             raise FileNotFound("No files are found.")
         self._logger.info("Files found %s" % files)
 
         super().io_files(files, func=self.convert)
 
     def convert(self, fi, fo):
-        df = pandas.read_csv(fi, dtype=str, encoding=self._encoding)
-        if set(self._column_order) - set(df.columns.values):
-            raise InvalidParameter(
-                "column_order define not included target file's column : %s"
-                % (set(self._column_order) - set(df.columns.values))
-            )
-        df = df.loc[:, self._column_order]
-        df.to_csv(
-            fo,
+        chunk_size_handling(self._read_csv_func, fi, fo)
+
+    def _read_csv_func(self, chunksize, fi, fo):
+        # Used in chunk_size_handling
+        first_write = True
+        tfr = pandas.read_csv(
+            fi,
+            dtype=str,
             encoding=self._encoding,
-            index=False,
+            chunksize=chunksize,
         )
+        for df in tfr:
+            if set(self._column_order) - set(df.columns.values):
+                raise InvalidParameter(
+                    "column_order define not included target file's column : %s"
+                    % (set(self._column_order) - set(df.columns.values))
+                )
+            df = df.loc[:, self._column_order]
+            df.to_csv(
+                fo,
+                encoding=self._encoding,
+                header=True if first_write else False,
+                index=False,
+                mode="w" if first_write else "a",
+            )
+            first_write = False
 
 
 class CsvConcat(FileBaseTransform):
     """
     Concat csv files
     """
 
@@ -513,16 +557,15 @@
     def execute(self, *args):
         # essential parameters check
         valid = EssentialParameters(
             self.__class__.__name__, [self._src_dir, self._dest_dir, self._dest_name]
         )
         valid()
 
-        if self._dest_dir:
-            os.makedirs(self._dest_dir, exist_ok=True)
+        os.makedirs(self._dest_dir, exist_ok=True)
 
         if not self._src_pattern and not self._src_filenames:
             raise InvalidParameter(
                 "Specifying either 'src_pattern' or 'src_filenames' is essential."
             )
         if self._src_pattern and self._src_filenames:
             raise InvalidParameter("Cannot specify both 'src_pattern' and 'src_filenames'.")
@@ -535,61 +578,77 @@
                 files.append(os.path.join(self._src_dir, file))
 
         if len(files) == 0:
             raise FileNotFound("No files are found.")
         elif len(files) == 1:
             self._logger.warning("Two or more input files are required.")
 
-        file = files.pop(0)
-        df1 = pandas.read_csv(
-            file,
-            dtype=str,
-            encoding=self._encoding,
-        )
+        # Create output headers to conform to the concat specification.
+        file_1 = files[0]
+        output_header = pandas.read_csv(file_1, dtype=str, encoding=self._encoding, nrows=0)
+        for file in files[1:]:
+            output_header = pandas.concat(
+                [
+                    output_header,
+                    pandas.read_csv(file, dtype=str, encoding=self._encoding, nrows=0),
+                ]
+            )
+
+        chunk_size_handling(self._read_csv_func, files, output_header)
 
+    def _read_csv_func(self, chunksize, files, output_header):
+        # Used in chunk_size_handling
+        first_write = True
         for file in files:
-            df2 = pandas.read_csv(
+            tfr = pandas.read_csv(
                 file,
                 dtype=str,
                 encoding=self._encoding,
+                chunksize=chunksize,
             )
-            df1 = pandas.concat([df1, df2])
-
-        dest_name = self._dest_name
-
-        df1.to_csv(
-            os.path.join(self._dest_dir, dest_name),
-            encoding=self._encoding,
-            index=False,
-        )
+            for df in tfr:
+                # Change the header order to the one you plan to output.
+                df = pandas.concat([output_header, df])
+                df.to_csv(
+                    os.path.join(self._dest_dir, self._dest_name),
+                    encoding=self._encoding,
+                    header=True if first_write else False,
+                    index=False,
+                    mode="w" if first_write else "a",
+                )
+                first_write = False
 
 
 class CsvConvert(FileBaseTransform):
     """
     Change csv format
     """
 
     def __init__(self):
         super().__init__()
         self._headers = []
         self._headers_existence = True
+        self._add_headers = None
         self._before_format = "csv"
         self._before_enc = self._encoding
         self._after_format = None
         self._after_enc = None
         self._after_nl = "LF"
-        self._reader_quote = "QUOTE_NONE"
+        self._reader_quote = "QUOTE_MINIMAL"
         self._quote = "QUOTE_MINIMAL"
 
     def headers(self, headers):
         self._headers = headers
 
     def headers_existence(self, headers_existence):
         self._headers_existence = headers_existence
 
+    def add_headers(self, add_headers):
+        self._add_headers = add_headers
+
     def before_format(self, before_format):
         self._before_format = before_format
 
     def before_enc(self, before_enc):
         self._before_enc = before_enc
 
     def after_format(self, after_format):
@@ -611,17 +670,14 @@
         # essential parameters check
         valid = EssentialParameters(
             self.__class__.__name__,
             [self._src_dir, self._src_pattern, self._before_format, self._before_enc],
         )
         valid()
 
-        if self._dest_dir:
-            os.makedirs(self._dest_dir, exist_ok=True)
-
         if self._after_format is None:
             self._after_format = self._before_format
 
         if self._after_enc is None:
             self._after_enc = self._before_enc
 
         files = super().get_target_files(self._src_dir, self._src_pattern)
@@ -644,15 +700,19 @@
                     lineterminator=Csv.newline_convert(self._after_nl),
                 )
 
                 for i, line in enumerate(reader):
                     if i == 0:
                         if self._headers_existence is False:
                             continue
-                        writer.writerow(self._replace_headers(line))
+                        if self._add_headers:
+                            writer.writerow(self._add_headers)
+                            writer.writerow(line)
+                        else:
+                            writer.writerow(self._replace_headers(line))
                     else:
                         writer.writerow(line)
 
     def _replace_headers(self, old_headers):
         """
         Replace old headers to new headers
         """
@@ -696,16 +756,15 @@
         # essential parameters check
         valid = EssentialParameters(
             self.__class__.__name__,
             [self._order, self._src_dir, self._src_pattern, self._dest_dir],
         )
         valid()
 
-        if self._dest_dir:
-            os.makedirs(self._dest_dir, exist_ok=True)
+        os.makedirs(self._dest_dir, exist_ok=True)
 
         files = super().get_target_files(self._src_dir, self._src_pattern)
         self.check_file_existence(files)
 
         ymd_hms = datetime.now().strftime("%Y%m%d%H%M%S%f")
         dbname = ".%s_%s.db" % (ymd_hms, StringUtil().random_str(8))
         tblname = "temp_table"
@@ -740,22 +799,165 @@
         super().__init__()
 
     def execute(self, *args):
         # essential parameters check
         valid = EssentialParameters(self.__class__.__name__, [self._src_dir, self._src_pattern])
         valid()
 
-        if self._dest_dir:
-            os.makedirs(self._dest_dir, exist_ok=True)
-
         files = super().get_target_files(self._src_dir, self._src_pattern)
         self.check_file_existence(files)
 
         super().io_files(files, ext="jsonl", func=self.convert)
 
     def convert(self, fi, fo):
         with open(fi, mode="r", encoding=self._encoding, newline="") as i, jsonlines.open(
             fo, mode="w"
         ) as writer:
             reader = csv.DictReader(i)
             for row in reader:
                 writer.write(row)
+
+
+class CsvColumnCopy(FileBaseTransform):
+    """
+    Copy column data (new or overwrite)
+    """
+
+    def __init__(self):
+        super().__init__()
+        self._src_column = None
+        self._dest_column = None
+
+    def src_column(self, src_column):
+        self._src_column = src_column
+
+    def dest_column(self, dest_column):
+        self._dest_column = dest_column
+
+    def execute(self, *args):
+        valid = EssentialParameters(
+            self.__class__.__name__,
+            [self._src_dir, self._src_pattern, self._dest_dir, self._src_column, self._dest_column],
+        )
+        valid()
+
+        files = super().get_target_files(self._src_dir, self._src_pattern)
+        self.check_file_existence(files)
+
+        super().io_files(files, func=self.convert)
+
+    def convert(self, fi, fo):
+        header = pandas.read_csv(fi, dtype=str, encoding=self._encoding, nrows=0)
+        if self._src_column not in header:
+            raise KeyError("Copy source column does not exist in file. [%s]" % self._src_column)
+
+        chunk_size_handling(self._read_csv_func, fi, fo)
+
+    def _read_csv_func(self, chunksize, fi, fo):
+        # Used in chunk_size_handling
+        first_write = True
+        tfr = pandas.read_csv(
+            fi,
+            dtype=str,
+            encoding=self._encoding,
+            chunksize=chunksize,
+        )
+
+        for df in tfr:
+            df[self._dest_column] = df[self._src_column]
+            df.to_csv(
+                fo,
+                encoding=self._encoding,
+                header=True if first_write else False,
+                index=False,
+                mode="w" if first_write else "a",
+            )
+            first_write = False
+
+
+class CsvColumnReplace(FileBaseTransform):
+    """
+    Replace matching regular expression values for a specific column from a csv file.
+    """
+
+    def __init__(self):
+        super().__init__()
+        self._column = None
+        self._regex_pattern = None
+        self._rep_str = None
+        self._regex_compile = None
+
+    def column(self, column):
+        self._column = column
+
+    def regex_pattern(self, regex_pattern):
+        self._regex_pattern = regex_pattern
+
+    def rep_str(self, rep_str):
+        self._rep_str = rep_str
+
+    def _replace_string(self, string):
+        return self._regex_compile.sub(self._rep_str, string)
+
+    def execute(self, *args):
+        valid = EssentialParameters(
+            self.__class__.__name__,
+            [self._src_dir, self._src_pattern, self._column],
+        )
+        valid()
+
+        files = super().get_target_files(self._src_dir, self._src_pattern)
+        self.check_file_existence(files)
+
+        if self._rep_str is None:
+            raise InvalidParameter("The converted string is not defined in yaml file: rep_str")
+        if self._regex_pattern is None:
+            raise InvalidParameter(
+                "The conversion pattern is not defined in yaml file: regex_pattern"
+            )
+        self._regex_compile = re.compile(self._regex_pattern)
+
+        super().io_files(files, func=self.convert)
+
+    def convert(self, fi, fo):
+        header = pandas.read_csv(fi, dtype=str, encoding=self._encoding, nrows=0)
+        if self._column not in header:
+            raise KeyError("Replace source column does not exist in file. [%s]" % self._column)
+
+        chunk_size_handling(self._read_csv_func, fi, fo)
+
+    def _read_csv_func(self, chunksize, fi, fo):
+        # Used in chunk_size_handling
+        first_write = True
+        tfr = pandas.read_csv(
+            fi,
+            dtype=str,
+            encoding=self._encoding,
+            chunksize=chunksize,
+        )
+
+        for df in tfr:
+            df[self._column] = df[self._column].apply(self._replace_string)
+            df.to_csv(
+                fo,
+                header=True if first_write else False,
+                encoding=self._encoding,
+                index=False,
+                mode="w" if first_write else "a",
+            )
+            first_write = False
+
+
+def chunk_size_handling(read_csv_func, *args, **kwd):
+    """
+    Processing to avoid memory errors in pandas's read_csv.
+    Use this function when you want to do the same handling when extending cliboa.
+    """
+    chunksize = 1024 * 1024
+    while 0 < chunksize:
+        try:
+            read_csv_func(chunksize, *args, **kwd)
+            break
+        except MemoryError as error:
+            if chunksize <= 1:
+                raise error
+            chunksize //= 2
```

### Comparing `cliboa-2.3.0b0/cliboa/scenario/transform/file.py` & `cliboa-2.3.1b0/cliboa/scenario/transform/file.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,24 +37,25 @@
 
     Basically transform class of Cliboa is that find files,
     do something, and output transformed files.
     When output files are created, name of the files will be the same name with the input files
     (original input files will be changed to the transformed files).
     If you would not like to remove the original files,
     give a path to the "dest_dir" for output directory.
+    (If a non-existent directory path is specified, the directory is automatically created.)
 
     Note:
     Output files are not always be the same name with the input file names.
     See documentation for individual classes for details.
     """
 
     def __init__(self):
         super().__init__()
-        self._src_dir = ""
-        self._src_pattern = ""
+        self._src_dir = None
+        self._src_pattern = None
         self._dest_dir = None
         self._dest_name = None
         self._encoding = "utf-8"
         self._nonfile_error = False
         self._force_continue = False
 
     def src_dir(self, src_dir):
@@ -103,14 +104,15 @@
                 output_name = os.path.splitext(name)[0] + ext
             else:
                 output_name = os.path.splitext(name)[0] + "." + ext
         else:
             output_name = name
 
         if self._dest_dir:
+            os.makedirs(self._dest_dir, exist_ok=True)
             output_dir = self._dest_dir
         else:
             output_dir = root
 
         output_path = os.path.join(output_dir, output_name)
 
         fd, temp_file = tempfile.mkstemp()
@@ -237,19 +239,19 @@
                         buf = i.read(self._chunk_size)
                         if buf == b"":
                             break
                         o.write(buf)
             elif ext == ".gz":
                 self._logger.info("Decompress gz file %s" % f)
                 dcom_name = os.path.splitext(os.path.basename(f))[0]
-                decom_path = (
-                    os.path.join(self._dest_dir, dcom_name)
-                    if self._dest_dir is not None
-                    else os.path.join(self._src_dir, dcom_name)
-                )
+                if self._dest_dir:
+                    os.makedirs(self._dest_dir, exist_ok=True)
+                    decom_path = os.path.join(self._dest_dir, dcom_name)
+                else:
+                    decom_path = os.path.join(self._src_dir, dcom_name)
                 with gzip.open(f, "rb") as i, open(decom_path, "wb") as o:
                     while True:
                         buf = i.read(self._chunk_size)
                         if buf == b"":
                             break
                         o.write(buf)
             else:
@@ -260,33 +262,38 @@
     """
     Compress files
     """
 
     def __init__(self):
         super().__init__()
         self._format = None
-        self._chunk_size = None
+        self._chunk_size = 1048576
 
     def format(self, format):
         self._format = format.lower()
 
     def chunk_size(self, chunk_size):
         self._chunk_size = chunk_size
 
     def execute(self, *args):
         # essential parameters check
         valid = EssentialParameters(
-            self.__class__.__name__, [self._src_dir, self._src_pattern, self._format]
+            self.__class__.__name__,
+            [self._src_dir, self._src_pattern, self._format],
         )
         valid()
 
         files = super().get_target_files(self._src_dir, self._src_pattern)
         self.check_file_existence(files)
 
-        dir = self._dest_dir if self._dest_dir is not None else self._src_dir
+        if self._dest_dir:
+            os.makedirs(self._dest_dir, exist_ok=True)
+            dir = self._dest_dir
+        else:
+            dir = self._src_dir
         for f in files:
             if self._format == "zip":
                 self._logger.info("Compress file %s to zip." % f)
                 with zipfile.ZipFile(
                     os.path.join(dir, (os.path.basename(f) + ".zip")),
                     "w",
                     zipfile.ZIP_DEFLATED,
@@ -426,18 +433,23 @@
             if self._header:
                 with open(file, encoding=self._encoding) as i:
                     self._header_row = i.readline()
 
             row = self._ifile_reader(file)
             newfilename = px + nameonly + ".%s" + ext
 
+            if self._dest_dir:
+                os.makedirs(self._dest_dir, exist_ok=True)
+                dest_dir = self._dest_dir
+            else:
+                dest_dir = self._src_dir
             has_left = True
             index = 1
             while has_left:
-                ofile_path = os.path.join(self._dest_dir, newfilename % str(index))
+                ofile_path = os.path.join(dest_dir, newfilename % str(index))
                 has_left = self._ofile_generator(ofile_path, row)
                 index = index + 1
 
     def _ifile_reader(self, filepath):
         with open(filepath, encoding=self._encoding) as i:
             if self._header is True:
                 i.readline()
@@ -598,15 +610,19 @@
             [self._src_dir, self._src_pattern, self._format],
         )
         valid()
 
         files = super().get_target_files(self._src_dir, self._src_pattern)
         self.check_file_existence(files)
 
-        dir = self._dest_dir if self._dest_dir is not None else self._src_dir
+        if self._dest_dir:
+            os.makedirs(self._dest_dir, exist_ok=True)
+            dir = self._dest_dir
+        else:
+            dir = self._src_dir
 
         valid = EssentialParameters(self.__class__.__name__, [self._dest_name])
         valid()
         dest_path = os.path.join(dir, (self._dest_name + ".%s" % self._format))
 
         if self._format == "tar":
             with tarfile.open(dest_path, "w") as tar:
```

### Comparing `cliboa-2.3.0b0/cliboa/scenario/transform/gpg.py` & `cliboa-2.3.1b0/cliboa/scenario/transform/gpg.py`

 * *Files 9% similar despite different names*

```diff
@@ -79,14 +79,16 @@
 
     def execute(self, *args):
         super().execute()
 
         valid = EssentialParameters(self.__class__.__name__, [self._dest_dir, self._name_email])
         valid()
 
+        os.makedirs(self._dest_dir, exist_ok=True)
+
         Gpg(self._gnupghome).generate_key(
             self._dest_dir,
             name_real=self._name_real,
             name_email=self._name_email,
             passphrase=self._passphrase,
         )
 
@@ -118,19 +120,19 @@
 
         if self._key_dir and self._key_pattern:
             key_files = super().get_target_files(self._key_dir, self._key_pattern)
             self._logger.info("Keys found %s" % key_files)
             self.key_import(gpg, key_files, self._trust_level)
 
         for file in files:
-            dest_path = (
-                os.path.join(self._dest_dir, os.path.basename(file))
-                if self._dest_dir is not None
-                else os.path.join(self._src_dir, os.path.basename(file))
-            )
+            if self._dest_dir is not None:
+                os.makedirs(self._dest_dir, exist_ok=True)
+                dest_path = os.path.join(self._dest_dir, os.path.basename(file))
+            else:
+                dest_path = os.path.join(self._src_dir, os.path.basename(file))
             gpg.encrypt(
                 file,
                 dest_path,
                 recipients=self._recipients,
                 passphrase=self._passphrase,
                 always_trust=self._always_trust,
             )
@@ -157,19 +159,19 @@
             self._logger.info("Keys found %s" % key_files)
             self.key_import(key_files, self._trust_level)
 
         gpg = Gpg(self._gnupghome)
         for file in files:
             root, ext = os.path.splitext(file)
             if ext == ".gpg":
-                dest_path = (
-                    os.path.join(self._dest_dir, os.path.basename(root))
-                    if self._dest_dir is not None
-                    else os.path.join(self._src_dir, os.path.basename(root))
-                )
+                if self._dest_dir is not None:
+                    os.makedirs(self._dest_dir, exist_ok=True)
+                    dest_path = os.path.join(self._dest_dir, os.path.basename(root))
+                else:
+                    dest_path = os.path.join(self._src_dir, os.path.basename(root))
                 gpg.decrypt(
                     file,
                     dest_path,
                     passphrase=self._passphrase,
                     always_trust=self._always_trust,
                 )
             else:
```

### Comparing `cliboa-2.3.0b0/cliboa/scenario/transform/json.py` & `cliboa-2.3.1b0/cliboa/scenario/transform/json.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
 #
 # The above copyright notice and this permission notice shall be included in
 # all copies or substantial portions of the Software.
 #
 import csv
-import os
 from abc import abstractmethod
 
 import jsonlines
 import pandas
 
 from cliboa.core.validator import EssentialParameters
 from cliboa.scenario.transform.file import FileBaseTransform
@@ -103,17 +102,14 @@
 
     def execute(self, *args):
         valid = EssentialParameters(
             self.__class__.__name__, [self._src_dir, self._src_pattern, self._pairs]
         )
         valid()
 
-        if self._dest_dir:
-            os.makedirs(self._dest_dir, exist_ok=True)
-
         if not isinstance(self._pairs, dict):
             raise InvalidParameter("argument 'pairs' only allow dict format.")
 
         files = super().get_target_files(self._src_dir, self._src_pattern)
         self.check_file_existence(files)
         super().io_files(files, func=self.convert)
```

### Comparing `cliboa-2.3.0b0/cliboa/scenario/transform/system.py` & `cliboa-2.3.1b0/cliboa/scenario/transform/system.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 class ExecuteShellScript(BaseStep):
     """
     Execute Shell Script
     """
 
     def __init__(self):
         super().__init__()
-        self._command = ""
-        self._work_dir = ""
+        self._command = None
+        self._work_dir = "./"
 
     def command(self, command):
         self._command = command
 
     def work_dir(self, work_dir):
         self._work_dir = work_dir
```

### Comparing `cliboa-2.3.0b0/cliboa/scenario/validator.py` & `cliboa-2.3.1b0/cliboa/scenario/validator.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.0b0/cliboa/template/Pipfile.above36` & `cliboa-2.3.1b0/cliboa/template/Pipfile.above36`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.0b0/cliboa/template/Pipfile.above37` & `cliboa-2.3.1b0/cliboa/template/Pipfile.above37`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.0b0/cliboa/template/Pipfile.above38` & `cliboa-2.3.1b0/cliboa/template/Pipfile.above38`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.0b0/cliboa/template/Pipfile.above39` & `cliboa-2.3.1b0/cliboa/template/Pipfile.above39`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.0b0/cliboa/template/bin/clibomanager.py` & `cliboa-2.3.1b0/cliboa/template/bin/clibomanager.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,12 +18,12 @@
 import sys
 
 if __name__ == "__main__":
     # setting of environment values
     sys.path.append(os.getcwd())
     os.environ.setdefault("CLIBOA_ENV", "common.environment")
     try:
-        from cliboa.client import run
+        from cliboa.interface import run
 
         run()
     except Exception as e:
         print("Exception occurred. %s ", e.args)
```

### Comparing `cliboa-2.3.0b0/cliboa/template/pyproject.above37.toml` & `cliboa-2.3.1b0/cliboa/template/pyproject.above37.toml`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.0b0/cliboa/template/pyproject.above38.toml` & `cliboa-2.3.1b0/cliboa/template/pyproject.above38.toml`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.0b0/cliboa/template/pyproject.above39.toml` & `cliboa-2.3.1b0/cliboa/template/pyproject.above39.toml`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.0b0/cliboa/util/cache.py` & `cliboa-2.3.1b0/cliboa/util/cache.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.0b0/cliboa/util/class_util.py` & `cliboa-2.3.1b0/cliboa/util/class_util.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.0b0/cliboa/util/csv.py` & `cliboa-2.3.1b0/cliboa/util/csv.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.0b0/cliboa/util/date.py` & `cliboa-2.3.1b0/cliboa/util/date.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.0b0/cliboa/util/exception.py` & `cliboa-2.3.1b0/cliboa/util/exception.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.0b0/cliboa/util/file.py` & `cliboa-2.3.1b0/cliboa/util/file.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.0b0/cliboa/util/ftp_util.py` & `cliboa-2.3.1b0/cliboa/util/ftp_util.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.0b0/cliboa/util/gpg.py` & `cliboa-2.3.1b0/cliboa/util/gpg.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.0b0/cliboa/util/helper.py` & `cliboa-2.3.1b0/cliboa/util/helper.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.0b0/cliboa/util/http.py` & `cliboa-2.3.1b0/cliboa/util/http.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.0b0/cliboa/util/parallel_with_config.py` & `cliboa-2.3.1b0/cliboa/util/parallel_with_config.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.0b0/cliboa/util/rdbms_util.py` & `cliboa-2.3.1b0/cliboa/util/rdbms_util.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.0b0/cliboa/util/sftp.py` & `cliboa-2.3.1b0/cliboa/util/sftp.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.0b0/cliboa/util/string.py` & `cliboa-2.3.1b0/cliboa/util/string.py`

 * *Files identical despite different names*

### Comparing `cliboa-2.3.0b0/cliboa.egg-info/SOURCES.txt` & `cliboa-2.3.1b0/cliboa.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
+LICENSE
 README.md
-pyproject.toml
 setup.cfg
 setup.py
 cliboa/__init__.py
-cliboa/client.py
+cliboa/interface.py
 cliboa.egg-info/PKG-INFO
 cliboa.egg-info/SOURCES.txt
 cliboa.egg-info/dependency_links.txt
 cliboa.egg-info/entry_points.txt
 cliboa.egg-info/top_level.txt
 cliboa/adapter/__init__.py
 cliboa/adapter/aws.py
@@ -62,14 +62,15 @@
 cliboa/scenario/load/azure.py
 cliboa/scenario/load/file.py
 cliboa/scenario/load/gcp.py
 cliboa/scenario/load/mysql.py
 cliboa/scenario/load/postgres.py
 cliboa/scenario/load/sftp.py
 cliboa/scenario/load/sqlite.py
+cliboa/scenario/transform/aes.py
 cliboa/scenario/transform/csv.py
 cliboa/scenario/transform/file.py
 cliboa/scenario/transform/gpg.py
 cliboa/scenario/transform/json.py
 cliboa/scenario/transform/system.py
 cliboa/template/Pipfile.above36
 cliboa/template/Pipfile.above37
@@ -86,15 +87,14 @@
 cliboa/util/class_util.py
 cliboa/util/constant.py
 cliboa/util/csv.py
 cliboa/util/date.py
 cliboa/util/exception.py
 cliboa/util/file.py
 cliboa/util/ftp_util.py
-cliboa/util/gcp.py
 cliboa/util/gpg.py
 cliboa/util/helper.py
 cliboa/util/http.py
 cliboa/util/lisboa_log.py
 cliboa/util/parallel_with_config.py
 cliboa/util/rdbms_util.py
 cliboa/util/sftp.py
```

### Comparing `cliboa-2.3.0b0/setup.py` & `cliboa-2.3.1b0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 def read(filename):
     with open(path.join(path.dirname(__file__), filename), encoding="utf-8") as f:
         return f.read()
 
 
 setup(
     name="cliboa",
-    version="2.3.0b0",
+    version="2.3.1b0",
     description="application framework for ETL(ELT) processing",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     url="https://github.com/BrainPad/cliboa",  # Optional
     author="BrainPad",
     # author_email='brainpad.co.jp',
     classifiers=[
```

