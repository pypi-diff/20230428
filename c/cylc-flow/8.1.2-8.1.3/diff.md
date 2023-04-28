# Comparing `tmp/cylc-flow-8.1.2.tar.gz` & `tmp/cylc-flow-8.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cylc-flow-8.1.2.tar", last modified: Mon Feb 20 17:09:41 2023, max compression
+gzip compressed data, was "cylc-flow-8.1.3.tar", last modified: Fri Apr 28 11:30:58 2023, max compression
```

## Comparing `cylc-flow-8.1.2.tar` & `cylc-flow-8.1.3.tar`

### file list

```diff
@@ -1,314 +1,315 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 17:09:41.408514 cylc-flow-8.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-02-20 17:09:41.408514 cylc-flow-8.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 17:09:41.384514 cylc-flow-8.1.2/cylc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 17:09:41.392514 cylc-flow-8.1.2/cylc/flow/
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14818 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/async_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    17180 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/broadcast_mgr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/broadcast_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/c3mro.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 17:09:41.392514 cylc-flow-8.1.2/cylc/flow/cfgspec/
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/cfgspec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/cfgspec/glbl_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)    71480 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/cfgspec/globalcfg.py
--rw-r--r--   0 runner    (1001) docker     (123)    83023 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/cfgspec/workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/command_polling.py
--rw-r--r--   0 runner    (1001) docker     (123)    97425 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/context_node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 17:09:41.392514 cylc-flow-8.1.2/cylc/flow/cycling/
--rw-r--r--   0 runner    (1001) docker     (123)    14593 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/cycling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23211 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/cycling/integer.py
--rw-r--r--   0 runner    (1001) docker     (123)    34928 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/cycling/iso8601.py
--rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/cycling/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/cycling/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/cylc_subproc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/daemonize.py
--rw-r--r--   0 runner    (1001) docker     (123)    22194 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/data_messages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    87818 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/data_store_mgr.py
--rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/dbstatecheck.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 17:09:41.396514 cylc-flow-8.1.2/cylc/flow/etc/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/etc/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     7934 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/etc/cylc
--rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/etc/cylc-completion.bash
--rw-r--r--   0 runner    (1001) docker     (123)    14460 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/etc/job.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 17:09:41.396514 cylc-flow-8.1.2/cylc/flow/etc/syntax/
--rw-r--r--   0 runner    (1001) docker     (123)     5210 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/etc/syntax/cylc-mode.el
--rw-r--r--   0 runner    (1001) docker     (123)    25250 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/etc/syntax/cylc.lang
--rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/etc/syntax/cylc.vim
--rw-r--r--   0 runner    (1001) docker     (123)    10612 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/etc/syntax/cylc.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 17:09:41.396514 cylc-flow-8.1.2/cylc/flow/etc/tutorial/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/etc/tutorial/api-keys
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 17:09:41.396514 cylc-flow-8.1.2/cylc/flow/etc/tutorial/consolidation-tutorial/
--rwxr-xr-x   0 runner    (1001) docker     (123)      802 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/etc/tutorial/consolidation-tutorial/.validate
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 17:09:41.396514 cylc-flow-8.1.2/cylc/flow/etc/tutorial/consolidation-tutorial/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4248 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/etc/tutorial/consolidation-tutorial/bin/consolidate-observations
--rwxr-xr-x   0 runner    (1001) docker     (123)     9151 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/etc/tutorial/consolidation-tutorial/bin/forecast
--rwxr-xr-x   0 runner    (1001) docker     (123)     7216 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/etc/tutorial/consolidation-tutorial/bin/get-observations
--rwxr-xr-x   0 runner    (1001) docker     (123)     6453 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/etc/tutorial/consolidation-tutorial/bin/get-rainfall
--rwxr-xr-x   0 runner    (1001) docker     (123)     3721 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/etc/tutorial/consolidation-tutorial/bin/post-process
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 17:09:41.396514 cylc-flow-8.1.2/cylc/flow/etc/tutorial/consolidation-tutorial/etc/
--rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/etc/tutorial/consolidation-tutorial/etc/met-office-sites.dat
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/etc/tutorial/consolidation-tutorial/etc/python-job.settings
--rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/etc/tutorial/consolidation-tutorial/flow.cylc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 17:09:41.384514 cylc-flow-8.1.2/cylc/flow/etc/tutorial/consolidation-tutorial/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 17:09:41.396514 cylc-flow-8.1.2/cylc/flow/etc/tutorial/consolidation-tutorial/lib/python/
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/etc/tutorial/consolidation-tutorial/lib/python/mercator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10018 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/etc/tutorial/consolidation-tutorial/lib/python/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 17:09:41.396514 cylc-flow-8.1.2/cylc/flow/etc/tutorial/consolidation-tutorial/lib/template/
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/etc/tutorial/consolidation-tutorial/lib/template/map.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 17:09:41.396514 cylc-flow-8.1.2/cylc/flow/etc/tutorial/cylc-forecasting-workflow/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1139 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/etc/tutorial/cylc-forecasting-workflow/.validate
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 17:09:41.396514 cylc-flow-8.1.2/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4248 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/consolidate-observations
--rwxr-xr-x   0 runner    (1001) docker     (123)     9151 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/forecast
--rwxr-xr-x   0 runner    (1001) docker     (123)     7216 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/get-observations
--rwxr-xr-x   0 runner    (1001) docker     (123)     6453 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/get-rainfall
--rwxr-xr-x   0 runner    (1001) docker     (123)     3721 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/post-process
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 17:09:41.396514 cylc-flow-8.1.2/cylc/flow/etc/tutorial/cylc-forecasting-workflow/etc/
--rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/etc/tutorial/cylc-forecasting-workflow/etc/met-office-sites.dat
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/etc/tutorial/cylc-forecasting-workflow/etc/python-job.settings
--rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/etc/tutorial/cylc-forecasting-workflow/flow.cylc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 17:09:41.384514 cylc-flow-8.1.2/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 17:09:41.396514 cylc-flow-8.1.2/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/python/
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/python/mercator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10018 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/python/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 17:09:41.396514 cylc-flow-8.1.2/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/template/
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/template/map.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 17:09:41.396514 cylc-flow-8.1.2/cylc/flow/etc/tutorial/forecast-script/
--rwxr-xr-x   0 runner    (1001) docker     (123)     9151 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/etc/tutorial/forecast-script/forecast
--rw-r--r--   0 runner    (1001) docker     (123)    10018 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/etc/tutorial/forecast-script/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 17:09:41.396514 cylc-flow-8.1.2/cylc/flow/etc/tutorial/inheritance-tutorial/
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/etc/tutorial/inheritance-tutorial/flow.cylc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 17:09:41.396514 cylc-flow-8.1.2/cylc/flow/etc/tutorial/map-template/
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/etc/tutorial/map-template/map-template.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 17:09:41.384514 cylc-flow-8.1.2/cylc/flow/etc/tutorial/message-trigger-tutorial/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 17:09:41.396514 cylc-flow-8.1.2/cylc/flow/etc/tutorial/message-trigger-tutorial/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      180 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/etc/tutorial/message-trigger-tutorial/bin/random.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 17:09:41.396514 cylc-flow-8.1.2/cylc/flow/etc/tutorial/retries-tutorial/
--rwxr-xr-x   0 runner    (1001) docker     (123)      819 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/etc/tutorial/retries-tutorial/.validate
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/etc/tutorial/retries-tutorial/flow.cylc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 17:09:41.396514 cylc-flow-8.1.2/cylc/flow/etc/tutorial/runtime-introduction/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1125 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/etc/tutorial/runtime-introduction/.validate
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 17:09:41.396514 cylc-flow-8.1.2/cylc/flow/etc/tutorial/runtime-introduction/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      459 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/etc/tutorial/runtime-introduction/bin/get-observations
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 17:09:41.396514 cylc-flow-8.1.2/cylc/flow/etc/tutorial/runtime-introduction/etc/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/etc/tutorial/runtime-introduction/etc/python-job.settings
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/etc/tutorial/runtime-introduction/flow.cylc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 17:09:41.396514 cylc-flow-8.1.2/cylc/flow/etc/tutorial/runtime-tutorial/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 17:09:41.400514 cylc-flow-8.1.2/cylc/flow/etc/tutorial/runtime-tutorial/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4248 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/etc/tutorial/runtime-tutorial/bin/consolidate-observations
--rwxr-xr-x   0 runner    (1001) docker     (123)     9151 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/etc/tutorial/runtime-tutorial/bin/forecast
--rwxr-xr-x   0 runner    (1001) docker     (123)     7216 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/etc/tutorial/runtime-tutorial/bin/get-observations
--rwxr-xr-x   0 runner    (1001) docker     (123)     6453 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/etc/tutorial/runtime-tutorial/bin/get-rainfall
--rwxr-xr-x   0 runner    (1001) docker     (123)     3721 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/etc/tutorial/runtime-tutorial/bin/post-process
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 17:09:41.400514 cylc-flow-8.1.2/cylc/flow/etc/tutorial/runtime-tutorial/etc/
--rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/etc/tutorial/runtime-tutorial/etc/met-office-sites.dat
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/etc/tutorial/runtime-tutorial/etc/python-job.settings
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/etc/tutorial/runtime-tutorial/flow.cylc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 17:09:41.384514 cylc-flow-8.1.2/cylc/flow/etc/tutorial/runtime-tutorial/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 17:09:41.400514 cylc-flow-8.1.2/cylc/flow/etc/tutorial/runtime-tutorial/lib/python/
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/etc/tutorial/runtime-tutorial/lib/python/mercator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10018 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/etc/tutorial/runtime-tutorial/lib/python/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 17:09:41.400514 cylc-flow-8.1.2/cylc/flow/etc/tutorial/runtime-tutorial/lib/template/
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/etc/tutorial/runtime-tutorial/lib/template/map.html
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/etc/tutorial/runtime-tutorial/runtime
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 17:09:41.400514 cylc-flow-8.1.2/cylc/flow/etc/tutorial/test-data/
--rw-r--r--   0 runner    (1001) docker     (123)    33085 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/etc/tutorial/test-data/rainfall.csv
--rw-r--r--   0 runner    (1001) docker     (123)    35829 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/etc/tutorial/test-data/wind_20171101T0000Z_x.csv
--rw-r--r--   0 runner    (1001) docker     (123)    38004 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/etc/tutorial/test-data/wind_20171101T0000Z_y.csv
--rw-r--r--   0 runner    (1001) docker     (123)    13602 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/flags.py
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/flow_mgr.py
--rw-r--r--   0 runner    (1001) docker     (123)    35572 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/graph_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/graphnode.py
--rw-r--r--   0 runner    (1001) docker     (123)    18192 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/host_select.py
--rw-r--r--   0 runner    (1001) docker     (123)    10636 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/hostuserutil.py
--rw-r--r--   0 runner    (1001) docker     (123)    24245 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/id.py
--rw-r--r--   0 runner    (1001) docker     (123)    17477 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/id_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/id_match.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 17:09:41.400514 cylc-flow-8.1.2/cylc/flow/install_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/install_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10942 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/install_plugins/log_vc_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 17:09:41.384514 cylc-flow-8.1.2/cylc/flow/jinja/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 17:09:41.400514 cylc-flow-8.1.2/cylc/flow/jinja/filters/
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/jinja/filters/duration_as.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/jinja/filters/pad.py
--rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/jinja/filters/strftime.py
--rw-r--r--   0 runner    (1001) docker     (123)    14670 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/job_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 17:09:41.400514 cylc-flow-8.1.2/cylc/flow/job_runner_handlers/
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/job_runner_handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/job_runner_handlers/at.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/job_runner_handlers/background.py
--rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/job_runner_handlers/loadleveler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/job_runner_handlers/lsf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/job_runner_handlers/moab.py
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/job_runner_handlers/pbs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/job_runner_handlers/pbs_multi_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/job_runner_handlers/sge.py
--rw-r--r--   0 runner    (1001) docker     (123)     6413 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/job_runner_handlers/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/job_runner_handlers/slurm_packjob.py
--rw-r--r--   0 runner    (1001) docker     (123)    38323 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/job_runner_mgr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/listify.py
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/log_diagnosis.py
--rw-r--r--   0 runner    (1001) docker     (123)    15368 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/loggingutil.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 17:09:41.400514 cylc-flow-8.1.2/cylc/flow/main_loop/
--rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/main_loop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9564 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/main_loop/auto_restart.py
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/main_loop/health_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/main_loop/log_data_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/main_loop/log_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/main_loop/log_main_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/main_loop/log_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/main_loop/reset_bad_hosts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 17:09:41.400514 cylc-flow-8.1.2/cylc/flow/network/
--rw-r--r--   0 runner    (1001) docker     (123)     9902 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/network/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/network/authorisation.py
--rw-r--r--   0 runner    (1001) docker     (123)    11918 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/network/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/network/client_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    16257 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/network/graphql.py
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/network/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/network/publisher.py
--rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/network/replier.py
--rw-r--r--   0 runner    (1001) docker     (123)    30538 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/network/resolvers.py
--rw-r--r--   0 runner    (1001) docker     (123)    16389 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/network/scan.py
--rw-r--r--   0 runner    (1001) docker     (123)    73613 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/network/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    14723 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/network/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/network/ssh_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/network/subscriber.py
--rw-r--r--   0 runner    (1001) docker     (123)    28535 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/option_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)    15646 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/param_expand.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 17:09:41.404514 cylc-flow-8.1.2/cylc/flow/parsec/
--rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/parsec/OrderedDict.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/parsec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10823 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/parsec/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/parsec/empysupport.py
--rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/parsec/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    21394 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/parsec/fileparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/parsec/include.py
--rw-r--r--   0 runner    (1001) docker     (123)    11240 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/parsec/jinja2support.py
--rw-r--r--   0 runner    (1001) docker     (123)     8819 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/parsec/upgrade.py
--rw-r--r--   0 runner    (1001) docker     (123)    14533 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/parsec/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    39684 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/parsec/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)    15818 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/pathutil.py
--rw-r--r--   0 runner    (1001) docker     (123)    25082 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/platforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    11173 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/prerequisite.py
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/print_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    13757 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     6932 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    39349 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/rundb.py
--rw-r--r--   0 runner    (1001) docker     (123)    80364 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    20200 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/scheduler_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 17:09:41.408514 cylc-flow-8.1.2/cylc/flow/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15346 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/scripts/broadcast.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15636 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/scripts/cat_log.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5028 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/scripts/check_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/scripts/clean.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2617 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/scripts/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/scripts/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    20478 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/scripts/completion_server.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6429 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/scripts/config.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8931 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/scripts/cycle_point.py
--rw-r--r--   0 runner    (1001) docker     (123)    20960 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/scripts/cylc.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6042 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/scripts/diff.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8083 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/scripts/dump.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4425 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/scripts/ext_trigger.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1491 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/scripts/function_run.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2514 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/scripts/get_resources.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1871 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/scripts/get_workflow_contact.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2311 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/scripts/get_workflow_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    14884 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/scripts/graph.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4378 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/scripts/hold.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10542 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/scripts/install.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1722 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/scripts/jobs_kill.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1697 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/scripts/jobs_poll.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2846 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/scripts/jobs_submit.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2483 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/scripts/kill.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24921 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/scripts/lint.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6228 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/scripts/list.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6094 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/scripts/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/scripts/pause.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3955 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/scripts/ping.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/scripts/play.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2548 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/scripts/poll.py
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/scripts/psutil.py
--rw-r--r--   0 runner    (1001) docker     (123)    12227 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/scripts/reinstall.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3711 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/scripts/release.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3254 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/scripts/reload.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2108 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/scripts/remote_init.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1533 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/scripts/remote_tidy.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2225 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/scripts/remove.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13206 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/scripts/report_timings.py
--rw-r--r--   0 runner    (1001) docker     (123)    15753 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/scripts/scan.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3504 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/scripts/set_outputs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2570 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/scripts/set_verbosity.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12679 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/scripts/show.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8360 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/scripts/stop.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3658 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/scripts/subscribe.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5272 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/scripts/trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/scripts/tui.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6321 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/scripts/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/scripts/validate_install_play.py
--rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/scripts/validate_reinstall.py
--rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/scripts/view.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10001 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/scripts/workflow_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     6439 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/subprocctx.py
--rw-r--r--   0 runner    (1001) docker     (123)    23031 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/subprocpool.py
--rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/task_action_timer.py
--rw-r--r--   0 runner    (1001) docker     (123)    63078 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/task_events_mgr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/task_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/task_job_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)    54673 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/task_job_mgr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/task_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     7701 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/task_outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    77856 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/task_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)    17292 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/task_proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 17:09:41.408514 cylc-flow-8.1.2/cylc/flow/task_queues/
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/task_queues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/task_queues/independent.py
--rw-r--r--   0 runner    (1001) docker     (123)     6610 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/task_remote_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)    22900 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/task_remote_mgr.py
--rw-r--r--   0 runner    (1001) docker     (123)    18078 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/task_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/task_state_prop.py
--rw-r--r--   0 runner    (1001) docker     (123)    10804 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/task_trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)    13504 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/taskdef.py
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/templatevars.py
--rw-r--r--   0 runner    (1001) docker     (123)    11265 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/terminal.py
--rw-r--r--   0 runner    (1001) docker     (123)    18999 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/time_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 17:09:41.408514 cylc-flow-8.1.2/cylc/flow/tui/
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/tui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18584 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/tui/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/tui/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6956 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/tui/overlay.py
--rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/tui/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)    13257 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/tui/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/unicode_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    10729 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/wallclock.py
--rw-r--r--   0 runner    (1001) docker     (123)    33592 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/workflow_db_mgr.py
--rw-r--r--   0 runner    (1001) docker     (123)    12023 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/workflow_events.py
--rw-r--r--   0 runner    (1001) docker     (123)    69723 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/workflow_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     6650 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/workflow_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    17888 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/xtrigger_mgr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 17:09:41.408514 cylc-flow-8.1.2/cylc/flow/xtriggers/
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/xtriggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/xtriggers/echo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/xtriggers/wall_clock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/xtriggers/workflow_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/cylc/flow/xtriggers/xrandom.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 17:09:41.408514 cylc-flow-8.1.2/cylc_flow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-02-20 17:09:41.000000 cylc-flow-8.1.2/cylc_flow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9254 2023-02-20 17:09:41.000000 cylc-flow-8.1.2/cylc_flow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-20 17:09:41.000000 cylc-flow-8.1.2/cylc_flow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-02-20 17:09:41.000000 cylc-flow-8.1.2/cylc_flow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-02-20 17:09:41.000000 cylc-flow-8.1.2/cylc_flow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-20 17:09:41.000000 cylc-flow-8.1.2/cylc_flow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-02-20 17:09:41.408514 cylc-flow-8.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-02-20 17:09:36.000000 cylc-flow-8.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.439959 cylc-flow-8.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-04-28 11:30:58.439959 cylc-flow-8.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.411959 cylc-flow-8.1.3/cylc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.423959 cylc-flow-8.1.3/cylc/flow/
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14818 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/async_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17180 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/broadcast_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/broadcast_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/c3mro.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.423959 cylc-flow-8.1.3/cylc/flow/cfgspec/
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/cfgspec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/cfgspec/glbl_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71511 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/cfgspec/globalcfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83023 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/cfgspec/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/command_polling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97151 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/context_node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.423959 cylc-flow-8.1.3/cylc/flow/cycling/
+-rw-r--r--   0 runner    (1001) docker     (123)    14593 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/cycling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23211 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/cycling/integer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34957 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/cycling/iso8601.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/cycling/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/cycling/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/cylc_subproc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/daemonize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22194 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/data_messages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89336 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/data_store_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/dbstatecheck.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.423959 cylc-flow-8.1.3/cylc/flow/etc/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7934 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/cylc
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/cylc-completion.bash
+-rw-r--r--   0 runner    (1001) docker     (123)    14460 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/job.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.427959 cylc-flow-8.1.3/cylc/flow/etc/syntax/
+-rw-r--r--   0 runner    (1001) docker     (123)     5210 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/syntax/cylc-mode.el
+-rw-r--r--   0 runner    (1001) docker     (123)    25186 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/syntax/cylc.lang
+-rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/syntax/cylc.vim
+-rw-r--r--   0 runner    (1001) docker     (123)    10612 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/syntax/cylc.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.427959 cylc-flow-8.1.3/cylc/flow/etc/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/api-keys
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.427959 cylc-flow-8.1.3/cylc/flow/etc/tutorial/consolidation-tutorial/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      802 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/consolidation-tutorial/.validate
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.427959 cylc-flow-8.1.3/cylc/flow/etc/tutorial/consolidation-tutorial/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4248 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/consolidation-tutorial/bin/consolidate-observations
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9151 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/consolidation-tutorial/bin/forecast
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7216 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/consolidation-tutorial/bin/get-observations
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6453 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/consolidation-tutorial/bin/get-rainfall
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3721 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/consolidation-tutorial/bin/post-process
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.427959 cylc-flow-8.1.3/cylc/flow/etc/tutorial/consolidation-tutorial/etc/
+-rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/consolidation-tutorial/etc/met-office-sites.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/consolidation-tutorial/etc/python-job.settings
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/consolidation-tutorial/flow.cylc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.411959 cylc-flow-8.1.3/cylc/flow/etc/tutorial/consolidation-tutorial/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.427959 cylc-flow-8.1.3/cylc/flow/etc/tutorial/consolidation-tutorial/lib/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/consolidation-tutorial/lib/python/mercator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10018 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/consolidation-tutorial/lib/python/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.427959 cylc-flow-8.1.3/cylc/flow/etc/tutorial/consolidation-tutorial/lib/template/
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/consolidation-tutorial/lib/template/map.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.427959 cylc-flow-8.1.3/cylc/flow/etc/tutorial/cylc-forecasting-workflow/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1139 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/cylc-forecasting-workflow/.validate
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.427959 cylc-flow-8.1.3/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4248 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/consolidate-observations
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9151 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/forecast
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7216 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/get-observations
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6453 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/get-rainfall
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3721 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/post-process
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.427959 cylc-flow-8.1.3/cylc/flow/etc/tutorial/cylc-forecasting-workflow/etc/
+-rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/cylc-forecasting-workflow/etc/met-office-sites.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/cylc-forecasting-workflow/etc/python-job.settings
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/cylc-forecasting-workflow/flow.cylc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.415959 cylc-flow-8.1.3/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.427959 cylc-flow-8.1.3/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/python/mercator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10018 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/python/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.427959 cylc-flow-8.1.3/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/template/
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/template/map.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.427959 cylc-flow-8.1.3/cylc/flow/etc/tutorial/forecast-script/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9151 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/forecast-script/forecast
+-rw-r--r--   0 runner    (1001) docker     (123)    10018 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/forecast-script/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.427959 cylc-flow-8.1.3/cylc/flow/etc/tutorial/inheritance-tutorial/
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/inheritance-tutorial/flow.cylc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.427959 cylc-flow-8.1.3/cylc/flow/etc/tutorial/map-template/
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/map-template/map-template.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.415959 cylc-flow-8.1.3/cylc/flow/etc/tutorial/message-trigger-tutorial/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.427959 cylc-flow-8.1.3/cylc/flow/etc/tutorial/message-trigger-tutorial/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      180 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/message-trigger-tutorial/bin/random.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.427959 cylc-flow-8.1.3/cylc/flow/etc/tutorial/retries-tutorial/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      819 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/retries-tutorial/.validate
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/retries-tutorial/flow.cylc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.427959 cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-introduction/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1125 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-introduction/.validate
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.427959 cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-introduction/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      459 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-introduction/bin/get-observations
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.427959 cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-introduction/etc/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-introduction/etc/python-job.settings
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-introduction/flow.cylc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.427959 cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-tutorial/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.427959 cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-tutorial/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4248 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-tutorial/bin/consolidate-observations
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9151 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-tutorial/bin/forecast
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7216 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-tutorial/bin/get-observations
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6453 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-tutorial/bin/get-rainfall
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3721 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-tutorial/bin/post-process
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.427959 cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-tutorial/etc/
+-rw-r--r--   0 runner    (1001) docker     (123)     7485 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-tutorial/etc/met-office-sites.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-tutorial/etc/python-job.settings
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-tutorial/flow.cylc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.415959 cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-tutorial/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.431959 cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-tutorial/lib/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-tutorial/lib/python/mercator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10018 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-tutorial/lib/python/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.431959 cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-tutorial/lib/template/
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-tutorial/lib/template/map.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-tutorial/runtime
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.431959 cylc-flow-8.1.3/cylc/flow/etc/tutorial/test-data/
+-rw-r--r--   0 runner    (1001) docker     (123)    33085 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/test-data/rainfall.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    35829 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/test-data/wind_20171101T0000Z_x.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    38004 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/etc/tutorial/test-data/wind_20171101T0000Z_y.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    14030 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/flow_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35572 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/graph_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/graphnode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18192 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/host_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/hostuserutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24245 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/id.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17477 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/id_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/id_match.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.431959 cylc-flow-8.1.3/cylc/flow/install_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/install_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10942 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/install_plugins/log_vc_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.415959 cylc-flow-8.1.3/cylc/flow/jinja/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.431959 cylc-flow-8.1.3/cylc/flow/jinja/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/jinja/filters/duration_as.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/jinja/filters/pad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/jinja/filters/strftime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14670 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/job_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.431959 cylc-flow-8.1.3/cylc/flow/job_runner_handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/job_runner_handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/job_runner_handlers/at.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/job_runner_handlers/background.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12788 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/job_runner_handlers/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/job_runner_handlers/loadleveler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/job_runner_handlers/lsf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/job_runner_handlers/moab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4358 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/job_runner_handlers/pbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/job_runner_handlers/pbs_multi_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/job_runner_handlers/sge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6413 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/job_runner_handlers/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/job_runner_handlers/slurm_packjob.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33912 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/job_runner_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/listify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/log_diagnosis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15363 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/loggingutil.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.431959 cylc-flow-8.1.3/cylc/flow/main_loop/
+-rw-r--r--   0 runner    (1001) docker     (123)    10622 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/main_loop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9564 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/main_loop/auto_restart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/main_loop/health_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/main_loop/log_data_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/main_loop/log_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/main_loop/log_main_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/main_loop/log_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/main_loop/reset_bad_hosts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.431959 cylc-flow-8.1.3/cylc/flow/network/
+-rw-r--r--   0 runner    (1001) docker     (123)     9902 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/network/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/network/authorisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11918 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/network/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/network/client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16257 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/network/graphql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/network/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/network/publisher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/network/replier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30538 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/network/resolvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16389 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/network/scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74542 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/network/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14723 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/network/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/network/ssh_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/network/subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28587 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/option_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15646 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/param_expand.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.435959 cylc-flow-8.1.3/cylc/flow/parsec/
+-rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/parsec/OrderedDict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/parsec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10823 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/parsec/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/parsec/empysupport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/parsec/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21394 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/parsec/fileparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/parsec/include.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11240 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/parsec/jinja2support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9056 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/parsec/upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14533 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/parsec/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40452 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/parsec/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17225 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/pathutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25192 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/platforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/prerequisite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/print_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    13757 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6932 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39289 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/rundb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80364 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20200 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scheduler_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.439959 cylc-flow-8.1.3/cylc/flow/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15346 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/broadcast.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19658 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/cat_log.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5028 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/check_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/clean.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2617 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20478 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/completion_server.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6429 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8931 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/cycle_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21083 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/cylc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6042 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/diff.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8083 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/dump.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4425 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/ext_trigger.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1491 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/function_run.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2514 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/get_resources.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1871 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/get_workflow_contact.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2311 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/get_workflow_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14884 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/graph.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4378 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/hold.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10639 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/install.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1722 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/jobs_kill.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1697 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/jobs_poll.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2846 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/jobs_submit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2483 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/kill.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24919 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/lint.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6228 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/list.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6419 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/pause.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3955 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/ping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/play.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2548 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/psutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12227 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/reinstall.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3711 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/release.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3254 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/reload.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2108 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/remote_init.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1533 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/remote_tidy.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2225 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/remove.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13206 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/report_timings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15753 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/scan.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3504 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/set_outputs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2536 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/set_verbosity.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12679 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/show.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8360 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/stop.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3658 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/subscribe.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5272 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/tui.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6321 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/validate_install_play.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/validate_reinstall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/view.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10001 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/scripts/workflow_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6439 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/subprocctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23404 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/subprocpool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/task_action_timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63362 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/task_events_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/task_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/task_job_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55110 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/task_job_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6885 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/task_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7701 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/task_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80010 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/task_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18451 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/task_proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.439959 cylc-flow-8.1.3/cylc/flow/task_queues/
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/task_queues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/task_queues/independent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6752 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/task_remote_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25327 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/task_remote_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18423 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/task_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/task_state_prop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10786 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/task_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14482 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/taskdef.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/templatevars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11265 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18999 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/time_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.439959 cylc-flow-8.1.3/cylc/flow/tui/
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/tui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18584 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/tui/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/tui/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6956 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/tui/overlay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/tui/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13257 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/tui/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/unicode_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10729 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/wallclock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33592 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/workflow_db_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12023 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/workflow_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69723 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/workflow_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6650 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/workflow_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17888 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/xtrigger_mgr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.439959 cylc-flow-8.1.3/cylc/flow/xtriggers/
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/xtriggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/xtriggers/echo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/xtriggers/wall_clock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/xtriggers/workflow_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/cylc/flow/xtriggers/xrandom.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:30:58.439959 cylc-flow-8.1.3/cylc_flow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-04-28 11:30:58.000000 cylc-flow-8.1.3/cylc_flow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9301 2023-04-28 11:30:58.000000 cylc-flow-8.1.3/cylc_flow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 11:30:58.000000 cylc-flow-8.1.3/cylc_flow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-04-28 11:30:58.000000 cylc-flow-8.1.3/cylc_flow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-04-28 11:30:58.000000 cylc-flow-8.1.3/cylc_flow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-28 11:30:58.000000 cylc-flow-8.1.3/cylc_flow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-04-28 11:30:58.443959 cylc-flow-8.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-28 11:30:54.000000 cylc-flow-8.1.3/setup.py
```

### Comparing `cylc-flow-8.1.2/COPYING` & `cylc-flow-8.1.3/COPYING`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/PKG-INFO` & `cylc-flow-8.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cylc-flow
-Version: 8.1.2
+Version: 8.1.3
 Summary: A workflow engine for cycling systems
 Home-page: https://cylc.org/
 Author: Hilary Oliver
 License: GPL
 Project-URL: Documentation, https://cylc.github.io/cylc-doc/stable/html/index.html
 Project-URL: Source, https://github.com/cylc/cylc-flow
 Project-URL: Tracker, https://github.com/cylc/cylc-flow/issues
```

### Comparing `cylc-flow-8.1.2/README.md` & `cylc-flow-8.1.3/README.md`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/__init__.py` & `cylc-flow-8.1.3/cylc/flow/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,35 +22,35 @@
 CYLC_LOG = 'cylc'
 
 LOG = logging.getLogger(CYLC_LOG)
 # Start with a null handler
 LOG.addHandler(logging.NullHandler())
 
 LOG_LEVELS = {
+    "DEBUG": logging.DEBUG,
     "INFO": logging.INFO,
     "NORMAL": logging.INFO,
     "WARNING": logging.WARNING,
     "ERROR": logging.ERROR,
     "CRITICAL": logging.CRITICAL,
-    "DEBUG": logging.DEBUG,
 }
 
 
 def environ_init():
     """Initialise cylc environment."""
     # Python output buffering delays appearance of stdout and stderr
     # when output is not directed to a terminal (this occurred when
     # running pre-5.0 cylc via the posix nohup command; is it still the
     # case in post-5.0 daemon-mode cylc?)
     os.environ['PYTHONUNBUFFERED'] = 'true'
 
 
 environ_init()
 
-__version__ = '8.1.2'
+__version__ = '8.1.3'
 
 
 def iter_entry_points(entry_point_name):
     """Iterate over Cylc entry points."""
     import pkg_resources
     yield from (
         entry_point
```

### Comparing `cylc-flow-8.1.2/cylc/flow/async_util.py` & `cylc-flow-8.1.3/cylc/flow/async_util.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/broadcast_mgr.py` & `cylc-flow-8.1.3/cylc/flow/broadcast_mgr.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/broadcast_report.py` & `cylc-flow-8.1.3/cylc/flow/broadcast_report.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/c3mro.py` & `cylc-flow-8.1.3/cylc/flow/c3mro.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/cfgspec/__init__.py` & `cylc-flow-8.1.3/cylc/flow/cfgspec/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/cfgspec/glbl_cfg.py` & `cylc-flow-8.1.3/cylc/flow/cfgspec/glbl_cfg.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/cfgspec/globalcfg.py` & `cylc-flow-8.1.3/cylc/flow/cfgspec/globalcfg.py`

 * *Files 1% similar despite different names*

```diff
@@ -1422,15 +1422,16 @@
 
                    {REPLACES}``global.rc[hosts][<host>]retrieve job logs
                    retry delays``.
                    {PLATFORM_REPLACES.format(
                        "[remote]retrieve job logs retry delays")}
             ''')
             Conf('tail command template',
-                 VDR.V_STRING, 'tail -n +1 -F %(filename)s', desc=f'''
+                 VDR.V_STRING, 'tail -n +1 --follow=name -F %(filename)s',
+                 desc=f'''
                 A command template (with ``%(filename)s`` substitution) to
                 tail-follow job logs this platform, by ``cylc cat-log``.
 
                 You are are unlikely to need to override this.
 
                 .. versionchanged:: 8.0.0
```

### Comparing `cylc-flow-8.1.2/cylc/flow/cfgspec/workflow.py` & `cylc-flow-8.1.3/cylc/flow/cfgspec/workflow.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/command_polling.py` & `cylc-flow-8.1.3/cylc/flow/command_polling.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/config.py` & `cylc-flow-8.1.3/cylc/flow/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -352,21 +352,14 @@
             parameter_values = {}
         try:
             parameter_templates = self.cfg['task parameters']['templates']
 
         except KeyError:
             parameter_templates = {}
 
-        # Check that parameter templates are a section
-        if not hasattr(parameter_templates, 'update'):
-            raise WorkflowConfigError(
-                '[task parameters][templates] is a section. Don\'t use it '
-                'as a parameter.'
-            )
-
         # parameter values and templates are normally needed together.
         self.parameters = (parameter_values, parameter_templates)
 
         LOG.debug("Expanding [runtime] namespace lists and parameters")
 
         # Set default parameter expansion templates if necessary.
         for pname, pvalues in parameter_values.items():
```

### Comparing `cylc-flow-8.1.2/cylc/flow/context_node.py` & `cylc-flow-8.1.3/cylc/flow/context_node.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/cycling/__init__.py` & `cylc-flow-8.1.3/cylc/flow/cycling/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/cycling/integer.py` & `cylc-flow-8.1.3/cylc/flow/cycling/integer.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/cycling/iso8601.py` & `cylc-flow-8.1.3/cylc/flow/cycling/iso8601.py`

 * *Files 0% similar despite different names*

```diff
@@ -851,14 +851,15 @@
     (WorkflowSpecifics.point_parser,
      WorkflowSpecifics.interval_parser,
      WorkflowSpecifics.recurrence_parser) = WorkflowSpecifics.iso8601_parsers
 
     WorkflowSpecifics.abbrev_util = CylcTimeParser(
         None, None, WorkflowSpecifics.iso8601_parsers
     )
+    return WorkflowSpecifics
 
 
 def get_dump_format():
     """Return cycle point string dump format."""
     return WorkflowSpecifics.DUMP_FORMAT
```

### Comparing `cylc-flow-8.1.2/cylc/flow/cycling/loader.py` & `cylc-flow-8.1.3/cylc/flow/cycling/loader.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/cycling/util.py` & `cylc-flow-8.1.3/cylc/flow/cycling/util.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/cylc_subproc.py` & `cylc-flow-8.1.3/cylc/flow/cylc_subproc.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/daemonize.py` & `cylc-flow-8.1.3/cylc/flow/daemonize.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/data_messages_pb2.py` & `cylc-flow-8.1.3/cylc/flow/data_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/data_store_mgr.py` & `cylc-flow-8.1.3/cylc/flow/data_store_mgr.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,14 +176,49 @@
     JOBS: {'messages'},
     TASKS: set(),
     TASK_PROXIES: {'prerequisites'},
     WORKFLOW: {'latest_state_tasks', 'state_totals', 'states'},
 }
 
 
+def setbuff(obj, key, value):
+    """Set an attribute on a protobuf object.
+
+    Although `None` is a valid value for an `optional` field in protobuf e.g:
+
+       >>> job = PbJob(job_id=None)
+
+    Attempting to set a field to none after initiation results in error:
+
+       >>> job.job_id = None
+       Traceback (most recent call last):
+       TypeError: ...
+
+    For safety this method only sets the attribute if the value is not None.
+
+    Note:
+        If the above doctest fails, then the behaviour of protobuf has changed
+        and this wrapper might not be necessary any more.
+
+    See:
+        https://github.com/cylc/cylc-flow/issues/5388
+
+    Example:
+        >>> from types import SimpleNamespace
+        >>> obj = SimpleNamespace()
+        >>> setbuff(obj, 'a', 1); obj
+        namespace(a=1)
+        >>> setbuff(obj, 'b', None); obj
+        namespace(a=1)
+
+    """
+    if value is not None:
+        setattr(obj, key, value)
+
+
 def generate_checksum(in_strings):
     """Generate cross platform & python checksum from strings."""
     # can't use hash(), it's not the same across 32-64bit or python invocations
     return zlib.adler32(''.join(sorted(in_strings)).encode()) & 0xffffffff
 
 
 def task_mean_elapsed_time(tdef):
@@ -542,15 +577,15 @@
                 depth=len(ancestors[name]) - 1,
             )
             task.namespace[:] = tdef.namespace_hierarchy
             task.first_parent = self.definition_id(ancestors[name][1])
             user_defined_meta = {}
             for key, val in dict(tdef.describe()).items():
                 if key in ['title', 'description', 'URL']:
-                    setattr(task.meta, key, val)
+                    setbuff(task.meta, key, val)
                 else:
                     user_defined_meta[key] = val
             task.meta.user_defined = json.dumps(user_defined_meta)
             elapsed_time = task_mean_elapsed_time(tdef)
             if elapsed_time:
                 task.mean_elapsed_time = elapsed_time
             task.parents.extend([
@@ -577,15 +612,15 @@
                     name=name,
                     depth=len(ancestors[name]) - 1,
                 )
                 famcfg = config.cfg['runtime'][name]
                 user_defined_meta = {}
                 for key, val in famcfg.get('meta', {}).items():
                     if key in ['title', 'description', 'URL']:
-                        setattr(family.meta, key, val)
+                        setbuff(family.meta, key, val)
                     else:
                         user_defined_meta[key] = val
                 family.meta.user_defined = json.dumps(user_defined_meta)
                 family.parents.extend(
                     self.definition_id(p_name)
                     for p_name in parents[name]
                 )
@@ -615,29 +650,29 @@
         workflow.owner = self.schd.owner
         workflow.host = self.schd.host
         workflow.port = self.schd.server.port or -1
         workflow.pub_port = self.schd.server.pub_port or -1
         user_defined_meta = {}
         for key, val in config.cfg['meta'].items():
             if key in ['title', 'description', 'URL']:
-                setattr(workflow.meta, key, val)
+                setbuff(workflow.meta, key, val)
             else:
                 user_defined_meta[key] = val
         workflow.meta.user_defined = json.dumps(user_defined_meta)
         workflow.tree_depth = max([
             len(val)
             for val in config.get_first_parent_ancestors(pruned=True).values()
         ]) - 1
 
         if get_utc_mode():
             time_zone_info = TIME_ZONE_UTC_INFO
         else:
             time_zone_info = TIME_ZONE_LOCAL_INFO
         for key, val in time_zone_info.items():
-            setattr(workflow.time_zone_info, key, val)
+            setbuff(workflow.time_zone_info, key, val)
 
         workflow.run_mode = config.run_mode()
         workflow.cycling_mode = config.cfg['scheduling']['cycling mode']
         workflow.workflow_log_dir = self.schd.workflow_log_dir
         workflow.job_log_names.extend(list(JOB_LOG_OPTS.values()))
         workflow.ns_def_order.extend(config.ns_defn_order)
 
@@ -686,28 +721,29 @@
                 Active/Other task proxy, passed in with pool invocation.
 
         Returns:
 
             None
 
         """
+        is_active = not (descendant or is_parent)
         # ID passed through recursion as reference to original/active node.
         if active_id is None:
             source_tokens = self.id_.duplicate(source_tokens)
             active_id = source_tokens.id
 
         # flag manual triggers for pruning on deletion.
         if is_manual_submit:
             self.prune_trigger_nodes.setdefault(active_id, set()).add(
                 source_tokens.id
             )
 
         # Setup and check if active node is another's boundary node
         # to flag its paths for pruning.
-        if edge_distance == 0:
+        if is_active:
             self.n_window_edges[active_id] = set()
             self.n_window_boundary_nodes[active_id] = {}
             self.n_window_nodes[active_id] = set()
             if active_id in self.prune_trigger_nodes:
                 self.prune_flagged_nodes.update(
                     self.prune_trigger_nodes[active_id])
                 del self.prune_trigger_nodes[active_id]
@@ -733,89 +769,91 @@
         self.n_window_nodes[active_id].add(source_tokens.id)
 
         edge_distance += 1
 
         # Don't expand window about orphan task.
         if not is_orphan:
             tdef = self.schd.config.taskdefs[source_tokens['task']]
-            if graph_children is None:
-                graph_children = generate_graph_children(tdef, point)
-            if (
-                    (not any(graph_children.values()) and descendant)
-                    or self.n_edge_distance == 0
-            ):
-                self.n_window_boundary_nodes[
-                    active_id
-                ].setdefault(edge_distance - 1, set()).add(source_tokens.id)
-
             # TODO: xtrigger is workflow_state edges too
             # Reference set for workflow relations
             final_point = self.schd.config.final_point
-            if edge_distance == 1:
-                descendant = True
-            # Children/downstream nodes
-            for items in graph_children.values():
-                for child_name, child_point, _ in items:
-                    if child_point > final_point:
-                        continue
-                    child_tokens = self.id_.duplicate(
-                        cycle=str(child_point),
-                        task=child_name,
-                    )
-                    # We still increment the graph one further to find
-                    # boundary nodes, but don't create elements.
-                    if edge_distance <= self.n_edge_distance:
-                        self.generate_edge(
-                            source_tokens,
+            if descendant or is_active:
+                if graph_children is None:
+                    graph_children = generate_graph_children(tdef, point)
+                if not any(graph_children.values()):
+                    self.n_window_boundary_nodes[active_id].setdefault(
+                        edge_distance - 1,
+                        set()
+                    ).add(source_tokens.id)
+
+                # Children/downstream nodes
+                for items in graph_children.values():
+                    for child_name, child_point, _ in items:
+                        if child_point > final_point:
+                            continue
+                        child_tokens = self.id_.duplicate(
+                            cycle=str(child_point),
+                            task=child_name,
+                        )
+                        # We still increment the graph one further to find
+                        # boundary nodes, but don't create elements.
+                        if edge_distance <= self.n_edge_distance:
+                            self.generate_edge(
+                                source_tokens,
+                                child_tokens,
+                                active_id
+                            )
+                        if child_tokens.id in self.n_window_nodes[active_id]:
+                            continue
+                        self.increment_graph_window(
                             child_tokens,
-                            active_id
+                            child_point,
+                            flow_nums,
+                            edge_distance,
+                            active_id,
+                            True,
+                            False
                         )
-                    if child_tokens.id in self.n_window_nodes[active_id]:
-                        continue
-                    self.increment_graph_window(
-                        child_tokens,
-                        child_point,
-                        flow_nums,
-                        edge_distance,
-                        active_id,
-                        descendant,
-                        False
-                    )
 
             # Parents/upstream nodes
-            for items in generate_graph_parents(tdef, point).values():
-                for parent_name, parent_point, _ in items:
-                    if parent_point > final_point:
-                        continue
-                    parent_tokens = self.id_.duplicate(
-                        cycle=str(parent_point),
-                        task=parent_name,
-                    )
-                    if edge_distance <= self.n_edge_distance:
-                        # reverse for parent
-                        self.generate_edge(
+            if is_parent or is_active:
+                for items in generate_graph_parents(
+                    tdef,
+                    point,
+                    self.schd.config.taskdefs
+                ).values():
+                    for parent_name, parent_point, _ in items:
+                        if parent_point > final_point:
+                            continue
+                        parent_tokens = self.id_.duplicate(
+                            cycle=str(parent_point),
+                            task=parent_name,
+                        )
+                        if edge_distance <= self.n_edge_distance:
+                            # reverse for parent
+                            self.generate_edge(
+                                parent_tokens,
+                                source_tokens,
+                                active_id
+                            )
+                        if parent_tokens.id in self.n_window_nodes[active_id]:
+                            continue
+                        self.increment_graph_window(
                             parent_tokens,
-                            source_tokens,
-                            active_id
+                            parent_point,
+                            flow_nums,
+                            edge_distance,
+                            active_id,
+                            False,
+                            True
                         )
-                    if parent_tokens.id in self.n_window_nodes[active_id]:
-                        continue
-                    self.increment_graph_window(
-                        parent_tokens,
-                        parent_point,
-                        flow_nums,
-                        edge_distance,
-                        active_id,
-                        False,
-                        True
-                    )
 
         # If this is the active task (edge_distance has been incremented),
         # then add the most distant child as a trigger to prune it.
-        if edge_distance == 1:
+        if is_active:
             levels = self.n_window_boundary_nodes[active_id].keys()
             # Could be self-reference node foo:failed => foo
             if not levels:
                 self.n_window_boundary_nodes[active_id][0] = {active_id}
                 levels = (0,)
             # Only trigger pruning for furthest set of boundary nodes
             for tp_id in self.n_window_boundary_nodes[active_id][max(levels)]:
@@ -1029,15 +1067,15 @@
             depth=1,
         )
         task.namespace[:] = tdef.namespace_hierarchy
         task.first_parent = self.definition_id('root')
         user_defined_meta = {}
         for key, val in dict(tdef.describe()).items():
             if key in ['title', 'description', 'URL']:
-                setattr(task.meta, key, val)
+                setbuff(task.meta, key, val)
             else:
                 user_defined_meta[key] = val
         task.meta.user_defined = json.dumps(user_defined_meta)
         elapsed_time = task_mean_elapsed_time(tdef)
         if elapsed_time:
             task.mean_elapsed_time = elapsed_time
         task.parents[:] = [task.first_parent]
@@ -1190,15 +1228,20 @@
             ] = satisfied if satisfied != '0' else False
 
         for ikey, prereqs in prereqs_map.items():
             for itask_prereq in (
                     self.db_load_task_proxies[ikey][0].state.prerequisites
             ):
                 for key in itask_prereq.satisfied.keys():
-                    itask_prereq.satisfied[key] = prereqs[key]
+                    try:
+                        itask_prereq.satisfied[key] = prereqs[key]
+                    except KeyError:
+                        # This prereq is not in the DB: new dependencies
+                        # added to an already-spawned task before restart.
+                        itask_prereq.satisfied[key] = False
 
         # Extract info from itasks to data-store.
         for task_info in self.db_load_task_proxies.values():
             self._process_internal_task_proxy(
                 task_info[0],
                 self.added[TASK_PROXIES][
                     self.id_.duplicate(task_info[0].tokens).id
@@ -2153,15 +2196,15 @@
             tokens['task'],
             tokens['cycle'],
             tokens['job'],
         )
         if not job:
             return
         j_delta = PbJob(stamp=f'{j_id}@{time()}')
-        setattr(j_delta, attr_key, attr_val)
+        setbuff(j_delta, attr_key, attr_val)
         self.updated[JOBS].setdefault(
             j_id,
             PbJob(id=j_id)
         ).MergeFrom(j_delta)
         self.updates_pending = True
 
     def delta_job_state(self, job_d, status):
@@ -2195,15 +2238,15 @@
             tokens['cycle'],
             tokens['job'],
         )
         if not job:
             return
         j_delta = PbJob(stamp=f'{j_id}@{time()}')
         time_attr = f'{event_key}_time'
-        setattr(j_delta, time_attr, time_str)
+        setbuff(j_delta, time_attr, time_str)
         self.updated[JOBS].setdefault(
             j_id,
             PbJob(id=j_id)
         ).MergeFrom(j_delta)
         self.updates_pending = True
 
     def store_node_fetcher(
```

### Comparing `cylc-flow-8.1.2/cylc/flow/dbstatecheck.py` & `cylc-flow-8.1.3/cylc/flow/dbstatecheck.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/etc/cylc` & `cylc-flow-8.1.3/cylc/flow/etc/cylc`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/etc/cylc-completion.bash` & `cylc-flow-8.1.3/cylc/flow/etc/cylc-completion.bash`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/etc/job.sh` & `cylc-flow-8.1.3/cylc/flow/etc/job.sh`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/etc/syntax/cylc-mode.el` & `cylc-flow-8.1.3/cylc/flow/etc/syntax/cylc-mode.el`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/etc/syntax/cylc.lang` & `cylc-flow-8.1.3/cylc/flow/etc/syntax/cylc.lang`

 * *Files 0% similar despite different names*

#### Comparing `cylc-flow-8.1.2/cylc/flow/etc/syntax/cylc.lang` & `cylc-flow-8.1.3/cylc/flow/etc/syntax/cylc.lang`

```diff
@@ -6,16 +6,15 @@
  = Instructions =
 
  To use it, place this file in
  ~/.local/share/gtksourceview-2.0/language-specs/ - or, if possible,
  /usr/share/gtksourceview-2.0/language-specs/
 
  If your installation uses GNOME 3, the '2.0' in the paths will need
- to be '3.0', and the version="2.0" string below will need changing
- as well.
+ to be '3.0'.
 
  If using gedit, gedit will need to be totally closed down and reloaded.
 
 
  = Licensing =
 
  Some content taken from sh.lang, which is licensed under GPLv2.
```

### Comparing `cylc-flow-8.1.2/cylc/flow/etc/syntax/cylc.vim` & `cylc-flow-8.1.3/cylc/flow/etc/syntax/cylc.vim`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/etc/syntax/cylc.xml` & `cylc-flow-8.1.3/cylc/flow/etc/syntax/cylc.xml`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/etc/tutorial/consolidation-tutorial/.validate` & `cylc-flow-8.1.3/cylc/flow/etc/tutorial/consolidation-tutorial/.validate`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/etc/tutorial/consolidation-tutorial/bin/consolidate-observations` & `cylc-flow-8.1.3/cylc/flow/etc/tutorial/consolidation-tutorial/bin/consolidate-observations`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/etc/tutorial/consolidation-tutorial/bin/forecast` & `cylc-flow-8.1.3/cylc/flow/etc/tutorial/consolidation-tutorial/bin/forecast`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/etc/tutorial/consolidation-tutorial/bin/get-observations` & `cylc-flow-8.1.3/cylc/flow/etc/tutorial/consolidation-tutorial/bin/get-observations`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/etc/tutorial/consolidation-tutorial/bin/get-rainfall` & `cylc-flow-8.1.3/cylc/flow/etc/tutorial/consolidation-tutorial/bin/get-rainfall`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/etc/tutorial/consolidation-tutorial/bin/post-process` & `cylc-flow-8.1.3/cylc/flow/etc/tutorial/consolidation-tutorial/bin/post-process`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/etc/tutorial/consolidation-tutorial/etc/met-office-sites.dat` & `cylc-flow-8.1.3/cylc/flow/etc/tutorial/consolidation-tutorial/etc/met-office-sites.dat`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/etc/tutorial/consolidation-tutorial/flow.cylc` & `cylc-flow-8.1.3/cylc/flow/etc/tutorial/consolidation-tutorial/flow.cylc`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/etc/tutorial/consolidation-tutorial/lib/python/mercator.py` & `cylc-flow-8.1.3/cylc/flow/etc/tutorial/consolidation-tutorial/lib/python/mercator.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/etc/tutorial/consolidation-tutorial/lib/python/util.py` & `cylc-flow-8.1.3/cylc/flow/etc/tutorial/consolidation-tutorial/lib/python/util.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/etc/tutorial/consolidation-tutorial/lib/template/map.html` & `cylc-flow-8.1.3/cylc/flow/etc/tutorial/consolidation-tutorial/lib/template/map.html`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/etc/tutorial/cylc-forecasting-workflow/.validate` & `cylc-flow-8.1.3/cylc/flow/etc/tutorial/cylc-forecasting-workflow/.validate`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/consolidate-observations` & `cylc-flow-8.1.3/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/consolidate-observations`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/forecast` & `cylc-flow-8.1.3/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/forecast`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/get-observations` & `cylc-flow-8.1.3/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/get-observations`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/get-rainfall` & `cylc-flow-8.1.3/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/get-rainfall`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/post-process` & `cylc-flow-8.1.3/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/post-process`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/etc/tutorial/cylc-forecasting-workflow/etc/met-office-sites.dat` & `cylc-flow-8.1.3/cylc/flow/etc/tutorial/cylc-forecasting-workflow/etc/met-office-sites.dat`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/etc/tutorial/cylc-forecasting-workflow/flow.cylc` & `cylc-flow-8.1.3/cylc/flow/etc/tutorial/cylc-forecasting-workflow/flow.cylc`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/python/mercator.py` & `cylc-flow-8.1.3/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/python/mercator.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/python/util.py` & `cylc-flow-8.1.3/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/python/util.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/template/map.html` & `cylc-flow-8.1.3/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/template/map.html`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/etc/tutorial/forecast-script/forecast` & `cylc-flow-8.1.3/cylc/flow/etc/tutorial/forecast-script/forecast`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/etc/tutorial/forecast-script/util.py` & `cylc-flow-8.1.3/cylc/flow/etc/tutorial/forecast-script/util.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/etc/tutorial/inheritance-tutorial/flow.cylc` & `cylc-flow-8.1.3/cylc/flow/etc/tutorial/inheritance-tutorial/flow.cylc`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/etc/tutorial/map-template/map-template.html` & `cylc-flow-8.1.3/cylc/flow/etc/tutorial/map-template/map-template.html`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/etc/tutorial/retries-tutorial/.validate` & `cylc-flow-8.1.3/cylc/flow/etc/tutorial/retries-tutorial/.validate`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/etc/tutorial/runtime-introduction/.validate` & `cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-introduction/.validate`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/etc/tutorial/runtime-introduction/flow.cylc` & `cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-introduction/flow.cylc`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/etc/tutorial/runtime-tutorial/bin/consolidate-observations` & `cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-tutorial/bin/consolidate-observations`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/etc/tutorial/runtime-tutorial/bin/forecast` & `cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-tutorial/bin/forecast`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/etc/tutorial/runtime-tutorial/bin/get-observations` & `cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-tutorial/bin/get-observations`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/etc/tutorial/runtime-tutorial/bin/get-rainfall` & `cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-tutorial/bin/get-rainfall`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/etc/tutorial/runtime-tutorial/bin/post-process` & `cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-tutorial/bin/post-process`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/etc/tutorial/runtime-tutorial/etc/met-office-sites.dat` & `cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-tutorial/etc/met-office-sites.dat`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/etc/tutorial/runtime-tutorial/flow.cylc` & `cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-tutorial/flow.cylc`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/etc/tutorial/runtime-tutorial/lib/python/mercator.py` & `cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-tutorial/lib/python/mercator.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/etc/tutorial/runtime-tutorial/lib/python/util.py` & `cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-tutorial/lib/python/util.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/etc/tutorial/runtime-tutorial/lib/template/map.html` & `cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-tutorial/lib/template/map.html`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/etc/tutorial/runtime-tutorial/runtime` & `cylc-flow-8.1.3/cylc/flow/etc/tutorial/runtime-tutorial/runtime`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/etc/tutorial/test-data/rainfall.csv` & `cylc-flow-8.1.3/cylc/flow/etc/tutorial/test-data/rainfall.csv`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/etc/tutorial/test-data/wind_20171101T0000Z_x.csv` & `cylc-flow-8.1.3/cylc/flow/etc/tutorial/test-data/wind_20171101T0000Z_x.csv`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/etc/tutorial/test-data/wind_20171101T0000Z_y.csv` & `cylc-flow-8.1.3/cylc/flow/etc/tutorial/test-data/wind_20171101T0000Z_y.csv`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/exceptions.py` & `cylc-flow-8.1.3/cylc/flow/exceptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """Exceptions for "expected" errors."""
 
 import errno
 from textwrap import wrap
 from typing import (
     Callable,
+    Dict,
     Iterable,
     NoReturn,
     Optional,
     Tuple,
     Type,
     Union,
 )
@@ -362,19 +363,18 @@
     """Unable to determine the correct job platform from the information
     given"""
 
 
 class HostSelectException(CylcError):
     """No hosts could be selected from the provided configuration."""
 
-    def __init__(self, data):
+    def __init__(self, data: Dict[str, dict]):
         self.data = data
-        CylcError.__init__(self)
 
-    def __str__(self):
+    def __str__(self) -> str:
         ret = 'Could not select host from:'
         for host, data in sorted(self.data.items()):
             if host != 'ranking':
                 ret += f'\n    {host}:'
                 for key, value in data.items():
                     ret += f'\n        {key}: {value}'
         hint = self.get_hint()
@@ -426,28 +426,43 @@
         return None
 
 
 class NoHostsError(CylcError):
     """None of the hosts of a given platform were reachable."""
     def __init__(self, platform):
         self.platform_name = platform['name']
-        super().__init__()
 
     def __str__(self):
         return f'Unable to find valid host for {self.platform_name}'
 
 
-class NoPlatformsError(CylcError):
-    """None of the platforms of a given group were reachable."""
-    def __init__(self, platform_group):
-        self.platform_group = platform_group
-        super().__init__()
+class NoPlatformsError(PlatformLookupError):
+    """None of the platforms of a given set were reachable.
+
+    Args:
+        identity: The name of the platform group or install target
+        set_type: Whether the set of platforms is a platform group or an
+            install target
+        place: Where the attempt to get the platform failed.
+    """
+    def __init__(
+        self, identity: str, set_type: str = 'group', place: str = ''
+    ):
+        self.identity = identity
+        self.type = set_type
+        if place:
+            self.place = f' during {place}.'
+        else:
+            self.place = '.'
 
     def __str__(self):
-        return f'Unable to find a platform from group {self.platform_group}.'
+        return (
+            f'Unable to find a platform from {self.type} {self.identity}'
+            f'{self.place}'
+        )
 
 
 class CylcVersionError(CylcError):
     """Contact file is for a Cylc Version not supported by this script."""
     def __init__(self, version=None):
         self.version = version
```

### Comparing `cylc-flow-8.1.2/cylc/flow/flags.py` & `cylc-flow-8.1.3/cylc/flow/flags.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/flow_mgr.py` & `cylc-flow-8.1.3/cylc/flow/flow_mgr.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/graph_parser.py` & `cylc-flow-8.1.3/cylc/flow/graph_parser.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/graphnode.py` & `cylc-flow-8.1.3/cylc/flow/graphnode.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/host_select.py` & `cylc-flow-8.1.3/cylc/flow/host_select.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/hostuserutil.py` & `cylc-flow-8.1.3/cylc/flow/hostuserutil.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,16 +193,16 @@
         """Return True if name has different IP address than the current host.
 
         Return False if name is None.
         Return True if host is unknown.
 
         """
         if name not in self._remote_hosts:
-            if not name or name.split(".")[0].startswith("localhost"):
-                # e.g. localhost.localdomain
+            if not name or name.startswith("localhost"):
+                # e.g. localhost4.localdomain4
                 self._remote_hosts[name] = False
             else:
                 try:
                     host_info = self._get_host_info(name)
                 except IOError:
                     self._remote_hosts[name] = True
                 else:
```

### Comparing `cylc-flow-8.1.2/cylc/flow/id.py` & `cylc-flow-8.1.3/cylc/flow/id.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/id_cli.py` & `cylc-flow-8.1.3/cylc/flow/id_cli.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/id_match.py` & `cylc-flow-8.1.3/cylc/flow/id_match.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/install_plugins/__init__.py` & `cylc-flow-8.1.3/cylc/flow/install_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/install_plugins/log_vc_info.py` & `cylc-flow-8.1.3/cylc/flow/install_plugins/log_vc_info.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/jinja/filters/duration_as.py` & `cylc-flow-8.1.3/cylc/flow/jinja/filters/duration_as.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/jinja/filters/pad.py` & `cylc-flow-8.1.3/cylc/flow/jinja/filters/pad.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/jinja/filters/strftime.py` & `cylc-flow-8.1.3/cylc/flow/jinja/filters/strftime.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/job_file.py` & `cylc-flow-8.1.3/cylc/flow/job_file.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/job_runner_handlers/__init__.py` & `cylc-flow-8.1.3/cylc/flow/job_runner_handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/job_runner_handlers/at.py` & `cylc-flow-8.1.3/cylc/flow/job_runner_handlers/at.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/job_runner_handlers/background.py` & `cylc-flow-8.1.3/cylc/flow/job_runner_handlers/background.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/job_runner_handlers/loadleveler.py` & `cylc-flow-8.1.3/cylc/flow/job_runner_handlers/loadleveler.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/job_runner_handlers/lsf.py` & `cylc-flow-8.1.3/cylc/flow/job_runner_handlers/lsf.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/job_runner_handlers/moab.py` & `cylc-flow-8.1.3/cylc/flow/job_runner_handlers/moab.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/job_runner_handlers/pbs.py` & `cylc-flow-8.1.3/cylc/flow/job_runner_handlers/pbs.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,18 @@
         # Change task/runM to task-runM in the job name
         # (PBS 19.2.1+ does not allow '/' in job names)
         tokens = Tokens(job_conf['task_id'], relative=True)
         directives["-N"] = (
             f'{tokens["task"]}.{tokens["cycle"]}'
             f".{job_conf['workflow_name'].replace('/', '-')}"
         )
-        job_name_len_max = job_conf['platform']["job name length maximum"]
+        job_name_len_max = job_conf['platform'].get(
+            "job name length maximum",
+            self.JOB_NAME_LEN_MAX
+        )
         if job_name_len_max:
             directives["-N"] = directives["-N"][0:job_name_len_max]
 
         directives["-o"] = job_file_path + ".out"
         directives["-e"] = job_file_path + ".err"
         if (job_conf["execution_time_limit"] and
                 directives.get("-l walltime") is None):
```

### Comparing `cylc-flow-8.1.2/cylc/flow/job_runner_handlers/pbs_multi_cluster.py` & `cylc-flow-8.1.3/cylc/flow/job_runner_handlers/pbs_multi_cluster.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/job_runner_handlers/sge.py` & `cylc-flow-8.1.3/cylc/flow/job_runner_handlers/sge.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/job_runner_handlers/slurm.py` & `cylc-flow-8.1.3/cylc/flow/job_runner_handlers/slurm.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/job_runner_handlers/slurm_packjob.py` & `cylc-flow-8.1.3/cylc/flow/job_runner_handlers/slurm_packjob.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/job_runner_mgr.py` & `cylc-flow-8.1.3/cylc/flow/job_runner_mgr.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,108 +12,18 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 """Manage submission, poll and kill of a job to the job runners.
 
-Export the JobRunnerManager class.
+The job runner interface is documented in
+cylc.flow.job_runner_handlers.documentation.
 
-Job runner handler (a.k.a. job submission method) modules should be placed
-under the "cylc.flow.job_runner_handlers" package. Each module should export
-the symbol "JOB_RUNNER_HANDLER" for the singleton instance that implements the
-job system handler logic.
-
-Each job runner handler class should instantiate with no argument, and may
-have the following constants and methods:
-
-job_runner.filter_poll_many_output(out) => job_ids
-    * Called after the job runner's poll many command. The method should read
-      the output and return a list of job IDs that are still in the
-      job runner.
-
-job_runner.filter_submit_output(out, err) => new_out, new_err
-    * Filter the standard output and standard error of the job submission
-      command. This is useful if the job submission command returns information
-      that should just be ignored. See also "job_runner.SUBMIT_CMD_TMPL".
-
-job_runner.format_directives(job_conf) => lines
-    * If relevant, this method formats the job directives for a job file, if
-      job file directives are relevant for the job runner. The argument
-      "job_conf" is a dict containing the job configuration.
-
-job_runner.get_poll_many_cmd(job-id-list) => list
-    * Return a list containing the shell command to poll the jobs in the
-      argument list.
-
-job_runner.get_submit_stdin(job_file_path: str, submit_opts: dict) => tuple
-    * Return a 2-element tuple `(proc_stdin_arg, proc_stdin_value)`.
-      Element 1 is suitable for the `stdin=...` argument of `subprocess.Popen`
-      so it can be a file handle, `subprocess.PIPE` or `None`. Element 2 is the
-      string content to pipe to STDIN of the submit command (relevant only if
-      `proc_stdin_arg` is `subprocess.PIPE`.
-
-job_runner.get_vacation_signal(job_conf) => str
-    * If relevant, return a string containing the name of the signal that
-      indicates the job has been vacated by the job runner.
-
-job_runner.submit(job_file_path, submit_opts) => ret_code, out, err
-    * Submit a job and return an instance of the Popen object for the
-      submission. This method is useful if the job submission requires logic
-      beyond just running a system or shell command. See also
-      "job_runner.SUBMIT_CMD". You must pass "env=submit_opts.get('env')" to
-      Popen - see background.py for example.
-
-job_runner.manip_job_id(job_id) => job_id
-    * Modify the job ID that is returned by the job submit command.
-
-job_runner.FAIL_SIGNALS => tuple<str>
-    * A tuple containing the names of signals to trap for reporting errors.
-      Default is ("EXIT", "ERR", "TERM", "XCPU"). ERR and EXIT are always
-      recommended.  EXIT is used to report premature stopping of the job
-      script, and its trap is unset at the end of the script.
-
-job_runner.KILL_CMD_TMPL
-    *  A Python string template for getting the job runner command to remove
-       and terminate a job ID. The command is formed using the logic:
-           job_runner.KILL_CMD_TMPL % {"job_id": job_id}
-
-job_runner.POLL_CANT_CONNECT_ERR
-    * A string containing an error message. If this is defined, when a poll
-      command returns a non-zero return code and its STDERR contains this
-      string, then the poll result will not be trusted, because it is assumed
-      that the job runner is currently unavailable. Jobs submitted to the
-      job runner will be assumed OK until we are able to connect to the
-      job runner again.
-
-job_runner.SHOULD_KILL_PROC_GROUP
-    * A boolean to indicate whether it is necessary to kill a job by sending
-      a signal to its Unix process group. This boolean also indicates that
-      a job submitted via this job runner will physically run on the same
-      host it is submitted to.
-
-job_runner.SHOULD_POLL_PROC_GROUP
-    * A boolean to indicate whether it is necessary to poll a job by its PID
-      as well as the job ID.
-
-job_runner.REC_ID_FROM_SUBMIT_ERR
-job_runner.REC_ID_FROM_SUBMIT_OUT
-    * A regular expression (compiled) to extract the job "id" from the standard
-      output or standard error of the job submission command.
-
-job_runner.SUBMIT_CMD_ENV
-    * A Python dict (or an iterable that can be used to update a dict)
-      containing extra environment variables for getting the job runner
-      command to submit a job file.
-
-job_runner.SUBMIT_CMD_TMPL
-    * A Python string template for getting the job runner command to submit a
-      job file. The command is formed using the logic:
-          job_runner.SUBMIT_CMD_TMPL % {"job": job_file_path}
-      See also "job_runner._job_submit_impl".
+Please update this file as the interface changes.
 
 """
 
 from contextlib import suppress
 import json
 import os
 from pathlib import Path
```

### Comparing `cylc-flow-8.1.2/cylc/flow/listify.py` & `cylc-flow-8.1.3/cylc/flow/listify.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/log_diagnosis.py` & `cylc-flow-8.1.3/cylc/flow/log_diagnosis.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/loggingutil.py` & `cylc-flow-8.1.3/cylc/flow/loggingutil.py`

 * *Files 1% similar despite different names*

```diff
@@ -349,15 +349,15 @@
     Args:
         logger: The logger to modify.
         stderr_handler: The existing stderr stream handler.
     """
     stdout_handler = logging.StreamHandler(sys.stdout)
     stdout_handler.setLevel(logging.DEBUG)
     # Filter out >= warnings from stdout
-    stdout_handler.addFilter(lambda rec: int(rec.levelno < logging.WARNING))
+    stdout_handler.addFilter(lambda rec: rec.levelno < logging.WARNING)
     if stderr_handler.formatter:
         stdout_handler.setFormatter(stderr_handler.formatter)
     logger.addHandler(stdout_handler)
 
     stderr_handler.setLevel(logging.WARNING)
```

### Comparing `cylc-flow-8.1.2/cylc/flow/main_loop/__init__.py` & `cylc-flow-8.1.3/cylc/flow/main_loop/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/main_loop/auto_restart.py` & `cylc-flow-8.1.3/cylc/flow/main_loop/auto_restart.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/main_loop/health_check.py` & `cylc-flow-8.1.3/cylc/flow/main_loop/health_check.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/main_loop/log_data_store.py` & `cylc-flow-8.1.3/cylc/flow/main_loop/log_data_store.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/main_loop/log_db.py` & `cylc-flow-8.1.3/cylc/flow/main_loop/log_db.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/main_loop/log_main_loop.py` & `cylc-flow-8.1.3/cylc/flow/main_loop/log_main_loop.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/main_loop/log_memory.py` & `cylc-flow-8.1.3/cylc/flow/main_loop/log_memory.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/main_loop/reset_bad_hosts.py` & `cylc-flow-8.1.3/cylc/flow/main_loop/reset_bad_hosts.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/network/__init__.py` & `cylc-flow-8.1.3/cylc/flow/network/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/network/authentication.py` & `cylc-flow-8.1.3/cylc/flow/network/authentication.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/network/authorisation.py` & `cylc-flow-8.1.3/cylc/flow/network/authorisation.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/network/client.py` & `cylc-flow-8.1.3/cylc/flow/network/client.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/network/client_factory.py` & `cylc-flow-8.1.3/cylc/flow/network/client_factory.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/network/graphql.py` & `cylc-flow-8.1.3/cylc/flow/network/graphql.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/network/multi.py` & `cylc-flow-8.1.3/cylc/flow/network/multi.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/network/publisher.py` & `cylc-flow-8.1.3/cylc/flow/network/publisher.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/network/replier.py` & `cylc-flow-8.1.3/cylc/flow/network/replier.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/network/resolvers.py` & `cylc-flow-8.1.3/cylc/flow/network/resolvers.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/network/scan.py` & `cylc-flow-8.1.3/cylc/flow/network/scan.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/network/schema.py` & `cylc-flow-8.1.3/cylc/flow/network/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 """GraphQL API schema via Graphene implementation."""
 
 from copy import deepcopy
 from functools import partial
 import json
-import logging
 from operator import attrgetter
 from textwrap import dedent
 from typing import (
     TYPE_CHECKING,
     AsyncGenerator,
     Any,
     List,
@@ -34,14 +33,15 @@
 from graphene import (
     Boolean, Field, Float, ID, InputObjectType, Int,
     Mutation, ObjectType, Schema, String, Argument, Interface
 )
 from graphene.types.generic import GenericScalar
 from graphene.utils.str_converters import to_snake_case
 
+from cylc.flow import LOG_LEVELS
 from cylc.flow.broadcast_mgr import ALL_CYCLE_POINTS_STRS, addict
 from cylc.flow.flow_mgr import FLOW_ALL, FLOW_NEW, FLOW_NONE
 from cylc.flow.id import Tokens
 from cylc.flow.task_outputs import SORT_ORDERS
 from cylc.flow.task_state import (
     TASK_OUTPUT_SUCCEEDED,
     TASK_STATUSES_ORDERED,
@@ -1422,17 +1422,19 @@
 
 class TimePoint(String):
     """A date-time in the ISO8601 format."""
 
 
 LogLevels = graphene.Enum(
     'LogLevels',
-    list(logging._nameToLevel.items()),
-    description=lambda x: f'Python logging level: {x.name} = {x.value}.'
-    if x else ''
+    list(LOG_LEVELS.items()),
+    description=lambda x: (
+        f'Logging level: {x.name} = {x.value}.'
+        if x else ''
+    )
 )
 
 
 class WorkflowStopMode(graphene.Enum):
     """The mode used to stop a running workflow."""
 
     # NOTE: using a different enum because:
@@ -1485,14 +1487,15 @@
             Active broadcasts can be revoked using the "clear" mode.
             Any broadcasts matching the specified cycle points and
             namespaces will be revoked.
 
             Note: a "clear" broadcast for a specific cycle or namespace does
             *not* clear all-cycle or all-namespace broadcasts.
 
+            Valid for: paused, running workflows.
         ''')
         resolver = mutator
 
     class Arguments:
         workflows = graphene.List(WorkflowID, required=True)
 
         mode = BroadcastMode(
@@ -1544,14 +1547,16 @@
 
 
 class SetHoldPoint(Mutation):
     class Meta:
         description = sstrip('''
             Set workflow hold after cycle point. All tasks after this point
             will be held.
+
+            Valid for: paused, running workflows.
         ''')
         resolver = mutator
 
     class Arguments:
         workflows = graphene.List(WorkflowID, required=True)
         point = CyclePoint(
             description='Hold all tasks after the specified cycle point.',
@@ -1561,16 +1566,17 @@
     result = GenericScalar()
 
 
 class Pause(Mutation):
     class Meta:
         description = sstrip('''
             Pause a workflow.
-
             This suspends submission of tasks.
+
+            Valid for: running workflows.
         ''')
         resolver = mutator
 
     class Arguments:
         workflows = graphene.List(WorkflowID, required=True)
 
     result = GenericScalar()
@@ -1586,14 +1592,16 @@
             - The job status file, if there is one.
             - The scheduler, if communication is possible.
 
             Jobs use this to record and report status such
             as success and failure. Applications run by jobs can use
             this command to report messages and to report registered task
             outputs.
+
+            Valid for: paused, running workflows.
         ''')
         resolver = partial(mutator, command='put_messages')
 
     class Arguments:
         workflows = graphene.List(WorkflowID, required=True)
         task_job = String(required=True)
         event_time = String(default_value=None)
@@ -1608,29 +1616,32 @@
 
 class ReleaseHoldPoint(Mutation):
     class Meta:
         description = sstrip('''
             Release all tasks and unset the workflow hold point, if set.
 
             Held tasks do not submit their jobs even if ready to run.
+
+            Valid for: paused, running workflows.
         ''')
         resolver = mutator
 
     class Arguments:
         workflows = graphene.List(WorkflowID, required=True)
 
     result = GenericScalar()
 
 
 class Resume(Mutation):
     class Meta:
         description = sstrip('''
             Resume a paused workflow.
-
             See also the opposite command `pause`.
+
+            Valid for: paused workflows.
         ''')
         resolver = mutator
 
     class Arguments:
         workflows = graphene.List(WorkflowID, required=True)
 
     result = GenericScalar()
@@ -1649,31 +1660,35 @@
             If the workflow was started with Jinja2 template variables on the
             command line (cylc play --set "FOO='bar'" REG) the same template
             settings apply to the reload (only changes to the flow.cylc
             file itself are reloaded).
 
             If the modified workflow config does not parse, failure to reload
             will be reported but no harm will be done to the running workflow.
+
+            Valid for: paused, running workflows.
         ''')
         resolver = partial(mutator, command='reload_workflow')
 
     class Arguments:
         workflows = graphene.List(WorkflowID, required=True)
 
     result = GenericScalar()
 
 
 class SetVerbosity(Mutation):
     class Meta:
         description = sstrip('''
             Change the logging severity level of a running workflow.
 
-            Only messages at or above the chosen severity level will be logged;
-            for example, if you choose `WARNING`, only warnings and critical
-            messages will be logged.
+            Only messages at or above the chosen severity level will be logged.
+            For example, if you choose `WARNING`, only warning, error and
+            critical level messages will be logged.
+
+            Valid for: paused, running workflows.
         ''')
         resolver = mutator
 
     class Arguments:
         workflows = graphene.List(WorkflowID, required=True)
         level = LogLevels(required=True)
 
@@ -1682,14 +1697,15 @@
 
 class SetGraphWindowExtent(Mutation):
     class Meta:
         description = sstrip('''
             Set the maximum graph distance (n) from an active node
             of the data-store graph window.
 
+            Valid for: paused, running workflows.
         ''')
         resolver = mutator
 
     class Arguments:
         workflows = graphene.List(WorkflowID, required=True)
         n_edge_distance = Int(required=True)
 
@@ -1707,14 +1723,16 @@
             with the "mode" option.
 
             Tasks that become ready after the shutdown is ordered will be
             submitted immediately if the workflow is restarted.
             Remaining task event handlers, job poll and kill commands, will
             be executed prior to shutdown, unless
             the stop mode is `{WorkflowStopMode.Now.name}`.
+
+            Valid for: paused, running workflows.
         ''')
         resolver = mutator
 
     class Arguments:
         workflows = graphene.List(WorkflowID, required=True)
         mode = WorkflowStopMode(
             default_value=WorkflowStopMode.Clean.name
@@ -1755,14 +1773,16 @@
             triggering system is responding to.
 
             Use the retry options in case the target workflow is down or out of
             contact.
 
             Note: To manually trigger a task use "Trigger" not
             "ExtTrigger".
+
+            Valid for: paused, running workflows.
         ''')
         resolver = partial(mutator, command='put_ext_trigger')
 
     class Arguments:
         workflows = graphene.List(WorkflowID, required=True)
         message = String(
             description='External trigger message.',
@@ -1833,33 +1853,39 @@
 
 class Hold(Mutation, TaskMutation):
     class Meta:
         description = sstrip('''
             Hold tasks within a workflow.
 
             Held tasks do not submit their jobs even if ready to run.
+
+            Valid for: paused, running workflows.
         ''')
         resolver = mutator
 
 
 class Release(Mutation, TaskMutation):
     class Meta:
         description = sstrip('''
             Release held tasks within a workflow.
 
             See also the opposite command `hold`.
+
+            Valid for: paused, running workflows.
         ''')
         resolver = mutator
 
 
 class Kill(Mutation, TaskMutation):
     # TODO: This should be a job mutation?
     class Meta:
         description = sstrip('''
             Kill running or submitted jobs.
+
+            Valid for: paused, running workflows.
         ''')
         resolver = partial(mutator, command='kill_tasks')
 
 
 class Poll(Mutation, TaskMutation):
     class Meta:
         description = sstrip('''
@@ -1867,39 +1893,44 @@
 
             This checks the job status file and queries the
             job runner on the job platform.
 
             Pollable tasks are those in the n=0 window with
             an associated job ID, including incomplete finished
             tasks.
+
+            Valid for: paused, running workflows.
         ''')
         resolver = partial(mutator, command='poll_tasks')
 
     class Arguments(TaskMutation.Arguments):
         ...
 
 
 class Remove(Mutation, TaskMutation):
     class Meta:
         description = sstrip('''
             Remove one or more task instances from a running workflow.
 
+            Valid for: paused, running workflows.
         ''')
         resolver = partial(mutator, command='remove_tasks')
 
 
 class SetOutputs(Mutation, TaskMutation):
     class Meta:
         description = sstrip('''
             Artificially mark task outputs as completed.
 
             This allows you to manually intervene with Cylc's scheduling
             algorithm by artificially satisfying outputs of tasks.
 
             By default this makes tasks appear as if they succeeded.
+
+            Valid for: paused, running workflows.
         ''')
         resolver = partial(mutator, command='force_spawn_children')
 
     class Arguments(TaskMutation.Arguments):
         outputs = graphene.List(
             String,
             default_value=[TASK_OUTPUT_SUCCEEDED],
@@ -1914,14 +1945,16 @@
             Manually trigger tasks.
 
             Warning: waiting tasks that are queue-limited will be queued if
             triggered, to submit as normal when released by the queue; queued
             tasks will submit immediately if triggered, even if that violates
             the queue limit (so you may need to trigger a queue-limited task
             twice to get it to submit immediately).
+
+            Valid for: paused, running workflows.
         ''')
         resolver = partial(mutator, command='force_trigger_tasks')
 
     class Arguments(TaskMutation.Arguments, FlowMutationArguments):
         ...
```

### Comparing `cylc-flow-8.1.2/cylc/flow/network/server.py` & `cylc-flow-8.1.3/cylc/flow/network/server.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/network/ssh_client.py` & `cylc-flow-8.1.3/cylc/flow/network/ssh_client.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/network/subscriber.py` & `cylc-flow-8.1.3/cylc/flow/network/subscriber.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/option_parsers.py` & `cylc-flow-8.1.3/cylc/flow/option_parsers.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,15 @@
     def __sub__(self, other):
         """Set difference on args."""
         return list(set(self.args) - set(other.args))
 
     def _in_list(self, others):
         """CLI arguments for this option found in any of a list of
         other options."""
-        return any([self & other for other in others])
+        return any(self & other for other in others)
 
     def _update_sources(self, other):
         """Update the sources from this and 1 other OptionSettings object"""
         self.sources = {*self.sources, *other.sources}
 
 
 ICP_OPTION = OptionSettings(
@@ -842,16 +842,18 @@
     # replace source path with workflow ID.
     if str(source) in sys.argv:
         sys.argv.remove(str(source))
     if workflow_id not in sys.argv:
         sys.argv.append(workflow_id)
 
 
-def log_subcommand(command, workflow_id):
+def log_subcommand(*args):
     """Log a command run as part of a sequence.
 
     Example:
         >>> log_subcommand('ruin', 'my_workflow')
         \x1b[1m\x1b[36m$ cylc ruin my_workflow\x1b[0m\x1b[1m\x1b[0m\n
     """
+    # Args might be posixpath or similar.
+    args = [str(a) for a in args]
     print(cparse(
-        f'<b><cyan>$ cylc {command} {workflow_id}</cyan></b>'))
+        f'<b><cyan>$ cylc {" ".join(args)}</cyan></b>'))
```

### Comparing `cylc-flow-8.1.2/cylc/flow/param_expand.py` & `cylc-flow-8.1.3/cylc/flow/param_expand.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/parsec/OrderedDict.py` & `cylc-flow-8.1.3/cylc/flow/parsec/OrderedDict.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/parsec/__init__.py` & `cylc-flow-8.1.3/cylc/flow/parsec/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/parsec/config.py` & `cylc-flow-8.1.3/cylc/flow/parsec/config.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/parsec/empysupport.py` & `cylc-flow-8.1.3/cylc/flow/parsec/empysupport.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/parsec/exceptions.py` & `cylc-flow-8.1.3/cylc/flow/parsec/exceptions.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/parsec/fileparse.py` & `cylc-flow-8.1.3/cylc/flow/parsec/fileparse.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/parsec/include.py` & `cylc-flow-8.1.3/cylc/flow/parsec/include.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/parsec/jinja2support.py` & `cylc-flow-8.1.3/cylc/flow/parsec/jinja2support.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/parsec/upgrade.py` & `cylc-flow-8.1.3/cylc/flow/parsec/upgrade.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,21 @@
                 'old': oldkeys, 'new': None, 'cvt': cvtr, 'silent': silent,
                 'is_section': is_section
             })
 
     def get_item(self, keys):
         item = self.cfg
         for key in keys:
-            item = item[key]
+            try:
+                item = item[key]
+            except TypeError:
+                raise UpgradeError(
+                    f'{self.show_keys(keys[:-1], True)}'
+                    f' ("{keys[-2]}" should be a [section] not a setting)'
+                )
         return item
 
     def put_item(self, keys, val):
         item = self.cfg
         for key in keys[:-1]:
             if key not in item:
                 item[key] = {}
```

### Comparing `cylc-flow-8.1.2/cylc/flow/parsec/util.py` & `cylc-flow-8.1.3/cylc/flow/parsec/util.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/parsec/validate.py` & `cylc-flow-8.1.3/cylc/flow/parsec/validate.py`

 * *Files 2% similar despite different names*

```diff
@@ -200,18 +200,36 @@
                         ):
                             raise IllegalItemError(keys, key)
                         speckey = '__MANY__'
 
                 else:
                     speckey = key
                 specval = spec[speckey]
-                if isinstance(value, dict) and not specval.is_leaf():
+
+                cfg_is_section = isinstance(value, dict)
+                spec_is_section = not specval.is_leaf()
+                if cfg_is_section and not spec_is_section:
+                    # config is a [section] but it should be a setting=
+                    raise IllegalItemError(
+                        keys,
+                        key,
+                        msg=f'"{key}" should be a setting not a [section]',
+                    )
+                if (not cfg_is_section) and spec_is_section:
+                    # config is a setting= but it should be a [section]
+                    raise IllegalItemError(
+                        keys,
+                        key,
+                        msg=f'"{key}" should be a [section] not a setting',
+                    )
+
+                if cfg_is_section and spec_is_section:
                     # Item is dict, push to queue
                     queue.append([value, specval, keys + [key]])
-                elif value is not None and specval.is_leaf():
+                elif value is not None and not spec_is_section:
                     # Item is value, coerce according to value type
                     cfg[key] = self.coercers[specval.vdr](value, keys + [key])
                     if specval.options:
                         voptions = specval.options
                         if (isinstance(cfg[key], list) and
                                 any(val not in voptions for val in cfg[key]) or
                                 not isinstance(cfg[key], list) and
```

### Comparing `cylc-flow-8.1.2/cylc/flow/pathutil.py` & `cylc-flow-8.1.3/cylc/flow/pathutil.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,24 +11,26 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """Functions to return paths to common workflow files and directories."""
 
+import errno
 import os
 from pathlib import Path
 import re
 from shutil import rmtree
+from time import sleep
 from typing import Dict, Iterable, Set, Union, Optional, Any
 
 from cylc.flow import LOG
 from cylc.flow.cfgspec.glbl_cfg import glbl_cfg
 from cylc.flow.exceptions import (
-    InputError, WorkflowFilesError, handle_rmtree_err
+    FileRemovalError, InputError, WorkflowFilesError
 )
 from cylc.flow.platforms import get_localhost_install_target
 
 
 # Note: do not import this elsewhere, as it might bypass unit test
 # monkeypatching:
 _CYLC_RUN_DIR = os.path.join('$HOME', 'cylc-run')
@@ -293,23 +295,62 @@
     if os.path.islink(path):
         if os.path.exists(path):
             target = os.path.realpath(path)
             LOG.info(
                 "Removing symlink and its target directory: "
                 f"{path} -> {target}"
             )
-            rmtree(target, onerror=handle_rmtree_err)
+            _rmtree(target)
         else:
             LOG.info(f'Removing broken symlink: {path}')
         os.remove(path)
     elif not os.path.exists(path):
         raise FileNotFoundError(path)
     else:
         LOG.info(f'Removing directory: {path}')
-        rmtree(path, onerror=handle_rmtree_err)
+        _rmtree(path)
+
+
+def _rmtree(
+    target: Union[Path, str],
+    retries: int = 10,
+    sleep_time: float = 1,
+):
+    """Make rmtree more robust to nfs issues.
+
+    If a file is deleted which is being held open for reading by
+    another process. NFS will create a ".nfs" file in the
+    containing directory to handle this.
+
+    If you try to delete the directory which contains these
+    files you will get either a ENOTEMPTY or EBUSY error.
+
+    A likely cause of open file handles in cylc-run directories
+    is `cylc cat-log -m t`. If the file being cat-log'ged is removed,
+    the command will fail on its next poll. The default poll
+    interval is one second, so if we wait a couple of seconds and
+    retry the removal it will likely work.
+
+    This command retries removal a specified number
+    of times at a specified interval before failing to
+    give cat-log process a chance to die gracefully and
+    release their filesystem locks. For more info see:
+    https://github.com/cylc/cylc-flow/pull/5359#issuecomment-1479989975
+    """
+    for _try_num in range(retries):
+        try:
+            rmtree(target)
+            return
+        except OSError as exc:
+            if exc.errno in {errno.ENOTEMPTY, errno.EBUSY}:
+                err = exc
+                sleep(sleep_time)
+            else:
+                raise
+    raise FileRemovalError(err)
 
 
 def remove_dir_or_file(path: Union[Path, str]) -> None:
     """Delete a directory tree, or a file, or a symlink.
     Does not follow symlinks.
 
     Args:
@@ -321,15 +362,15 @@
         LOG.info(f"Removing symlink: {path}")
         os.remove(path)
     elif os.path.isfile(path):
         LOG.info(f"Removing file: {path}")
         os.remove(path)
     else:
         LOG.info(f"Removing directory: {path}")
-        rmtree(path, onerror=handle_rmtree_err)
+        _rmtree(path)
 
 
 def remove_empty_parents(
     path: Union[Path, str], tail: Union[Path, str]
 ) -> None:
     """Work our way up the tail of path, removing empty dirs only.
 
@@ -423,15 +464,19 @@
                 # not files, when globbing
                 part += os.sep
             result.add(part)
     return result
 
 
 def is_relative_to(path1: Union[Path, str], path2: Union[Path, str]) -> bool:
-    """Return whether or not path1 is relative to path2."""
+    """Return whether or not path1 is relative to path2.
+
+    Normalizes both paths to avoid trickery with paths containing `..`
+    somewhere in them.
+    """
     # In future, we can just use pathlib.Path.is_relative_to()
     # when Python 3.9 becomes the minimum supported version
     try:
         Path(os.path.normpath(path1)).relative_to(os.path.normpath(path2))
     except ValueError:
         return False
     return True
```

### Comparing `cylc-flow-8.1.2/cylc/flow/platforms.py` & `cylc-flow-8.1.3/cylc/flow/platforms.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,16 @@
 #
 """Functions relating to (job) platforms."""
 
 import random
 import re
 from copy import deepcopy
 from typing import (
-    TYPE_CHECKING, Any, Dict, Iterable, List, Optional, Set, Union, overload
+    TYPE_CHECKING, Any, Dict, Iterable,
+    List, Optional, Set, Union, overload
 )
 
 from cylc.flow import LOG
 
 from cylc.flow.exceptions import (
     GlobalConfigError,
     PlatformLookupError, CylcError, NoHostsError, NoPlatformsError)
@@ -113,19 +114,30 @@
     Looking at a task config this method decides whether to get platform from
     name, or Cylc7 config items.
 
     Args:
         task_conf: If str this is assumed to be the platform name, otherwise
             this should be a configuration for a task.
         task_name: Help produce more helpful error messages.
+        bad_hosts: A set of hosts known to be unreachable (had an ssh 255
+            error)
 
     Returns:
         platform: A platform definition dictionary. Uses either
             get_platform() or platform_name_from_job_info(), but to the
             user these look the same.
+
+    Raises:
+        NoPlatformsError:
+            Platform group has no platforms with usable hosts.
+            This should be caught if this function is used on a raw config,
+            or in any other context where a platform group might be selected.
+        PlatformLookupError:
+            Raised if the name of a platform cannot be selected based on the
+            information given.
     """
     if task_conf is None or isinstance(task_conf, str):  # noqa: SIM 114
         # task_conf is a platform name, or get localhost if None
         return platform_from_name(task_conf, bad_hosts=bad_hosts)
 
     # NOTE: Do NOT use .get() on OrderedDictWithDefaults -
     # https://github.com/cylc/cylc-flow/pull/4975
@@ -174,49 +186,58 @@
     Verifies selected platform is present in global.cylc file and returns it,
     raises error if platform is not in global.cylc or returns 'localhost' if
     no platform is initially selected.
 
     Args:
         platform_name: name of platform to be retrieved.
         platforms: global.cylc platforms given as a dict.
+        bad_hosts: A set of hosts known to be unreachable (had an ssh 255
+            error)
 
     Returns:
         platform: object containing settings for a platform, loaded from
             Global Config.
+
+    Raises:
+        NoPlatformsError: Platform group has no platforms with usable hosts.
     """
     if platforms is None:
         platforms = glbl_cfg().get(['platforms'])
     platform_groups = glbl_cfg().get(['platform groups'])
 
     if platform_name is None:
         platform_name = 'localhost'
 
-    platform_group = None
+    # The list is reversed to allow user-set platform groups (which are
+    # appended to site set platform groups) to be matched first and override
+    # site defined platform groups.
     for platform_name_re in reversed(list(platform_groups)):
         # Platform is member of a group.
         if re.fullmatch(platform_name_re, platform_name):
             platform_name = get_platform_from_group(
                 platform_groups[platform_name_re], group_name=platform_name,
                 bad_hosts=bad_hosts
             )
+            break
 
     for platform_name_re in list(platforms):
         if (
             # If the platform_name_re contains special regex chars
             re.escape(platform_name_re) != platform_name_re
             and re.match(platform_name_re, 'localhost')
         ):
             raise PlatformLookupError(
                 'The "localhost" platform cannot be defined using a '
                 'regular expression. See the documentation for '
                 '"global.cylc[platforms][localhost]" for more information.'
             )
-    # The list is reversed to allow user-set platforms (which are loaded
-    # later than site set platforms) to be matched first and override site
-    # defined platforms.
+
+    # The list is reversed to allow user-set platforms (which are appended to
+    # than site set platforms) to be matched first and override site defined
+    # platforms.
     for platform_name_re in reversed(list(platforms)):
         # We substitute commas with or without spaces to
         # allow lists of platforms
         if (
             re.fullmatch(
                 re.sub(
                     r'\s*(?!{[\s\d]*),(?![\s\d]*})\s*',
@@ -238,16 +259,14 @@
             if (
                 'hosts' not in platform_data.keys() or
                 not platform_data['hosts']
             ):
                 platform_data['hosts'] = [platform_name]
             # Fill in the "private" name field.
             platform_data['name'] = platform_name
-            if platform_group:
-                platform_data['group'] = platform_group
             return platform_data
 
     raise PlatformLookupError(
         f"No matching platform \"{platform_name}\" found")
 
 
 def get_platform_from_group(
@@ -479,18 +498,18 @@
     else:
         job_generic = job
 
     for task_section in [job_generic, remote_generic]:
         # Get a set of items actually set in both platform and task_section.
         shared_items = set(task_section).intersection(set(platform_spec))
         # If any set items do not match, we can't use this platform.
-        if not all([
+        if not all(
             platform_spec[item] == task_section[item]
             for item in shared_items
-        ]):
+        ):
             return False
     return True
 
 
 def get_host_from_platform(
     platform: Dict[str, Any], bad_hosts: Optional[Set[str]] = None
 ) -> str:
@@ -499,14 +518,18 @@
 
     Args:
         platform: A dict representing a platform.
         bad_hosts: A set of hosts Cylc knows to be unreachable.
 
     Returns:
         hostname: The name of a host.
+
+    Raises:
+        NoHostsError:
+            This error should be caught by caller to prevent workflow shutdown.
     """
     # Get list of goodhosts:
     if bad_hosts:
         goodhosts = [i for i in platform['hosts'] if i not in bad_hosts]
     else:
         goodhosts = platform['hosts']
 
@@ -604,26 +627,37 @@
     if not platform['install target']:
         platform['install target'] = platform['name']
 
     return platform['install target']
 
 
 def get_install_target_to_platforms_map(
-        platform_names: Iterable[str]
+    platform_names: Iterable[str],
+    quiet: bool = False
 ) -> Dict[str, List[Dict[str, Any]]]:
     """Get a dictionary of unique install targets and the platforms which use
     them.
 
     Args:
         platform_names: List of platform names to look up in the global config.
+        quiet: Supress PlatformNotFound Errors
 
     Return {install_target_1: [platform_1_dict, platform_2_dict, ...], ...}
     """
     platform_names = set(platform_names)
-    platforms = [platform_from_name(p_name) for p_name in platform_names]
+    platforms: List[Dict[str, Any]] = []
+    for p_name in platform_names:
+        try:
+            platform = platform_from_name(p_name)
+        except PlatformLookupError as exc:
+            if not quiet:
+                raise exc
+        else:
+            platforms.append(platform)
+
     install_targets = {
         get_install_target_from_platform(platform)
         for platform in platforms
     }
     return {
         target: [
             platform
@@ -641,42 +675,14 @@
     """Determines whether install target is in the list of platforms"""
     return any(
         install_target == distinct_platform['install target']
         for distinct_platform in distinct_platforms_list
     )
 
 
-def get_all_platforms_for_install_target(
-    install_target: str
-) -> List[Dict[str, Any]]:
-    """Return list of platform dictionaries for given install target."""
-    platforms: List[Dict[str, Any]] = []
-    all_platforms = glbl_cfg(cached=True).get(['platforms'], sparse=False)
-    for k, v in all_platforms.iteritems():  # noqa: B301 (iteritems valid here)
-        if (v.get('install target', k) == install_target):
-            v_copy = deepcopy(v)
-            v_copy['name'] = k
-            platforms.append(v_copy)
-    return platforms
-
-
-def get_random_platform_for_install_target(
-    install_target: str
-) -> Dict[str, Any]:
-    """Return a randomly selected platform (dict) for given install target."""
-    platforms = get_all_platforms_for_install_target(install_target)
-    try:
-        return random.choice(platforms)  # nosec (not crypto related)
-    except IndexError:
-        # No platforms to choose from
-        raise PlatformLookupError(
-            f'Could not select platform for install target: {install_target}'
-        )
-
-
 def get_localhost_install_target() -> str:
     """Returns the install target of localhost platform"""
     localhost = get_platform()
     return get_install_target_from_platform(localhost)
 
 
 def _validate_single_host(
```

### Comparing `cylc-flow-8.1.2/cylc/flow/prerequisite.py` & `cylc-flow-8.1.3/cylc/flow/prerequisite.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,34 +38,30 @@
     corresponding to parenthesised expressions in Cylc graphs (e.g.
     `(a & b) => c` or `(a | b) => c`). For the OR operator (`|`), only one
     message has to be satisfied for the Prerequisite to be satisfied.
     """
 
     # Memory optimization - constrain possible attributes to this list.
     __slots__ = ["satisfied", "_all_satisfied",
-                 "target_point_strings", "start_point",
+                 "target_point_strings",
                  "conditional_expression", "point"]
 
     # Extracts T from "foo.T succeeded" etc.
     SATISFIED_TEMPLATE = 'bool(self.satisfied[("%s", "%s", "%s")])'
     MESSAGE_TEMPLATE = r'%s/%s %s'
 
     DEP_STATE_SATISFIED = 'satisfied naturally'
     DEP_STATE_OVERRIDDEN = 'force satisfied'
     DEP_STATE_UNSATISFIED = False
 
-    def __init__(self, point, start_point=None):
+    def __init__(self, point):
         # The cycle point to which this prerequisite belongs.
         # cylc.flow.cycling.PointBase
         self.point = point
 
-        # Start point for prerequisite validity.
-        # cylc.flow.cycling.PointBase
-        self.start_point = start_point
-
         # List of cycle point strings that this prerequisite depends on.
         self.target_point_strings = []
 
         # Dictionary of messages pertaining to this prerequisite.
         # {('point string', 'task name', 'output'): DEP_STATE_X, ...}
         self.satisfied = {}
 
@@ -75,14 +71,25 @@
 
         # The cached state of this prerequisite:
         # * `None` (no cached state)
         # * `True` (prerequisite satisfied)
         # * `False` (prerequisite unsatisfied).
         self._all_satisfied = None
 
+    def instantaneous_hash(self):
+        """Generate a hash of this prerequisite in its current state.
+
+        Note not using `__hash__` because Prerequisite objects are mutable.
+        """
+        return hash((
+            self.point,
+            self.conditional_expression,
+            tuple(self.satisfied.keys()),
+        ))
+
     def add(self, name, point, output, pre_initial=False):
         """Register an output with this prerequisite.
 
         Args:
             name (str): The name of the task to which the output pertains.
             point (str/cylc.flow.cycling.PointBase): The cycle point at which
                 this dependent output should appear.
@@ -186,15 +193,15 @@
                 err_msg += (
                     " (could be unmatched parentheses in the graph string?)")
             raise TriggerExpressionError(
                 '"%s":\n%s' % (self.get_raw_conditional_expression(), err_msg))
         return res
 
     def satisfy_me(self, all_task_outputs):
-        """Evaluate pre-requisite against known outputs.
+        """Evaluate prerequisite against known outputs.
 
         Updates cache with the evaluation result.
 
         """
         relevant_messages = all_task_outputs & set(self.satisfied)
         for message in relevant_messages:
             self.satisfied[message] = self.DEP_STATE_SATISFIED
```

### Comparing `cylc-flow-8.1.2/cylc/flow/print_tree.py` & `cylc-flow-8.1.3/cylc/flow/print_tree.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/profiler.py` & `cylc-flow-8.1.3/cylc/flow/profiler.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/remote.py` & `cylc-flow-8.1.3/cylc/flow/remote.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/resources.py` & `cylc-flow-8.1.3/cylc/flow/resources.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/rundb.py` & `cylc-flow-8.1.3/cylc/flow/rundb.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from os.path import expandvars
 from pprint import pformat
 import sqlite3
 import traceback
 from typing import TYPE_CHECKING, List, Optional, Tuple, Union
 
 from cylc.flow import LOG
+from cylc.flow.exceptions import PlatformLookupError
 from cylc.flow.util import deserialise
 import cylc.flow.flags
 
 if TYPE_CHECKING:
     from pathlib import Path
 
 
@@ -833,14 +834,19 @@
             callback(row_idx, list(row))
 
     def select_task_pool_for_restart(self, callback):
         """Select from task_pool+task_states+task_jobs for restart.
 
         Invoke callback(row_idx, row) on each row, where each row contains:
         the fields in the SELECT statement below.
+
+        Raises:
+            PlatformLookupError: Do not start up if platforms for running
+            tasks cannot be found in global.cylc. This exception should
+            not be caught.
         """
         form_stmt = r"""
             SELECT
                 %(task_pool)s.cycle,
                 %(task_pool)s.name,
                 %(task_pool)s.flow_nums,
                 %(task_states)s.flow_wait,
@@ -886,16 +892,32 @@
             "task_states": self.TABLE_TASK_STATES,
             "task_late_flags": self.TABLE_TASK_LATE_FLAGS,
             "task_timeout_timers": self.TABLE_TASK_TIMEOUT_TIMERS,
             "task_jobs": self.TABLE_TASK_JOBS,
             "task_outputs": self.TABLE_TASK_OUTPUTS,
         }
         stmt = form_stmt % form_data
+
+        # Run the callback, collecting any platform errors to be handled later:
+        platform_errors = []
         for row_idx, row in enumerate(self.connect().execute(stmt)):
-            callback(row_idx, list(row))
+            platform_error = callback(row_idx, list(row))
+            if platform_error:
+                platform_errors.append(platform_error)
+
+        # If any of the platforms could not be found, raise an exception
+        # and stop trying to play this workflow:
+        if platform_errors:
+            msg = (
+                "The following platforms are not defined in"
+                " the global.cylc file:"
+            )
+            for platform in platform_errors:
+                msg += f"\n * {platform}"
+            raise PlatformLookupError(msg)
 
     def select_task_prerequisites(
         self, cycle: str, name: str, flow_nums: str
     ) -> List[Tuple[str, str, str, str]]:
         """Return prerequisites of a task of the given name & cycle point."""
         stmt = rf"""
             SELECT
@@ -1051,50 +1073,7 @@
         }
         stmt = form_stmt % form_data
         return list(self.connect().execute(stmt))
 
     def vacuum(self):
         """Vacuum to the database."""
         return self.connect().execute("VACUUM")
-
-    def remove_columns(self, table, to_drop):
-        conn = self.connect()
-
-        # get list of columns to keep
-        schema = conn.execute(
-            rf'''
-                PRAGMA table_info({table})
-            '''
-        )
-        new_cols = [
-            name
-            for _, name, *_ in schema
-            if name not in to_drop
-        ]
-
-        # copy table
-        conn.execute(
-            rf'''
-                CREATE TABLE {table}_new AS
-                SELECT {', '.join(new_cols)}
-                FROM {table}
-            '''
-        )
-
-        # remove original
-        conn.execute(
-            rf'''
-                DROP TABLE {table}
-            '''
-        )
-
-        # copy table
-        conn.execute(
-            rf'''
-                CREATE TABLE {table} AS
-                SELECT {', '.join(new_cols)}
-                FROM {table}_new
-            '''
-        )
-
-        # done
-        conn.commit()
```

### Comparing `cylc-flow-8.1.2/cylc/flow/scheduler.py` & `cylc-flow-8.1.3/cylc/flow/scheduler.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/scheduler_cli.py` & `cylc-flow-8.1.3/cylc/flow/scheduler_cli.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/scripts/__init__.py` & `cylc-flow-8.1.3/cylc/flow/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/scripts/broadcast.py` & `cylc-flow-8.1.3/cylc/flow/scripts/broadcast.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/scripts/cat_log.py` & `cylc-flow-8.1.3/cylc/flow/scripts/cat_log.py`

 * *Files 16% similar despite different names*

```diff
@@ -40,20 +40,29 @@
 
 Examples:
   # for a task "2020/bar" in workflow "foo"
 
   # Print workflow log:
   $ cylc cat-log foo
 
+  # Print specific workflow log:
+  $ cylc cat-log foo -f scheduler/02-start-01.log
+
   # Print task stdout:
   $ cylc cat-log foo//2020/bar
   $ cylc cat-log -f o foo//2020/bar
 
   # Print task stderr:
   $ cylc cat-log -f e foo//2020/bar
+
+  # Print a custom file in a job's log directory:
+  $ cylc cat-log -f my-log-file foo//2020/bar
+
+  # Follow a log file:
+  $ cylc cat-log foo//2020/bar -m f
 """
 
 import os
 from contextlib import suppress
 from glob import glob
 from pathlib import Path
 import shlex
@@ -61,38 +70,69 @@
 import sys
 from typing import TYPE_CHECKING
 
 from cylc.flow.exceptions import InputError
 import cylc.flow.flags
 from cylc.flow.hostuserutil import is_remote_platform
 from cylc.flow.id_cli import parse_id
-from cylc.flow.loggingutil import LOG_FILE_EXTENSION
 from cylc.flow.option_parsers import (
     ID_MULTI_ARG_DOC,
     CylcOptionParser as COP,
     verbosity_to_opts,
 )
 from cylc.flow.pathutil import (
     expand_path,
     get_remote_workflow_run_job_dir,
     get_workflow_run_job_dir,
     get_workflow_run_pub_db_path,
-    get_workflow_run_scheduler_log_path)
+    get_workflow_run_dir,
+)
 from cylc.flow.remote import remote_cylc_cmd, watch_and_kill
 from cylc.flow.rundb import CylcWorkflowDAO
 from cylc.flow.task_job_logs import (
     JOB_LOG_OUT, JOB_LOG_ERR, JOB_LOG_OPTS, NN, JOB_LOG_ACTIVITY)
 from cylc.flow.terminal import cli_function
 from cylc.flow.platforms import get_platform
 
 
 if TYPE_CHECKING:
     from optparse import Values
 
 
+WORKFLOW_LOG_OPTS = {
+    'c': ('workflow configuration file (raw)', r'config/*-start-*.cylc'),
+    'p': (
+        'workflow configuration file (processed)',
+        r'config/flow-processed.cylc'
+    ),
+    'i': ('install log', r'install/*-*install.log'),
+    's': ('scheduler log', r'scheduler/*-*start*.log'),
+}
+
+
+# add workflow and job log file options to the CLI help output
+__doc__ += r'''
+
+Log Files:
+  Select the log file to view with the --file option.
+  Either provide the file path or use one of the short options:
+
+  Job Logs:
+''' + '    ' + '\n    '.join(
+    f'{key:4} {value}'
+    for key, value in JOB_LOG_OPTS.items()
+) + '''
+
+  Workflow Logs:
+''' + '    ' + '\n    '.join(
+    f'{key:4} {value[0]}'
+    for key, value in WORKFLOW_LOG_OPTS.items()
+) + '\n\n  Use "--mode=l" to list available log files for a workflow/job.'
+
+
 # Immortal tail-follow processes on job hosts can be cleaned up by killing
 # my subprocesses if my PPID or PPPID changes (due to parent ssh connection
 # dying). This works even if the sshd-invoked
 # "$(SHELL) -c <remote-command>" does not
 # exec <remote-command> (affects whether my parent process or I get inherited
 # by init).
 #
@@ -152,57 +192,109 @@
             stdout=stdout,
         )
         return color_proc.communicate(cat_proc.communicate()[0])
     else:
         cat_proc.wait()
 
 
-def view_log(logpath, mode, tailer_tmpl, batchview_cmd=None, remote=False,
-             color=False):
+def _check_fs_path(path):
+    """Ensure a path is relative and normalised.
+
+    Useful for checking input paths which are intended to be
+    relative to a specified directory.
+
+    Examples:
+        # good paths
+        >>> _check_fs_path('a')
+        >>> _check_fs_path('a/b')
+        >>> _check_fs_path('a/b/')
+
+        # bad paths
+        >>> _check_fs_path('/a')
+        Traceback (most recent call last):
+         ...
+        InputError: ...
+        >>> _check_fs_path('a/../b')
+        Traceback (most recent call last):
+         ...
+        InputError: ...
+        >>> _check_fs_path('../a')
+        Traceback (most recent call last):
+         ...
+        InputError: ...
+        >>> _check_fs_path('./a')
+        Traceback (most recent call last):
+         ...
+        InputError: ...
+
+    Raises:
+        InputError
+
+    """
+    # join the path onto something to test normalisation
+    _path = os.path.join('x', path).rstrip(os.sep)
+    if os.path.isabs(path) or os.path.normpath(_path) != _path:
+        raise InputError(
+            f'File paths must be relative to the job log directory: {path}'
+        )
+
+
+def view_log(
+    logpath,
+    mode,
+    tailer_tmpl,
+    batchview_cmd=None,
+    remote=False,
+    color=False,
+    prepend_path=False,
+):
     """View (by mode) local log file. This is only called on the file host.
 
     batchview_cmd is a job-runner-specific job stdout or stderr cat or tail
     command (e.g. 'qcat') that may be implemented for job runners that don't
     write logs to their final locations until after the job completes.
 
     If remote is True, we are executing on a remote host for a log file there.
 
     """
     # The log file path may contain '$USER' to be evaluated on the job host.
     if mode == 'print':
         # Print location even if the workflow does not exist yet.
         print(logpath)
         return 0
-    elif not os.path.exists(logpath) and batchview_cmd is None:
+    if not os.path.exists(logpath) and batchview_cmd is None:
         # Note: batchview_cmd may not need to have access to logpath, so don't
         # test for existence of path if it is set.
         sys.stderr.write('file not found: %s\n' % logpath)
         return 1
-    elif mode == 'print-dir':
+    if mode == 'print-dir':
         print(os.path.dirname(logpath))
         return 0
-    elif mode == 'list-dir':
+    if mode == 'list-dir':
         for entry in sorted(os.listdir(os.path.dirname(logpath))):
             print(entry)
         return 0
-    elif mode == 'cat':
+    if prepend_path:
+        from cylc.flow.hostuserutil import get_host
+        print(f'# {get_host()}:{logpath}')
+    if mode == 'cat':
         # print file contents to stdout.
         if batchview_cmd is not None:
             cmd = shlex.split(batchview_cmd)
         else:
             cmd = ['cat', logpath]
         proc1 = Popen(  # nosec
             cmd,
             stdin=DEVNULL,
             stdout=PIPE if color else None
         )
         # * batchview command is user configurable
         colorise_cat_log(proc1, color=color)
         return 0
-    elif mode == 'tail':
+    if mode == 'tail':
         if batchview_cmd is not None:
             cmd = batchview_cmd
         else:
             cmd = tailer_tmpl % {"filename": logpath}
         proc = Popen(shlex.split(cmd), stdin=DEVNULL)  # nosec
         # * batchview command is user configurable
         with suppress(KeyboardInterrupt):
@@ -217,49 +309,61 @@
         argdoc=[
             ID_MULTI_ARG_DOC,
         ]
     )
 
     parser.add_option(
         "-f", "--file",
-        help="  Job log: %s; default o(out)." % (
-             ', '.join(['%s(%s)' % (i, j)
-                       for i, j in JOB_LOG_OPTS.items()])) +
-             "  Or <filename> for custom (and standard) job logs.",
-        metavar="LOG", action="store", default=None, dest="filename")
+        help=(
+            'The file to view. Default for job logs "out", default for'
+            ' workflow logs "scheduler/log". See "Log Files" above for'
+            ' possible values.'
+        ),
+        metavar="LOG",
+        action="store",
+        default=None,
+        dest="filename",
+    )
 
     parser.add_option(
         "-m", "--mode",
         help="Mode: %s. Default c(cat)." % (
             ', '.join(['%s(%s)' % (i, j) for i, j in MODES.items()])),
         action="store", choices=list(MODES.keys()) + list(MODES.values()),
         default='c', dest="mode")
 
     parser.add_option(
         "-r", "--rotation",
         help="Workflow log integer rotation number. 0 for current, 1 for "
         "next oldest, etc.",
-        metavar="INT", action="store", dest="rotation_num")
+        metavar="INT", action="store", dest="rotation_num", type=int)
 
     parser.add_option(
         "-o", "--force-remote",
         help="View remote logs remotely even if they have been retrieved"
         " to the workflow host (default False).",
         action="store_true", default=False, dest="force_remote")
 
     parser.add_option(
         "-s", "--submit-number", "-t", "--try-number",
         help="Job submit number (default=%s, i.e. latest)." % NN,
-        metavar="INT", action="store", dest="submit_num", default=NN)
+        metavar="INT", action="store", dest="submit_num", default=None)
 
     parser.add_option(
         "--remote-arg",
         help="(for internal use: continue processing on job host)",
         action="append", dest="remote_args")
 
+    parser.add_option(
+        '--prepend-path',
+        help='Prepend the file path to the output in the format <host>:<path>',
+        action='store_true',
+        default=False,
+    )
+
     return parser
 
 
 def get_task_job_attrs(workflow_id, point, task, submit_num):
     """Return job (platform, job_runner_name, live_job_id).
 
     live_job_id is the job ID if job is running, else None.
@@ -293,82 +397,127 @@
 
     Determine log path, user@host, batchview_cmd, and action (print, dir-list,
     cat, or tail), and then if the log path is:
       a) local: perform action on log path, or
       b) remote: re-invoke cylc cat-log as a) on the remote account
 
     """
+    if options.filename is not None:
+        _check_fs_path(options.filename)
+
     if options.remote_args:
         # Invoked on job hosts for job logs only, as a wrapper to view_log().
         # Tail and batchview commands from global config on workflow host).
         logpath, mode, tail_tmpl = options.remote_args[0:3]
+        _check_fs_path(logpath)
         logpath = expand_path(logpath)
         tail_tmpl = expand_path(tail_tmpl)
         try:
             batchview_cmd = options.remote_args[3]
         except IndexError:
             batchview_cmd = None
-        res = view_log(logpath, mode, tail_tmpl, batchview_cmd, remote=True,
-                       color=color)
+        res = view_log(
+            logpath,
+            mode,
+            tail_tmpl,
+            batchview_cmd,
+            remote=True,
+            color=color,
+            prepend_path=options.prepend_path,
+        )
         if res == 1:
             sys.exit(res)
         return
 
     workflow_id, tokens, _ = parse_id(*ids, constraint='mixed')
 
     # Get long-format mode.
     try:
         mode = MODES[options.mode]
     except KeyError:
         mode = options.mode
 
+    if tokens and tokens.get('cycle') and not tokens.get('task'):
+        print('Please provide a workflow, task or job ID', file=sys.stderr)
+        sys.exit(1)
+
     if not tokens or not tokens.get('task'):
-        # Cat workflow logs, local only.
-        if options.filename is not None:
-            raise InputError("The '-f' option is for job logs only.")
-
-        logpath = get_workflow_run_scheduler_log_path(workflow_id)
-        if options.rotation_num:
-            log_dir = Path(logpath).parent
-            logs = glob(f'{log_dir}/*{LOG_FILE_EXTENSION}')
-            logs.sort(key=os.path.getmtime, reverse=True)
+        # no task provided - user has requested a workflow log
+        log_dir: str = get_workflow_run_dir(workflow_id, 'log')
+        file_name: str = options.filename or 's'
+        log_file_path: Path
+
+        if mode == 'list-dir':
+            # list workflow logs
+            print('\n'.join(sorted(
+                str(path.relative_to(log_dir))
+                for dirpath in {
+                    # set of log/<x> directories to scan for files in
+                    Path(log_dir, _file_name).parent
+                    for _, _file_name in WORKFLOW_LOG_OPTS.values()
+                    # don't try to list directories which aren't there
+                    if Path(log_dir, _file_name).parent.exists()
+                }
+                for path in dirpath.iterdir()
+                # strip out file aliases such as scheduler/log
+                if not path.is_symlink()
+            )))
+            return
+
+        if file_name in WORKFLOW_LOG_OPTS:
+            rotation_number = options.rotation_num or 0
+            pattern = WORKFLOW_LOG_OPTS[file_name][1]
+            logs = sorted(
+                glob(
+                    str(Path(log_dir, pattern))
+                ),
+                reverse=True
+            )
             try:
-                logpath = logs[int(options.rotation_num)]
+                log_file_path = Path(logs[rotation_number])
             except IndexError:
-                raise InputError(
-                    "max rotation %d" % (len(logs) - 1))
+                raise InputError("max rotation %d" % (len(logs) - 1))
+        else:
+            log_file_path = Path(log_dir, file_name)
+
         tail_tmpl = os.path.expandvars(
             get_platform()["tail command template"]
         )
-        out = view_log(logpath, mode, tail_tmpl, color=color)
-        if out == 1:
-            sys.exit(1)
-        return
+        out = view_log(
+            log_file_path,
+            mode,
+            tail_tmpl,
+            color=color,
+            prepend_path=options.prepend_path,
+        )
+        sys.exit(out)
 
     else:
         # Cat task job logs, may be on workflow or job host.
         if options.rotation_num is not None:
             raise InputError(
                 "only workflow (not job) logs get rotated")
         task = tokens['task']
         point = tokens['cycle']
-        if options.submit_num != NN:
+
+        submit_num = options.submit_num or tokens.get('job') or NN
+        if submit_num != NN:
             try:
-                options.submit_num = "%02d" % int(options.submit_num)
+                submit_num = "%02d" % int(submit_num)
             except ValueError:
-                parser.error("Illegal submit number: %s" % options.submit_num)
+                parser.error("Illegal submit number: %s" % submit_num)
         if options.filename is None:
             options.filename = JOB_LOG_OUT
         else:
             # Convert short filename args to long (e.g. 'o' to 'job.out').
             with suppress(KeyError):
                 options.filename = JOB_LOG_OPTS[options.filename]
                 # KeyError: Is already long form (standard log, or custom).
         platform_name, job_runner_name, live_job_id = get_task_job_attrs(
-            workflow_id, point, task, options.submit_num)
+            workflow_id, point, task, submit_num)
         platform = get_platform(platform_name)
         batchview_cmd = None
         if live_job_id is not None:
             # Job is currently running. Get special job runner log view
             # command (e.g. qcat) if one exists, and the log is out or err.
             conf_key = None
             if options.filename == JOB_LOG_OUT:
@@ -391,23 +540,25 @@
 
         log_is_remote = (is_remote_platform(platform)
                          and (options.filename != JOB_LOG_ACTIVITY))
         log_is_retrieved = (platform['retrieve job logs']
                             and live_job_id is None)
         if log_is_remote and (not log_is_retrieved or options.force_remote):
             logpath = os.path.normpath(get_remote_workflow_run_job_dir(
-                workflow_id, point, task, options.submit_num,
+                workflow_id, point, task, submit_num,
                 options.filename))
             tail_tmpl = platform["tail command template"]
             # Reinvoke the cat-log command on the remote account.
             cmd = ['cat-log', *verbosity_to_opts(cylc.flow.flags.verbosity)]
             for item in [logpath, mode, tail_tmpl]:
                 cmd.append('--remote-arg=%s' % shlex.quote(item))
             if batchview_cmd:
                 cmd.append('--remote-arg=%s' % shlex.quote(batchview_cmd))
+            if options.prepend_path:
+                cmd.append('--prepend-path')
             cmd.append(workflow_id)
             # TODO: Add Intelligent Host selection to this
             with suppress(KeyboardInterrupt):
                 # (Ctrl-C while tailing)
                 # NOTE: This will raise NoHostsError if the platform is not
                 # contactable
                 remote_cylc_cmd(
@@ -416,13 +567,19 @@
                     capture_process=False,
                     manage=(mode == 'tail'),
                     text=False
                 )
         else:
             # Local task job or local job log.
             logpath = os.path.normpath(get_workflow_run_job_dir(
-                workflow_id, point, task, options.submit_num,
+                workflow_id, point, task, submit_num,
                 options.filename))
             tail_tmpl = os.path.expandvars(platform["tail command template"])
-            out = view_log(logpath, mode, tail_tmpl, batchview_cmd,
-                           color=color)
+            out = view_log(
+                logpath,
+                mode,
+                tail_tmpl,
+                batchview_cmd,
+                color=color,
+                prepend_path=options.prepend_path,
+            )
             sys.exit(out)
```

### Comparing `cylc-flow-8.1.2/cylc/flow/scripts/check_versions.py` & `cylc-flow-8.1.3/cylc/flow/scripts/check_versions.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/scripts/clean.py` & `cylc-flow-8.1.3/cylc/flow/scripts/clean.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,23 +189,25 @@
         LOG.warning(f"No workflows matching {', '.join(ids)}")
         return
 
     workflows.sort()
     if multi_mode and not opts.skip_interactive:
         prompt(workflows)  # prompt for approval or exit
 
-    failed = []
+    failed = {}
     for workflow in sorted(workflows):
         try:
             init_clean(workflow, opts)
         except Exception as exc:
-            failed.append(workflow)
-            LOG.warning(exc)
+            failed[workflow] = exc
     if failed:
-        raise CylcError(f"Clean failed: {', '.join(failed)}")
+        msg = "Clean failed:"
+        for workflow, exc_message in failed.items():
+            msg += f"\nWorkflow: {workflow}\nError: {exc_message}"
+        raise CylcError(msg)
 
 
 @cli_function(get_option_parser)
 def main(_, opts: 'Values', *ids: str):
     if cylc.flow.flags.verbosity < 2:
         disable_timestamps(LOG)
```

### Comparing `cylc-flow-8.1.2/cylc/flow/scripts/client.py` & `cylc-flow-8.1.3/cylc/flow/scripts/client.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/scripts/common.py` & `cylc-flow-8.1.3/cylc/flow/scripts/common.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/scripts/completion_server.py` & `cylc-flow-8.1.3/cylc/flow/scripts/completion_server.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/scripts/config.py` & `cylc-flow-8.1.3/cylc/flow/scripts/config.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/scripts/cycle_point.py` & `cylc-flow-8.1.3/cylc/flow/scripts/cycle_point.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/scripts/cylc.py` & `cylc-flow-8.1.3/cylc/flow/scripts/cylc.py`

 * *Files 1% similar despite different names*

```diff
@@ -387,20 +387,23 @@
         yield (cmd, desc, usage)
 
 
 def print_id_help():
     print(ID_HELP)
 
 
-def print_license():
-    print(
-        pkg_resources.get_distribution('cylc-flow').get_resource_string(
-            __name__, 'COPYING'
-        ).decode()
-    )
+def print_license() -> None:
+    try:
+        from importlib.metadata import files
+    except ImportError:
+        from importlib_metadata import files
+    license_file = next(filter(
+        lambda f: f.name == 'COPYING', files('cylc-flow')
+    ))
+    print(license_file.read_text())
 
 
 def print_command_list(commands=None, indent=0):
     """Print list of Cylc commands.
 
     Args:
         commands (list):
```

### Comparing `cylc-flow-8.1.2/cylc/flow/scripts/diff.py` & `cylc-flow-8.1.3/cylc/flow/scripts/diff.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/scripts/dump.py` & `cylc-flow-8.1.3/cylc/flow/scripts/dump.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/scripts/ext_trigger.py` & `cylc-flow-8.1.3/cylc/flow/scripts/ext_trigger.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/scripts/function_run.py` & `cylc-flow-8.1.3/cylc/flow/scripts/function_run.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/scripts/get_resources.py` & `cylc-flow-8.1.3/cylc/flow/scripts/get_resources.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/scripts/get_workflow_contact.py` & `cylc-flow-8.1.3/cylc/flow/scripts/get_workflow_contact.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/scripts/get_workflow_version.py` & `cylc-flow-8.1.3/cylc/flow/scripts/get_workflow_version.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/scripts/graph.py` & `cylc-flow-8.1.3/cylc/flow/scripts/graph.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/scripts/hold.py` & `cylc-flow-8.1.3/cylc/flow/scripts/hold.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/scripts/install.py` & `cylc-flow-8.1.3/cylc/flow/scripts/install.py`

 * *Files 0% similar despite different names*

```diff
@@ -211,20 +211,24 @@
     """Print any instances of wf_name that are already active."""
     opts = Values({
         'name': [f'{wf_name}/*'],
         'states': {'running', 'paused', 'stopping'},
         'source': False,
         'ping': ping,  # get status of scanned workflows
     })
-    active = [
-        item async for item in get_pipe(
-            opts, None,
-            scan_dir=get_workflow_run_dir(wf_name)  # restricted scan
-        )
-    ]
+    active = sorted(
+        [
+            item async for item in get_pipe(
+                opts,
+                None,
+                scan_dir=get_workflow_run_dir(wf_name)  # restricted scan
+            )
+        ],
+        key=lambda flow: flow['name']
+    )
     if active:
         n = len(active)
         grammar = (
             ["s", "are", "them all"]
             if n > 1 else
             ["", "is", "it"]
         )
```

### Comparing `cylc-flow-8.1.2/cylc/flow/scripts/jobs_kill.py` & `cylc-flow-8.1.3/cylc/flow/scripts/jobs_kill.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/scripts/jobs_poll.py` & `cylc-flow-8.1.3/cylc/flow/scripts/jobs_poll.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/scripts/jobs_submit.py` & `cylc-flow-8.1.3/cylc/flow/scripts/jobs_submit.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/scripts/kill.py` & `cylc-flow-8.1.3/cylc/flow/scripts/kill.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/scripts/lint.py` & `cylc-flow-8.1.3/cylc/flow/scripts/lint.py`

 * *Files 0% similar despite different names*

```diff
@@ -269,15 +269,15 @@
     if tomlfile.is_file():
         try:
             loadeddata = tomli.loads(tomlfile.read_text())
         except tomli.TOMLDecodeError as exc:
             raise CylcError(f'pyproject.toml did not load: {exc}')
 
         if any(
-            [i in loadeddata for i in ['cylc-lint', 'cylclint', 'cylc_lint']]
+            i in loadeddata for i in ['cylc-lint', 'cylclint', 'cylc_lint']
         ):
             for key in keys:
                 tomldata[key] = loadeddata.get('cylc-lint').get(key, [])
             validate_toml_items(tomldata)
     if not tomldata:
         tomldata = {key: [] for key in keys}
     return tomldata
```

### Comparing `cylc-flow-8.1.2/cylc/flow/scripts/list.py` & `cylc-flow-8.1.3/cylc/flow/scripts/list.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/scripts/message.py` & `cylc-flow-8.1.3/cylc/flow/scripts/message.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,26 @@
 
 Each message can be prefixed with a severity level using the syntax
 'SEVERITY:MESSAGE' (colons cannot be used unless such a prefix is provided).
 
 The default message severity is INFO. The --severity=SEVERITY option can be
 used to set the default severity level for all unprefixed messages.
 
+Increased severity will make messages more visible in workflow logs, using
+colour and format changes. DEBUG messages will not be shown in logs by default.
+
+The severity levels are those of the Python Logging Library
+https://docs.python.org/3/library/logging.html#logging-levels:
+
+- CRITICAL
+- ERROR
+- WARNING
+- INFO
+- DEBUG
+
 Note:
   To abort a job script with a custom error message, use cylc__job_abort:
     cylc__job_abort 'message...'
   (For technical reasons this is a shell function, not a cylc sub-command).
 
 For backward compatibility, if number of arguments is less than or equal to 2,
 the command assumes the classic interface, where all arguments are messages.
```

### Comparing `cylc-flow-8.1.2/cylc/flow/scripts/pause.py` & `cylc-flow-8.1.3/cylc/flow/scripts/pause.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/scripts/ping.py` & `cylc-flow-8.1.3/cylc/flow/scripts/ping.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/scripts/play.py` & `cylc-flow-8.1.3/cylc/flow/scripts/play.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/scripts/poll.py` & `cylc-flow-8.1.3/cylc/flow/scripts/poll.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/scripts/psutil.py` & `cylc-flow-8.1.3/cylc/flow/scripts/psutil.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/scripts/reinstall.py` & `cylc-flow-8.1.3/cylc/flow/scripts/reinstall.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/scripts/release.py` & `cylc-flow-8.1.3/cylc/flow/scripts/release.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/scripts/reload.py` & `cylc-flow-8.1.3/cylc/flow/scripts/reload.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/scripts/remote_init.py` & `cylc-flow-8.1.3/cylc/flow/scripts/remote_init.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/scripts/remote_tidy.py` & `cylc-flow-8.1.3/cylc/flow/scripts/remote_tidy.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/scripts/remove.py` & `cylc-flow-8.1.3/cylc/flow/scripts/remove.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/scripts/report_timings.py` & `cylc-flow-8.1.3/cylc/flow/scripts/report_timings.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/scripts/scan.py` & `cylc-flow-8.1.3/cylc/flow/scripts/scan.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/scripts/set_outputs.py` & `cylc-flow-8.1.3/cylc/flow/scripts/set_outputs.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/scripts/set_verbosity.py` & `cylc-flow-8.1.3/cylc/flow/scripts/set_verbosity.py`

 * *Files 10% similar despite different names*

```diff
@@ -62,32 +62,30 @@
             ('LEVEL', ', '.join(LOG_LEVELS.keys())),
             WORKFLOW_ID_MULTI_ARG_DOC,
         ]
     )
     return parser
 
 
-async def run(options: 'Values', severity, workflow_id) -> None:
+async def run(options: 'Values', severity: str, workflow_id: str) -> None:
     pclient = get_client(workflow_id, timeout=options.comms_timeout)
 
     mutation_kwargs = {
         'request_string': MUTATION,
         'variables': {
             'wFlows': [workflow_id],
             'level': severity,
         }
     }
 
     await pclient.async_request('graphql', mutation_kwargs)
 
 
 @cli_function(get_option_parser)
-def main(parser: COP, options: 'Values', severity_str: str, *ids) -> None:
-    try:
-        severity = LOG_LEVELS[severity_str]
-    except KeyError:
-        raise InputError("Illegal logging level, %s" % severity_str)
+def main(parser: COP, options: 'Values', severity: str, *ids: str) -> None:
+    if severity not in LOG_LEVELS:
+        raise InputError(f"Illegal logging level, {severity}")
     call_multi(
         partial(run, options, severity),
         *ids,
         constraint='workflows',
     )
```

### Comparing `cylc-flow-8.1.2/cylc/flow/scripts/show.py` & `cylc-flow-8.1.3/cylc/flow/scripts/show.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/scripts/stop.py` & `cylc-flow-8.1.3/cylc/flow/scripts/stop.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/scripts/subscribe.py` & `cylc-flow-8.1.3/cylc/flow/scripts/subscribe.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/scripts/trigger.py` & `cylc-flow-8.1.3/cylc/flow/scripts/trigger.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/scripts/tui.py` & `cylc-flow-8.1.3/cylc/flow/scripts/tui.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/scripts/validate.py` & `cylc-flow-8.1.3/cylc/flow/scripts/validate.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/scripts/validate_install_play.py` & `cylc-flow-8.1.3/cylc/flow/scripts/validate_install_play.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/scripts/validate_reinstall.py` & `cylc-flow-8.1.3/cylc/flow/scripts/validate_reinstall.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,14 +121,15 @@
 
 
 def vro_cli(parser: COP, options: 'Values', workflow_id: str):
     """Run Cylc (re)validate - reinstall - reload in sequence."""
     # Attempt to work out whether the workflow is running.
     # We are trying to avoid reinstalling then subsequently being
     # unable to play or reload because we cannot identify workflow state.
+    unparsed_wid = workflow_id
     workflow_id, *_ = parse_id(
         workflow_id,
         constraint='workflows',
     )
 
     # Use this interface instead of scan, because it can have an ambiguous
     # outcome which we want to capture before we install.
@@ -174,18 +175,18 @@
         log_subcommand('reload', workflow_id)
         cylc_reload(options, workflow_id)
 
     # run play anyway, to play a stopped workflow:
     else:
         cleanup_sysargv(
             'play',
-            workflow_id,
+            unparsed_wid,
             options,
             compound_script_opts=VR_OPTIONS,
             script_opts=(
                 PLAY_OPTIONS + CYLC_ROSE_OPTIONS
                 + parser.get_std_options()
             ),
             source='',  # Intentionally blank
         )
-        log_subcommand('play', workflow_id)
+        log_subcommand(*sys.argv[1:])
         scheduler_cli(options, workflow_id)
```

### Comparing `cylc-flow-8.1.2/cylc/flow/scripts/view.py` & `cylc-flow-8.1.3/cylc/flow/scripts/view.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/scripts/workflow_state.py` & `cylc-flow-8.1.3/cylc/flow/scripts/workflow_state.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/subprocctx.py` & `cylc-flow-8.1.3/cylc/flow/subprocctx.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/subprocpool.py` & `cylc-flow-8.1.3/cylc/flow/subprocpool.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 from time import time
 from subprocess import DEVNULL, run  # nosec
 from typing import Any, Callable, List, Optional
 
 from cylc.flow import LOG
 from cylc.flow.cfgspec.glbl_cfg import glbl_cfg
 from cylc.flow.cylc_subproc import procopen
+from cylc.flow.exceptions import PlatformLookupError
 from cylc.flow.hostuserutil import is_remote_host
 from cylc.flow.platforms import (
     log_platform_event,
     get_platform,
 )
 from cylc.flow.task_events_mgr import TaskJobLogsRetrieveContext
 from cylc.flow.wallclock import get_current_time_string
@@ -483,15 +484,22 @@
                 return False
         ctx.timestamp = get_current_time_string()
 
         # If cmd is fileinstall, which uses rsync, get a platform so
         # that you can use that platform's ssh command.
         platform = None
         if isinstance(ctx.cmd_key, TaskJobLogsRetrieveContext):
-            platform = get_platform(ctx.cmd_key.platform_name)
+            try:
+                platform = get_platform(ctx.cmd_key.platform_name)
+            except PlatformLookupError:
+                log_platform_event(
+                    'Unable to retrieve job logs.',
+                    {'name': ctx.cmd_key.platform_name},
+                    level='warning',
+                )
         elif callback_args:
             platform = callback_args[0]
             if not (
                 isinstance(platform, dict)
                 and 'ssh command' in platform
                 and 'name' in platform
             ):
@@ -571,17 +579,18 @@
                 else 'ssh'
             )
             ssh_test_cmd = shlex.split(f'{ssh_cmd} {ctx.host} true')
             LOG.info(
                 f'testing connectivity for {ctx.host} using {ssh_test_cmd}'
             )
             ssh_test = run(
-                shlex.split(f'{ssh_cmd} {ctx.host} true'),
+                shlex.split(f'{ssh_cmd} {ctx.host} true'),  # nosec B603 *
                 capture_output=True
             )
+            # * (command is trusted input)
             if ssh_test.returncode == 255:
                 rsync_255_fail = True
         elif (
             ctx.cmd[0] == rsync_cmd[0]
             and ctx.ret_code == 255
         ):
             rsync_255_fail = True
```

### Comparing `cylc-flow-8.1.2/cylc/flow/task_action_timer.py` & `cylc-flow-8.1.3/cylc/flow/task_action_timer.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/task_events_mgr.py` & `cylc-flow-8.1.3/cylc/flow/task_events_mgr.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,26 +33,29 @@
 from shlex import quote
 import shlex
 from time import time
 from typing import TYPE_CHECKING, Optional, Union, cast
 
 from cylc.flow import LOG, LOG_LEVELS
 from cylc.flow.cfgspec.glbl_cfg import glbl_cfg
-from cylc.flow.exceptions import NoHostsError
+from cylc.flow.exceptions import NoHostsError, PlatformLookupError
 from cylc.flow.hostuserutil import get_host, get_user, is_remote_platform
 from cylc.flow.parsec.config import ItemNotFoundError
 from cylc.flow.pathutil import (
     get_remote_workflow_run_job_dir,
     get_workflow_run_job_dir)
 from cylc.flow.subprocctx import SubFuncContext, SubProcContext
 from cylc.flow.task_action_timer import (
     TaskActionTimer,
     TimerFlags
 )
-from cylc.flow.platforms import get_platform, get_host_from_platform
+from cylc.flow.platforms import (
+    get_platform, get_host_from_platform,
+    log_platform_event
+)
 from cylc.flow.task_job_logs import (
     get_task_job_log,
     get_task_job_activity_log,
     JOB_LOG_OUT,
     JOB_LOG_ERR,
 )
 from cylc.flow.task_message import (
@@ -937,16 +940,16 @@
                 if value is not None:
                     return value
         return default
 
     def _process_job_logs_retrieval(self, schd, ctx, id_keys):
         """Process retrieval of task job logs from remote user@host."""
         # get a host to run retrieval on
-        platform = get_platform(ctx.platform_name)
         try:
+            platform = get_platform(ctx.platform_name)
             host = get_host_from_platform(platform, bad_hosts=self.bad_hosts)
         except NoHostsError:
             # All of the platforms hosts have been found to be uncontactable.
             # Reset the bad hosts to allow retrieval retry to take place.
             self.bad_hosts -= set(platform['hosts'])
             try:
                 # Get a new host and try again.
@@ -957,14 +960,21 @@
             except NoHostsError:
                 # We really can't get a host to try on e.g. no hosts
                 # configured (shouldn't happen). Nothing more we can do here,
                 # move onto the next submission retry.
                 for id_key in id_keys:
                     self.unset_waiting_event_timer(id_key)
                 return
+        except PlatformLookupError:
+            log_platform_event(
+                'Unable to retrieve job logs.',
+                {'name': ctx.platform_name},
+                level='warning',
+            )
+            return
 
         # construct the retrieval command
         ssh_str = str(platform["ssh command"])
         rsync_str = str(platform["retrieve job logs command"])
         cmd = shlex.split(rsync_str) + ["--rsh=" + ssh_str]
         if LOG.isEnabledFor(DEBUG):
             cmd.append("-v")
```

### Comparing `cylc-flow-8.1.2/cylc/flow/task_id.py` & `cylc-flow-8.1.3/cylc/flow/task_id.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/task_job_logs.py` & `cylc-flow-8.1.3/cylc/flow/task_job_logs.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/task_job_mgr.py` & `cylc-flow-8.1.3/cylc/flow/task_job_mgr.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,16 +54,14 @@
 from cylc.flow.job_file import JobFileWriter
 from cylc.flow.parsec.util import (
     pdeepcopy,
     poverride
 )
 from cylc.flow.pathutil import get_remote_workflow_run_job_dir
 from cylc.flow.platforms import (
-    HOST_REC_COMMAND,
-    PLATFORM_REC_COMMAND,
     get_host_from_platform,
     get_install_target_from_platform,
     get_localhost_install_target,
     get_platform,
 )
 from cylc.flow.remote import construct_ssh_cmd
 from cylc.flow.subprocctx import SubProcContext
@@ -153,15 +151,15 @@
         self.task_events_mgr = task_events_mgr
         self.data_store_mgr = data_store_mgr
         self.job_file_writer = JobFileWriter()
         self.job_runner_mgr = self.job_file_writer.job_runner_mgr
         self.bad_hosts = bad_hosts
         self.bad_hosts_to_clear = set()
         self.task_remote_mgr = TaskRemoteMgr(
-            workflow, proc_pool, self.bad_hosts)
+            workflow, proc_pool, self.bad_hosts, self.workflow_db_mgr)
 
     def check_task_jobs(self, workflow, task_pool):
         """Check submission and execution timeout and polling timers.
 
         Poll tasks that have timed out and/or have reached next polling time.
         """
         now = time()
@@ -306,15 +304,15 @@
                     use_next_platform_in_group = False
                     if itask.tdef.rtconfig['platform']:
                         try:
                             platform = get_platform(
                                 itask.tdef.rtconfig['platform'],
                                 bad_hosts=self.bad_hosts
                             )
-                        except NoPlatformsError:
+                        except PlatformLookupError:
                             pass
                         else:
                             # If were able to select a new platform;
                             if platform and platform != itask.platform:
                                 use_next_platform_in_group = True
 
                     if use_next_platform_in_group:
@@ -626,19 +624,20 @@
             timestamp, _, content = line.split("|")
         except ValueError:
             pass
         else:
             line = "%s %s" % (timestamp, content)
         job_activity_log = get_task_job_activity_log(
             workflow, itask.point, itask.tdef.name)
+        if not line.endswith("\n"):
+            line += "\n"
+        line = host + line
         try:
-            with open(os.path.expandvars(job_activity_log), "ab") as handle:
-                if not line.endswith("\n"):
-                    line += "\n"
-                handle.write((host + line).encode())
+            with open(os.path.expandvars(job_activity_log), "a") as handle:
+                handle.write(line)
         except IOError as exc:
             LOG.warning("%s: write failed\n%s" % (job_activity_log, exc))
             LOG.warning(f"[{itask}] {host}{line}")
 
     def _kill_task_jobs_callback(self, ctx, workflow, itasks):
         """Callback when kill tasks command exits."""
         self._manip_task_jobs_callback(
@@ -908,15 +907,27 @@
             platform_name = itask.platform['name']
             if platform_name not in auth_itasks:
                 auth_itasks[platform_name] = []
             auth_itasks[platform_name].append(itask)
 
         # Go through each list of itasks and carry out commands as required.
         for platform_name, itasks in sorted(auth_itasks.items()):
-            platform = get_platform(platform_name)
+            try:
+                platform = get_platform(platform_name)
+            except NoPlatformsError:
+                LOG.error(
+                    f'Unable to run command {cmd_key}: Unable to find'
+                    f' platform {platform_name} with accessible hosts.'
+                )
+            except PlatformLookupError:
+                LOG.error(
+                    f'Unable to run command {cmd_key}: Unable to find'
+                    f' platform {platform_name}.'
+                )
+                continue
             if is_remote_platform(platform):
                 remote_mode = True
                 cmd = [cmd_key]
             else:
                 cmd = ["cylc", cmd_key]
                 remote_mode = False
             if LOG.isEnabledFor(DEBUG):
@@ -1116,20 +1127,20 @@
                 "logic should not be used. In this case for the task "
                 f"\"{itask.identity}\" the following are not compatible:\n"
             )
 
         host_n, platform_name = None, None
         try:
             if rtconfig['remote']['host'] is not None:
-                host_n = self.task_remote_mgr.subshell_eval(
-                    rtconfig['remote']['host'], HOST_REC_COMMAND
+                host_n = self.task_remote_mgr.eval_host(
+                    rtconfig['remote']['host']
                 )
             else:
-                platform_name = self.task_remote_mgr.subshell_eval(
-                    rtconfig['platform'], PLATFORM_REC_COMMAND
+                platform_name = self.task_remote_mgr.eval_platform(
+                    rtconfig['platform']
                 )
         except PlatformError as exc:
             itask.waiting_on_job_prep = False
             itask.summary['platforms_used'][itask.submit_num] = ''
             # Retry delays, needed for the try_num
             self._create_job_log_path(workflow, itask)
             self._set_retry_timers(itask, rtconfig)
@@ -1161,15 +1172,14 @@
                 )
                 rtconfig['remote']['host'] = host_n
 
             try:
                 platform = get_platform(
                     rtconfig, itask.tdef.name, bad_hosts=self.bad_hosts
                 )
-
             except PlatformLookupError as exc:
                 itask.waiting_on_job_prep = False
                 itask.summary['platforms_used'][itask.submit_num] = ''
                 # Retry delays, needed for the try_num
                 self._create_job_log_path(workflow, itask)
                 self._prep_submit_task_job_error(
                     workflow, itask, '(platform not defined)', exc)
@@ -1281,15 +1291,16 @@
     ):
         """Return a job config.
 
         Note that rtconfig should have any broadcasts applied.
         """
         return {
             # NOTE: these fields should match get_simulation_job_conf
-            # TODO: turn this into a namedtuple or similar
+            # TODO: formalise this
+            # https://github.com/cylc/cylc-flow/issues/5387
             'job_runner_name': itask.platform['job runner'],
             'job_runner_command_template': (
                 itask.platform['job runner command template']
             ),
             'dependencies': itask.state.get_resolved_dependencies(),
             'directives': {
                 **itask.platform['directives'], **rtconfig['directives']
```

### Comparing `cylc-flow-8.1.2/cylc/flow/task_message.py` & `cylc-flow-8.1.3/cylc/flow/task_message.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/task_outputs.py` & `cylc-flow-8.1.3/cylc/flow/task_outputs.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/task_pool.py` & `cylc-flow-8.1.3/cylc/flow/task_pool.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,23 +17,30 @@
 """Wrangle task proxies to manage the workflow."""
 
 from contextlib import suppress
 from collections import Counter
 import json
 from time import time
 from typing import (
-    Dict, Iterable, List, Optional,
-    Set, TYPE_CHECKING, Tuple
+    Dict,
+    Iterable,
+    List,
+    Optional,
+    Set,
+    TYPE_CHECKING,
+    Tuple,
+    Union,
 )
 import logging
 
 import cylc.flow.flags
 from cylc.flow import LOG
 from cylc.flow.cycling.loader import get_point, standardise_point_string
-from cylc.flow.exceptions import WorkflowConfigError, PointParsingError
+from cylc.flow.exceptions import (
+    WorkflowConfigError, PointParsingError, PlatformLookupError)
 from cylc.flow.id import Tokens, detokenise
 from cylc.flow.id_cli import contains_fnmatch
 from cylc.flow.id_match import filter_ids
 from cylc.flow.network.resolvers import TaskMsg
 from cylc.flow.workflow_status import StopMode
 from cylc.flow.task_action_timer import TaskActionTimer, TimerFlags
 from cylc.flow.task_events_mgr import (
@@ -124,24 +131,24 @@
         self.abort_task_failed = False
         self.expected_failed_tasks = self.config.get_expected_failed_tasks()
 
         self.orphans: List[str] = []
         self.task_name_list = self.config.get_task_name_list()
         self.task_queue_mgr = IndepQueueManager(
             self.config.cfg['scheduling']['queues'],
-            self.config.get_task_name_list(),
+            self.task_name_list,
             self.config.runtime['descendants']
         )
         self.tasks_to_hold: Set[Tuple[str, 'PointBase']] = set()
 
     def set_stop_task(self, task_id):
         """Set stop after a task."""
         tokens = Tokens(task_id, relative=True)
         name = tokens['task']
-        if name in self.config.get_task_name_list():
+        if name in self.config.taskdefs:
             task_id = TaskID.get_standardised_taskid(task_id)
             LOG.info("Setting stop task: " + task_id)
             self.stop_task_id = task_id
             self.stop_task_finished = False
             self.workflow_db_mgr.put_workflow_stop_task(task_id)
         else:
             LOG.warning("Requested stop task name does not exist: %s" % name)
@@ -170,15 +177,15 @@
         """Load the task pool for the workflow start point.
 
         Add every parentless task out to the runahead limit.
         """
         flow_num = self.flow_mgr.get_new_flow(
             f"original flow from {self.config.start_point}")
         self.compute_runahead()
-        for name in self.config.get_task_name_list():
+        for name in self.task_name_list:
             tdef = self.config.get_taskdef(name)
             point = tdef.first_point(self.config.start_point)
             self.spawn_to_rh_limit(tdef, point, {flow_num})
 
     def db_add_new_flow_rows(self, itask: TaskProxy) -> None:
         """Add new rows to DB task tables that record flow_nums.
 
@@ -417,21 +424,48 @@
             flow_nums_seen.update(itask.flow_nums)
         self.flow_mgr.load_from_db(flow_nums_seen)
 
     def load_abs_outputs_for_restart(self, row_idx, row):
         cycle, name, output = row
         self.abs_outputs_done.add((cycle, name, output))
 
+    def check_task_output(
+        self,
+        cycle: str,
+        task: str,
+        output: str,
+        flow_nums: 'FlowNums',
+    ) -> Union[str, bool]:
+        """Returns truthy if the specified output is satisfied in the DB."""
+        for task_outputs, task_flow_nums in (
+            self.workflow_db_mgr.pri_dao.select_task_outputs(task, cycle)
+        ).items():
+            # loop through matching tasks
+            if flow_nums.intersection(task_flow_nums):
+                # this task is in the right flow
+                task_outputs = json.loads(task_outputs)
+                return (
+                    'satisfied from database'
+                    if output in task_outputs
+                    else False
+                )
+        else:
+            # no matching entries
+            return False
+
     def load_db_task_pool_for_restart(self, row_idx, row):
         """Load tasks from DB task pool/states/jobs tables.
 
         Output completion status is loaded from the DB, and tasks recorded
         as submitted or running are polled to confirm their true status.
         Tasks are added to queues again on release from runahead pool.
 
+        Returns:
+            Names of platform if attempting to look up that platform
+            has led to a PlatformNotFoundError.
         """
         if row_idx == 0:
             LOG.info("LOADING task proxies")
         # Create a task proxy corresponding to this DB entry.
         (cycle, name, flow_nums, flow_wait, is_manual_submit, is_late, status,
          is_held, submit_num, _, platform_name, time_submit, time_run, timeout,
          outputs_str) = row
@@ -443,29 +477,35 @@
                 status=status,
                 is_held=is_held,
                 submit_num=submit_num,
                 is_late=bool(is_late),
                 flow_wait=bool(flow_wait),
                 is_manual_submit=bool(is_manual_submit)
             )
+
         except WorkflowConfigError:
             LOG.exception(
                 f'ignoring task {name} from the workflow run database\n'
                 '(its task definition has probably been deleted).')
         except Exception:
             LOG.exception(f'could not load task {name}')
         else:
             if status in (
                     TASK_STATUS_SUBMITTED,
                     TASK_STATUS_RUNNING,
                     TASK_STATUS_FAILED,
                     TASK_STATUS_SUCCEEDED
             ):
                 # update the task proxy with platform
-                itask.platform = get_platform(platform_name)
+                # If we get a failure from the platform selection function
+                # set task status to submit-failed.
+                try:
+                    itask.platform = get_platform(platform_name)
+                except PlatformLookupError:
+                    return platform_name
 
                 if time_submit:
                     itask.set_summary_time('submitted', time_submit)
                 if time_run:
                     itask.set_summary_time('started', time_run)
                 if timeout is not None:
                     itask.timeout = timeout
@@ -496,20 +536,37 @@
             for prereq_name, prereq_cycle, prereq_output, satisfied in (
                     self.workflow_db_mgr.pri_dao.select_task_prerequisites(
                         cycle,
                         name,
                         flow_nums,
                     )
             ):
-                key = (prereq_cycle, prereq_name, prereq_output)
-                sat[key] = satisfied if satisfied != '0' else False
+                # Prereq satisfaction as recorded in the DB.
+                sat[
+                    (prereq_cycle, prereq_name, prereq_output)
+                ] = satisfied if satisfied != '0' else False
 
             for itask_prereq in itask.state.prerequisites:
-                for key, _ in itask_prereq.satisfied.items():
-                    itask_prereq.satisfied[key] = sat[key]
+                for key in itask_prereq.satisfied.keys():
+                    try:
+                        itask_prereq.satisfied[key] = sat[key]
+                    except KeyError:
+                        # This prereq is not in the DB: new dependencies
+                        # added to an already-spawned task before restart.
+                        # Look through task outputs to see if is has been
+                        # satisfied
+                        prereq_cycle, prereq_task, prereq_output = key
+                        itask_prereq.satisfied[key] = (
+                            self.check_task_output(
+                                prereq_cycle,
+                                prereq_task,
+                                prereq_output,
+                                itask.flow_nums,
+                            )
+                        )
 
             if itask.state_reset(status, is_runahead=True):
                 self.data_store_mgr.delta_task_runahead(itask)
             self.add_to_pool(itask)
 
             # All tasks load as runahead-limited, but finished and manually
             # triggered tasks (incl. --start-task's) can be released now.
@@ -904,16 +961,20 @@
                         f"[{itask}] will not spawn children "
                         "- task definition removed"
                     )
             else:
                 new_task = TaskProxy(
                     self.config.get_taskdef(itask.tdef.name),
                     itask.point, itask.flow_nums, itask.state.status)
-                itask.copy_to_reload_successor(new_task)
+                itask.copy_to_reload_successor(
+                    new_task,
+                    self.check_task_output,
+                )
                 self._swap_out(new_task)
+                self.data_store_mgr.delta_task_prerequisite(new_task)
                 LOG.info(f"[{itask}] reloaded task definition")
                 if itask.state(*TASK_STATUSES_ACTIVE):
                     LOG.warning(
                         f"[{itask}] active with pre-reload settings"
                     )
                 elif itask.state(TASK_STATUS_PREPARING):
                     # Job file might have been written at this point?
@@ -921,15 +982,15 @@
                         f"[{itask}] may be active with pre-reload settings"
                     )
 
         # Reassign live tasks to the internal queue
         del self.task_queue_mgr
         self.task_queue_mgr = IndepQueueManager(
             self.config.cfg['scheduling']['queues'],
-            self.config.get_task_name_list(),
+            self.task_name_list,
             self.config.runtime['descendants']
         )
 
         # Now queue all tasks that are ready to run
         for itask in self.get_tasks():
             # Recreate data store elements from main pool.
             self.create_data_store_elements(itask)
@@ -1381,15 +1442,15 @@
                     and c_task.point <= self.runahead_limit_point
                 ):
                     self.rh_release_and_queue(c_task)
 
     def can_spawn(self, name: str, point: 'PointBase') -> bool:
         """Return True if the task with the given name & point is within
         various workflow limits."""
-        if name not in self.config.get_task_name_list():
+        if name not in self.config.taskdefs:
             LOG.debug('No task definition %s', name)
             return False
         # Don't spawn outside of graph limits.
         # TODO: is it possible for initial_point to not be defined??
         # (see also the similar check + log message in scheduler.py)
         if self.config.initial_point and point < self.config.initial_point:
             # Attempted manual trigger prior to FCP
```

### Comparing `cylc-flow-8.1.2/cylc/flow/task_proxy.py` & `cylc-flow-8.1.3/cylc/flow/task_proxy.py`

 * *Files 4% similar despite different names*

```diff
@@ -267,15 +267,15 @@
         return (
             f"{self.identity} "
             f"{self.state} "
             f"job:{self.submit_num:02d}"
             f" flows:{','.join(str(i) for i in self.flow_nums) or 'none'}"
         )
 
-    def copy_to_reload_successor(self, reload_successor):
+    def copy_to_reload_successor(self, reload_successor, check_output):
         """Copy attributes to successor on reload of this task proxy."""
         self.reload_successor = reload_successor
         reload_successor.submit_num = self.submit_num
         reload_successor.flow_wait = self.flow_wait
         reload_successor.is_manual_submit = self.is_manual_submit
         reload_successor.summary = self.summary
         reload_successor.local_job_file_path = self.local_job_file_path
@@ -284,15 +284,42 @@
         reload_successor.job_vacated = self.job_vacated
         reload_successor.poll_timer = self.poll_timer
         reload_successor.timeout = self.timeout
         reload_successor.state.outputs = self.state.outputs
         reload_successor.state.is_held = self.state.is_held
         reload_successor.state.is_runahead = self.state.is_runahead
         reload_successor.state.is_updated = self.state.is_updated
-        reload_successor.state.prerequisites = self.state.prerequisites
+
+        # Prerequisites: the graph might have changed before reload, so
+        # we need to use the new prerequisites but update them with the
+        # pre-reload state of prerequisites that still exist post-reload.
+
+        # Get all prereq states, e.g. {('1', 'c', 'succeeded'): False, ...}
+        pre_reload = {
+            k: v
+            for pre in self.state.prerequisites
+            for (k, v) in pre.satisfied.items()
+        }
+        # Use them to update the new prerequisites.
+        # - unchanged prerequisites will keep their pre-reload state.
+        # - removed prerequisites will not be carried over
+        # - added prerequisites will be recorded as unsatisfied
+        #   NOTE: even if the corresponding output was completed pre-reload!
+        for pre in reload_successor.state.prerequisites:
+            for k in pre.satisfied.keys():
+                try:
+                    pre.satisfied[k] = pre_reload[k]
+                except KeyError:
+                    # Look through task outputs to see if is has been
+                    # satisfied
+                    pre.satisfied[k] = check_output(
+                        *k,
+                        self.flow_nums,
+                    )
+
         reload_successor.state.xtriggers.update({
             # copy across any special "_cylc" xtriggers which were added
             # dynamically at runtime (i.e. execution retry xtriggers)
             key: value
             for key, value in self.state.xtriggers.items()
             if key.startswith('_cylc')
         })
```

### Comparing `cylc-flow-8.1.2/cylc/flow/task_queues/__init__.py` & `cylc-flow-8.1.3/cylc/flow/task_queues/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/task_queues/independent.py` & `cylc-flow-8.1.3/cylc/flow/task_queues/independent.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/task_remote_cmd.py` & `cylc-flow-8.1.3/cylc/flow/task_remote_cmd.py`

 * *Files 5% similar despite different names*

```diff
@@ -147,18 +147,19 @@
     oldcwd = os.getcwd()
     os.chdir(rund)
     # Extract job.sh from library, for use in job scripts.
     get_resources(
         'job.sh',
         os.path.join(WorkflowFiles.Service.DIRNAME, 'etc')
     )
+    # Extract sent contact file from stdin:
     try:
-        tarhandle = tarfile.open(fileobj=sys.stdin.buffer, mode='r|')
-        tarhandle.extractall()
-        tarhandle.close()
+        with tarfile.open(fileobj=sys.stdin.buffer, mode='r|') as tarhandle:
+            tarhandle.extractall()  # nosec B202 - there should not be any
+            # untrusted members in the tar stream, only the contact file
     finally:
         os.chdir(oldcwd)
     print("KEYSTART", end='')
     with open(client_pub_keyinfo.full_key_path) as keyfile:
         print(keyfile.read(), end='KEYEND')
     print(REMOTE_INIT_DONE)
     return
```

### Comparing `cylc-flow-8.1.2/cylc/flow/task_remote_mgr.py` & `cylc-flow-8.1.3/cylc/flow/task_remote_mgr.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,34 +28,38 @@
 from cylc.flow.option_parsers import verbosity_to_opts
 import os
 from shlex import quote
 import re
 from subprocess import Popen, PIPE, DEVNULL
 import tarfile
 from time import sleep, time
-from typing import Any, Deque, Dict, TYPE_CHECKING, List, NamedTuple, Tuple
+from typing import (
+    Any, Deque, Dict, TYPE_CHECKING, List,
+    NamedTuple, Optional, Set, Tuple
+)
 
 from cylc.flow import LOG
-from cylc.flow.exceptions import PlatformError
+from cylc.flow.exceptions import (
+    PlatformError, PlatformLookupError, NoHostsError, NoPlatformsError
+)
 import cylc.flow.flags
-from cylc.flow.hostuserutil import is_remote_host
 from cylc.flow.network.client_factory import CommsMeth
 from cylc.flow.pathutil import (
     get_dirs_to_symlink,
     get_remote_workflow_run_dir,
     get_workflow_file_install_log_dir,
     get_workflow_run_dir,
 )
 from cylc.flow.platforms import (
-    NoHostsError,
-    PlatformLookupError,
+    HOST_REC_COMMAND,
+    PLATFORM_REC_COMMAND,
     get_host_from_platform,
     get_install_target_from_platform,
+    get_install_target_to_platforms_map,
     get_localhost_install_target,
-    get_random_platform_for_install_target,
     log_platform_event,
 )
 from cylc.flow.remote import construct_rsync_over_ssh_cmd, construct_ssh_cmd
 from cylc.flow.subprocctx import SubProcContext
 from cylc.flow.util import format_cmd
 from cylc.flow.workflow_files import (
     KeyInfo,
@@ -63,14 +67,15 @@
     KeyType,
     WorkflowFiles,
     get_contact_file_path,
     get_workflow_srv_dir,
 )
 
 from cylc.flow.loggingutil import get_next_log_number, get_sorted_logs_by_time
+from cylc.flow.hostuserutil import is_remote_host
 
 if TYPE_CHECKING:
     from zmq.auth.thread import ThreadAuthenticator
 
 # Remote installation literals
 REMOTE_INIT_DONE = 'REMOTE INIT DONE'
 REMOTE_INIT_FAILED = 'REMOTE INIT FAILED'
@@ -87,97 +92,107 @@
     host: str
     proc: 'Popen[str]'
 
 
 class TaskRemoteMgr:
     """Manage task remote initialisation, tidy, selection."""
 
-    def __init__(self, workflow, proc_pool, bad_hosts):
+    def __init__(self, workflow, proc_pool, bad_hosts, db_mgr):
         self.workflow = workflow
         self.proc_pool = proc_pool
         # self.remote_command_map = {command: host|PlatformError|None}
         self.remote_command_map = {}
         # self.remote_init_map = {(install target): status, ...}
         self.remote_init_map = {}
         self.uuid_str = None
         # This flag is turned on when a host init/select command completes
         self.ready = False
         self.rsync_includes = None
         self.bad_hosts = bad_hosts
         self.is_reload = False
         self.is_restart = False
+        self.db_mgr = db_mgr
 
-    def subshell_eval(self, command, command_pattern, host_check=True):
-        """Evaluate a task platform from a subshell string.
-
-        At Cylc 7, from a host string.
+    def _subshell_eval(
+        self, eval_str: str, command_pattern: re.Pattern
+    ) -> Optional[str]:
+        """Evaluate a platform or host from a possible subshell string.
 
         Arguments:
-            command (str):
-                An explicit host name, a command in back-tick or $(command)
-                format, or an environment variable holding a hostname.
-            command_pattern (re.Pattern):
+            eval_str:
+                An explicit host/platform name, a command, or an environment
+                variable holding a host/patform name.
+            command_pattern:
                 A compiled regex pattern designed to match subshell strings.
-            host_check (bool):
-                A flag to enable remote testing. If True, and if the command
-                is running locally, then it will return 'localhost'.
 
-        Return (str):
+        Return:
             - None if evaluation of command is still taking place.
-            - If command is not defined or the evaluated name is equivalent
-              to 'localhost', _and_ host_check is set to True then
-              'localhost'
-            - Otherwise, return the evaluated host name on success.
+            - 'localhost' if string is empty/not defined.
+            - Otherwise, return the evaluated host/platform name on success.
 
         Raise PlatformError on error.
 
         """
-        # BACK COMPAT: references to "host"
-        # remove at:
-        #     Cylc8.x
-        if not command:
+        if not eval_str:
             return 'localhost'
 
         # Host selection command: $(command) or `command`
-        match = command_pattern.match(command)
+        match = command_pattern.match(eval_str)
         if match:
             cmd_str = match.groups()[1]
             if cmd_str in self.remote_command_map:
                 # Command recently launched
                 value = self.remote_command_map[cmd_str]
                 if isinstance(value, PlatformError):
                     raise value  # command failed
-                elif value is None:
-                    return  # command not yet ready
-                else:
-                    command = value  # command succeeded
+                if value is None:
+                    return None  # command not yet ready
+                eval_str = value  # command succeeded
             else:
                 # Command not launched (or already reset)
                 self.proc_pool.put_command(
                     SubProcContext(
                         'remote-host-select',
                         ['bash', '-c', cmd_str],
-                        env=dict(os.environ)),
+                        env=dict(os.environ)
+                    ),
                     callback=self._subshell_eval_callback,
                     callback_args=[cmd_str]
                 )
                 self.remote_command_map[cmd_str] = None
-                return self.remote_command_map[cmd_str]
+                return None
 
         # Environment variable substitution
-        command = os.path.expandvars(command)
-        # Remote?
-        # TODO - Remove at Cylc 8.x as this only makes sense with host logic
-        if host_check is True:
-            if is_remote_host(command):
-                return command
-            else:
-                return 'localhost'
-        else:
-            return command
+        return os.path.expandvars(eval_str)
+
+    # BACK COMPAT: references to "host"
+        # remove at:
+        #     Cylc8.x
+    def eval_host(self, host_str: str) -> Optional[str]:
+        """Evaluate a host from a possible subshell string.
+
+        Args:
+            host_str: An explicit host name, a command in back-tick or
+                $(command) format, or an environment variable holding
+                a hostname.
+
+        Returns 'localhost' if evaluated name is equivalent
+        (e.g. localhost4.localdomain4).
+        """
+        host = self._subshell_eval(host_str, HOST_REC_COMMAND)
+        return host if is_remote_host(host) else 'localhost'
+
+    def eval_platform(self, platform_str: str) -> Optional[str]:
+        """Evaluate a platform from a possible subshell string.
+
+        Args:
+            platform_str: An explicit platform name, a command in $(command)
+                format, or an environment variable holding a platform name.
+        """
+        return self._subshell_eval(platform_str, PLATFORM_REC_COMMAND)
 
     def subshell_eval_reset(self):
         """Reset remote eval subshell results.
 
         This is normally called after the results are consumed.
         """
         for key, value in list(self.remote_command_map.copy().items()):
@@ -208,29 +223,30 @@
 
         # Set status of install target to in progress while waiting for remote
         # initialisation to finish
         self.remote_init_map[install_target] = REMOTE_INIT_IN_PROGRESS
 
         # Determine what items to install
         comms_meth: CommsMeth = CommsMeth(platform['communication method'])
-        items = self._remote_init_items(comms_meth)
+        remote_init_items = self._remote_init_items(comms_meth)
 
         # Create a TAR archive with the service files,
         # so they can be sent later via SSH's STDIN to the task remote.
         tmphandle = self.proc_pool.get_temporary_file()
-        tarhandle = tarfile.open(fileobj=tmphandle, mode='w')
-        for path, arcname in items:
-            tarhandle.add(path, arcname=arcname)
-        tarhandle.close()
+        with tarfile.open(fileobj=tmphandle, mode='w') as tarhandle:
+            for path, arcname in remote_init_items:
+                tarhandle.add(path, arcname=arcname)
         tmphandle.seek(0)
         # Build the remote-init command to be run over ssh
-        cmd = ['remote-init']
-        cmd.extend(verbosity_to_opts(cylc.flow.flags.verbosity))
-        cmd.append(str(install_target))
-        cmd.append(get_remote_workflow_run_dir(self.workflow))
+        cmd = [
+            'remote-init',
+            *verbosity_to_opts(cylc.flow.flags.verbosity),
+            str(install_target),
+            get_remote_workflow_run_dir(self.workflow)
+        ]
         dirs_to_symlink = get_dirs_to_symlink(install_target, self.workflow)
         for key, value in dirs_to_symlink.items():
             if value is not None:
                 cmd.append(f"{key}={quote(value)} ")
         # Create the ssh command
         try:
             host = get_host_from_platform(
@@ -281,52 +297,100 @@
         cmd.append(get_remote_workflow_run_dir(self.workflow))
         host = get_host_from_platform(
             platform, bad_hosts=self.bad_hosts
         )
         cmd = construct_ssh_cmd(cmd, platform, host, timeout='10s')
         return cmd, host
 
+    @staticmethod
+    def _get_remote_tidy_targets(
+        platform_names: List[str],
+        install_targets: Set[str]
+    ) -> Dict[str, List[Dict[str, Any]]]:
+        """Finds valid platforms for install targets, warns about in invalid
+        install targets.
+
+        logs:
+            A list of install targets where no platform can be found.
+
+        returns:
+            A mapping of install targets to valid platforms only where
+            platforms are available.
+        """
+        if install_targets and not platform_names:
+            install_targets_map: Dict[str, List[Dict[str, Any]]] = {
+                t: [] for t in install_targets}
+            unreachable_targets = install_targets
+        else:
+            install_targets_map = get_install_target_to_platforms_map(
+                platform_names, quiet=True)
+            # If we couldn't find a platform for a target, we cannot tidy it -
+            # raise an Error:
+            unreachable_targets = install_targets.difference(
+                install_targets_map)
+
+        if unreachable_targets:
+            msg = 'No platforms available to remote tidy install targets:'
+            for unreachable_target in unreachable_targets:
+                msg += f'\n * {unreachable_target}'
+            LOG.error(msg)
+
+        return install_targets_map
+
     def remote_tidy(self) -> None:
         """Remove workflow contact files and keys from initialised remotes.
 
         Call "cylc remote-tidy".
         This method is called on workflow shutdown, so we want nothing to hang.
         Timeout any incomplete commands after 10 seconds.
         """
+        # Get a list of all platforms used from workflow database:
+        platforms_used = (
+            self.db_mgr.get_pri_dao().select_task_job_platforms())
+        # For each install target compile a list of platforms:
+        install_targets = {
+            target for target, msg
+            in self.remote_init_map.items()
+            if msg == REMOTE_FILE_INSTALL_DONE
+        }
+        install_targets_map = self._get_remote_tidy_targets(
+            platforms_used, install_targets)
+
         # Issue all SSH commands in parallel
         queue: Deque[RemoteTidyQueueTuple] = deque()
-        for install_target, message in self.remote_init_map.items():
-            if message != REMOTE_FILE_INSTALL_DONE:
-                continue
+        for install_target, platforms in install_targets_map.items():
             if install_target == get_localhost_install_target():
                 continue
-            try:
-                platform = get_random_platform_for_install_target(
-                    install_target
-                )
-                cmd, host = self.construct_remote_tidy_ssh_cmd(platform)
-            except (NoHostsError, PlatformLookupError) as exc:
-                LOG.warning(
-                    PlatformError(
-                        f'{PlatformError.MSG_TIDY}\n{exc}',
-                        platform['name'],
+            for platform in platforms:
+                try:
+                    cmd, host = self.construct_remote_tidy_ssh_cmd(platform)
+                except NoHostsError as exc:
+                    LOG.warning(
+                        PlatformError(
+                            f'{PlatformError.MSG_TIDY}\n{exc}',
+                            platform['name'],
+                        )
                     )
-                )
-            else:
-                log_platform_event('remote tidy', platform, host)
-                queue.append(
-                    RemoteTidyQueueTuple(
-                        platform,
-                        host,
-                        Popen(  # nosec
-                            cmd, stdout=PIPE, stderr=PIPE, stdin=DEVNULL,
-                            text=True
-                        )  # * command constructed by internal interface
+                else:
+                    log_platform_event('remote tidy', platform, host)
+                    queue.append(
+                        RemoteTidyQueueTuple(
+                            platform,
+                            host,
+                            Popen(  # nosec
+                                cmd, stdout=PIPE, stderr=PIPE, stdin=DEVNULL,
+                                text=True
+                            )  # * command constructed by internal interface
+                        )
                     )
-                )
+                    break
+            else:
+                LOG.error(
+                    NoPlatformsError(
+                        install_target, 'install target', 'remote tidy'))
         # Wait for commands to complete for a max of 10 seconds
         timeout = time() + 10.0
         while queue and time() < timeout:
             item = queue.popleft()
             if item.proc.poll() is None:  # proc still running
                 queue.append(item)
                 continue
@@ -580,27 +644,31 @@
             self.is_reload = False  # reset marker
         elif self.is_restart:
             load_type = "restart"
             self.is_restart = False  # reset marker
         file_name = f"{log_num:02d}-{load_type}-{install_target}.log"
         return file_name
 
-    def _remote_init_items(self, comms_meth: CommsMeth):
+    def _remote_init_items(
+        self, comms_meth: CommsMeth
+    ) -> List[Tuple[str, str]]:
         """Return list of items to install based on communication method.
 
+        (At the moment this is only the contact file.)
+
         Return (list):
             Each item is (source_path, dest_path) where:
             - source_path is the path to the source file to install.
             - dest_path is relative path under workflow run directory
               at target remote.
         """
-        items = []
-
-        if comms_meth in [CommsMeth.SSH, CommsMeth.ZMQ]:
-            # Contact file
-            items.append((
+        if comms_meth not in {CommsMeth.SSH, CommsMeth.ZMQ}:
+            return []
+        return [
+            (
                 get_contact_file_path(self.workflow),
                 os.path.join(
                     WorkflowFiles.Service.DIRNAME,
-                    WorkflowFiles.Service.CONTACT)))
-
-        return items
+                    WorkflowFiles.Service.CONTACT
+                )
+            )
+        ]
```

### Comparing `cylc-flow-8.1.2/cylc/flow/task_state.py` & `cylc-flow-8.1.3/cylc/flow/task_state.py`

 * *Files 3% similar despite different names*

```diff
@@ -464,39 +464,47 @@
     def _add_prerequisites(self, point, tdef):
         """Add task prerequisites."""
         # Triggers for sequence_i only used if my cycle point is a
         # valid member of sequence_i's sequence of cycle points.
         self._is_satisfied = None
         self._suicide_is_satisfied = None
 
+        # Use dicts to avoid generating duplicate prerequisites from sequences
+        # with coincident cycle points.
+        prerequisites = {}
+        suicide_prerequisites = {}
+
         for sequence, dependencies in tdef.dependencies.items():
             if not sequence.is_valid(point):
                 continue
             for dependency in dependencies:
                 cpre = dependency.get_prerequisite(point, tdef)
                 if dependency.suicide:
-                    self.suicide_prerequisites.append(cpre)
+                    suicide_prerequisites[cpre.instantaneous_hash()] = cpre
                 else:
-                    self.prerequisites.append(cpre)
+                    prerequisites[cpre.instantaneous_hash()] = cpre
 
         if tdef.sequential:
             # Add a previous-instance succeeded prerequisite.
             adjusted = []
             for seq in tdef.sequences:
                 prv = seq.get_nearest_prev_point(point)
                 if prv:
                     # None if out of sequence bounds.
                     adjusted.append(prv)
             if adjusted:
                 p_prev = max(adjusted)
-                cpre = Prerequisite(point, tdef.start_point)
+                cpre = Prerequisite(point)
                 cpre.add(tdef.name, p_prev, TASK_STATUS_SUCCEEDED,
                          p_prev < tdef.start_point)
                 cpre.set_condition(tdef.name)
-                self.prerequisites.append(cpre)
+                prerequisites[cpre.instantaneous_hash()] = cpre
+
+        self.suicide_prerequisites = list(suicide_prerequisites.values())
+        self.prerequisites = list(prerequisites.values())
 
     def add_xtrigger(self, label, satisfied=False):
         self.xtriggers[label] = satisfied
 
     def get_xtrigger(self, label):
         return self.xtriggers[label]
```

### Comparing `cylc-flow-8.1.2/cylc/flow/task_state_prop.py` & `cylc-flow-8.1.3/cylc/flow/task_state_prop.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/task_trigger.py` & `cylc-flow-8.1.3/cylc/flow/task_trigger.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,15 +196,15 @@
                 task.
 
         Returns:
             cylc.flow.prerequisite.Prerequisite
 
         """
         # Create Prerequisite.
-        cpre = Prerequisite(point, tdef.start_point)
+        cpre = Prerequisite(point)
 
         # Loop over TaskTrigger instances.
         for task_trigger in self.task_triggers:
             if task_trigger.cycle_point_offset is not None:
                 # Compute trigger cycle point from offset.
                 if task_trigger.offset_is_from_icp:
                     prereq_offset_point = get_point_relative(
```

### Comparing `cylc-flow-8.1.2/cylc/flow/taskdef.py` & `cylc-flow-8.1.3/cylc/flow/taskdef.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 from cylc.flow.task_outputs import SORT_ORDERS
 
 if TYPE_CHECKING:
     from cylc.flow.cycling import PointBase
 
 
 def generate_graph_children(tdef, point):
-    """Determine graph children of this task (for spawning)."""
+    """Determine graph children of this task at point."""
     graph_children = {}
     for seq, dout in tdef.graph_children.items():
         for output, downs in dout.items():
             if output not in graph_children:
                 graph_children[output] = []
             for name, trigger in downs:
                 child_point = trigger.get_child_point(point, seq)
@@ -69,34 +69,52 @@
                 graph_children[TASK_OUTPUT_SUCCEEDED] = []
             graph_children[TASK_OUTPUT_SUCCEEDED].append(
                 (tdef.name, min(nexts), False))
 
     return graph_children
 
 
-def generate_graph_parents(tdef, point):
-    """Determine graph parents of this task."""
+def generate_graph_parents(tdef, point, taskdefs):
+    """Determine concrent graph parents of task tdef at point.
+
+    Infer parents be reversing upstream triggers that lead to point/task.
+    """
     graph_parents = {}
-    for seq, ups in tdef.graph_parents.items():
+    for seq, triggers in tdef.graph_parents.items():
+        if not seq.is_valid(point):
+            # Don't infer parents if the trigger belongs to a sequence that
+            # does not include the child point. E.g.:
+            #   T06 = "waz[-PT6H] => foo"
+            # here waz[-PT6H] is a parent of T06/foo but not of T12/foo.
+            continue
         graph_parents[seq] = []
-        for name, trigger in ups:
+        for parent_name, trigger in triggers:
             parent_point = trigger.get_parent_point(point)
+            if (
+                parent_point != point and
+                not taskdefs[parent_name].is_valid_point(parent_point)
+            ):
+                # Don't infer inter-cycle parents if the upstream point is
+                # not valid for the parent (which depends on its sequences).
+                # NOTE this includes pre-initial dependence where the offset
+                # extends back beyond the initial point AND erroneous offsets
+                # when different tasks are involved, e.g.:
+                #   woo[-Px] => foo
+                # where (point -Px) does not land on a valid point for woo.
+                # TODO ideally validation would flag this as an error.
+                continue
             is_abs = (trigger.offset_is_absolute or
                       trigger.offset_is_from_icp)
             if is_abs and parent_point != point:
                 # If 'foo[^] => bar' only spawn off of '^'.
                 continue
-            if seq.is_valid(parent_point):
-                # E.g.: foo should trigger only on T06:
-                #   PT6H = "waz"
-                #   T06 = "waz[-PT6H] => foo"
-                graph_parents[seq].append((name, parent_point, is_abs))
+            graph_parents[seq].append((parent_name, parent_point, is_abs))
 
     if tdef.sequential:
-        # Add prev-instance parent.
+        # Add implicit previous-instance parent.
         prevs = []
         for seq in tdef.sequences:
             prev = seq.get_prev_point(point)
             if prev is not None:
                 # Within sequence bounds.
                 prevs.append(prev)
         if prevs:
```

### Comparing `cylc-flow-8.1.2/cylc/flow/templatevars.py` & `cylc-flow-8.1.3/cylc/flow/templatevars.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/terminal.py` & `cylc-flow-8.1.3/cylc/flow/terminal.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/time_parser.py` & `cylc-flow-8.1.3/cylc/flow/time_parser.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/timer.py` & `cylc-flow-8.1.3/cylc/flow/timer.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/tui/__init__.py` & `cylc-flow-8.1.3/cylc/flow/tui/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/tui/app.py` & `cylc-flow-8.1.3/cylc/flow/tui/app.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/tui/data.py` & `cylc-flow-8.1.3/cylc/flow/tui/data.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/tui/overlay.py` & `cylc-flow-8.1.3/cylc/flow/tui/overlay.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/tui/tree.py` & `cylc-flow-8.1.3/cylc/flow/tui/tree.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/tui/util.py` & `cylc-flow-8.1.3/cylc/flow/tui/util.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/unicode_rules.py` & `cylc-flow-8.1.3/cylc/flow/unicode_rules.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/util.py` & `cylc-flow-8.1.3/cylc/flow/util.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/wallclock.py` & `cylc-flow-8.1.3/cylc/flow/wallclock.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/workflow_db_mgr.py` & `cylc-flow-8.1.3/cylc/flow/workflow_db_mgr.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/workflow_events.py` & `cylc-flow-8.1.3/cylc/flow/workflow_events.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/workflow_files.py` & `cylc-flow-8.1.3/cylc/flow/workflow_files.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/workflow_status.py` & `cylc-flow-8.1.3/cylc/flow/workflow_status.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/xtrigger_mgr.py` & `cylc-flow-8.1.3/cylc/flow/xtrigger_mgr.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/xtriggers/__init__.py` & `cylc-flow-8.1.3/cylc/flow/xtriggers/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/xtriggers/echo.py` & `cylc-flow-8.1.3/cylc/flow/xtriggers/echo.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/xtriggers/wall_clock.py` & `cylc-flow-8.1.3/cylc/flow/xtriggers/wall_clock.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/xtriggers/workflow_state.py` & `cylc-flow-8.1.3/cylc/flow/xtriggers/workflow_state.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc/flow/xtriggers/xrandom.py` & `cylc-flow-8.1.3/cylc/flow/xtriggers/xrandom.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc_flow.egg-info/PKG-INFO` & `cylc-flow-8.1.3/cylc_flow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cylc-flow
-Version: 8.1.2
+Version: 8.1.3
 Summary: A workflow engine for cycling systems
 Home-page: https://cylc.org/
 Author: Hilary Oliver
 License: GPL
 Project-URL: Documentation, https://cylc.github.io/cylc-doc/stable/html/index.html
 Project-URL: Source, https://github.com/cylc/cylc-flow
 Project-URL: Tracker, https://github.com/cylc/cylc-flow/issues
```

### Comparing `cylc-flow-8.1.2/cylc_flow.egg-info/SOURCES.txt` & `cylc-flow-8.1.3/cylc_flow.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -145,14 +145,15 @@
 cylc/flow/install_plugins/log_vc_info.py
 cylc/flow/jinja/filters/duration_as.py
 cylc/flow/jinja/filters/pad.py
 cylc/flow/jinja/filters/strftime.py
 cylc/flow/job_runner_handlers/__init__.py
 cylc/flow/job_runner_handlers/at.py
 cylc/flow/job_runner_handlers/background.py
+cylc/flow/job_runner_handlers/documentation.py
 cylc/flow/job_runner_handlers/loadleveler.py
 cylc/flow/job_runner_handlers/lsf.py
 cylc/flow/job_runner_handlers/moab.py
 cylc/flow/job_runner_handlers/pbs.py
 cylc/flow/job_runner_handlers/pbs_multi_cluster.py
 cylc/flow/job_runner_handlers/sge.py
 cylc/flow/job_runner_handlers/slurm.py
```

### Comparing `cylc-flow-8.1.2/cylc_flow.egg-info/entry_points.txt` & `cylc-flow-8.1.3/cylc_flow.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.1.2/cylc_flow.egg-info/requires.txt` & `cylc-flow-8.1.3/cylc_flow.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,17 @@
 urwid==2.*
 rx
 promise
 
 [:python_version < "3.11"]
 tomli>=2
 
+[:python_version < "3.8"]
+importlib_metadata
+
 [all]
 EmPy==3.3.*
 pillow
 pympler
 matplotlib
 sqlparse
 matplotlib
```

### Comparing `cylc-flow-8.1.2/setup.cfg` & `cylc-flow-8.1.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 	graphene>=2.1,<3
 	jinja2==3.0.*
 	metomi-isodatetime==1!3.0.*
 	protobuf>=4.21.2,<4.22.0
 	psutil>=5.6.0
 	pyzmq==22.*
 	setuptools>=49, <67
+	importlib_metadata; python_version < "3.8"
 	urwid==2.*
 	rx
 	promise
 	tomli>=2; python_version < "3.11"
 
 [options.packages.find]
 include = cylc*
```

### Comparing `cylc-flow-8.1.2/setup.py` & `cylc-flow-8.1.3/setup.py`

 * *Files identical despite different names*

