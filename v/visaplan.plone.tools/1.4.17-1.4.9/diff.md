# Comparing `tmp/visaplan.plone.tools-1.4.17.tar.gz` & `tmp/visaplan.plone.tools-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/visaplan.plone.tools-1.4.17.tar", last modified: Wed Apr  5 16:01:15 2023, max compression
+gzip compressed data, was "dist/visaplan.plone.tools-1.4.9.tar", last modified: Mon Dec 13 12:03:32 2021, max compression
```

## Comparing `visaplan.plone.tools-1.4.17.tar` & `visaplan.plone.tools-1.4.9.tar`

### file list

```diff
@@ -1,115 +1,98 @@
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-04-05 16:01:15.000000 visaplan.plone.tools-1.4.17/
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-04-05 16:01:15.000000 visaplan.plone.tools-1.4.17/docs/
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    18092 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.4.17/docs/LICENSE.GPL
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      669 2019-11-06 14:05:55.000000 visaplan.plone.tools-1.4.17/docs/LICENSE.rst
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      615 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.4.17/docs/Makefile
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     5494 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.4.17/docs/conf.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      103 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.4.17/docs/conf.rst
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      501 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.4.17/docs/index.rst
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      822 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.4.17/docs/make.bat
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      102 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.4.17/docs/modules.rst
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      106 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.4.17/docs/setup.rst
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      233 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.4.17/docs/visaplan.plone.rst
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      181 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.4.17/docs/visaplan.plone.tools.functions.rst
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      258 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.4.17/docs/visaplan.plone.tools.rst
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      209 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.4.17/docs/visaplan.rst
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-04-05 16:01:15.000000 visaplan.plone.tools-1.4.17/src/
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-04-05 16:01:15.000000 visaplan.plone.tools-1.4.17/src/visaplan/
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-04-05 16:01:15.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-04-05 16:01:15.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-04-05 16:01:15.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/Extensions/
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      476 2022-08-26 10:56:37.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/Extensions/install.py
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-04-05 16:01:15.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/groups/
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      443 2022-08-26 11:15:00.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/groups/__init__.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      839 2022-08-26 11:15:00.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/groups/_data.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     8596 2023-03-23 16:31:02.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/groups/_group.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     3413 2023-03-23 16:31:02.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/groups/_group_pio.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     8675 2022-08-26 11:15:00.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/groups/_helpers.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      687 2022-01-20 18:12:16.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/groups/_imports.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     8339 2023-03-23 16:31:02.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/groups/_membership.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     5968 2023-03-23 16:31:02.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/groups/_user.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     3418 2023-03-23 16:31:02.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/groups/_user_pio.py
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-04-05 16:01:15.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/infofact/
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     5483 2022-01-20 18:17:48.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/infofact/_group.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     3215 2022-01-20 14:33:44.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/infofact/_membership.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     3431 2022-01-20 14:32:17.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/infofact/_user.py
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-04-05 16:01:15.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/setup/
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     3074 2022-08-26 11:11:41.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/setup/__init__.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    19711 2022-08-26 10:54:06.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/setup/_args.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     2416 2022-08-26 10:54:06.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/setup/_attr.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     9046 2022-08-26 11:23:49.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/setup/_decorator.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     1680 2020-12-17 14:06:08.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/setup/_exc.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    12742 2022-12-06 12:33:47.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/setup/_get_object.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     4632 2022-08-26 11:13:17.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/setup/_gs.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     7747 2022-08-26 10:54:06.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/setup/_make_folder.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     1224 2020-12-17 14:06:08.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/setup/_misc.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    22871 2022-08-26 11:14:12.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/setup/_o_tools.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     4425 2022-01-20 18:12:16.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/setup/_query.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    13564 2022-08-26 11:24:57.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/setup/_reindex.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     8117 2022-08-26 10:54:06.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/setup/_rename.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     5543 2022-08-26 10:54:06.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/setup/_roles.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     1563 2022-01-20 13:56:58.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/setup/_switch.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    32525 2022-12-06 12:33:55.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/setup/_tree.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     1651 2022-01-20 18:12:16.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/setup/_types.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    10604 2022-08-26 10:54:06.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/setup/_uid.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     3153 2020-12-17 14:06:08.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/setup/_watch.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    24264 2022-08-26 10:54:06.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/setup/_workflow.py
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-04-05 16:01:15.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/views/
--rw-r--r--   0 tobias    (1000) plone_group  (1003)       45 2020-12-17 14:06:08.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/views/__init__.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     1137 2020-12-17 14:06:08.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/views/check-blobs-delete-selected.pt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     2143 2020-12-17 14:06:08.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/views/check-blobs.pt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      884 2020-12-17 14:06:08.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/views/configure.zcml
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    13282 2022-08-26 10:54:06.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/views/fixblobs.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)        0 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/__init__.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     1557 2022-08-26 11:11:41.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/_at0.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      921 2022-08-26 11:11:41.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/_at1.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    13055 2022-08-26 11:11:41.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/_at2.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      916 2022-08-26 10:56:37.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/_at3.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     3023 2023-03-23 16:31:02.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/_at4.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     3897 2023-03-29 11:52:04.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/_at5.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      539 2023-04-05 16:01:12.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/_at6.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     3108 2022-08-26 11:11:41.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/_dx4.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     3601 2022-08-26 11:11:41.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/_dx5.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     1583 2022-08-26 10:54:06.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/_have.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     1317 2023-03-29 11:52:04.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/attools.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     8290 2022-08-26 10:56:37.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/brains.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    14072 2023-03-29 08:46:13.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/cfg.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      202 2022-08-26 10:56:37.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/configure.zcml
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    18028 2023-03-24 16:18:11.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/context.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     1158 2023-03-23 16:31:02.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/decorators.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      346 2022-08-26 11:11:41.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/dxtools.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      970 2023-03-23 16:31:02.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/env.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    30889 2023-03-23 16:31:02.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/forms.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     5045 2023-03-24 16:18:11.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/functions.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     1692 2022-01-20 18:12:16.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/indexes.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     7325 2023-03-29 08:46:13.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/log.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     3539 2020-12-17 14:06:08.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/mock.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     1802 2023-03-29 08:46:13.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/mock_cfg.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      817 2022-08-26 10:56:37.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/profiles.zcml
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    11691 2022-08-26 11:23:24.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/search.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     4920 2023-03-23 16:31:02.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/seo.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      832 2022-08-26 10:56:37.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/setuphandlers.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      291 2022-12-06 12:33:06.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/strings.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    12714 2023-03-29 08:46:13.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/zcmlgen.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)       80 2019-11-06 14:14:59.000000 visaplan.plone.tools-1.4.17/src/visaplan/plone/__init__.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)       80 2019-11-06 14:14:59.000000 visaplan.plone.tools-1.4.17/src/visaplan/__init__.py
-drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2023-04-05 16:01:15.000000 visaplan.plone.tools-1.4.17/src/visaplan.plone.tools.egg-info/
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    24710 2023-04-05 16:01:14.000000 visaplan.plone.tools-1.4.17/src/visaplan.plone.tools.egg-info/PKG-INFO
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     3551 2023-04-05 16:01:14.000000 visaplan.plone.tools-1.4.17/src/visaplan.plone.tools.egg-info/SOURCES.txt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)        1 2023-04-05 16:01:14.000000 visaplan.plone.tools-1.4.17/src/visaplan.plone.tools.egg-info/dependency_links.txt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)       53 2023-04-05 16:01:14.000000 visaplan.plone.tools-1.4.17/src/visaplan.plone.tools.egg-info/entry_points.txt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)       24 2023-04-05 16:01:14.000000 visaplan.plone.tools-1.4.17/src/visaplan.plone.tools.egg-info/namespace_packages.txt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)        1 2019-03-25 17:32:23.000000 visaplan.plone.tools-1.4.17/src/visaplan.plone.tools.egg-info/not-zip-safe
--rw-r--r--   0 tobias    (1000) plone_group  (1003)       68 2023-04-05 16:01:14.000000 visaplan.plone.tools-1.4.17/src/visaplan.plone.tools.egg-info/requires.txt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)        9 2023-04-05 16:01:14.000000 visaplan.plone.tools-1.4.17/src/visaplan.plone.tools.egg-info/top_level.txt
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    13136 2023-04-05 16:00:16.000000 visaplan.plone.tools-1.4.17/CHANGES.rst
--rw-r--r--   0 tobias    (1000) plone_group  (1003)       67 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.4.17/CONTRIBUTORS.rst
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      183 2020-01-14 11:15:58.000000 visaplan.plone.tools-1.4.17/MANIFEST.in
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     3933 2023-03-23 16:31:02.000000 visaplan.plone.tools-1.4.17/README.rst
--rw-r--r--   0 tobias    (1000) plone_group  (1003)      218 2022-08-26 11:13:17.000000 visaplan.plone.tools-1.4.17/TODO.rst
--rw-r--r--   0 tobias    (1000) plone_group  (1003)        7 2023-03-29 09:07:53.000000 visaplan.plone.tools-1.4.17/VERSION
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     9342 2020-09-04 22:52:51.000000 visaplan.plone.tools-1.4.17/long-description.rst
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     1539 2023-04-05 16:01:15.000000 visaplan.plone.tools-1.4.17/setup.cfg
--rw-r--r--   0 tobias    (1000) plone_group  (1003)     7238 2023-03-23 16:31:02.000000 visaplan.plone.tools-1.4.17/setup.py
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    15845 2022-01-28 16:14:00.000000 visaplan.plone.tools-1.4.17/test.rst
--rw-r--r--   0 tobias    (1000) plone_group  (1003)    24710 2023-04-05 16:01:15.000000 visaplan.plone.tools-1.4.17/PKG-INFO
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2021-12-13 12:03:32.000000 visaplan.plone.tools-1.4.9/
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2021-12-13 12:03:32.000000 visaplan.plone.tools-1.4.9/docs/
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    18092 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.4.9/docs/LICENSE.GPL
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      669 2019-11-06 14:05:55.000000 visaplan.plone.tools-1.4.9/docs/LICENSE.rst
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      615 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.4.9/docs/Makefile
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     5494 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.4.9/docs/conf.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      103 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.4.9/docs/conf.rst
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      501 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.4.9/docs/index.rst
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      822 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.4.9/docs/make.bat
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      102 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.4.9/docs/modules.rst
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      106 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.4.9/docs/setup.rst
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      233 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.4.9/docs/visaplan.plone.rst
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      181 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.4.9/docs/visaplan.plone.tools.functions.rst
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      258 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.4.9/docs/visaplan.plone.tools.rst
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      209 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.4.9/docs/visaplan.rst
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2021-12-13 12:03:32.000000 visaplan.plone.tools-1.4.9/src/
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2021-12-13 12:03:32.000000 visaplan.plone.tools-1.4.9/src/visaplan/
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2021-12-13 12:03:32.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2021-12-13 12:03:32.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2021-12-13 12:03:32.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/Extensions/
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      476 2021-12-06 14:37:37.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/Extensions/install.py
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2021-12-13 12:03:32.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     3074 2021-12-06 14:46:05.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/__init__.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    19711 2021-08-11 12:42:23.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_args.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     2416 2021-08-11 12:42:23.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_attr.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     8765 2021-08-11 12:42:23.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_decorator.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1680 2020-12-17 14:06:08.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_exc.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    12742 2021-12-06 14:37:37.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_get_object.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     4632 2021-12-06 14:46:05.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_gs.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     7747 2021-12-06 14:37:37.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_make_folder.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1224 2020-12-17 14:06:08.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_misc.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    22901 2021-12-06 14:46:05.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_o_tools.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     4425 2021-12-06 14:37:37.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_query.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    13482 2021-12-06 14:46:05.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_reindex.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     8117 2021-12-06 14:37:37.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_rename.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     5543 2021-08-11 12:42:23.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_roles.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1563 2021-08-11 12:42:23.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_switch.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    32525 2021-12-06 14:46:05.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_tree.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1651 2021-12-06 14:37:37.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_types.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    10604 2021-12-06 14:37:37.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_uid.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     3153 2020-12-17 14:06:08.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_watch.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    24264 2021-12-06 14:37:37.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_workflow.py
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2021-12-13 12:03:32.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/views/
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)       45 2020-12-17 14:06:08.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/views/__init__.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1137 2020-12-17 14:06:08.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/views/check-blobs-delete-selected.pt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     2143 2020-12-17 14:06:08.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/views/check-blobs.pt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      884 2020-12-17 14:06:08.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/views/configure.zcml
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    13282 2021-12-06 14:37:37.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/views/fixblobs.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)        0 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/__init__.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1557 2021-12-06 14:46:05.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/_at0.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      921 2021-12-06 14:46:05.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/_at1.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    13055 2021-12-06 14:46:05.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/_at2.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      916 2021-11-29 09:44:56.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/_at3.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     3023 2021-12-06 14:46:05.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/_at4.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     3740 2021-12-06 14:46:05.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/_at5.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     3108 2021-12-06 14:46:05.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/_dx4.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     3601 2021-12-06 14:46:05.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/_dx5.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1583 2021-08-11 12:42:23.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/_have.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      753 2021-12-06 14:46:05.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/attools.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     8290 2021-11-29 09:44:56.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/brains.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    14072 2021-12-06 14:46:05.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/cfg.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      202 2021-11-29 09:44:57.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/configure.zcml
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    18026 2021-12-06 14:46:05.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/context.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      882 2021-01-20 13:47:52.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/decorators.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      346 2021-12-06 14:46:05.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/dxtools.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    30708 2021-08-11 12:42:23.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/forms.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     3171 2021-08-11 12:42:23.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/functions.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    23246 2021-12-06 14:37:37.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/groups.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1692 2021-12-06 14:37:37.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/indexes.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     7265 2021-12-06 14:46:05.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/log.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     3539 2020-12-17 14:06:08.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/mock.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1802 2021-12-06 14:46:05.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/mock_cfg.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      817 2021-11-29 09:44:56.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/profiles.zcml
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    11970 2021-12-06 14:46:05.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/search.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      832 2021-12-06 14:37:37.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setuphandlers.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    12730 2021-12-06 14:46:05.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/zcmlgen.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)       80 2019-11-06 14:14:59.000000 visaplan.plone.tools-1.4.9/src/visaplan/plone/__init__.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)       80 2019-11-06 14:14:59.000000 visaplan.plone.tools-1.4.9/src/visaplan/__init__.py
+drwxr-sr-x   0 tobias    (1000) plone_group  (1003)        0 2021-12-13 12:03:32.000000 visaplan.plone.tools-1.4.9/src/visaplan.plone.tools.egg-info/
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    21741 2021-12-13 12:03:32.000000 visaplan.plone.tools-1.4.9/src/visaplan.plone.tools.egg-info/PKG-INFO
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     2923 2021-12-13 12:03:32.000000 visaplan.plone.tools-1.4.9/src/visaplan.plone.tools.egg-info/SOURCES.txt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)        1 2021-12-13 12:03:32.000000 visaplan.plone.tools-1.4.9/src/visaplan.plone.tools.egg-info/dependency_links.txt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)       53 2021-12-13 12:03:32.000000 visaplan.plone.tools-1.4.9/src/visaplan.plone.tools.egg-info/entry_points.txt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)       24 2021-12-13 12:03:32.000000 visaplan.plone.tools-1.4.9/src/visaplan.plone.tools.egg-info/namespace_packages.txt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)        1 2019-03-25 17:32:23.000000 visaplan.plone.tools-1.4.9/src/visaplan.plone.tools.egg-info/not-zip-safe
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)       68 2021-12-13 12:03:32.000000 visaplan.plone.tools-1.4.9/src/visaplan.plone.tools.egg-info/requires.txt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)        9 2021-12-13 12:03:32.000000 visaplan.plone.tools-1.4.9/src/visaplan.plone.tools.egg-info/top_level.txt
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    11351 2021-12-13 12:02:22.000000 visaplan.plone.tools-1.4.9/CHANGES.rst
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)       67 2019-01-30 12:47:07.000000 visaplan.plone.tools-1.4.9/CONTRIBUTORS.rst
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      183 2020-01-14 11:15:58.000000 visaplan.plone.tools-1.4.9/MANIFEST.in
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     3742 2021-11-29 09:44:57.000000 visaplan.plone.tools-1.4.9/README.rst
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)      218 2021-12-13 12:02:16.000000 visaplan.plone.tools-1.4.9/TODO.rst
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)        6 2021-12-06 14:47:42.000000 visaplan.plone.tools-1.4.9/VERSION
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     9342 2020-09-04 22:52:51.000000 visaplan.plone.tools-1.4.9/long-description.rst
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     1404 2021-12-13 12:03:32.000000 visaplan.plone.tools-1.4.9/setup.cfg
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)     6854 2021-12-13 12:01:11.000000 visaplan.plone.tools-1.4.9/setup.py
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    15408 2021-12-13 12:00:01.000000 visaplan.plone.tools-1.4.9/test.rst
+-rw-r--r--   0 tobias    (1000) plone_group  (1003)    21741 2021-12-13 12:03:32.000000 visaplan.plone.tools-1.4.9/PKG-INFO
```

### Comparing `visaplan.plone.tools-1.4.17/docs/LICENSE.GPL` & `visaplan.plone.tools-1.4.9/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.17/docs/LICENSE.rst` & `visaplan.plone.tools-1.4.9/docs/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.17/docs/Makefile` & `visaplan.plone.tools-1.4.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.17/docs/conf.py` & `visaplan.plone.tools-1.4.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.17/docs/make.bat` & `visaplan.plone.tools-1.4.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/setup/__init__.py` & `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/__init__.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/setup/_args.py` & `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_args.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/setup/_attr.py` & `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_attr.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/setup/_decorator.py` & `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_decorator.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,17 +21,14 @@
 # Python compatibility:
 from __future__ import absolute_import
 
 # Standard library:
 from functools import wraps
 from time import time
 
-# Local imports:
-from visaplan.plone.tools.env import worker_name
-
 # Logging / Debugging:
 import logging
 
 __all__ = [
         # decorators:
         'step',
         # noch unfertig:
@@ -63,20 +60,15 @@
     # "site") leider nicht möglich; dafür würden zusätzliche Argumente
     # benötigt, und mithin eine Änderung der Signatur.
 
     @wraps(func)
     def wrapper(context, logger=None):
         funcname = func.__name__
         if logger is None:
-            label = ':'.join(filter(None, [
-                                    'setup',
-                                    worker_name(),
-                                    funcname,
-                                    ]))
-            logger = logging.getLogger(label)
+            logger = logging.getLogger('setup:'+funcname)
         _started = time()
         try:
             res = func(context, logger)
         except Exception as e:
             delta = time() - _started
             if isinstance(e, KeyboardInterrupt):
                 logger.error('%(funcname)s aborted after %(delta)5.2f seconds',
```

### Comparing `visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/setup/_exc.py` & `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_exc.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/setup/_get_object.py` & `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_get_object.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/setup/_gs.py` & `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_gs.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/setup/_make_folder.py` & `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_make_folder.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/setup/_misc.py` & `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_misc.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/setup/_o_tools.py` & `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_o_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from __future__ import absolute_import
 
 from six import string_types as six_string_types
 from six.moves import map
 
 # Standard library:
 from collections import defaultdict
+from pprint import pprint
 
 # Zope:
 from Products.CMFCore.utils import getToolByName
 
 # Local imports:
 from visaplan.plone.tools._have import HAS_SUBPORTALS, HAS_VPSEARCH
 from visaplan.plone.tools.setup._args import (
@@ -305,15 +306,15 @@
             if canonical and canonical != o:
                 _NFO('Setting canonical to %(canonical)r', locals())
                 try:
                     o.addTranslationReference(canonical)
                 except AlreadyTranslated as e:
                     _ERR('%(o)r is already translated!', locals())
                     _ERR(str(CantAddTranslationReference(o, canonical)), {})
-                    if 0: pp({
+                    if 0: pprint({
                         'o': o, 'canonical': canonical,
                         'identical?': canonical is o,
                         })
                     set_trace()
                     nochmal = 0
                     if nochmal:
                         o.addTranslationReference(canonical)
```

### Comparing `visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/setup/_query.py` & `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_query.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/setup/_reindex.py` & `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_reindex.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 metadata attribute, you might want to use collective.metadataversion,
 which as well allows you to adjust this subset.
 Because of the slightly changed focus, the function there is named differently
 as well: .utils.make_metadata_updater.
 """
 
 # Python compatibility:
-from __future__ import absolute_import, print_function
+from __future__ import absolute_import
 
 # Setup tools:
 import pkg_resources
 
 try:
     pkg_resources.get_distribution('collective.metadataversion')
 except pkg_resources.DistributionNotFound:
@@ -61,17 +61,14 @@
         ]
 
 
 if HAVE_METADATAVERSION:
     # Zope:
     from zope.component import getUtility
 
-    # Plone:
-    from plone.registry.interfaces import IRegistry
-
     # 3rd party:
     from collective.metadataversion.config import DEFAULT_IDXS, FULL_IDXS_KEY
 
     def get_default_idxs():
         """
         We have collective.metadataversion
         """
```

### Comparing `visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/setup/_rename.py` & `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_rename.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/setup/_roles.py` & `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_roles.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/setup/_switch.py` & `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_switch.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/setup/_tree.py` & `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_tree.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/setup/_types.py` & `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_types.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/setup/_uid.py` & `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_uid.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/setup/_watch.py` & `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_watch.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/setup/_workflow.py` & `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setup/_workflow.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/views/check-blobs-delete-selected.pt` & `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/views/check-blobs-delete-selected.pt`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/views/check-blobs.pt` & `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/views/check-blobs.pt`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/views/configure.zcml` & `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/views/configure.zcml`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/views/fixblobs.py` & `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/views/fixblobs.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/_at0.py` & `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/_at0.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/_at1.py` & `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/_at1.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/_at2.py` & `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/_at2.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/_at3.py` & `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/_at3.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/_at4.py` & `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/_at4.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
     - ignore_empty (default: True) --
         If a field exists but is empty (or contains a non-string value),
         try the next one;
         with ignore_empty=False,
         any value of the first existing field would be used.
 
-    - decode (default: visaplan.tools.coding.safe_decode) --
+    - decode (default: visaplan.plone.coding.safe_decode) --
         a function to decode a bytes string to unicode.
         Specify a falsy value to suppress decoding.
 
     If the field contains text/plain (i.e., the content doesn't start with
     '<'), it is converted to HTML, using a simple function, which
 
     - creates paragraphs for each line (or sequence of lines), delimited by
```

### Comparing `visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/_at5.py` & `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/_at5.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*- vim: tw=79 cc=+1 sw=4 sts=4 et si
 """
-visaplan.plone.tools: attools: Archetypes-related tools (_at5)
+visaplan.plone.tools: attools: Archetypes-related tools (_at4)
 """
 
 # Python compatibility:
 from __future__ import absolute_import
 
 from six import string_types as six_string_types
 from six import text_type as six_text_type
@@ -15,20 +15,14 @@
 # visaplan:
 from visaplan.tools.coding import safe_decode
 from visaplan.tools.html import from_plain_text
 
 # Local imports:
 from ._at3 import getter_name
 
-__all__ = [
-    'generate_all_texts',  # yield (name, val) tuples
-  # 'is_nonempty_string',  # copied to visaplan.tools v1.3.10+
-    'get_all_texts',
-    ]
-
 
 def generate_all_texts(context, *fieldnames, **kwargs):
     """
     Generate all (existing) text fields as (fieldname, value) tuples
 
     Keyword options:
```

### Comparing `visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/_dx4.py` & `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/_dx4.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/_dx5.py` & `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/_dx5.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/_have.py` & `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/_have.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/brains.py` & `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/brains.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/cfg.py` & `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/cfg.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/context.py` & `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/context.py`

 * *Files 0% similar despite different names*

```diff
@@ -413,25 +413,23 @@
         res = tool(*args, **kwargs)
         print('...' + ci + '.')
         return res
 
     decorated.__doc__ = '%(toolname)s tool (decorated)' % locals()
     return decorated
 
-
 def message(context, message, messageType='info', mapping=None):
     """
     Ersetzt den gleichnamigen Tomcom-Adapter
     """
     pu = getToolByName(context, 'plone_utils')
     pu.addPortalMessage(pmf(safe_decode(message),
                             mapping=mapping),
                         messageType)
 
-
 def getMessenger(context, decode=safe_decode):
     """
     Return a 'message' function which doesn't require
     (nor accept) a context argument
     """
     pu = getToolByName(context, 'plone_utils')
     apm = pu.addPortalMessage
```

### Comparing `visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/forms.py` & `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/forms.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,21 +56,21 @@
 except ImportError:
     if __name__ == '__main__':
         print('Some tests will fail due to import problem')
     else:
         raise
     UIDCHARS_UNICODE = frozenset(u'0123456789abcdef')
     def is_uid_shaped(s, onerror='raise'):
-        if isinstance(s, six_text_type):
-            pass
-        elif isinstance(s, bytes):
+        if isinstance(s, str):
             try:
                 s = s.decode('ascii')
             except UnicodeDecodeError:
                 return False
+        elif isinstance(s, six_text_type):
+            pass
         elif onerror == 'raise':
             raise ValueError('String expected: %(s)r'
                              % locals())
         else:
             return False
         return len(s) == 32 and UIDCHARS_UNICODE.issuperset(s)
     def as_new_list(val, splitfunc=None):
@@ -705,18 +705,14 @@
     Das Limit kann explizit angegeben oder auch aufgehoben werden:
     >>> uid_or_number('10001', limit=None)['number']
     10001
 
     Wenn eine Zahl übergeben wurde, gibt es keine solche Beschränkung:
     >>> uid_or_number(10001)['number']
     10001
-
-    We might use this as well to prefix our lesson ids in course xml:
-    >>> sorted(uid_or_number('lesson-5').items())
-    [('number', 5), ('prefix', 'lesson-'), ('uid', None)]
     """
     res = {'uid':    None,
            'number': None,
            'prefix': '',
            }
     if val is None:
         return res
```

### Comparing `visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/indexes.py` & `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/indexes.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/log.py` & `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/log.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 
 # Logging / Debugging:
 import logging
 from visaplan.tools.debug import arginfo, pretty_funcname
 
 __all__ = ['getLogSupport',
            'make_textlogger',
-           'locked_open',  # a context manager
            ]
 
 TIMEFORMAT_VERBOSE = u'%Y-%m-%d %T %Z (%A) '
 TIMEFORMAT_LASTCHARS = u' |-\t'
 _DEVMODE_STRING = str(DevelopmentMode)
 
 def getLogSupport(name=None,
@@ -67,15 +66,15 @@
     if 'stack_limit' not in kwargs:
         kwargs['stack_limit'] = 3
     name, label = split_filename(fn, name,  # stack_limit=stack_limit,
                                  **kwargs)
     logger = logging.getLogger(label)
     if default is None:
         default = defaultFromDevMode and _DEVMODE_STRING or 'False'
-    elif not isinstance(default, six_string_types):
+    elif not isinstance(default, str):
         raise ValueError('default must be a string! (%(default)r)'
                          % locals())
     tmp = get_debug_active(name,
                            default)
     if DevelopmentMode:
         debug_active = tmp
     else:
```

### Comparing `visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/mock.py` & `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/mock.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/mock_cfg.py` & `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/mock_cfg.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/profiles.zcml` & `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/profiles.zcml`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/search.py` & `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -364,10 +364,21 @@
                              for tup in language_tool.listSupportedLanguages()
                              ]
         values.update(all_languages)
     return sorted(values)
 
 
 if __name__ == "__main__":
+  if 0:
+      # Standard library:
+      from pprint import pprint
+
+      # Logging / Debugging:
+      from pdb import set_trace
+      set_trace()
+      mqs = make_querystring_mangle(None, mangle_umlauts)
+      lst = mqs(u'entkoppelte Förderschnecke ')
+      pprint(lst)
+  else:
     # Standard library:
     import doctest
     doctest.testmod()
```

### Comparing `visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/setuphandlers.py` & `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.17/src/visaplan/plone/tools/zcmlgen.py` & `visaplan.plone.tools-1.4.9/src/visaplan/plone/tools/zcmlgen.py`

 * *Files 0% similar despite different names*

```diff
@@ -208,15 +208,16 @@
         # are common to both
         if [difference
             for difference in difflines
             if not difference.startswith('  ')  # unchanged lines
             and difference not in ('+ ', '- ')  # empty lines added/removed
             ]:
             print('\n'.join(difflines))
-            if sys.stdout.isatty(): set_trace()
+            if sys.stdout.isatty():
+                set_trace()
             return False
         return True
 
 
 class ResourceGenerator(BasicGenerator):
     """
     implementiert die fehlenden Methoden der BasicGenerator-Klasse
```

### Comparing `visaplan.plone.tools-1.4.17/src/visaplan.plone.tools.egg-info/PKG-INFO` & `visaplan.plone.tools-1.4.9/src/visaplan.plone.tools.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visaplan.plone.tools
-Version: 1.4.17
+Version: 1.4.9
 Summary: General tools for Plone sites
 Home-page: UNKNOWN
 Author: Tobias Herp
 Author-email: tobias.herp@visaplan.com
 License: GPL version 2
 Project-URL: Source, https://github.com/visaplan/plone.tools
 Project-URL: Documentation, https://pypi.org/project/visaplan.plone.tools
@@ -117,20 +117,14 @@
           - ``@returns_json``:
         
             Wraps the function call and returns the JSON_-encoded result,
             including HTTP headers.
         
             Uses simplejson_ if available.
         
-            **NOT** to be used for functions which simply provide JSON_ data for
-            insertion in page templates!
-        
-            Otherwise, the browser might try to parse your HTML page as JSON
-            and fail.
-        
         Documentation
         -------------
         
         Sorry, we don't have real user documentation yet.
         
         Most functions are documented by doctests, anyway;
         it helps to understand some German.
@@ -196,135 +190,18 @@
         
         Contributors
         ============
         
         - Tobias Herp, tobias.herp@visaplan.com
         
         
-        .. vim: sw=2 sts=2 tw=79 cc=+1
-        
         Changelog
         =========
         
         
-        1.4.17 (2023-04-05)
-        -------------------
-        
-        New features: 
-        
-        - function .attools.can_be_html(field)
-        
-        [tobiasherp]
-        
-        
-        1.4.16 (2023-03-24)
-        -------------------
-        
-        New features: 
-        
-        - New function `short_hostname` in .functions
-        
-        [tobiasherp]
-        
-        
-        1.4.15 (2023-03-08)
-        -------------------
-        
-        Bugfixes:
-        
-        - Py3K support fixes for
-        
-          - .functions.is_uid_shaped
-          - .log.getLogSupport
-        
-        New features: 
-        
-        - New (still tiny) module .seo for SEO support;
-          for now, focused on structured data.
-          Functions:
-        
-          - `parse_title`, returning a dict
-        
-        [tobiasherp]
-        
-        
-        1.4.14 (2022-04-22)
-        -------------------
-        
-        Bugfixes:
-        
-        - Missing imports fixed for
-        
-          - .groups.is_member_of__factory
-          - .setup.get_default_idxs
-        
-        [tobiasherp]
-        
-        
-        1.4.13 (2022-03-04)
-        -------------------
-        
-        Bugfixes:
-        
-        - Fixed a bug in .groups.groupinfo_factory(pretty);
-          for this to work, we need visaplan.plone.groups.
-        
-        Improvements:
-        
-        - The label of the default logger of the ``@@step`` decorator
-          now includes the name of the worker, e.g. ``instance`` or ``client``
-        
-        New features: 
-        
-        - New `.env` module, providing the `worker_name()`
-        
-        [tobiasherp]
-        
-        
-        1.4.12 (2022-02-15)
-        -------------------
-        
-        Bugfixes:
-        
-        - Fixed a bug in .groups.groupinfo_factory(pretty);
-          for this to work, we need visaplan.plone.groups.
-        
-        [tobiasherp]
-        
-        
-        1.4.11 (2022-02-05)
-        -------------------
-        
-        Bugfixes:
-        
-        - Fixed a regression for .groups.groupinfo_factory
-        
-        [tobiasherp]
-        
-        
-        1.4.10 (2022-02-03)
-        -------------------
-        
-        Improvements:
-        
-        - Converted the .groups module in a subpackage
-        
-        New features: 
-        
-        - New option `missing=False` for
-        
-          - .groups.groupinfo_factory
-        
-          If `True`, the resulting function creates an `existing` key,
-          and for missing groups, the `group_title` is `None`;
-          otherwise, an empty dict is returned in such cases.
-        
-        [tobiasherp]
-        
-        
         1.4.9 (2021-12-13)
         ------------------
         
         Improvements:
         
         - If collective.metadataversion_ is installed, use the configured default set of
           indexes (if no `idxs` explicitly given but metadata recreation is requested)
@@ -399,17 +276,16 @@
         
           We keep the the ``uninstall`` profile *for now;*
           it will be removed in an near-future version.
         
           So, *don't "install"* this package (Quick-Installer, Plone add-ons);
           just use it in Python_ code!
         
-          We keep the ``configure.zcml`` file and the autoinclude entry point
-          for now, though;
-          we can imagine to use e.g. the Plone registry for some settings.
+          We keep the ``configure.zcml`` file and the autoinclude entry point, though;
+          we can image to use e.g. the Plone registry for some settings.
         
         [tobiasherp]
         
         
         1.4.4 (2021-08-31)
         ------------------
```

### Comparing `visaplan.plone.tools-1.4.17/src/visaplan.plone.tools.egg-info/SOURCES.txt` & `visaplan.plone.tools-1.4.9/src/visaplan.plone.tools.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -34,51 +34,36 @@
 src/visaplan/plone/tools/__init__.py
 src/visaplan/plone/tools/_at0.py
 src/visaplan/plone/tools/_at1.py
 src/visaplan/plone/tools/_at2.py
 src/visaplan/plone/tools/_at3.py
 src/visaplan/plone/tools/_at4.py
 src/visaplan/plone/tools/_at5.py
-src/visaplan/plone/tools/_at6.py
 src/visaplan/plone/tools/_dx4.py
 src/visaplan/plone/tools/_dx5.py
 src/visaplan/plone/tools/_have.py
 src/visaplan/plone/tools/attools.py
 src/visaplan/plone/tools/brains.py
 src/visaplan/plone/tools/cfg.py
 src/visaplan/plone/tools/configure.zcml
 src/visaplan/plone/tools/context.py
 src/visaplan/plone/tools/decorators.py
 src/visaplan/plone/tools/dxtools.py
-src/visaplan/plone/tools/env.py
 src/visaplan/plone/tools/forms.py
 src/visaplan/plone/tools/functions.py
+src/visaplan/plone/tools/groups.py
 src/visaplan/plone/tools/indexes.py
 src/visaplan/plone/tools/log.py
 src/visaplan/plone/tools/mock.py
 src/visaplan/plone/tools/mock_cfg.py
 src/visaplan/plone/tools/profiles.zcml
 src/visaplan/plone/tools/search.py
-src/visaplan/plone/tools/seo.py
 src/visaplan/plone/tools/setuphandlers.py
-src/visaplan/plone/tools/strings.py
 src/visaplan/plone/tools/zcmlgen.py
 src/visaplan/plone/tools/Extensions/install.py
-src/visaplan/plone/tools/groups/__init__.py
-src/visaplan/plone/tools/groups/_data.py
-src/visaplan/plone/tools/groups/_group.py
-src/visaplan/plone/tools/groups/_group_pio.py
-src/visaplan/plone/tools/groups/_helpers.py
-src/visaplan/plone/tools/groups/_imports.py
-src/visaplan/plone/tools/groups/_membership.py
-src/visaplan/plone/tools/groups/_user.py
-src/visaplan/plone/tools/groups/_user_pio.py
-src/visaplan/plone/tools/infofact/_group.py
-src/visaplan/plone/tools/infofact/_membership.py
-src/visaplan/plone/tools/infofact/_user.py
 src/visaplan/plone/tools/setup/__init__.py
 src/visaplan/plone/tools/setup/_args.py
 src/visaplan/plone/tools/setup/_attr.py
 src/visaplan/plone/tools/setup/_decorator.py
 src/visaplan/plone/tools/setup/_exc.py
 src/visaplan/plone/tools/setup/_get_object.py
 src/visaplan/plone/tools/setup/_gs.py
```

### Comparing `visaplan.plone.tools-1.4.17/CHANGES.rst` & `visaplan.plone.tools-1.4.9/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,128 +1,11 @@
-.. vim: sw=2 sts=2 tw=79 cc=+1
-
 Changelog
 =========
 
 
-1.4.17 (2023-04-05)
--------------------
-
-New features: 
-
-- function .attools.can_be_html(field)
-
-[tobiasherp]
-
-
-1.4.16 (2023-03-24)
--------------------
-
-New features: 
-
-- New function `short_hostname` in .functions
-
-[tobiasherp]
-
-
-1.4.15 (2023-03-08)
--------------------
-
-Bugfixes:
-
-- Py3K support fixes for
-
-  - .functions.is_uid_shaped
-  - .log.getLogSupport
-
-New features: 
-
-- New (still tiny) module .seo for SEO support;
-  for now, focused on structured data.
-  Functions:
-
-  - `parse_title`, returning a dict
-
-[tobiasherp]
-
-
-1.4.14 (2022-04-22)
--------------------
-
-Bugfixes:
-
-- Missing imports fixed for
-
-  - .groups.is_member_of__factory
-  - .setup.get_default_idxs
-
-[tobiasherp]
-
-
-1.4.13 (2022-03-04)
--------------------
-
-Bugfixes:
-
-- Fixed a bug in .groups.groupinfo_factory(pretty);
-  for this to work, we need visaplan.plone.groups.
-
-Improvements:
-
-- The label of the default logger of the ``@@step`` decorator
-  now includes the name of the worker, e.g. ``instance`` or ``client``
-
-New features: 
-
-- New `.env` module, providing the `worker_name()`
-
-[tobiasherp]
-
-
-1.4.12 (2022-02-15)
--------------------
-
-Bugfixes:
-
-- Fixed a bug in .groups.groupinfo_factory(pretty);
-  for this to work, we need visaplan.plone.groups.
-
-[tobiasherp]
-
-
-1.4.11 (2022-02-05)
--------------------
-
-Bugfixes:
-
-- Fixed a regression for .groups.groupinfo_factory
-
-[tobiasherp]
-
-
-1.4.10 (2022-02-03)
--------------------
-
-Improvements:
-
-- Converted the .groups module in a subpackage
-
-New features: 
-
-- New option `missing=False` for
-
-  - .groups.groupinfo_factory
-
-  If `True`, the resulting function creates an `existing` key,
-  and for missing groups, the `group_title` is `None`;
-  otherwise, an empty dict is returned in such cases.
-
-[tobiasherp]
-
-
 1.4.9 (2021-12-13)
 ------------------
 
 Improvements:
 
 - If collective.metadataversion_ is installed, use the configured default set of
   indexes (if no `idxs` explicitly given but metadata recreation is requested)
@@ -197,17 +80,16 @@
 
   We keep the the ``uninstall`` profile *for now;*
   it will be removed in an near-future version.
 
   So, *don't "install"* this package (Quick-Installer, Plone add-ons);
   just use it in Python_ code!
 
-  We keep the ``configure.zcml`` file and the autoinclude entry point
-  for now, though;
-  we can imagine to use e.g. the Plone registry for some settings.
+  We keep the ``configure.zcml`` file and the autoinclude entry point, though;
+  we can image to use e.g. the Plone registry for some settings.
 
 [tobiasherp]
 
 
 1.4.4 (2021-08-31)
 ------------------
```

### Comparing `visaplan.plone.tools-1.4.17/README.rst` & `visaplan.plone.tools-1.4.9/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -106,20 +106,14 @@
   - ``@returns_json``:
 
     Wraps the function call and returns the JSON_-encoded result,
     including HTTP headers.
 
     Uses simplejson_ if available.
 
-    **NOT** to be used for functions which simply provide JSON_ data for
-    insertion in page templates!
-
-    Otherwise, the browser might try to parse your HTML page as JSON
-    and fail.
-
 Documentation
 -------------
 
 Sorry, we don't have real user documentation yet.
 
 Most functions are documented by doctests, anyway;
 it helps to understand some German.
```

### Comparing `visaplan.plone.tools-1.4.17/long-description.rst` & `visaplan.plone.tools-1.4.9/long-description.rst`

 * *Files identical despite different names*

### Comparing `visaplan.plone.tools-1.4.17/setup.cfg` & `visaplan.plone.tools-1.4.9/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -17,17 +17,15 @@
 import_heading_setup = Setup tools:
 known_plone = plone,Products.CMFPlone
 import_heading_plone = Plone:
 import_heading_stdlib = Standard library:
 import_heading_stdlibold = Standard library (Python 2):
 import_heading_thirdparty = 3rd party:
 import_heading_localfolder = Local imports:
-known_pdfreactor = pdfreactor
-import_heading_pdfreactor = PDFreactor (by RealObjects; Python integration by visaplan GmbH):
-sections = FUTURE,COMPATIBILITY,SETUP,STDLIB,STDLIBOLD,PDFREACTOR,ZOPE,PLONE,THIRDPARTY,VISAPLAN,FIRSTPARTY,LOCALFOLDER,DEVEL
+sections = FUTURE,COMPATIBILITY,SETUP,STDLIB,STDLIBOLD,ZOPE,PLONE,THIRDPARTY,VISAPLAN,FIRSTPARTY,LOCALFOLDER,DEVEL
 dedup_headings = True
 multi_line_output = 8
 include_trailing_comma = True
 
 [check-manifest]
 ignore = 
 	*.cfg
```

### Comparing `visaplan.plone.tools-1.4.17/setup.py` & `visaplan.plone.tools-1.4.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 def valid_suffix(suffix):
     """
     Enforce our suffix convention
     """
     suffix = suffix.strip()
     if not suffix:
         return suffix
-    allowed = set('edv.0123456789rcpost')
+    allowed = set('dev.0123456789rcpost')
     disallowed = set(suffix).difference(allowed)
     if disallowed:
         disallowed = ''.join(sorted(disallowed))
         raise ValueError('Version suffix contains disallowed characters'
                          ' (%(disallowed)s)'
                          % locals())
     chunks = suffix.split('.')
@@ -54,15 +54,14 @@
             raise ValueError('Chunk %(chunk)r of version suffix %(suffix)r'
                              ' starts with a digit'
                              % locals())
         char = chunk[-1]
         if char not in '0123456789':
             raise ValueError('Chunk %(chunk)r of version suffix %(suffix)r'
                              ' doesn\'t end with a digit'
-                             ' (normalization would append a "0")'
                              % locals())
     return suffix  # ... valid_suffix
     # ... get the version ...
     # ... get the version ...
 VERSION = read_version('VERSION',
                        'VERSION_SUFFIX')
 # -------------------------------------------- ] ... get the version ]
@@ -112,25 +111,20 @@
     if pop_user:
         assert 'pick_user' not in kwargs
         assert 'user' not in kwargs
         user = pkg_list.pop(0)
         package = '.'.join(pkg_list)
     else:
         pick_user = pop('pick_user', 'user' not in kwargs)
-        given_user = pop('user', None)
         if pick_user:
             user = pkg_list[0]
-            if given_user is not None and given_user != user:
-                raise ValueError('given user %(given_user)r mismatches '
-                                 'user picked from package %(user)r!'
-                                 % locals())
-        elif given_user is not None:
-            user = given_user
+            if 'user' in kwargs:
+                assert pop('user') == user
         else:
-            raise ValueError('no user given nor picked!')
+            user = pop('user')
     if pop('travis', False):  # reqires github to be trueish
         res.update({  # CHECKME: is there a de-facto standard key for this?
             'Tests': 'https://travis-ci.org/%(user)s/%(package)s' % locals()
             })
     base = 'https://github.com/%(user)s/%(package)s' % locals()
     res.update({
         'Source': base,
@@ -175,15 +169,15 @@
     zip_safe=False,
     install_requires=[
         'setuptools',
         'six',
         'Products.CMFCore', # getToolByName
         # -*- Extra requirements: -*-
         'visaplan.tools >=1.3.1',  # list_of_strings improved
-        # 'visaplan.plone.infohubs >=1.1.1', ".hubs2 module" (prob. earlier)
+        # 'visaplan.plone.infohubs >=1.1.1.dev1',  # .hubs2 module
         # ... further requirements removed
     ],
     entry_points="""
     [z3c.autoinclude.plugin]
     target = plone
     """,
     extras_require={
```

### Comparing `visaplan.plone.tools-1.4.17/test.rst` & `visaplan.plone.tools-1.4.9/test.rst`

 * *Files 2% similar despite different names*

```diff
@@ -160,67 +160,34 @@
 .. _Plone: https://plone.org/
 .. _simplejson: https://pypi.org/project/simplejson
 .. _`visaplan GmbH`: http://visaplan.com
 
 .. vim: tw=79 cc=+1 sw=4 sts=4 si et
 
 
-To Do
-=====
-
-- Breaking changes:
-
-  - ``forms.tryagain_url``:
-
-    - all options (which are all arguments except the request)
-      will `need to` be given by name
-      (which is possible and `recommended already`).
-
-
-
 Contributors
 ============
 
 - Tobias Herp, tobias.herp@visaplan.com
 
 
 Changelog
 =========
 
 
-1.4.10 (unreleased)
--------------------
+2.0.0 (estimated)
+-----------------
 
-Breaking changes:
-
-Bugfixes:
-
-Improvements:
-
-- Converted the .groups module in a subpackage
-
-New features: 
-
-- New option `missing=False` for
-
-  - .groups.groupinfo_factory
-
-  If `True`, the resulting function creates an `existing` key,
-  and for missing groups, the `group_title` is `None`;
-  otherwise, an empty dict is returned in such cases.
-
-Profile changes:
-
-Requirements:
-
-Miscellaneous:
+- Breaking changes:
 
-Hints:
+  - ``forms.tryagain_url``:
 
-[tobiasherp]
+    - all options (which are all arguments except the request)
+      will `need to` be given by name
+      (which is possible and `recommended already`).
 
 
 1.4.9 (2021-12-13)
 ------------------
 
 Improvements:
```

### Comparing `visaplan.plone.tools-1.4.17/PKG-INFO` & `visaplan.plone.tools-1.4.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visaplan.plone.tools
-Version: 1.4.17
+Version: 1.4.9
 Summary: General tools for Plone sites
 Home-page: UNKNOWN
 Author: Tobias Herp
 Author-email: tobias.herp@visaplan.com
 License: GPL version 2
 Project-URL: Source, https://github.com/visaplan/plone.tools
 Project-URL: Documentation, https://pypi.org/project/visaplan.plone.tools
@@ -117,20 +117,14 @@
           - ``@returns_json``:
         
             Wraps the function call and returns the JSON_-encoded result,
             including HTTP headers.
         
             Uses simplejson_ if available.
         
-            **NOT** to be used for functions which simply provide JSON_ data for
-            insertion in page templates!
-        
-            Otherwise, the browser might try to parse your HTML page as JSON
-            and fail.
-        
         Documentation
         -------------
         
         Sorry, we don't have real user documentation yet.
         
         Most functions are documented by doctests, anyway;
         it helps to understand some German.
@@ -196,135 +190,18 @@
         
         Contributors
         ============
         
         - Tobias Herp, tobias.herp@visaplan.com
         
         
-        .. vim: sw=2 sts=2 tw=79 cc=+1
-        
         Changelog
         =========
         
         
-        1.4.17 (2023-04-05)
-        -------------------
-        
-        New features: 
-        
-        - function .attools.can_be_html(field)
-        
-        [tobiasherp]
-        
-        
-        1.4.16 (2023-03-24)
-        -------------------
-        
-        New features: 
-        
-        - New function `short_hostname` in .functions
-        
-        [tobiasherp]
-        
-        
-        1.4.15 (2023-03-08)
-        -------------------
-        
-        Bugfixes:
-        
-        - Py3K support fixes for
-        
-          - .functions.is_uid_shaped
-          - .log.getLogSupport
-        
-        New features: 
-        
-        - New (still tiny) module .seo for SEO support;
-          for now, focused on structured data.
-          Functions:
-        
-          - `parse_title`, returning a dict
-        
-        [tobiasherp]
-        
-        
-        1.4.14 (2022-04-22)
-        -------------------
-        
-        Bugfixes:
-        
-        - Missing imports fixed for
-        
-          - .groups.is_member_of__factory
-          - .setup.get_default_idxs
-        
-        [tobiasherp]
-        
-        
-        1.4.13 (2022-03-04)
-        -------------------
-        
-        Bugfixes:
-        
-        - Fixed a bug in .groups.groupinfo_factory(pretty);
-          for this to work, we need visaplan.plone.groups.
-        
-        Improvements:
-        
-        - The label of the default logger of the ``@@step`` decorator
-          now includes the name of the worker, e.g. ``instance`` or ``client``
-        
-        New features: 
-        
-        - New `.env` module, providing the `worker_name()`
-        
-        [tobiasherp]
-        
-        
-        1.4.12 (2022-02-15)
-        -------------------
-        
-        Bugfixes:
-        
-        - Fixed a bug in .groups.groupinfo_factory(pretty);
-          for this to work, we need visaplan.plone.groups.
-        
-        [tobiasherp]
-        
-        
-        1.4.11 (2022-02-05)
-        -------------------
-        
-        Bugfixes:
-        
-        - Fixed a regression for .groups.groupinfo_factory
-        
-        [tobiasherp]
-        
-        
-        1.4.10 (2022-02-03)
-        -------------------
-        
-        Improvements:
-        
-        - Converted the .groups module in a subpackage
-        
-        New features: 
-        
-        - New option `missing=False` for
-        
-          - .groups.groupinfo_factory
-        
-          If `True`, the resulting function creates an `existing` key,
-          and for missing groups, the `group_title` is `None`;
-          otherwise, an empty dict is returned in such cases.
-        
-        [tobiasherp]
-        
-        
         1.4.9 (2021-12-13)
         ------------------
         
         Improvements:
         
         - If collective.metadataversion_ is installed, use the configured default set of
           indexes (if no `idxs` explicitly given but metadata recreation is requested)
@@ -399,17 +276,16 @@
         
           We keep the the ``uninstall`` profile *for now;*
           it will be removed in an near-future version.
         
           So, *don't "install"* this package (Quick-Installer, Plone add-ons);
           just use it in Python_ code!
         
-          We keep the ``configure.zcml`` file and the autoinclude entry point
-          for now, though;
-          we can imagine to use e.g. the Plone registry for some settings.
+          We keep the ``configure.zcml`` file and the autoinclude entry point, though;
+          we can image to use e.g. the Plone registry for some settings.
         
         [tobiasherp]
         
         
         1.4.4 (2021-08-31)
         ------------------
```

