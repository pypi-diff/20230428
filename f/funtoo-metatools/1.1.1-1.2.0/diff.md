# Comparing `tmp/funtoo-metatools-1.1.1.tar.gz` & `tmp/funtoo-metatools-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/funtoo-metatools-1.1.1.tar", last modified: Sat Sep 17 01:38:26 2022, max compression
+gzip compressed data, was "dist/funtoo-metatools-1.2.0.tar", last modified: Fri Apr 28 13:38:27 2023, max compression
```

## Comparing `funtoo-metatools-1.1.1.tar` & `funtoo-metatools-1.2.0.tar`

### file list

```diff
@@ -1,99 +1,103 @@
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2022-09-17 01:38:26.000000 funtoo-metatools-1.1.1/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)       68 2022-04-15 16:54:39.000000 funtoo-metatools-1.1.1/.gitignore
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1046 2022-04-15 16:54:39.000000 funtoo-metatools-1.1.1/.pre-commit-config.yaml
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      230 2022-04-15 16:54:39.000000 funtoo-metatools-1.1.1/.pylintrc
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1237 2022-09-17 01:38:26.000000 funtoo-metatools-1.1.1/PKG-INFO
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      755 2022-04-15 18:46:15.000000 funtoo-metatools-1.1.1/README.rst
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2022-09-17 01:38:26.000000 funtoo-metatools-1.1.1/bin/
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1370 2022-07-01 21:12:13.000000 funtoo-metatools-1.1.1/bin/blos
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1735 2022-04-15 18:46:15.000000 funtoo-metatools-1.1.1/bin/deepdive
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      978 2022-04-15 16:54:39.000000 funtoo-metatools-1.1.1/bin/deepquery
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)       90 2022-07-05 16:37:27.000000 funtoo-metatools-1.1.1/bin/direct-sync
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     4602 2022-07-05 16:37:27.000000 funtoo-metatools-1.1.1/bin/distfile-kit-fetch
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     4497 2022-04-15 18:46:15.000000 funtoo-metatools-1.1.1/bin/distfile-stats
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     2831 2022-08-07 23:24:58.000000 funtoo-metatools-1.1.1/bin/doit
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     4115 2022-07-02 21:37:50.000000 funtoo-metatools-1.1.1/bin/fastpull-daemon
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     2201 2022-07-06 16:00:01.000000 funtoo-metatools-1.1.1/bin/fastpull-daemon-ng
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1534 2022-04-15 18:46:15.000000 funtoo-metatools-1.1.1/bin/fastpull-fixer
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      928 2022-04-15 16:54:39.000000 funtoo-metatools-1.1.1/bin/interkit-links
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      628 2022-04-15 18:46:15.000000 funtoo-metatools-1.1.1/bin/list-kits
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      528 2022-04-15 18:46:15.000000 funtoo-metatools-1.1.1/bin/mcafee-tool
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1020 2022-04-15 18:46:15.000000 funtoo-metatools-1.1.1/bin/merge-gentoo-staging
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     2271 2022-08-17 14:46:41.000000 funtoo-metatools-1.1.1/bin/merge-kits
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      974 2022-04-15 16:54:39.000000 funtoo-metatools-1.1.1/bin/missing-links
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      441 2022-04-15 16:54:39.000000 funtoo-metatools-1.1.1/bin/prod-regen
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1256 2022-04-15 18:46:15.000000 funtoo-metatools-1.1.1/bin/release-yaml-test
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     3559 2022-05-27 22:00:31.000000 funtoo-metatools-1.1.1/bin/reposcan
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      525 2022-05-07 21:05:04.000000 funtoo-metatools-1.1.1/bin/storage-test
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1638 2022-04-15 16:54:39.000000 funtoo-metatools-1.1.1/bin/test-metadata-extract
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2022-09-17 01:38:26.000000 funtoo-metatools-1.1.1/deprecated/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     3991 2022-04-15 18:46:15.000000 funtoo-metatools-1.1.1/deprecated/mongo_backends.py
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2022-09-17 01:38:26.000000 funtoo-metatools-1.1.1/docs/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      580 2022-04-15 16:54:39.000000 funtoo-metatools-1.1.1/docs/Makefile
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2022-09-17 01:38:26.000000 funtoo-metatools-1.1.1/docs/_ext/
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2022-09-17 01:38:26.000000 funtoo-metatools-1.1.1/docs/_ext/_static/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1184 2022-04-15 16:54:39.000000 funtoo-metatools-1.1.1/docs/_ext/_static/consoleoutput.css
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6297 2022-04-15 16:54:39.000000 funtoo-metatools-1.1.1/docs/_ext/consoleoutput.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    17066 2022-04-15 16:54:39.000000 funtoo-metatools-1.1.1/docs/autogen-dev.rst
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4994 2022-04-15 16:54:39.000000 funtoo-metatools-1.1.1/docs/autogen.rst
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2063 2022-04-15 16:54:39.000000 funtoo-metatools-1.1.1/docs/conf.py
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2022-09-17 01:38:26.000000 funtoo-metatools-1.1.1/docs/drafts/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    11938 2022-04-15 18:46:15.000000 funtoo-metatools-1.1.1/docs/drafts/fastpull_object_store.rst
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4297 2022-04-15 18:46:15.000000 funtoo-metatools-1.1.1/docs/drafts/repo_defs.rst
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2022-09-17 01:38:26.000000 funtoo-metatools-1.1.1/docs/features/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    10086 2022-08-04 19:07:50.000000 funtoo-metatools-1.1.1/docs/features/dynamic-archives.rst
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4371 2022-04-15 16:54:39.000000 funtoo-metatools-1.1.1/docs/index.rst
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2524 2022-04-15 16:54:39.000000 funtoo-metatools-1.1.1/docs/install.rst
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6051 2022-04-15 16:54:39.000000 funtoo-metatools-1.1.1/docs/intro.rst
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6159 2022-04-15 16:54:39.000000 funtoo-metatools-1.1.1/docs/meta-repo.rst
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2022-09-17 01:38:26.000000 funtoo-metatools-1.1.1/examples/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      192 2022-04-15 16:54:39.000000 funtoo-metatools-1.1.1/examples/reposcan.gentoo.yaml
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2022-09-17 01:38:26.000000 funtoo-metatools-1.1.1/funtoo/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2022-04-15 16:54:39.000000 funtoo-metatools-1.1.1/funtoo/__init__.py
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2022-09-17 01:38:26.000000 funtoo-metatools-1.1.1/funtoo/pkgtools/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2022-04-15 16:54:39.000000 funtoo-metatools-1.1.1/funtoo/pkgtools/__init__.py
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)    25664 2022-09-17 01:36:50.000000 funtoo-metatools-1.1.1/funtoo/pkgtools/autogen.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    20185 2022-08-07 23:24:58.000000 funtoo-metatools-1.1.1/funtoo/pkgtools/ebuild.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6511 2022-05-27 17:28:23.000000 funtoo-metatools-1.1.1/funtoo/pkgtools/fetch.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    17561 2022-09-17 01:36:50.000000 funtoo-metatools-1.1.1/funtoo/pkgtools/github.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2241 2022-04-15 16:54:39.000000 funtoo-metatools-1.1.1/funtoo/pkgtools/golang.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2404 2022-05-07 03:22:09.000000 funtoo-metatools-1.1.1/funtoo/pkgtools/http.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2915 2022-04-15 18:46:15.000000 funtoo-metatools-1.1.1/funtoo/pkgtools/meson.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     3148 2022-04-15 16:54:39.000000 funtoo-metatools-1.1.1/funtoo/pkgtools/pages.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    10039 2022-08-17 14:46:41.000000 funtoo-metatools-1.1.1/funtoo/pkgtools/pyhelper.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1947 2022-04-15 16:54:39.000000 funtoo-metatools-1.1.1/funtoo/pkgtools/rust.py
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2022-09-17 01:38:26.000000 funtoo-metatools-1.1.1/funtoo_metatools.egg-info/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1237 2022-09-17 01:38:26.000000 funtoo-metatools-1.1.1/funtoo_metatools.egg-info/PKG-INFO
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1835 2022-09-17 01:38:26.000000 funtoo-metatools-1.1.1/funtoo_metatools.egg-info/SOURCES.txt
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        1 2022-09-17 01:38:26.000000 funtoo-metatools-1.1.1/funtoo_metatools.egg-info/dependency_links.txt
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      121 2022-09-17 01:38:26.000000 funtoo-metatools-1.1.1/funtoo_metatools.egg-info/requires.txt
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)       17 2022-09-17 01:38:26.000000 funtoo-metatools-1.1.1/funtoo_metatools.egg-info/top_level.txt
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2022-09-17 01:38:26.000000 funtoo-metatools-1.1.1/metatools/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2022-04-15 18:46:15.000000 funtoo-metatools-1.1.1/metatools/__init__.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1049 2022-07-01 21:12:17.000000 funtoo-metatools-1.1.1/metatools/blos.py
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2022-09-17 01:38:26.000000 funtoo-metatools-1.1.1/metatools/config/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2022-04-15 18:46:15.000000 funtoo-metatools-1.1.1/metatools/config/__init__.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4891 2022-08-04 18:45:58.000000 funtoo-metatools-1.1.1/metatools/config/autogen.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2485 2022-07-05 16:37:27.000000 funtoo-metatools-1.1.1/metatools/config/base.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    21269 2022-07-05 16:37:27.000000 funtoo-metatools-1.1.1/metatools/config/merge.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      197 2022-04-15 18:46:15.000000 funtoo-metatools-1.1.1/metatools/config/mongodb.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1708 2022-04-15 18:46:15.000000 funtoo-metatools-1.1.1/metatools/context.py
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2022-09-17 01:38:26.000000 funtoo-metatools-1.1.1/metatools/fastpull/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2022-04-15 18:46:15.000000 funtoo-metatools-1.1.1/metatools/fastpull/__init__.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     7704 2022-08-04 17:15:49.000000 funtoo-metatools-1.1.1/metatools/fastpull/core.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    19448 2022-07-05 16:37:27.000000 funtoo-metatools-1.1.1/metatools/fastpull/spider.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4759 2022-05-27 17:28:01.000000 funtoo-metatools-1.1.1/metatools/fetch_cache.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      653 2022-07-01 21:12:17.000000 funtoo-metatools-1.1.1/metatools/hashutils.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    34092 2022-08-17 15:16:10.000000 funtoo-metatools-1.1.1/metatools/kit.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     5743 2022-07-11 21:19:25.000000 funtoo-metatools-1.1.1/metatools/kit_cache.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    14331 2022-07-07 19:53:49.000000 funtoo-metatools-1.1.1/metatools/metadata.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1225 2022-07-05 16:37:27.000000 funtoo-metatools-1.1.1/metatools/model.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     7351 2022-04-15 18:46:15.000000 funtoo-metatools-1.1.1/metatools/pretty_logging.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    21593 2022-08-17 15:16:10.000000 funtoo-metatools-1.1.1/metatools/steps.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    11361 2022-07-02 21:37:50.000000 funtoo-metatools-1.1.1/metatools/store.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      221 2022-04-15 18:46:15.000000 funtoo-metatools-1.1.1/metatools/thread.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    18172 2022-08-07 23:24:58.000000 funtoo-metatools-1.1.1/metatools/tree.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1711 2022-04-15 18:46:15.000000 funtoo-metatools-1.1.1/metatools/yaml_util.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)       38 2022-09-17 01:38:26.000000 funtoo-metatools-1.1.1/setup.cfg
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1093 2022-09-17 01:37:53.000000 funtoo-metatools-1.1.1/setup.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)       45 2022-04-15 16:54:39.000000 funtoo-metatools-1.1.1/subpop.yaml
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-04-28 13:38:27.000000 funtoo-metatools-1.2.0/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)       68 2022-04-15 16:54:39.000000 funtoo-metatools-1.2.0/.gitignore
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1046 2022-04-15 16:54:39.000000 funtoo-metatools-1.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      230 2022-04-15 16:54:39.000000 funtoo-metatools-1.2.0/.pylintrc
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1237 2023-04-28 13:38:27.000000 funtoo-metatools-1.2.0/PKG-INFO
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      755 2023-04-28 13:33:54.000000 funtoo-metatools-1.2.0/README.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        6 2023-04-28 13:35:25.000000 funtoo-metatools-1.2.0/VERSION
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-04-28 13:38:27.000000 funtoo-metatools-1.2.0/bin/
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1370 2022-07-01 21:12:13.000000 funtoo-metatools-1.2.0/bin/blos
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1736 2022-09-30 18:57:30.000000 funtoo-metatools-1.2.0/bin/deepdive
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      978 2022-04-15 16:54:39.000000 funtoo-metatools-1.2.0/bin/deepquery
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)       90 2022-07-05 16:37:27.000000 funtoo-metatools-1.2.0/bin/direct-sync
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     4602 2022-07-05 16:37:27.000000 funtoo-metatools-1.2.0/bin/distfile-kit-fetch
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     4497 2022-04-15 18:46:15.000000 funtoo-metatools-1.2.0/bin/distfile-stats
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     2845 2023-04-24 17:38:15.000000 funtoo-metatools-1.2.0/bin/doit
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     4115 2022-07-02 21:37:50.000000 funtoo-metatools-1.2.0/bin/fastpull-daemon
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     2201 2022-07-06 16:00:01.000000 funtoo-metatools-1.2.0/bin/fastpull-daemon-ng
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1534 2022-04-15 18:46:15.000000 funtoo-metatools-1.2.0/bin/fastpull-fixer
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1738 2023-04-24 17:38:15.000000 funtoo-metatools-1.2.0/bin/fetch
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      928 2022-04-15 16:54:39.000000 funtoo-metatools-1.2.0/bin/interkit-links
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      628 2022-04-15 18:46:15.000000 funtoo-metatools-1.2.0/bin/list-kits
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      528 2022-04-15 18:46:15.000000 funtoo-metatools-1.2.0/bin/mcafee-tool
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1171 2023-03-12 20:53:30.000000 funtoo-metatools-1.2.0/bin/merge-gentoo-staging
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     2271 2022-09-30 18:59:25.000000 funtoo-metatools-1.2.0/bin/merge-kits
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      974 2022-04-15 16:54:39.000000 funtoo-metatools-1.2.0/bin/missing-links
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      452 2023-03-12 20:53:30.000000 funtoo-metatools-1.2.0/bin/prod-regen
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1256 2022-04-15 18:46:15.000000 funtoo-metatools-1.2.0/bin/release-yaml-test
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     3559 2022-05-27 22:00:31.000000 funtoo-metatools-1.2.0/bin/reposcan
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      525 2022-05-07 21:05:04.000000 funtoo-metatools-1.2.0/bin/storage-test
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1638 2022-04-15 16:54:39.000000 funtoo-metatools-1.2.0/bin/test-metadata-extract
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-04-28 13:38:27.000000 funtoo-metatools-1.2.0/deprecated/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     3991 2022-04-15 18:46:15.000000 funtoo-metatools-1.2.0/deprecated/mongo_backends.py
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-04-28 13:38:27.000000 funtoo-metatools-1.2.0/docs/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      580 2022-04-15 16:54:39.000000 funtoo-metatools-1.2.0/docs/Makefile
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-04-28 13:38:27.000000 funtoo-metatools-1.2.0/docs/_ext/
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-04-28 13:38:27.000000 funtoo-metatools-1.2.0/docs/_ext/_static/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1184 2022-04-15 16:54:39.000000 funtoo-metatools-1.2.0/docs/_ext/_static/consoleoutput.css
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6297 2022-04-15 16:54:39.000000 funtoo-metatools-1.2.0/docs/_ext/consoleoutput.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    17066 2022-04-15 16:54:39.000000 funtoo-metatools-1.2.0/docs/autogen-dev.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4994 2022-04-15 16:54:39.000000 funtoo-metatools-1.2.0/docs/autogen.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2063 2022-04-15 16:54:39.000000 funtoo-metatools-1.2.0/docs/conf.py
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-04-28 13:38:27.000000 funtoo-metatools-1.2.0/docs/drafts/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    11938 2022-04-15 18:46:15.000000 funtoo-metatools-1.2.0/docs/drafts/fastpull_object_store.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4297 2022-04-15 18:46:15.000000 funtoo-metatools-1.2.0/docs/drafts/repo_defs.rst
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-04-28 13:38:27.000000 funtoo-metatools-1.2.0/docs/features/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    14475 2022-09-30 18:57:30.000000 funtoo-metatools-1.2.0/docs/features/dynamic-archives.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4371 2022-04-15 16:54:39.000000 funtoo-metatools-1.2.0/docs/index.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2524 2022-04-15 16:54:39.000000 funtoo-metatools-1.2.0/docs/install.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6051 2022-04-15 16:54:39.000000 funtoo-metatools-1.2.0/docs/intro.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6159 2022-04-15 16:54:39.000000 funtoo-metatools-1.2.0/docs/meta-repo.rst
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-04-28 13:38:27.000000 funtoo-metatools-1.2.0/examples/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      192 2022-04-15 16:54:39.000000 funtoo-metatools-1.2.0/examples/reposcan.gentoo.yaml
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-04-28 13:38:27.000000 funtoo-metatools-1.2.0/funtoo/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2022-04-15 16:54:39.000000 funtoo-metatools-1.2.0/funtoo/__init__.py
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-04-28 13:38:27.000000 funtoo-metatools-1.2.0/funtoo/pkgtools/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2022-04-15 16:54:39.000000 funtoo-metatools-1.2.0/funtoo/pkgtools/__init__.py
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)    25389 2023-04-24 17:38:15.000000 funtoo-metatools-1.2.0/funtoo/pkgtools/autogen.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    23084 2023-04-24 17:38:15.000000 funtoo-metatools-1.2.0/funtoo/pkgtools/ebuild.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6697 2023-04-26 20:36:15.000000 funtoo-metatools-1.2.0/funtoo/pkgtools/fetch.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    18724 2023-03-18 22:08:03.000000 funtoo-metatools-1.2.0/funtoo/pkgtools/github.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     9201 2023-04-24 17:38:15.000000 funtoo-metatools-1.2.0/funtoo/pkgtools/golang.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1851 2023-04-24 17:38:15.000000 funtoo-metatools-1.2.0/funtoo/pkgtools/http.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2915 2022-04-15 18:46:15.000000 funtoo-metatools-1.2.0/funtoo/pkgtools/meson.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     3148 2022-04-15 16:54:39.000000 funtoo-metatools-1.2.0/funtoo/pkgtools/pages.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    10039 2022-08-17 14:46:41.000000 funtoo-metatools-1.2.0/funtoo/pkgtools/pyhelper.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     8465 2023-04-24 17:38:15.000000 funtoo-metatools-1.2.0/funtoo/pkgtools/rust.py
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-04-28 13:38:27.000000 funtoo-metatools-1.2.0/funtoo_metatools.egg-info/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1237 2023-04-28 13:38:27.000000 funtoo-metatools-1.2.0/funtoo_metatools.egg-info/PKG-INFO
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1874 2023-04-28 13:38:27.000000 funtoo-metatools-1.2.0/funtoo_metatools.egg-info/SOURCES.txt
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        1 2023-04-28 13:38:27.000000 funtoo-metatools-1.2.0/funtoo_metatools.egg-info/dependency_links.txt
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      126 2023-04-28 13:38:27.000000 funtoo-metatools-1.2.0/funtoo_metatools.egg-info/requires.txt
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)       17 2023-04-28 13:38:27.000000 funtoo-metatools-1.2.0/funtoo_metatools.egg-info/top_level.txt
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      535 2023-04-28 13:37:35.000000 funtoo-metatools-1.2.0/make.sh
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-04-28 13:38:27.000000 funtoo-metatools-1.2.0/metatools/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2022-04-15 18:46:15.000000 funtoo-metatools-1.2.0/metatools/__init__.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1049 2022-07-01 21:12:17.000000 funtoo-metatools-1.2.0/metatools/blos.py
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-04-28 13:38:27.000000 funtoo-metatools-1.2.0/metatools/config/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2022-04-15 18:46:15.000000 funtoo-metatools-1.2.0/metatools/config/__init__.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4770 2023-04-24 17:38:15.000000 funtoo-metatools-1.2.0/metatools/config/autogen.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2739 2023-04-24 17:38:15.000000 funtoo-metatools-1.2.0/metatools/config/base.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    21759 2023-04-24 17:38:15.000000 funtoo-metatools-1.2.0/metatools/config/merge.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      197 2022-04-15 18:46:15.000000 funtoo-metatools-1.2.0/metatools/config/mongodb.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1695 2023-04-24 17:38:15.000000 funtoo-metatools-1.2.0/metatools/context.py
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-04-28 13:38:27.000000 funtoo-metatools-1.2.0/metatools/fastpull/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2022-04-15 18:46:15.000000 funtoo-metatools-1.2.0/metatools/fastpull/__init__.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     8855 2023-04-24 17:38:15.000000 funtoo-metatools-1.2.0/metatools/fastpull/core.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    27581 2023-04-26 20:35:17.000000 funtoo-metatools-1.2.0/metatools/fastpull/spider.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4759 2022-05-27 17:28:01.000000 funtoo-metatools-1.2.0/metatools/fetch_cache.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      653 2022-07-01 21:12:17.000000 funtoo-metatools-1.2.0/metatools/hashutils.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    34325 2023-03-12 20:53:30.000000 funtoo-metatools-1.2.0/metatools/kit.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     5829 2023-04-26 21:05:34.000000 funtoo-metatools-1.2.0/metatools/kit_cache.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    14331 2022-07-07 19:53:49.000000 funtoo-metatools-1.2.0/metatools/metadata.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1225 2022-07-05 16:37:27.000000 funtoo-metatools-1.2.0/metatools/model.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     7351 2022-04-15 18:46:15.000000 funtoo-metatools-1.2.0/metatools/pretty_logging.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    21883 2023-04-24 17:38:15.000000 funtoo-metatools-1.2.0/metatools/steps.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    11361 2022-07-02 21:37:50.000000 funtoo-metatools-1.2.0/metatools/store.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    18518 2023-04-24 17:38:15.000000 funtoo-metatools-1.2.0/metatools/tree.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)       22 2023-04-28 13:38:24.000000 funtoo-metatools-1.2.0/metatools/version.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1711 2022-04-15 18:46:15.000000 funtoo-metatools-1.2.0/metatools/yaml_util.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)       38 2023-04-28 13:38:27.000000 funtoo-metatools-1.2.0/setup.cfg
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1101 2023-04-28 13:38:24.000000 funtoo-metatools-1.2.0/setup.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1107 2023-04-28 13:37:51.000000 funtoo-metatools-1.2.0/setup.py.in
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)       45 2022-04-15 16:54:39.000000 funtoo-metatools-1.2.0/subpop.yaml
```

### Comparing `funtoo-metatools-1.1.1/.pre-commit-config.yaml` & `funtoo-metatools-1.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.1.1/PKG-INFO` & `funtoo-metatools-1.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: funtoo-metatools
-Version: 1.1.1
+Version: 1.2.0
 Summary: Funtoo framework for auto-creation of ebuilds.
 Home-page: https://code.funtoo.org/bitbucket/users/drobbins/repos/funtoo-metatools/browse
 Author: Daniel Robbins
 Author-email: drobbins@funtoo.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 
 ****************
 Funtoo Metatools
 ****************
 
-Copyright 2020-2022 Daniel Robbins, Funtoo Solutions, Inc.
+Copyright 2020-2023 Daniel Robbins, Funtoo Solutions, Inc.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `funtoo-metatools-1.1.1/README.rst` & `funtoo-metatools-1.2.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ****************
 Funtoo Metatools
 ****************
 
-Copyright 2020-2022 Daniel Robbins, Funtoo Solutions, Inc.
+Copyright 2020-2023 Daniel Robbins, Funtoo Solutions, Inc.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `funtoo-metatools-1.1.1/bin/blos` & `funtoo-metatools-1.2.0/bin/blos`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.1.1/bin/deepdive` & `funtoo-metatools-1.2.0/bin/deepdive`

 * *Files 0% similar despite different names*

```diff
@@ -49,7 +49,8 @@
 
 	merge.model.DEEPDIVE.delete_many({})
 	for source in pipeline_keys:
 		kit_dict_list = pipeline_groups[source]
 		for kit_dict in kit_dict_list:
 			ctx = NamespaceDict({"kit": NamespaceDict(kit_dict)})
 			hub.LOOP.run_until_complete(insert_kit(ctx))
+
```

### Comparing `funtoo-metatools-1.1.1/bin/deepquery` & `funtoo-metatools-1.2.0/bin/deepquery`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.1.1/bin/distfile-kit-fetch` & `funtoo-metatools-1.2.0/bin/distfile-kit-fetch`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.1.1/bin/distfile-stats` & `funtoo-metatools-1.2.0/bin/distfile-stats`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.1.1/bin/doit` & `funtoo-metatools-1.2.0/bin/doit`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!/usr/bin/env python3
 
 import argparse
 import asyncio
+import os
 import sys
 from datetime import timedelta
 
 from subpop.hub import Hub
 
 from metatools.config.autogen import AutogenConfig
 
@@ -55,22 +56,24 @@
 	for arg in set(CLI_CONFIG.keys()) - {"immediate"}:
 		kwargs[arg] = getattr(hub.OPT, arg)
 	if hub.OPT.immediate:
 		kwargs['fetch_cache_interval'] = timedelta(seconds=0)
 	await pkgtools.launch(AutogenConfig, **kwargs)
 	result = await pkgtools.autogen.start()
 	pkgtools.model.log.debug("Stopping spider...")
-	pkgtools.model.spider.stop()
+	await pkgtools.model.spider.stop()
 	pkgtools.model.log.debug("Spider stopped.")
 
 	return result
 
 if __name__ == "__main__":
-	success = hub.LOOP.run_until_complete(main_thread())
-	hub.LOOP.close()
+	success = asyncio.run(main_thread())
+
 	if not success:
 		sys.exit(1)
+	#	os._exit(1)
+	##	os._exit(0)
 
 # TODO: add 'facts' database concept to allow more resiliency on failures (fall back to cached facts from last
 #       successful run)
 
 # vim: ts=4 sw=4 noet
```

### Comparing `funtoo-metatools-1.1.1/bin/fastpull-daemon` & `funtoo-metatools-1.2.0/bin/fastpull-daemon`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.1.1/bin/fastpull-daemon-ng` & `funtoo-metatools-1.2.0/bin/fastpull-daemon-ng`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.1.1/bin/fastpull-fixer` & `funtoo-metatools-1.2.0/bin/fastpull-fixer`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.1.1/bin/interkit-links` & `funtoo-metatools-1.2.0/bin/interkit-links`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.1.1/bin/list-kits` & `funtoo-metatools-1.2.0/bin/list-kits`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.1.1/bin/mcafee-tool` & `funtoo-metatools-1.2.0/bin/mcafee-tool`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.1.1/bin/merge-gentoo-staging` & `funtoo-metatools-1.2.0/bin/merge-gentoo-staging`

 * *Files 15% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 #!/usr/bin/env python3
 
+from subpop.hub import Hub
+
 from metatools.tree import GitTree
 from metatools.steps import SyncFromTree
-from subpop.hub import Hub
+from metatools.config.base import MinimalConfig
+from metatools.kit import SimpleKitGenerator
 
 hub = Hub()
 
-import dyne.org.funtoo.metatools.merge as merge
-
 # This function updates the gentoo-staging tree with all the latest gentoo updates:
 
-
 async def gentoo_staging_update():
+	model = MinimalConfig()
+	await model.initialize()
 	gentoo_staging_w = GitTree(
 		"gentoo-staging",
 		"master",
 		url="ssh://git@code.funtoo.org:7999/auto/gentoo-staging.git",
-		root=merge.MERGE_CONFIG.dest_trees + "/gentoo-staging",
+		root=model.dest_trees + "/gentoo-staging",
+		model=model
 	)
 	gentoo_staging_w.initialize()
 
-	gentoo_src = GitTree("gentoo-x86", "master", "https://gitmerge.com/gentoo/gentoo.git", pull=True)
+	kit_gen = SimpleKitGenerator(out_tree=gentoo_staging_w)
+	gentoo_src = GitTree("gentoo-x86", "master", url="https://github.com/gentoo/gentoo.git", pull=True, model=model)
 	gentoo_src.initialize()
 
-	all_steps = [
-		SyncFromTree(
+	step = SyncFromTree(
 			gentoo_src,
 			exclude=[".gitignore", "eclass/.gitignore", "metadata/.gitignore", "/metadata/cache/**", "dev-util/metro"],
-		),
-	]
+		)
 
-	await gentoo_staging_w.run(all_steps)
-	gentoo_staging_w.gitCommit(message="gentoo updates")
+	await step.run(kit_gen)
+	gentoo_staging_w.gitCommit(message="gentoo updates", push=True)
 
 
 if __name__ == "__main__":
-
 	hub.LOOP.run_until_complete(gentoo_staging_update())
 
 # vim: ts=4 sw=4 noet
```

### Comparing `funtoo-metatools-1.1.1/bin/merge-kits` & `funtoo-metatools-1.2.0/bin/merge-kits`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.1.1/bin/missing-links` & `funtoo-metatools-1.2.0/bin/missing-links`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.1.1/bin/release-yaml-test` & `funtoo-metatools-1.2.0/bin/release-yaml-test`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.1.1/bin/reposcan` & `funtoo-metatools-1.2.0/bin/reposcan`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.1.1/bin/storage-test` & `funtoo-metatools-1.2.0/bin/storage-test`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.1.1/bin/test-metadata-extract` & `funtoo-metatools-1.2.0/bin/test-metadata-extract`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.1.1/deprecated/mongo_backends.py` & `funtoo-metatools-1.2.0/deprecated/mongo_backends.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.1.1/docs/Makefile` & `funtoo-metatools-1.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.1.1/docs/_ext/_static/consoleoutput.css` & `funtoo-metatools-1.2.0/docs/_ext/_static/consoleoutput.css`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.1.1/docs/_ext/consoleoutput.py` & `funtoo-metatools-1.2.0/docs/_ext/consoleoutput.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.1.1/docs/autogen-dev.rst` & `funtoo-metatools-1.2.0/docs/autogen-dev.rst`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.1.1/docs/autogen.rst` & `funtoo-metatools-1.2.0/docs/autogen.rst`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.1.1/docs/conf.py` & `funtoo-metatools-1.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.1.1/docs/drafts/fastpull_object_store.rst` & `funtoo-metatools-1.2.0/docs/drafts/fastpull_object_store.rst`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.1.1/docs/drafts/repo_defs.rst` & `funtoo-metatools-1.2.0/docs/drafts/repo_defs.rst`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.1.1/docs/features/dynamic-archives.rst` & `funtoo-metatools-1.2.0/docs/features/dynamic-archives.rst`

 * *Files 16% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 need to take manual steps to upload your special archive anywhere to get your ebuild to
 work -- instead, your autogen can simply create it. It's magic.
 
 How It Works
 ------------
 
 The development of this feature was tracked in Funtoo Linux issue FL-9270, and this issue
-also includes a diagram of the technical implementation of this feature.
+also includes a diagram of the technical implementation of this feature. The initial
+implementation has been improved as part of discussion/evaluation in FL-10403.
 
 A stand-alone Python autogen can now create an ``Archive``, which is now a base class
 for ``Artifact``. This archive is created locally, on a developer's system, by the autogen
 itself. When a PR is submitted with a new autogen, it is added to the official Funtoo tree,
 and then the autogen will also create this dynamic archive on the official tree regen system.
 The dynamic archive created during official tree regen will end up on the CDN automatically.
 Thus, a Funtoo developer has a way for an autogen to create an archive which it in turn can
@@ -25,18 +26,43 @@
 The thing to understand about the ``Archive`` is that from an ebuild perspective, it's
 identical to an ``Artifact``. This means you will still pass it to the ``artifacts=``
 keyword argument of your ``BreezyBuild``. This is actually required, as just like an
 ``Artifact``, an ``Archive`` is a file downloaded by ``ebuild``/``emerge`` and thus it
 will need to have a ``Manifest`` entry generated for it. Therefore, it will need to be
 in ``artifacts=`` and referenced in ``SRC_URI`` in the ebuild template itself.
 
-How To Use
-----------
+Autogen Workflow Overview
+-------------------------
 
-Let's go through a gradual process to get familiar with how to use the ``Archive``:
+The dynamic archive API has been designed to allow several possible workflows, depending
+on scenario.
+
+The basic workflow that all autogens should follow is to first search for
+the desired dynamic archive to see if it was created on a previous autogen run, and
+then optionally perform additional processing/introspection to see if it wants to use
+this previously-created archive.
+
+If the dynamic archive is found and seems acceptable, the autogen should use it as-is. If
+not, it should create a new dynamic archive, store it using this API, and use it for ebuild
+creation. It will then be available for future autogen runs to retrieve.
+
+Storage and Retrieval
+---------------------
+
+There are two supported mechanisms for storing and retrieving archives -- retrieval
+by *filename* (optionally with an associated *key*), and retrieval purely by *key*.
+
+Rather than go into the details right away, let's look at how to store and retrieve
+dynamic archives by *filename*. You can use this approach if your autogen workflow
+allows you to *know the name of the archive you want to use in advance.*
+
+How To Use Retrieval By Filename
+--------------------------------
+
+Let's go through a gradual process to get familiar using retrieval by filename.
 
 To create a new archive, you will specify a ``final_name``, which is the name of the
 archive on disk. This is done as follows:
 
 .. code-block:: python
 
    my_archive = hub.Archive("foobar-go-modules-1.2.3.tar.xz")
@@ -44,83 +70,146 @@
 Once the ``Archive`` has been created, files can be added to it, and then it can be stored.
 When storing the archive, a dictionary key containing arbitrary values can optionally be
 supplied, as follows:
 
 .. code-block:: python
 
    master_gosum = "abcdef0123456789"
-   my_archive.store(key={"gosum": master_gosum})
+   my_archive.store_by_name(key={"gosum": master_gosum})
 
 This is not complete code, as if you just create an ``Archive`` and store it, you will
 have an archive with nothing in it. We're just getting familiar with the basic constructor
-and ``store()`` method right now. You will notice the use of a ``key``.
+and ``store_by_name()`` method right now. You will notice the use of a ``key``.
 
 This key is optional and is used to uniquely identify the archive and can be used to
 differentiate it from previously-created archives that might otherwise seem identical due
-to having the same name. So this key is a very powerful tool to ensure your autogen is
-getting a correct and up-to-date archive, and you are encouraged to use it to include any
-unique values that are associated with the particular archive being created.
+to having the same name. This means the key is used at *retrieval time* to further
+specify a distinct archive, and if the key doesn't match what was stored, no archive
+will be found.(Internally, the dynamic archive implementation
+uses cryptographic digests to differentiate between otherwise-identical archives.)
 
 Now that we have looked at these two methods, let's look at a full run of how you should
-use an ``Archive`` in your code. The basic workflow is to:
+use an ``Archive`` in your code to store and retrieve by filename. The basic workflow is to:
 
 1. Try to retrieve an existing ``Archive`` that might have been created in a previous
-   autogen run that meets your criteria (i.e. ``final_name`` and any optional ``key``
+   autogen run that has a matching name (and any optional ``key``
    data matching.)
 2. If found, you will simply using this retrieved previously-created archive and pass
    it your ``BreezyBuild`` ``artifacts=`` keyword argument and use it like a regular
    ``Artifact``.
 3. If *not* found, then you will have code *create* the ``Archive`` in real-time, and
-   call the ``.store()`` method to store it. You will then use this newly-created archive
+   call the ``.store_by_name()`` method to store it. You will then use this newly-created archive
    by passing it to your ``BreezyBuild`` ``artifacts=`` keyword argument.
 
 Here is a snippet of code that uses an ``Archive`` properly:
 
 .. code-block:: python
 
    master_gosum = "abcdef0123456789"
-   my_archive = hub.Archive.find("foobar-go-modules-1.2.3.tar.xz", key={"gosum" : master_gosum})
+   my_archive, metadata = hub.Archive.find_by_name("foobar-go-modules-1.2.3.tar.xz", key={"gosum" : master_gosum}))
    if my_archive is None:
        my_archive = hub.Archive("foobar-go-modules-1.2.3.tar.xz")
        my_archive.initialize("dynamic-archive-1.0")
        with open(os.path.join(my_archive.top_path, "README"), "w") as myf:
            myf.write("HELLO")
-       my_archive.store(key={"gosum": master_gosum})
-
-    # At this point in your code, your my_archive exists, whether it was created in this
-    # run or retrieved from the local object store as it was created in a previous run.
-
-    my_eb = hub.pkgtools.ebuild.BreezyBuild(**pkginfo, artifacts=[my_archive])
-
-Some things to note here -- when looking for an existing archive, the final name is
-specified, as well as the exact key that was used to store the archive. This key must match
-exactly for the archive to be retrieved. For clarity it is often helpful to put a part of
-the key in the filename to avoid confusion for users as well as Portage if multiple variants
-of the same filename may be downloaded to ``/var/cache/portage/distfiles``. Here's an example
-of how one might do that:
-
-.. code-block:: python
-
-   my_archive = hub.Archive.find(f"foobar-go-modules-1.2.3-{master_gosum[:7]}.tar.xz", key={"gosum" : master_gosum})
+       my_archive.store_by_name(key={"gosum": master_gosum})
 
 Please also note the ``.initialize()`` method. This creates a new temporary on-disk location
 for the archive that you can copy files into. It has an optional argument which you should generally
 specify, which is the ``top_directory`` that will exist when the archive is extracted -- it's
 best practice to create archives where all your files are themselves within a directory so that
 others extracting your archive get a directory created for them.
 
 Then you will see use of the ``.top_path`` property, which will give you the path *inside*
 the top directory of your archive, and within ``.top_path`` is where you should create files. In
 our case, this is where we create a ``README`` file that will become a part of our archive.
 
-Finally, we ``.store`` our new ``Archive``, using the unique key we want to associate with our
-archive, which could be some kind of master gosum or a GitHub commit hash. Then, we use our
+Finally, we ``.store_by_name`` our new ``Archive``, using an optional unique key we want to associate with our
+archive, which could be some kind of master gosum or a GitHub commit hash which *must* match
+for the ``Archive`` to be returned. Then, we use our
 ``Archive`` just like an ``Artifact``, and voila -- we have the ability to create tarballs
 from autogens!
 
+How To Use Retrieval By Key
+---------------------------
+
+There may be autogen workflows where you do not know the exact name of the Archive in
+advance, but want to retrieve the archive based on other criteria you *do* know -- don't
+worry, we have a method for that too! This approach is more advanced, but you will see
+that the code is very similar.
+
+Using a pure key allows unlimited flexibility and
+adaptability to pretty much any possible autogen workflow. Here's an example where we
+can retrieve an Archive just by knowing the unique key it was stored under:
+
+.. code-block:: python
+
+   master_gosum = "abcdef0123456789"
+   key={"catpkg": catpkg, "gosum" : master_gosum}
+   my_archive, metadata = hub.Archive.find(key=key))
+   if my_archive is None:
+       my_archive = hub.Archive(f"foobar-go-modules-{version}.tar.xz")
+       my_archive.initialize(f"dynamic-archive-{version}")
+       with open(os.path.join(my_archive.top_path, "README"), "w") as myf:
+           myf.write("HELLO")
+       my_archive.store(key=key)
+
+    # At this point in your code, your my_archive exists, whether it was created in this
+    # run or retrieved from the local object store as it was created in a previous run.
+
+    my_eb = hub.pkgtools.ebuild.BreezyBuild(**pkginfo, artifacts=[my_archive])
+
+Above, we store the ``Archive``, indexed exclusively by the catpkg of the ebuild, and
+the master gosum. This means we don't need to know the exact filename used to store the
+``Archive``. However, if the ``Archive`` can be retrieved, it will be populated with the
+name that it had when it was created.
+
+Why is this useful? There are several scenarios:
+
+Maybe we have several ebuilds that share a dynamic archive. It may be easier to store by
+an agreed-upon key rather than specific filename.
+
+Maybe our autogen doesn't care about the version of the dynamic archive it is using -- it
+simply wants to use the "latest" archive. This allows easy retrieval in this case.
+
+Maybe our autogen wants to avoid using a version in the archive name altogether, and
+instead use some kind of arbitrary hash. This is also now possible.
+
+Maybe our autogen wants to retrieve an Archive, but do additional investigation to see if
+the archive can still be used. Maybe, if it needs replacement, the autogen will want to
+increment the version number or revision of the archive itself, so "extras-1.0.0.tar.xz"
+becomes "extras-1.0.1.tar.gz", etc. This is now possible!
+
+Using Metadata
+--------------
+
+You will notice that our calls to ``Archive.find()`` and ``Archive.find_by_name()`` return
+a ``metadata`` value:
+
+.. code-block:: python
+
+   my_archive, metadata = hub.Archive.find_by_name("foobar-go-modules-1.2.3.tar.xz", key={"gosum" : master_gosum}))
+
+What is metadata, and what is it useful for? Well, the metadata can store things just like
+the key, but it is not used to match when retrieving the object. So you can always store additional
+information in the metadata as follows, if you do not want it used to find the archive, but might
+have use for this data later in processing. Both ``archive.store()`` and ``archive.store_by_name()``
+accept an optional metadata dictionary:
+
+.. code-block:: python
+
+    my_archive.store(key=key, metadata={ "author" : "drobbins was here!" })
+
+You can use this metadata to perform further processing to determine if the archive you retrieved
+is truly acceptable to your autogen. You could also store a version counter or build number here
+if you wanted to dynamically increment it.
+
+Bonus feature of metadata: your ``metadata`` will always contain a ``created_on`` timestamp containing the UTC
+time of when the archive was created by the autogen process.
+
 Q&A
 ---
 
 What archive formats are supported?
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Currently, ".tar.xz" and ".tar.zstd" format archives are supported, and the compression format is
@@ -132,14 +221,18 @@
 ``key=`` must be a dictionary, but it can contain a lot of things, including booleans, strings, integers,
 floating-point, DateTime, lists and other dictionaries. So you can organize the data within ``key=`` so
 that it makes sense for your needs and it's definitely possible to create nested and more
 complex structures that contain different kinds of data. For a complete list of supported object types,
 see https://pymongo.readthedocs.io/en/stable/api/bson/index.html for a list of objects that are listed
 as "both" for "Supported direction"
 
+What can I store in the ``metadata=`` keyword argument?
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+Same as ``key=``. See above.
+
 How does my archive end up on the CDN?
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 When your autogen is run during official tree regeneration, it will create a dynamic archive which
 gets automatically populated to our CDN. In addition, any ebuild(s) autogenerated during this tree
 regeneration will specifically reference this archive.
```

### Comparing `funtoo-metatools-1.1.1/docs/index.rst` & `funtoo-metatools-1.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.1.1/docs/install.rst` & `funtoo-metatools-1.2.0/docs/install.rst`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.1.1/docs/intro.rst` & `funtoo-metatools-1.2.0/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.1.1/docs/meta-repo.rst` & `funtoo-metatools-1.2.0/docs/meta-repo.rst`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.1.1/funtoo/pkgtools/autogen.py` & `funtoo-metatools-1.2.0/funtoo/pkgtools/autogen.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import asyncio
 import inspect
 import os
 import threading
 import subprocess
 from asyncio import FIRST_EXCEPTION, Task
 from collections import defaultdict
-from concurrent.futures.thread import ThreadPoolExecutor
+from typing import Tuple, List
 
 import dyne.org.funtoo.metatools.pkgtools as pkgtools
 from yaml import safe_load
 
 from subpop.util import load_plugin
 
 """
@@ -20,15 +20,14 @@
 are defined multiple times and other errors that we should catch before processing begins. The work is organized
 by the generator (pop plugin) that will be used to generate a list of catpkgs. Before we start, we have
 everything organized so that we only need to call `execute_generator` once for each generator. It will start
 work for all catpkgs in that generator, and wait for completion of this work before returning.
 """
 
 PENDING_QUE = []
-AUTOGEN_FAILURES = []
 GENNED_BREEZYBUILDS = {}
 GENNED_BREEZYBUILDS_LOCK = threading.Lock()
 
 SUB_FP_MAP_LOCK = asyncio.Lock()
 SUB_FP_MAP = {}
 
 """
@@ -125,14 +124,15 @@
 			out_dict[key] = dict2[key]
 	return out_dict
 
 
 def recursive_merge_many(*dicts, overwrite=True):
 	"""
 	This function applies `recursive_merge` to multiple `dicts`, going from left to right.
+	TODO: upgrade pkginfo to an attrdict, because attrs are nicer to use.
 	"""
 	result = {}
 	for current_dict in dicts:
 		if not current_dict:
 			continue
 
 		result = recursive_merge(result, current_dict, overwrite=overwrite)
@@ -168,45 +168,39 @@
 				"template_path": os.path.join(subpath, "templates"),
 				"pkginfo_list": [{"name": pkg_name, "cat": pkg_cat}],
 			}
 		)
 		pkgtools.model.log.debug(f"Added to queue of pending autogens: {PENDING_QUE[-1]}")
 
 
-async def gather_pending_tasks(name, task_list):
+async def gather_pending_tasks(name, task_list) -> Tuple[List, List]:
 	"""
-	This function collects completed asyncio coroutines, catches any exceptions recorded during their execution.
+	This function collects completed asyncio coroutines, catches any exceptions recorded during their execution,
+	and will any tasks that returned execptions to the returned list.
+
+	This function returns a tuple: a list of results from each successful tasks that weren't just None, and a
+	list of tasks that failed (threw exceptions) -- so you can inspect them further.
 
 	Use "name" to specify the kinds of tasks you are collecting. This will assist with error reporting.
 	"""
-	results = []
 	cur_tasks = task_list
-	exceptions = 0
+	failures = []
+	results = []
 	if not len(cur_tasks):
 		return [], []
 	while True:
 		done_list, cur_tasks = await asyncio.wait(cur_tasks, return_when=FIRST_EXCEPTION)
-		# Because we are setting add_done_callback(_handle_task_result) for each task we are trying to gather, and
-		# using the callback to look at the result and detect exceptions, we don't have to do this here anymore.
-		# The callback is preferred because we can set the proper kind of exception handling for the particular
-		# task rather than having to figure that out here.
 		for done_item in done_list:
 			try:
-				result = done_item.result()
-				results.append(result)
-			except Exception as e:
-				exceptions += 1
-			pkgtools.model.log.debug(f"Gathered task: {done_item} {result}")
+				results.append(done_item.result())
+			except Exception:
+				failures.append(done_item)
 		if not len(cur_tasks):
 			break
-	if exceptions:
-		pkgtools.model.log.critical(f"{name} exceptions encountered: {exceptions}")
-		raise RuntimeError("One or more tasks failed.")
-
-	return results
+	return results, failures
 
 
 def init_pkginfo_for_package(pkginfo, sub_path, template_path=None, gen_path=None):
 	"""
 	This function generates the final pkginfo that is passed to the generate() function in the generator sub
 	for each catpkg being generated. If an autogen.yaml is being used, then these settings come from YAML. If
 	an autogen.py is used, there are still some basic things that are auto-defined like the cat and name.
@@ -245,45 +239,14 @@
 	# This is the path where the autogen lives. Either the autogen.py or the autogen.yaml:
 	common_prefix = os.path.commonprefix([pkgtools.model.locator.root, gen_path])
 	path_from_root = gen_path[len(common_prefix):].lstrip("/")
 	pkginfo["gen_path"] = f"${{REPODIR}}/{path_from_root}"
 	return pkginfo
 
 
-def _handle_task_result(task: Task):
-	try:
-		success = task.result()
-		if not success:
-			fail_info = getattr(task, 'info', None)
-			if fail_info:
-				AUTOGEN_FAILURES.append(fail_info)
-			else:
-				AUTOGEN_FAILURES.append("Unknown Autogen!")
-	except asyncio.CancelledError:
-		pass
-	except Exception as e:
-		fail_info = getattr(task, 'info', None)
-		if fail_info:
-			AUTOGEN_FAILURES.append(fail_info)
-		else:
-			AUTOGEN_FAILURES.append("Unknown Autogen (2)!")
-
-
-def _artifact_handle_task_result(task: Task):
-	try:
-		task.result()
-	except asyncio.CancelledError:
-		pass
-	except Exception as e:
-		pkgtools.model.log.error(e, exc_info=True)
-
-
-# TODO: record these failures in a global place if this is still a valid exception-catching path.
-
-
 async def execute_generator(
 		generator_sub_path=None,
 		generator_sub_name="autogen",
 		template_path=None,
 		defaults=None,
 		pkginfo_list=None,
 		gen_path=None,
@@ -363,15 +326,15 @@
 
 		# Perform selective filtering of autogens we may want to exclude via command-line:
 
 		if pkgtools.model.filter is not None:
 			filtered_pkginfo_list = []
 			for item in pkginfo_list:
 				catpkg = item['cat'] if 'cat' in item else "(None)"
-				catpkg += item['name'] if 'name' in item else "(None)"
+				catpkg += '/' + item['name'] if 'name' in item else "(None)"
 				if pkgtools.model.filter_cat:
 					if 'cat' not in item or item['cat'] != pkgtools.model.filter_cat:
 						pkgtools.model.log.debug(f"Filtered due to cat: {catpkg}")
 						continue
 				if pkgtools.model.filter_pkg:
 					if 'name' not in item or item['name'] != pkgtools.model.filter_pkg:
 						pkgtools.model.log.debug(f"Filtered due to name: {catpkg}")
@@ -476,20 +439,19 @@
 
 			task = Task(gen_wrapper(pkginfo, generator_sub))
 
 			# task.info is used for error messages. Try to add catpkg info in it if it exists:
 			task.info = sub_path
 			if "cat" in pkginfo and "name" in pkginfo:
 				task.info += f" ({pkginfo['cat']}/{pkginfo['name']})"
-
-			task.add_done_callback(_handle_task_result)
 			hub.THREAD_CTX.running_autogens.append(task)
 
-		await gather_pending_tasks("autogen", hub.THREAD_CTX.running_autogens)
-		await gather_pending_tasks("breezybuild", hub.THREAD_CTX.running_breezybuilds)
+		a_results, a_failures = await gather_pending_tasks("autogen", hub.THREAD_CTX.running_autogens)
+		b_results, b_failures = await gather_pending_tasks("breezybuild", hub.THREAD_CTX.running_breezybuilds)
+		return a_failures + b_failures
 
 	return generator_thread_task, pkginfo_list
 
 
 def parse_yaml_rule(package_section=None):
 	pkginfo_list = []
 	defaults = {}
@@ -623,29 +585,34 @@
 					}
 				)
 				pkgtools.model.log.debug(f"Added to queue of pending autogens: {PENDING_QUE[-1]}")
 
 
 async def execute_all_queued_generators():
 	futures = []
-	loop = asyncio.get_running_loop()
-	with ThreadPoolExecutor(max_workers=16) as executor:
-		while len(PENDING_QUE):
-			task_args = PENDING_QUE.pop(0)
-
-			# The "autogen_id" entry here is going to be used like an ID for distfile integrity Artifacts that aren't
-			# attached to a specific BreezyBuild.
-
-			base = os.path.commonprefix([task_args["gen_path"], pkgtools.model.locator.root])
-			task_args["autogen_id"] = f"{pkgtools.model.kit_spy}:{task_args['gen_path'][len(base) + 1:]}"
-			async_func, pkginfo_list = await execute_generator(**task_args)
-			future = loop.run_in_executor(executor, hub.run_async_adapter, async_func, pkginfo_list)
-			futures.append(future)
+	all_failures = []
+	while len(PENDING_QUE):
+		task_args = PENDING_QUE.pop(0)
+
+		# The "autogen_id" entry here is going to be used like an ID for distfile integrity Artifacts that aren't
+		# attached to a specific BreezyBuild.
+
+		base = os.path.commonprefix([task_args["gen_path"], pkgtools.model.locator.root])
+		task_args["autogen_id"] = f"{pkgtools.model.kit_spy}:{task_args['gen_path'][len(base) + 1:]}"
+		async_func, pkginfo_list = await execute_generator(**task_args)
+		future = async_func(pkginfo_list)
+		futures.append(future)
+
+	results, failures = await gather_pending_tasks("generator", futures)
+	# All the "results" of the async_func are lists of failures -- so we should aggregate all of these:
+	all_fails = pkgtools.ebuild.aggregate(results)
+	all_fails += pkgtools.ebuild.aggregate(failures)
+	all_failures += all_fails
 
-		await gather_pending_tasks("generator", futures)
+	return all_failures
 
 
 async def start():
 	# This is a hack to iterate through all plugins to ensure they are all loaded prior to starting threads, so we
 	# don't experience race conditions loading modules, as this clobbers sys.modules in a non-threadsafe way currently.
 	for plugin in pkgtools:
 		pass
@@ -668,28 +635,41 @@
 			else:
 				raise TypeError(f"Unrecognized file type: {abs_path}")
 
 	queue_all_indy_autogens(indy_autogens)
 	queue_all_yaml_autogens(yaml_autogens)
 
 	failure = False
+	fail_list = []
 	try:
-		await execute_all_queued_generators()
+		fail_list = await execute_all_queued_generators()
 	except RuntimeError:
 		failure = True
-
+	if fail_list:
+		failure = True
 	if not failure:
 		generate_manifests()
-		pkgtools.model.log.debug("generate_manifests() complete.")
+		pkgtools.model.log.debug(f"FINISH: start() complete for {pkgtools.model.current_repo.root} - path 1, return True")
 		return True
 	else:
-		if len(AUTOGEN_FAILURES):
-			if len(AUTOGEN_FAILURES) == 1:
-				pkgtools.model.log.error(f"An error was encountered when processing {AUTOGEN_FAILURES[0]}")
-			else:
-				pkgtools.model.log.error(f"Errors were encountered when processing the following autogens:")
-				for fail in AUTOGEN_FAILURES:
-					pkgtools.model.log.error(f" * {fail}")
-			return False
-
+		pkgtools.model.log.error(f"Autogen failed (count: {len(fail_list)}).")
+		extra_info = []
+		if len(fail_list):
+
+			for fail in fail_list:
+				fail_info = getattr(fail, 'info', None)
+				if fail_info:
+					extra_info.append(fail_info)
+		if len(extra_info):
+			# This will remove all duplicates
+			extra_info_dedup = sorted(list(set(extra_info)))
+			if len(extra_info_dedup) != len(extra_info):
+				# TODO: this duplicate failure issue is an ongoing, unresolved bug.
+				pkgtools.model.log.error(
+					f"Number of failures ({len(extra_info)}) had duplicates {len(extra_info) - len(extra_info_dedup)})")
+			pkgtools.model.log.error(f"Errors were encountered when processing the following autogens:")
+			for fail in extra_info:
+				pkgtools.model.log.error(f" * {fail}")
+			pkgtools.model.log.error(f"End of report.")
+		return False
 
 # vim: ts=4 sw=4 noet
```

### Comparing `funtoo-metatools-1.1.1/funtoo/pkgtools/ebuild.py` & `funtoo-metatools-1.2.0/funtoo/pkgtools/ebuild.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 #!/usr/bin/env python3
 
+from __future__ import annotations
 import asyncio
 import logging
 import os
 import shutil
 import threading
 from asyncio import Task
 from collections import OrderedDict
+from datetime import datetime
 from subprocess import getstatusoutput
-from typing import Optional
+from typing import Optional, Tuple
 
 import jinja2
 
+from metatools.steps import run_bg
 from metatools.store import StoreObject
 from metatools.fastpull.spider import FetchError, FetchRequest
 
 log = logging.getLogger('metatools.autogen')
 
 import dyne.org.funtoo.metatools.pkgtools as pkgtools
 
@@ -95,91 +98,135 @@
 		:return:
 		"""
 		self._top_directory = top_directory
 		if os.path.exists(self.extract_path):
 			shutil.rmtree(self.extract_path)
 		os.makedirs(self.top_path, exist_ok=False)
 
-	# TODO: add a method to try to retrieve the archive and create it from our dynamic
-	#       store.
 
-	def store(self, key=None):
+	async def store(self, key: dict = None, metadata: dict = None):
 		"""
-		This method is designed to archive the contents of files in extract_path, store it as
-		final_name, add it to the BLOS, and create or update the dynamic integrity database.
-		:param format:
-		:return:
+		This method will store an archive as a dynamic archive, indexed by ``key``. If you want
+		to store a dynamic archive for later retrieval *by name*, then use the ``Archive.store_by_name``
+		method instead.
+
+		An optional ``metadata`` dictionary can be provided, which will also be stored with the
+		dynamic archive. A datestamp will automatically be stored in ``metadata['created_on']`` for
+		you. All other metadata can be provided by you. This metadata, unlike the key, is not used
+		to *find*/*match* the object when retrieval is attempted; instead, the metadata is just made
+		available to you upon retrieval. So you can use it to store extra things that are of
+		interest to you.
 		"""
 		if key is None:
 			key = {}
 
+		if metadata is None:
+			metadata = {}
+		metadata["created_on"] = datetime.utcnow()
+
 		temp_archive = self.temp_archive_path
 
 		# Ensure we have a clean location for creating a new temporary archive:
 
 		if not os.path.exists(os.path.dirname(temp_archive)):
 			os.makedirs(os.path.dirname(temp_archive), exist_ok=True)
 
 		if os.path.exists(temp_archive):
 			os.unlink(temp_archive)
 
 		# Create the archive:
 
 		if self.final_name.endswith(".tar.xz"):
 			cmd = f"tar -C {self.extract_path} -cJf {temp_archive} ."
-		elif self.final_name.endswith(".tar.zstd"):
+		elif self.final_name.endswith(".tar.gz"):
+			cmd = f"tar -C {self.extract_path} -czf {temp_archive} ."
+		elif self.final_name.endswith(".tar.zst"):
 			cmd = f"tar -C {self.extract_path} -c --zstd -f {temp_archive} ."
 		else:
-			raise ValueError(f"Unrecognized archive format: {self.final_name}")
+			raise ValueError(f"Unrecognized archive format: {self.final_name}. Supported formats: tar.gz, tar.xz, tar.zst")
 		log.debug(f"store: command: {cmd}")
-		s, o = getstatusoutput(cmd)
-		if s != 0:
-			raise pkgtools.ebuild.BreezyError(f"Couldn't create archive {self.final_name}. Error: {o}")
 
-		# Insert the archive. We will unconditionally store 'final_name' in the key, as
-		# all files should at least be referenced by their expected name, and we will need
-		# this for checking for this particular file's existence.
-
-		key["final_name"] = self.final_name
-		assert isinstance(key, dict)
+		proc, out = await run_bg(cmd)
+		if proc.returncode != 0:
+			raise pkgtools.ebuild.BreezyError(f"Couldn't execute {cmd}. Output: {out.decode()}")
 
 		# Store in BLOS and create integrity database reference:
 
 		self.blos_object = pkgtools.model.blos.insert_blob(temp_archive)
-		pkgtools.model.fastpull_session.store_file_dynamic(key, temp_archive)
+		pkgtools.model.fastpull_session.store_file_dynamic(key, temp_archive, metadata=metadata)
 
 		# If we are running in non-production mode, then attempt to copy the generated distfile into
 		# /var/cache/portage/distfiles so it is "already fetched" as it will not exist on the CDN yet.
 		# This allows local testing of the autogenerated ebuild:
+
 		if not pkgtools.model.prod:
 			dist_path = f"/var/cache/portage/distfiles/{self.final_name}"
 			# try to link file into /var/cache/portage/distfiles:
 			try:
 				if os.path.exists(dist_path):
 					os.unlink(dist_path)
 				shutil.copy(self.blos_object.blob.path, dist_path)
 			except PermissionError:
 				log.warning(f"Unable to copy dynamic archive to {dist_path}. Make sure you are in the portage group.")
 
+	async def store_by_name(self, key: dict = None, metadata: dict = None):
+		"""
+		This method will store the current archive as a dynamic archive, and will be indexed by name, and with
+		an optional provided key, so that it can be retrieved by name using the ``Archive.find_by_name``
+		classmethod.
+		"""
+		if key is None:
+			key = {}
+		# We must make final_name part of the key used to find the archive:
+		key["final_name"] = self.final_name
+		return await self.store(key, metadata)
+
+
 	@classmethod
-	def find(cls, final_name, key=None):
+	def find(cls, key: dict = None, final_name: str = None) -> Tuple[Archive, dict] | Tuple[None, None]:
+		"""
+		This classmethod is the big brother of ``Archive.find_by_name()`` and is more flexible. It allows
+		dynamic archives to be found by an arbitrary key. This allows archives to be found where you may not
+		exactly know the final_name (aka filename) of the archive.
+
+		This classmethod is used to implement ``Archive.find_by_name()`` as well. It accepts a key, which
+		is assumed to be "final" -- i.e. "ready to go", unless a ``final_name`` is specified, in which case
+		it will be added to the key to look for that specific named file.
+		"""
 		if pkgtools.model.force_dynamic:
 			# force auto-generation of dynamic archive by purposely returning "not found".
-			return None
+			return None, None
 		if key is None:
 			key = {}
-		key["final_name"] = final_name
-		blos_object = pkgtools.model.fastpull_session.get_file_dynamic(key)
+		if final_name:
+			key["final_name"] = final_name
+		blos_object, metadata = pkgtools.model.fastpull_session.get_file_dynamic(key)
 		log.debug(f"In find, blos object found: {blos_object} using key {key}")
 		if blos_object is None:
-			return None
+			return None, None
 		else:
+			if not final_name:
+				final_name = metadata["final_name"]
 			found_archive = Archive(final_name)
 			found_archive.blos_object = blos_object
-			return found_archive
+			return found_archive, metadata
+
+	@classmethod
+	def find_by_name(cls, final_name: str, key: dict = None) -> Tuple[Archive, dict] | Tuple[None, None]:
+		"""
+		This classmethod is used to attempt to find a dynamic archive (see docs/features/dynamic_archives.rst) by
+		*name*. This means you are looking for a file with a specific, known filename.
+
+		Specify the filename as an argument, along with an optional dictionary key containing data that *must*
+		match for the archive to be considered acceptable for your purposes.
+
+		A tuple containing the Archive and a dictionary containing metadata stored with the Archive is returned,
+		or a (None, None) tuple if nothing was found that met the criteria.
+		"""
+		return cls.find(key=key, final_name=final_name)
 
 	def extract(self):
 		ep = self.extract_path
 		os.makedirs(ep, exist_ok=True)
 		if self.final_name.endswith(".zip"):
 			cmd = f"unzip {ep} -d {self.final_path}"
 		else:
@@ -243,15 +290,15 @@
 
 		super().__init__(self.final_name)
 
 		assert self._url is not None
 		try:
 			assert self._url.split(':')[0] in ['http', 'https', 'ftp']
 		except (IndexError, AssertionError):
-			raise ValueError(f"url= argument of Artifact is '{_url}', which appears malformed or an unsupported protocol.")
+			raise ValueError(f"url= argument of Artifact is '{self._url}', which appears malformed or an unsupported protocol.")
 		self.key = key
 		self.extra_http_headers = extra_http_headers
 
 	@property
 	def url(self):
 		return self._url
 
@@ -289,15 +336,16 @@
 			return True
 		try:
 			# TODO: add extra headers, retry,
 			req = FetchRequest(self.url,
 				extra_headers=self.extra_http_headers,
 				# TODO: we currently don't support authenticating to retrieve an Artifact (just HTTP requests for API)
 				username=None,
-				password=None
+				password=None,
+				final_name=self.final_name
 			)
 			log.debug(f'Artifact.ensure_fetched:{threading.get_ident()} now fetching {self.url} using FetchRequest {req}')
 			# TODO: this used to be indexed by catpkg, and by final_name. So we are now indexing by source URL.
 			# TODO: what exceptions are we interested in here?
 			self.blos_object = await pkgtools.model.fastpull_session.get_file_by_url(req)
 		except FetchError as fe:
 			# We encountered some error retrieving the resource.
@@ -420,14 +468,21 @@
 				yield artifact
 		elif type(self.artifacts) in (dict, OrderedDict):
 			for key, artifact in self.artifacts.items():
 				yield artifact
 		else:
 			raise TypeError("Invalid type for artifacts passed to BreezyBuild -- should be list or dict.")
 
+	@property
+	def src_uri(self):
+		out = ""
+		for artifact in self.iter_artifacts():
+			out += f"{artifact.src_uri}\n"
+		return out.rstrip()
+
 	async def setup(self):
 		"""
 		This method performs some special setup steps. We tend to treat Artifacts as stand-alone objects -- and they
 		can be -- such as if you instantiate an Artifact in `generate()` and fetch it because you need to extract it
 		and look inside it.
 
 		But when associated with a BreezyBuild, as is commonly the case, this means that there is a relationship between
@@ -458,23 +513,30 @@
 						status = await a.ensure_completed()
 						return a, status
 					except Exception as e:
 						pkgtools.model.log.error(e, exc_info=True)
 						raise e
 
 				fetch_task = asyncio.Task(lil_coroutine(artifact))
-				fetch_task.add_done_callback(pkgtools.autogen._artifact_handle_task_result)
 				fetch_tasks_dict[artifact] = fetch_task
 
 		# Wait for any artifacts that are still fetching:
-		results = await pkgtools.autogen.gather_pending_tasks("fetch", fetch_tasks_dict.values())
+		results, failures = await pkgtools.autogen.gather_pending_tasks("fetch", fetch_tasks_dict.values())
 		completion_list = aggregate(results)
+		if failures:
+			for fail_task in failures:
+				logging.exception("Fetch exception", exc_info=fail_task.exception())
+			raise BreezyError("Fetch exceptions encountered.")
+		fetch_fail = False
 		for artifact, status in completion_list:
 			if status is False:
-				raise BreezyError(f"Artifact for url {artifact.url} referenced in {artifact.catpkgs} could not be fetched.")
+				log.error(f"Artifact for url {artifact.url} referenced in {artifact.catpkgs} could not be fetched.")
+				fetch_fail = True
+		if fetch_fail:
+			raise BreezyError("Unable to fetch at least one artifact.")
 
 	def push(self):
 		#
 		# https://stackoverflow.com/questions/1408171/thread-local-storage-in-python
 
 		with pkgtools.autogen.GENNED_BREEZYBUILDS_LOCK:
 			if self.output_pkgdir in pkgtools.autogen.GENNED_BREEZYBUILDS and pkgtools.autogen.GENNED_BREEZYBUILDS[self.output_pkgdir] != self.autogen_id:
@@ -484,23 +546,22 @@
 
 		async def wrapper(self):
 			try:
 				await self.generate()
 				return True
 			except Exception as e:
 				pkgtools.model.log.error(e, exc_info=True)
-				return False
+				raise e
 
 		# This will cause the BreezyBuild to start autogeneration immediately, appending the task to the thread-
 		# local context so we can grab the result later. The return value will be the BreezyBuild object itself,
 		# thanks to the wrapper.
 		bzb_task = Task(wrapper(self))
 		bzb_task.bzb = self
 		bzb_task.info = self.catpkg_version_rev
-		bzb_task.add_done_callback(pkgtools.autogen._handle_task_result)
 		hub.THREAD_CTX.running_breezybuilds.append(bzb_task)
 
 	@property
 	def pkgdir(self):
 		if self._pkgdir is None:
 			self._pkgdir = os.path.join(self.source_tree, self.cat, self.name)
 			os.makedirs(self._pkgdir, exist_ok=True)
@@ -580,15 +641,16 @@
 					except Exception as te:
 						raise BreezyError(f"Unknown error processing {template_file}: {repr(te)}")
 			except FileNotFoundError as e:
 				log.error(f"Could not find template: {template_file}")
 				raise BreezyError(f"Template file not found: {template_file}")
 		else:
 			template = jinja2.Template(self.template_text)
-
+		# allow "src_uri" to be used inside all templates to print out official src_uri of all artifacts.
+		template.globals.update({"src_uri": self.src_uri})
 		with open(self.output_ebuild_path, "wb") as myf:
 			try:
 				myf.write(template.render(**self.template_args).encode("utf-8"))
 			except Exception as te:
 				raise BreezyError(f"Error rendering template: {repr(te)}")
 		log.info("Created: " + os.path.relpath(self.output_ebuild_path))
```

### Comparing `funtoo-metatools-1.1.1/funtoo/pkgtools/fetch.py` & `funtoo-metatools-1.2.0/funtoo/pkgtools/fetch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #!/usr/bin/env python3
 import asyncio
 import re
+from datetime import timedelta
 
 from metatools.fastpull.spider import FetchError
 from metatools.fetch_cache import CacheMiss
 
 """
 This sub implements high-level fetching pkgtools.model.log.c. Not the lower-level HTTP stuff. Things involving
 retrying, using our fetch cache, etc.
@@ -39,14 +40,16 @@
 	fail_reason = None
 	if refresh_interval is None:
 		if pkgtools.model.fetch_cache_interval is not None:
 			# pkgtools.model.fetch_cache_interval defaults to 15 minutes and will allow caching of stuff within that window
 			# by default unless overridden by the doit --immediate option, or if there was an explicit refresh interval passed
 			# to this function.
 			refresh_interval = pkgtools.model.fetch_cache_interval
+		else:
+			refresh_interval = timedelta(minutes=15)
 
 	# This may have "is_json", "encoding":
 	key_dict = kwargs.copy()
 	key_dict.update({
 		"method_name": fetch_method.__name__,
 		"url": url
 	})
@@ -75,14 +78,15 @@
 			result = await fetch_method(url, **kwargs)
 			await pkgtools.model.fetch_cache.write(key_dict=key_dict, body=result)
 			return result
 		except FetchError as e:
 			if e.retry and attempts + 1 < pkgtools.model.fetch_attempts:
 				pkgtools.model.log.error(f"Fetch method {fetch_method.__name__}: {e.msg}; retrying...")
 				continue
+			# TODO: I need a lot more info here -- if something failed -- why? this is important for IPv6 debug
 			# if we got here, we are on our LAST retry attempt or retry is False:
 			pkgtools.model.log.warning(f"Unable to retrieve {url}... trying to used cached version instead...")
 			# TODO: these should be logged persistently so they can be investigated.
 			try:
 				# TODO: add kwargs here....
 				got = await pkgtools.model.fetch_cache.read(key_dict=key_dict)
 				return got["body"]
```

### Comparing `funtoo-metatools-1.1.1/funtoo/pkgtools/github.py` & `funtoo-metatools-1.2.0/funtoo/pkgtools/github.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import re
+import types
+
 import packaging.version
 
 # tag_gen and release_gen are higher-level functions that return a dict of items, suitable for
 # augmenting the pkginfo dict, and thus easy to integrate into yaml-based autogens.
 
 from enum import Enum
 
@@ -331,16 +333,18 @@
 
 			if crates_dict:
 				out_dict.update(crates_dict)
 			return out_dict
 
 	else:
 		version, release = versions_and_release_elements[0]
+
 		# We want to grab the default tarball for the associated tag:
 		desired_tag = release['tag_name']
+		hub.pkgtools.model.log.debug(f"github:release_gen: selected release version: {version}, desired tag {desired_tag}")
 		tag_data = await fetch_tag_data(hub, github_user, github_repo)
 		sha = None
 		for tag_ent in tag_data:
 			if tag_ent["name"] != desired_tag:
 				continue
 			else:
 				sha = tag_ent['commit']['sha']
@@ -359,15 +363,15 @@
 			"artifacts": [
 				hub.pkgtools.ebuild.Artifact(url=url, final_name=f'{github_repo}-{version}-{sha[:7]}.tar.gz')],
 			"sha": sha,
 			"tag": desired_tag,
 		}
 
 
-def iter_tag_versions(tags_list, select=None, filter=None, matcher=None, transform=None, version=None):
+async def iter_tag_versions(tags_list, select=None, filter=None, matcher=None, transform=None, version=None):
 	"""
 	This method iterates over each tag in tags_list, extracts the version information, and
 	yields a tuple of that version as well as the entire GitHub tag data for that tag.
 
 	``select`` specifies a regex string that must match for the tag version to be considered.
 
 	``filter`` can be either a regex string or a list of regex strings. Anything that matches
@@ -382,23 +386,53 @@
 
 	``matcher`` is an optional function that accepts a single argument of the tag we are
 	processing. By default we will use the ``regex_matcher`` to search for a basic version
 	pattern somewhere within the tag.
 	"""
 	if matcher is None:
 		matcher = TagRegexMatcher(select=select, filter=filter)
-	for tag_data in tags_list:
+
+	# To simplify the code, if we don't get tags_list as an async generator, let's just wrap our list so
+	# that it's in an async generator. This may be unnecessary, but need to do some testing
+	# to see, so let's just do it this way for now:
+
+	if not isinstance(tags_list, types.AsyncGeneratorType):
+		async def tags_list_gen(t_list):
+			for tag in t_list:
+				yield tag
+		tags_gen = tags_list_gen(tags_list)
+	else:
+		# We already have an async generator:
+		tags_gen = tags_list
+
+	async for tag_data in tags_gen:
 		match = matcher.match(tag_data['name'], select=select, filter=filter, transform=transform)
 		if match:
 			if version:
 				if match != version:
 					continue
 			yield match, tag_data
 
 
+async def iter_tags_pages(hub, github_user, github_repo):
+	page = 1
+	while True:
+		current_page = await hub.pkgtools.fetch.get_page(f"https://api.github.com/repos/{github_user}/{github_repo}/tags?per_page=100&page={page}", is_json=True)
+		if not len(current_page):
+			break
+		yield current_page
+		page += 1
+
+
+async def iter_all_tags(hub, github_user, github_repo):
+	async for tags_page in iter_tags_pages(hub, github_user, github_repo):
+		for tag_data in tags_page:
+			yield tag_data
+
+
 async def latest_tag_version(hub, github_user, github_repo, tag_data=None, transform=None, select=None, filter=None,
 							 matcher=None, version=None):
 	"""
 	This method will look at all the tags in a repository, look for a version string in each tag,
 	find the most recent version, and return the version and entire tag data as a tuple.
 
 	``select`` specifies a regex string that must match for the tag version to be considered.
@@ -407,17 +441,18 @@
 	ignore all versions unless we find this specific version.
 
 	If no matching versions, None is returned.
 	"""
 	if matcher is None:
 		matcher = TagRegexMatcher(select=select, filter=filter)
 	if tag_data is None:
-		tag_data = await fetch_tag_data(hub, github_user, github_repo)
-	versions_and_tag_elements = list(
-		iter_tag_versions(tag_data, select=select, filter=filter, matcher=matcher, transform=transform, version=version))
+		tag_data = iter_all_tags(hub, github_user, github_repo)
+	versions_and_tag_elements = []
+	async for v_tagel in iter_tag_versions(tag_data, select=select, filter=filter, matcher=matcher, transform=transform, version=version):
+		versions_and_tag_elements.append(v_tagel)
 	if not len(versions_and_tag_elements):
 		return
 	else:
 		return max(versions_and_tag_elements, key=lambda v: matcher.sortable(v[0]))
 
 
 async def tag_gen(hub, github_user, github_repo, tag_data=None, select=None, filter=None, matcher=None, transform=None,
```

### Comparing `funtoo-metatools-1.1.1/funtoo/pkgtools/http.py` & `funtoo-metatools-1.2.0/funtoo/pkgtools/http.py`

 * *Files 15% similar despite different names*

```diff
@@ -37,27 +37,16 @@
 	set_basic_auth(request)
 	# Leverage the spider for this fetch. This bypasses the FPOS, etc:
 	result = await pkgtools.model.spider.http_fetch(request, encoding=encoding, is_json=is_json)
 	return result
 
 
 async def get_url_from_redirect(url):
-	"""
-	This function will take a URL that redirects and grab what it redirects to. This is useful
-	for /download URLs that redirect to a tarball 'foo-1.3.2.tar.xz' that you want to download,
-	when you want to grab the '1.3.2' without downloading the file (yet).
-	"""
-	logging.info(f"Getting redirect URL from {url}...")
-	async with httpx.AsyncClient() as client:
-		try:
-			resp = await client.get(url=url, follow_redirects=False)
-			if resp.status_code == 302:
-				return resp.headers["location"]
-		except httpx.RequestError as e:
-			raise FetchError(url, f"Couldn't get_url_from_redirect due to exception {repr(e)}")
+	return await pkgtools.model.spider.get_url_from_redirect(url)
+
 
 
 async def get_response_headers(url):
 	"""
 	This function will take a URL and grab its response headers. This is useful for obtaining
 	information about a URL without fetching its body.
 	"""
```

### Comparing `funtoo-metatools-1.1.1/funtoo/pkgtools/meson.py` & `funtoo-metatools-1.2.0/funtoo/pkgtools/meson.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.1.1/funtoo/pkgtools/pages.py` & `funtoo-metatools-1.2.0/funtoo/pkgtools/pages.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.1.1/funtoo/pkgtools/pyhelper.py` & `funtoo-metatools-1.2.0/funtoo/pkgtools/pyhelper.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.1.1/funtoo_metatools.egg-info/PKG-INFO` & `funtoo-metatools-1.2.0/funtoo_metatools.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: funtoo-metatools
-Version: 1.1.1
+Version: 1.2.0
 Summary: Funtoo framework for auto-creation of ebuilds.
 Home-page: https://code.funtoo.org/bitbucket/users/drobbins/repos/funtoo-metatools/browse
 Author: Daniel Robbins
 Author-email: drobbins@funtoo.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 
 ****************
 Funtoo Metatools
 ****************
 
-Copyright 2020-2022 Daniel Robbins, Funtoo Solutions, Inc.
+Copyright 2020-2023 Daniel Robbins, Funtoo Solutions, Inc.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `funtoo-metatools-1.1.1/funtoo_metatools.egg-info/SOURCES.txt` & `funtoo-metatools-1.2.0/funtoo_metatools.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 .gitignore
 .pre-commit-config.yaml
 .pylintrc
 README.rst
+VERSION
+make.sh
 setup.py
+setup.py.in
 subpop.yaml
 bin/blos
 bin/deepdive
 bin/deepquery
 bin/direct-sync
 bin/distfile-kit-fetch
 bin/distfile-stats
 bin/doit
 bin/fastpull-daemon
 bin/fastpull-daemon-ng
 bin/fastpull-fixer
+bin/fetch
 bin/interkit-links
 bin/list-kits
 bin/mcafee-tool
 bin/merge-gentoo-staging
 bin/merge-kits
 bin/missing-links
 bin/prod-regen
@@ -65,16 +69,16 @@
 metatools/kit.py
 metatools/kit_cache.py
 metatools/metadata.py
 metatools/model.py
 metatools/pretty_logging.py
 metatools/steps.py
 metatools/store.py
-metatools/thread.py
 metatools/tree.py
+metatools/version.py
 metatools/yaml_util.py
 metatools/config/__init__.py
 metatools/config/autogen.py
 metatools/config/base.py
 metatools/config/merge.py
 metatools/config/mongodb.py
 metatools/fastpull/__init__.py
```

### Comparing `funtoo-metatools-1.1.1/metatools/blos.py` & `funtoo-metatools-1.2.0/metatools/blos.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.1.1/metatools/config/autogen.py` & `funtoo-metatools-1.2.0/metatools/config/autogen.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,17 +47,14 @@
 
 
 	logger_name = 'metatools.spider'
 
 	async def initialize(self, fastpull_scope=None, debug=False):
 		self.spider = WebSpider(os.path.join(self.temp_path, "spider"), hashes=self.hashes)
 		await super().initialize(fastpull_scope=fastpull_scope, debug=debug)
-		# This turns on periodic logging of active downloads (to get rid of 'dots')
-		await self.spider.start_asyncio_tasks()
-
 
 
 class AutogenConfig(StoreSpiderConfig):
 	"""
 	This class is used for the autogen workflow -- i.e. the 'doit' command.
 	"""
```

### Comparing `funtoo-metatools-1.1.1/metatools/config/base.py` & `funtoo-metatools-1.2.0/metatools/config/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 #!/usr/bin/python3
-
+import atexit
 import logging
 import os
 
 from metatools.model import set_model
 from metatools.pretty_logging import TornadoPrettyLogFormatter
 from subpop.config import SubPopModel
 
+import logging
+from rich.logging import RichHandler
+
 
 class MinimalConfig(SubPopModel):
 	"""
 	This class contains configuration settings common to all the metatools plugins and tools.
 	"""
 
-	logger_name = "metatools"
+	logger_name = "metatools.merge"
 
 	def __init__(self):
 		super().__init__()
 
 	async def initialize(self, debug=False):
 		self.log = logging.getLogger(self.logger_name)
 		self.log.propagate = False
 		if debug:
 			self.debug = debug
 			self.log.setLevel(logging.DEBUG)
 		else:
 			self.log.setLevel(logging.INFO)
-		channel = logging.StreamHandler()
-		channel.setFormatter(TornadoPrettyLogFormatter())
-		self.log.addHandler(channel)
+		handler = RichHandler(show_path=False)
+		self.log.addHandler(handler)
+		atexit.register(lambda: print("\x1b[?25h"))
 		if debug:
 			self.log.warning("DEBUG enabled")
 		set_model(self.logger_name, self)
 
 	@property
 	def work_path(self):
 		home = self.home()
@@ -83,10 +86,19 @@
 		In any case, some resiliency in the code for multiple creation of the same symlink (and thus symlink
 		creation failure) would be a good idea.
 
 		"""
 
 		return os.path.join(self.work_path, "fastpull")
 
+	@property
+	def metadata_cache(self):
+		return os.path.join(self.work_path, "metadata-cache")
+
+	@property
+	def dest_trees(self):
+		return os.path.join(self.work_path, "dest-trees")
+
+
```

### Comparing `funtoo-metatools-1.1.1/metatools/config/merge.py` & `funtoo-metatools-1.2.0/metatools/config/merge.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,28 +92,19 @@
 		else:
 
 			# In this mode, we're actually wanting to update real kits, and likely are going to push our updates to remotes (unless
 			# --nopush is specified as an arg.) This might be used by people generating their own custom kits for use on other systems,
 			# or by Funtoo itself for updating official kits and meta-repo.
 			self.push = push
 			self.nest_kits = False
-			self.push = push
 			self.mirror_repos = push
 			self.git_class = GitTree
 			self.git_kwargs = {"checkout_all_branches": True}
 		self.log.debug("Model initialization complete.")
 
-	@property
-	def metadata_cache(self):
-		return os.path.join(self.work_path, "metadata-cache")
-
-	@property
-	def dest_trees(self):
-		return os.path.join(self.work_path, "dest-trees")
-
 
 class SourceRepository:
 	"""
 	This SourceRepository represents a single source repository referenced in the YAML. This source repository
 	is used as a source tree for copying in ebuilds and eclasses into a kit.
 	"""
 
@@ -127,27 +118,35 @@
 		self.eclasses = eclasses
 		self.src_sha1 = src_sha1
 		self.branch = branch if branch else "master"
 		self.notes = notes
 		# This can be used to track a GitTree associated with the source repository.
 		self.tree = None
 
-	def initialize(self):
-		self.yaml.model.log.info(f"Initializing Source Repository {self.name} {self.branch} {self.url}")
-		self.tree = GitTree(
-			self.name,
-			url=self.url,
-			root="%s/%s" % (self.yaml.model.source_trees, self.name),
-			branch=self.branch,
-			commit_sha1=self.src_sha1,
-			origin_check=False,
-			reclone=False,
-			model=self.yaml.model
-		)
-		self.tree.initialize()
+	def initialize(self, branch="master"):
+		if self.tree:
+			if branch == self.branch:
+				return
+			else:
+				self.yaml.model.log.info(f"Checkout: Source Repository {self.name} {self.branch} {self.url}")
+				self.branch = branch
+				self.tree.gitCheckout(self.branch)
+		else:
+			self.yaml.model.log.info(f"Initializing: Source Repository {self.name} {self.branch} {self.url}")
+			self.tree = GitTree(
+				self.name,
+				url=self.url,
+				root="%s/%s" % (self.yaml.model.source_trees, self.name),
+				branch=self.branch,
+				commit_sha1=self.src_sha1,
+				origin_check=False,
+				reclone=False,
+				model=self.yaml.model
+			)
+			self.tree.initialize()
 
 	def find_license(self, license):
 		try:
 			return self.tree.find_license(license)
 		except FileNotFoundError:
 			self.yaml.model.log.error(f"No license named '{license}' found in SourceRepository {self.name}")
 
@@ -164,54 +163,51 @@
 
 class SourceCollection:
 	"""
 	A SourceCollection in the YAML is, as the name says, a collection of source repositories. Each kit can reference
 	one SourceCollection and copy ebuilds and eclasses from the SourceRepositories defined in each collection.
 	"""
 
-	def __init__(self, name=None, yaml=None, repositories=None):
+	def __init__(self, name=None, yaml=None, repo_defs=None):
 		self.yaml = yaml
 		self.name = name
+		# Contains abstract definitions of repos, which we can instantiate
+		self.repo_defs = repo_defs
 		self.repositories = OrderedDict()
-		for repo in repositories:
-			self.repositories[repo.name] = repo
 
 	def find_license(self, license):
 		for repo in reversed(self.repositories.keys()):
 			try:
 				license = self.repositories[repo].tree.find_license(license)
 			except FileNotFoundError:
 				continue
 			return license
 		self.yaml.model.log.error(f"No license named '{license}' found in SourceCollection {self.name}")
 
-	def initialize(self):
+	def initialize(self, repo_names=None):
 
 		"""
 		This method initializes the source repositories referenced by the kit to ensure that they are all initialized to the
 		proper branch and/or SHA1. Some internal checking is done to avoid re-initializing repositories unnecessarily, so if
 		they are already set up properly then no action will be taken.
 		"""
 
-		# If we are already using this SourceCollection, no action is needed:
-		self.yaml.model.log.info(
-			f"Initializing source collection {self.name} with {len(self.repositories)} repositories")
-		if self.yaml.model.current_source_def == self:
-			return
-
-		# If we need to switch SourceCollection, we can still avoid unnecessary work:
-		# We will go through each of our repositories, and only (re-)initialize it if:
-		#
-		# 1. Our repo is missing.
-		# 2. Our repo exists with same name but is referencing a different branch/sha1.
-
 		repo_futures = []
-		with ThreadPoolExecutor(max_workers=4) as executor:
+		with ThreadPoolExecutor(max_workers=2) as executor:
+			for repo_name, repo_def in self.repo_defs.items():
+				# Skip any repos that we aren't using right now....
+				if repo_names is not None and repo_name not in repo_names:
+					continue
+				# If repo already exists, don't create it from scratch. Should be faster:
+				if repo_name in self.yaml.all_repo_objs:
+					self.repositories[repo_name] = self.yaml.all_repo_objs[repo_name]
+				else:
+					self.yaml.all_repo_objs[repo_name] = self.repositories[repo_name] = SourceRepository(**repo_def, yaml=self.yaml, name=repo_name)
 			for repo_name, repo in self.repositories.items():
-				fut = executor.submit(repo.initialize)
+				fut = executor.submit(repo.initialize, repo_def["branch"] if "branch" in repo_def else "master")
 				repo_futures.append(fut)
 			for repo_fut in as_completed(repo_futures):
 				# Getting .result() will also cause any exception to be thrown:
 				repo_dict = repo_fut.result()
 				continue
 
 		self.yaml.model.current_source_def = self
@@ -281,14 +277,24 @@
 
 	@property
 	def package_data(self):
 		if self._package_data is None:
 			self._package_data = self._get_package_data()
 		return self._package_data
 
+	def initialize_sources(self):
+		repo_names = []
+		for repo_name, extra in self.get_kit_items():
+			repo_names.append(repo_name)
+		for repo_name, extra in self.get_kit_items(section="copyfiles"):
+			repo_names.append(repo_name)
+		for repo_name, extra in self.get_kit_items(section="eclasses"):
+			repo_names.append(repo_name)
+		self.source.initialize(repo_names=repo_names)
+
 	def _get_package_data(self):
 
 		# Look for branch-specific packages.yaml:
 		fn = f"{self.kit_fixups.root}/{self.name}/{self.branch}/packages.yaml"
 		# Fallback to curated packages.yaml:
 		if not os.path.exists(fn):
 			fn = f"{self.kit_fixups.root}/{self.name}/curated/packages.yaml"
@@ -398,14 +404,15 @@
 	"""
 
 	source_collections = None
 	kits = None
 	filename = None
 	remotes = None
 	masters = None
+	all_repo_objs = dict()
 
 	def __init__(self, model: MergeConfig):
 		self.model = model
 		self.mode = "prod" if self.model.prod is True else "dev"
 		filename = f'{self.model.locator.root}/releases/{self.model.release}/repositories.yaml'
 		if not os.path.exists(filename):
 			raise ConfigurationError(f"Cannot find expected {filename}")
@@ -472,14 +479,15 @@
 		passed to the kit's constructor.
 		"""
 		source_collections = OrderedDict()
 		repositories = self._repositories()
 		for collection_name, collection_items in self.iter_groups("release/source-collections"):
 			collection_objs = []
 			names = set()
+			repo_defs = OrderedDict()
 			for repo_def in collection_items:
 				repo_name = None
 				if isinstance(repo_def, str):
 					# str -> actual pre-defined repository dict
 					repo_name = repo_def
 					repo_def = repositories[repo_def]
 				elif isinstance(repo_def, dict):
@@ -490,18 +498,16 @@
 						raise KeyError(
 							f"Referenced repository '{repo_name}' in source collection '{collection_name}' not found in repositories list.")
 					repo_def = repositories[repo_name].copy()
 					repo_def.update(repo_dict)
 				if repo_name in names:
 					raise ValueError(f"Duplicate repository name {repo_name} in source collection {collection_name}")
 				names.add(repo_name)
-				repo_obj = SourceRepository(yaml=self, name=repo_name, **repo_def)
-				collection_objs.append(repo_obj)
-			source_collections[collection_name] = SourceCollection(yaml=self, name=collection_name,
-																   repositories=collection_objs)
+				repo_defs[repo_name] = repo_def
+			source_collections[collection_name] = SourceCollection(yaml=self, name=collection_name, repo_defs=repo_defs)
 		return source_collections
 
 	def _remotes(self):
 		return self.get_elem("release/remotes")
 
 	def _kits(self):
 		"""
```

### Comparing `funtoo-metatools-1.1.1/metatools/context.py` & `funtoo-metatools-1.2.0/metatools/context.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-from portage import os
+import os
 from subpop.config import ConfigurationError
 
 
 class Locator:
 	start_path = None
 	root: str = None
 	expected_files = []
```

### Comparing `funtoo-metatools-1.1.1/metatools/fastpull/core.py` & `funtoo-metatools-1.2.0/metatools/fastpull/core.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,49 @@
 #!/usr/bin/env python3
 
+from __future__ import annotations
 import logging
 from datetime import datetime
+from typing import Tuple
 
 from metatools.blos import BaseLayerObjectStore
 from metatools.fastpull.spider import FetchRequest, Download
+from metatools.steps import run_bg
 from metatools.store import Store, FileStorageBackend, DerivedKey, StoreObject
 
 log = logging.getLogger('metatools.autogen')
 
 
+class FileIntegrityError(Exception):
+	pass
+
+
 class IntegrityScope:
 
-    def __init__(self, parent, scope, validate_hashes=None):
-        if validate_hashes is None:
-            validate_hashes = {"sha512"}
-        self.validate_hashes = validate_hashes
-        self.parent = parent
-        self.scope = scope
-        self.store = Store(
-            collection="integrity",
-            prefix=self.scope,
-            backend=FileStorageBackend(db_base_path=self.parent.db_base_path),
-            key_spec=DerivedKey(["url"])
-        )
-        self.dynamic = Store(
-            collection="dynamic",
-            prefix=self.scope,
-            backend=FileStorageBackend(db_base_path=self.parent.db_base_path),
-            key_spec=DerivedKey(["key"])
-        )
+	def __init__(self, parent, scope, validate_hashes=None):
+		if validate_hashes is None:
+			validate_hashes = {"sha512"}
+		self.validate_hashes = validate_hashes
+		self.parent = parent
+		self.scope = scope
+		self.store = Store(
+			collection="integrity",
+			prefix=self.scope,
+			backend=FileStorageBackend(db_base_path=self.parent.db_base_path),
+			key_spec=DerivedKey(["url"])
+		)
+		self.dynamic = Store(
+			collection="dynamic",
+			prefix=self.scope,
+			backend=FileStorageBackend(db_base_path=self.parent.db_base_path),
+			key_spec=DerivedKey(["key"])
+		)
 
-    async def get_file_by_url(self, request: FetchRequest) -> StoreObject:
-        """
+	async def get_file_by_url(self, request: FetchRequest) -> StoreObject:
+		"""
 
 		This method will attempt to return a StoreObject reference to binary data which is associated with
 		a URL, referenced by ``request.url``, in this ``IntegrityScope``. Typically, this means that a
 		tarball is being requested, and we may have this tarball already available locally, or we may
 		need to use the ``Spider`` to download it. This is the method used to retrieve ``Artifact``s
 		from the interwebs.
 
@@ -70,79 +77,118 @@
 		Whether we initiated the download or not, we will get back the result of this pipeline and get the
 		BLOSObject for the inserted object returned to us. We will pass this object back to the caller.
 
 		If there is some kind of FetchError that could not be managed, it will be raised by the Spider, so that
 		the root cause of the fetch error can be propagated to the caller.
 		"""
 
-        existing_ref: StoreObject = self.store.read({"url": request.url})
-        if existing_ref is not None:
-            obj = self.parent.blos.read({"hashes.sha512": existing_ref.data['sha512']})
-            if obj is not None:
-                log.debug(
-                    f"IntegrityScope:{self.scope}._get_file_by_url_new: existing object found for ref {request.url}")
-                return obj
-        new_ref = await self.parent.spider.download(request,
-                                                    completion_pipeline=[self.parent.fetch_completion_callback])
-        assert isinstance(new_ref, StoreObject)
-        self.store.write(
-            {"url": request.url, "sha512": new_ref.data["hashes"]["sha512"], "updated_on": datetime.utcnow()})
-        return new_ref
-
-    def get_file_dynamic(self, key_dict: dict) -> StoreObject:
-        existing_ref: StoreObject = self.dynamic.read({"key": key_dict})
-        if existing_ref:
-            log.debug(f"get_file_dynamic: existing_ref: {existing_ref.data}")
-        if existing_ref is not None:
-            obj = self.parent.blos.read({"hashes.sha512": existing_ref.data['hashes']['sha512']})
-            if obj is not None:
-                return obj
-
-    def store_file_dynamic(self, key_dict: dict, obj_path):
-        store_obj = self.parent.blos.insert_blob(obj_path)
-        self.dynamic.write({"key": key_dict, "hashes": store_obj.data["hashes"]})
+		existing_ref: StoreObject = self.store.read({"url": request.url})
+		if existing_ref is not None:
+			obj = self.parent.blos.read({"hashes.sha512": existing_ref.data['sha512']})
+			if obj is not None:
+				log.debug(
+					f"IntegrityScope:{self.scope}._get_file_by_url_new: existing object found for ref {request.url}")
+				return obj
+		new_ref = await self.parent.spider.download(request,
+		                                            completion_pipeline=[
+														self.parent.verify_callback,
+														self.parent.fetch_completion_callback])
+		assert isinstance(new_ref, StoreObject)
+		self.store.write(
+			{"url": request.url, "sha512": new_ref.data["hashes"]["sha512"], "updated_on": datetime.utcnow()})
+		return new_ref
+
+	def get_file_dynamic(self, key_dict: dict) -> Tuple[StoreObject, dict] | Tuple[None, None]:
+		existing_ref: StoreObject = self.dynamic.read({"key": key_dict})
+		if existing_ref:
+			log.debug(f"get_file_dynamic: existing_ref: {existing_ref.data}")
+		if existing_ref is not None:
+			obj = self.parent.blos.read({"hashes.sha512": existing_ref.data['hashes']['sha512']})
+			if obj is not None:
+				if "metadata" in existing_ref.data:
+					metadata = existing_ref.data["metadata"]
+				else:
+					metadata = {}
+				return obj, metadata
+		return None, None
+
+	def store_file_dynamic(self, key_dict: dict, obj_path, metadata: dict = None):
+		store_obj = self.parent.blos.insert_blob(obj_path)
+		self.dynamic.write({"key": key_dict, "hashes": store_obj.data["hashes"], "metadata": metadata if metadata else {}})
 
 
 class IntegrityDatabase:
 
-    def __init__(self, db_base_path, blos: BaseLayerObjectStore = None, spider=None, hashes: set = None):
-        """
+	def __init__(self, db_base_path, blos: BaseLayerObjectStore = None, spider=None, hashes: set = None):
+		"""
 		``blos`` is an instance of a Base Layer Object Store (used to store distfiles, indexed by their hashes,
 		and also takes care of all integrity checking tasks for us.
 
 		``spider`` is an instance of a WebSpider, which handles all downloading tasks for us.
 
 		``hashes`` is a set of cryptographic hashes
 
 		The fastpull database uses sha512 as a 'linking mechanism' to the Base Layer Object Store (BLOS). So only
 		one hash needs to be recorded, since this is not an exhaustive integrity check (that is performed by the
 		BLOS itself upon retrieval). This is stored in the 'sha512' key, which is not placed inside 'hashes' like
 		it is in the BLOS. But we do not create an index for it, since we don't encourage retrieval of objects from
 		fastpull by their hash. They should be retrieved by target URL (and scope). So we always want to retrieve
 		the ref by the URL, then from the returned record, use the sha512 to see if the BLOS entry exists.
 		"""
-        assert hashes
-        self.db_base_path = db_base_path
-        self.hashes = hashes
-        self.blos: BaseLayerObjectStore = blos
-        self.spider = spider
-        self.scopes = {}
+		assert hashes
+		self.db_base_path = db_base_path
+		self.hashes = hashes
+		self.blos: BaseLayerObjectStore = blos
+		self.spider = spider
+		self.scopes = {}
 
-    def get_scope(self, scope_id):
-        """
+	def get_scope(self, scope_id):
+		"""
 		This method returns an 'IntegrityScope', which is basically like a session for doit (autogen) to
 		associate URLs with entries in the BLOS, or Base Layer Object Store.
 		"""
-        if scope_id not in self.scopes:
-            self.scopes[scope_id] = IntegrityScope(self, scope_id)
-        log.debug(f"FastPull Integrity Scope: {scope_id}")
-        return self.scopes[scope_id]
+		if scope_id not in self.scopes:
+			self.scopes[scope_id] = IntegrityScope(self, scope_id)
+		log.debug(f"FastPull Integrity Scope: {scope_id}")
+		return self.scopes[scope_id]
+
+	async def verify_callback(self, download: Download) -> Download:
+		fn = download.request.filename
+		run_cmd = None
+		arc_desc = None
+		if fn.endswith(".tar.gz"):
+			run_cmd = "tar tzf {archive}"
+			arc_desc = "tar.gz"
+		elif fn.endswith(".tar.bz2"):
+			run_cmd = "tar tjf {archive}"
+			arc_desc = "tar.bz2"
+		elif fn.endswith(".tar.xz"):
+			run_cmd = "tar tJf {archive}"
+			arc_desc = "tar.xz"
+		elif fn.endswith(".tar.zst"):
+			run_cmd = "tar -t --zstd -f {archive}"
+			arc_desc = "tar.xz"
+		elif fn.endswith(".gz"):
+			run_cmd = "gzip -dc {archive} > /dev/null"
+			arc_desc = "gzip"
+		elif fn.endswith(".bz2"):
+			run_cmd = "bzip2 -dc {archive} > /dev/null"
+			arc_desc = "bzip2"
+		elif fn.endswith(".xz"):
+			run_cmd = "xz -dc {archive} > /dev/null"
+			arc_desc = "xz"
+		if run_cmd:
+			proc, out = await run_bg(run_cmd.format(archive=download.temp_path))
+			if proc.returncode != 0:
+				raise FileIntegrityError(f"File {download.temp_path} downloaded from {download.request.url} does not appear to be a valid {arc_desc} archive!")
+			log.info(f"Download from {download.request.url} verified as valid {arc_desc} archive.")
+		return download
 
-    def fetch_completion_callback(self, download: Download) -> StoreObject:
-        """
+	async def fetch_completion_callback(self, download: Download) -> StoreObject:
+		"""
 		This method is intended to be called *once* when an actual in-progress download of a tarball (by
 		the Spider) has completed. It performs several important finalization actions upon successful
 		download:
 
 		1. The downloaded file will be stored in the BLOS, and the resultant BLOSObject will be assigned to
 		``response.blos_object``.
 
@@ -150,11 +196,11 @@
 		   anyone -- only the permanent file inserted into the BLOS will be handed back (via
 		   ``response.blos_object``.
 
 		We pass this to any Download() object we instantiate so that it has proper post-actions defined
 		for it.
 		"""
 
-        store_obj: StoreObject = self.blos.insert_download(download)
-        if self.spider:
-            self.spider.cleanup(download)
-        return store_obj
+		store_obj: StoreObject = self.blos.insert_download(download)
+		if self.spider:
+			self.spider.cleanup(download)
+		return store_obj
```

### Comparing `funtoo-metatools-1.1.1/metatools/fastpull/spider.py` & `funtoo-metatools-1.2.0/metatools/fastpull/spider.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,47 +1,61 @@
 import asyncio
 import hashlib
 import logging
 import os
 import random
 import string
 import threading
-from asyncio import Semaphore
 from collections import defaultdict
 from contextlib import asynccontextmanager
+from datetime import datetime, timedelta
+from json import JSONDecodeError
 from urllib.parse import urlparse
 
 import httpx
+import rich.progress
 
 log = logging.getLogger('metatools.autogen')
 
 
 class FetchRequest:
 
-	def __init__(self, url, retry=True, extra_headers=None, mirror_urls=None, username=None, password=None, expected_hashes=None):
+	def __init__(self, url, retry=True, extra_headers=None, mirror_urls=None, username=None, password=None, expected_hashes=None, final_name=None):
 		assert url is not None
 		self.url = url
 		self.retry = retry
 		self.extra_headers = extra_headers if extra_headers else {}
 		self.mirror_urls = mirror_urls if mirror_urls else []
 		# for basic auth
 		self.username = username
 		self.password = password
 		# TODO: this was a last-minute add to FetchRequest and we could possibly leverage this in the BLOS.
 		self.expected_hashes = expected_hashes if expected_hashes is not None else {}
+		self.final_name = final_name
 
 	@property
 	def hostname(self):
 		parsed_url = urlparse(self.url)
 		return parsed_url.hostname
 
+	@property
+	def filename(self):
+		if self.final_name:
+			return self.final_name
+		else:
+			parsed_url = urlparse(self.url)
+			return parsed_url.path.split("/")[-1]
+
 	def set_auth(self, username=None, password=None):
 		self.username = username
 		self.password = password
 
+	def __repr__(self):
+		return f"metatools.fastpull.spider.FetchRequest<{self.url}>"
+
 
 class FetchResponse:
 
 	"""
 	FetchResponse will be returned in the case of a successful download of a file. ``fetch_request``, the
 	only argument, references the original request associated with this response.
 
@@ -71,15 +85,20 @@
 		self.spider = spider
 		self.request = request
 		self.waiters = []
 		self.completion_pipeline = [] if completion_pipeline is None else completion_pipeline
 		self.hashes = hashes
 		self.final_data = None
 		self._temp_path = None
-		self.filesize = 0
+		self.filesize = None
+		self.total = None
+		self.fd = None
+		self.hash_calc_dict = None
+		self.download_task = None
+		self.start_time = None
 
 	def get_download_future(self):
 		log.debug(f"Download.await_existing:{threading.get_ident()} {self.request.url}")
 		fut = asyncio.get_running_loop().create_future()
 		self.waiters.append(fut)
 		return fut
 
@@ -102,111 +121,140 @@
 			# Use MD5 to create the path for the temporary file to avoid collisions, but also add a random string to allow
 			# multiple downloads of the same file from different instances or autogens to avoid collision.
 			rand_str = ''.join(random.choice(string.ascii_uppercase + string.digits) for _ in range(8))
 			temp_name = hashlib.md5(self.request.url.encode('utf-8')).hexdigest()
 			self._temp_path = os.path.join(self.spider.temp_path, f"{rand_str}-{temp_name}")
 		return self._temp_path
 
-	async def _http_fetch_stream(self, on_chunk, chunk_size=262144):
+	async def _http_fetch_stream(self, on_chunk):
 		"""
 		This is a low-level streaming HTTP fetcher that will call on_chunk(bytes) for each chunk. On_chunk is called with
 		literal bytes from the response body so no decoding is performed. The final_data attribute still needs
 		to be filled out (this is done by self.launch(), which calls this.)
 
 		Also note that this method will now raise FetchError if it truly fails, though it also will capture some error
 		conditions internally do to proper robustifying of downloads and handle common download failure conditions itself.
 		"""
-		hostname = self.request.hostname
-		semi = await self.spider.acquire_host_semaphore(hostname)
-		rec_bytes = 0
+		client = await self.spider.acquire_http_client(self.request)
+		headers, auth = self.spider.get_headers_and_auth(self.request)
+
 		attempts = 0
 		if self.request.retry:
 			max_attempts = 3
 		else:
 			max_attempts = 1
 		completed = False
 
-		async with semi:
-			while not completed and attempts < max_attempts:
-				try:
-					async with httpx.AsyncClient() as client:
-						headers, auth = self.spider.get_headers_and_auth(self.request)
-						async with client.stream("GET", url=self.request.url, headers=headers, auth=auth, follow_redirects=True, timeout=12) as response:
-							if response.status_code not in [200, 206]:
-								if response.status_code in [400, 404, 410]:
-									# These are legitimate responses that indicate that the file does not exist. Therefore, we
-									# should not retry, as we should expect to get the same result.
-									retry = False
-								else:
-									retry = True
-								raise FetchError(self.request, f"HTTP fetch_stream Error {response.status_code}: {response.reason_phrase[:120]}", retry=retry)
-							async for chunk in response.aiter_bytes():
-								rec_bytes += len(chunk)
-								if not chunk:
-									completed = True
-									break
-								else:
-									on_chunk(chunk)
-				except httpx.RequestError as e:
-					log.error(f"Download failure for {self.request.url}: {str(e)}")
-					if attempts + 1 < max_attempts:
-						attempts += 1
-						log.warning(f"Retrying after download failure... {str(e)}")
-						continue
+		while not completed and attempts < max_attempts:
+			try:
+				self.reset()
+				async with client.stream("GET", url=self.request.url, headers=headers, auth=auth, follow_redirects=True) as response:
+					if response.status_code not in [200, 206]:
+						if response.status_code in [400, 404, 410]:
+							# These are legitimate responses that indicate that the file does not exist. Therefore, we
+							# should not retry, as we should expect to get the same result.
+							retry = False
+						else:
+							retry = True
+						raise FetchError(self.request, f"HTTP fetch_stream Error {response.status_code}: {response.reason_phrase[:120]}", retry=retry)
+					if "Content-Length" in response.headers:
+						self.total = int(response.headers["Content-Length"])
 					else:
-						raise FetchError(self.request, f"{e.__class__.__name__}: {str(e)}")
+						self.total = 0
+					# download_task can legitimately be zero, so check explicitly against None (our "null"):
+					if self.download_task is None:
+						# Only start download progress display if the download takes a minimum # of seconds...
+						filename = self.request.filename
+						if self.total == 0:
+							filename = f"(stream) {filename}"
+						self.download_task = self.spider.progress.add_task("Download", filename=filename, total=self.total)
+						log.debug(f"Added download task {self.download_task}, total {self.total}")
+					# DO NOT USE aiter_raw(), below!! It will result in invalid downloads from some sites!
+					async for chunk in response.aiter_bytes():
+						on_chunk(chunk, response)
+					completed = True
+			except httpx.RequestError as e:
+				log.error(f"Download failure for {self.request.url}: {str(e)}")
+				if attempts + 1 < max_attempts:
+					attempts += 1
+					log.warning(f"Retrying after download failure... {str(e)}")
+					continue
+				else:
+					break
+			finally:
+				if self.download_task is not None:
+					self.spider.progress.remove_task(self.download_task)
+					self.download_task = None
+
+		if not completed:
+			raise FetchError(self.request, "http_fetch_stream failure")
+
+	def reset(self):
+		"""
+		Reset all necessary things after an aborted download that we will retry. We have to start from the beginning.
+		:return:
+		"""
+		os.makedirs(os.path.dirname(self.temp_path), exist_ok=True)
+		if self.fd:
+			self.fd.close()
+		self.fd = open(self.temp_path, "wb")
+		self.hash_calc_dict = {}
+		self.filesize = 0
+		self.total = None
+		self.start_time = datetime.utcnow()
+		for h in self.hashes:
+			self.hash_calc_dict[h] = getattr(hashlib, h)()
+
+	def on_chunk(self, chunk, response):
+		self.fd.write(chunk)
+		for hash in self.hashes:
+			self.hash_calc_dict[hash].update(chunk)
+		self.filesize += len(chunk)
+		log.debug(f"chunk! {self.download_task} {self.request.filename}: total {self.total, type(self.total)}: {response.num_bytes_downloaded}/{self.total}")
+		if self.download_task is not None:
+			if self.total:
+				self.spider.progress.update(self.download_task, completed=response.num_bytes_downloaded)
+			else:
+				self.spider.progress.update(self.download_task, completed=response.num_bytes_downloaded, total=response.num_bytes_downloaded)
 
 	async def launch(self) -> None:
 		"""
 		This is the lower-level download method that wraps the _http_fetch_stream() call, and ensures hashes are generated.
 
 		Upon successful completion of the download, this function will set self.final_data to the final_data (hashes and
 		size) of the downloaded file. It will also execute the completion pipeline, if any. It will return None if you
 		have no completion pipeline, and will otherwise return the result of the execution of the pipeline.
 
 		This method throw a FetchError if it encounters some kind of fetching problem, though _http_fetch_stream()
 		will try to recover from many (and will catch some FetchErrors internally to do this.)
 		"""
 
 		log.debug(f"WebSpider.launch:{threading.get_ident()} spidering {self.request.url}...")
-		os.makedirs(os.path.dirname(self.temp_path), exist_ok=True)
-		log.info(f"Spidering {self.request.url}")
-		fd = open(self.temp_path, "wb")
-		hashes = {}
-
-		for h in self.hashes:
-			hashes[h] = getattr(hashlib, h)()
-
-		def on_chunk(chunk):
-			fd.write(chunk)
-			for hash in self.hashes:
-				hashes[hash].update(chunk)
-			self.filesize += len(chunk)
+		if not self.spider.rich:
+			log.info(f"Spidering {self.request.url}")
 
 		try:
-			await self._http_fetch_stream(on_chunk)
+			await self._http_fetch_stream(self.on_chunk)
 		except FetchError as fe:
 			raise fe
 		finally:
-			fd.close()
+			self.fd.close()
 
 		final_data = {}
 		for h in self.hashes:
-			final_data[h] = hashes[h].hexdigest()
+			final_data[h] = self.hash_calc_dict[h].hexdigest()
 		final_data['size'] = self.filesize
 		self.final_data = final_data
 
-		# TODO: Handle error 416, requested range not satisfiable. ^Z during download and resume seems to break our resume functionality.
-
 		if self.completion_pipeline:
 			# start by handing this Download object to the start of the pipeline:
 			completion_result = self
 			for completion_fn in self.completion_pipeline:
 				log.debug(f"Calling completion function {completion_fn} with argument {completion_result}")
-				completion_result = completion_fn(completion_result)
+				completion_result = await completion_fn(completion_result)
 			self.notify_waiters(completion_result)
 			# TODO: we may have a race condition here, or an unhandled case for aborted download (traceback seen in output)
 			#       File "/home/drobbins/development/funtoo-metatools/metatools/fastpull/core.py", line 75, in get_file_by_url
 			#         blos_obj = await self.parent.spider.download(request, completion_pipeline=[self.parent.fetch_completion_callback])
 			#       File "/home/drobbins/development/funtoo-metatools/metatools/fastpull/spider.py", line 322, in download
 			#         response = await download.launch()
 			#       File "/home/drobbins/development/funtoo-metatools/metatools/fastpull/spider.py", line 217, in launch
@@ -263,41 +311,112 @@
 	value= parameter) of downloads active at once. Each active download will acquire a slot. When all
 	slots are exhausted, any pending downloads will wait for an active slot before they can begin.
 	"""
 
 	DL_ACTIVE_LOCK = threading.Lock()
 	DL_ACTIVE = dict()
 	DOWNLOAD_SLOT = threading.Semaphore(value=20)
-	thread_ctx = threading.local()
+	FETCH_SLOT = defaultdict(lambda: threading.Semaphore(value=20))
 	fetch_headers = {"User-Agent": "funtoo-metatools (support@funtoo.org)"}
 	status_logger_task = None
 	keep_running = True
+	thread_ctx = threading.local()
+	transport = None
+	started = None
+	limits = httpx.Limits(keepalive_expiry=30, max_keepalive_connections=100, max_connections=100)
 
 	def __init__(self, temp_path, hashes):
+		self.fetch_count = 0
 		self.temp_path = temp_path
 		self.hashes = hashes - {'size'}
+		self.rich = True
+		self.progress = rich.progress.Progress(
+				"[progress.percentage]{task.percentage:>3.0f}%",
+				rich.progress.TextColumn("[bold blue]{task.fields[filename]}", justify="right"),
+				rich.progress.BarColumn(bar_width=None),
+				rich.progress.DownloadColumn(),
+				rich.progress.TransferSpeedColumn(),
+				transient=True
+		)
+
+
+	@property
+	def http_clients(self):
+		http_clients = getattr(self.thread_ctx, "http_clients", None)
+		if http_clients is None:
+			http_clients = self.thread_ctx.http_clients = {}
+		return http_clients
 
 	async def status_logger(self):
 		while self.keep_running:
-			await asyncio.sleep(1)
+			await asyncio.sleep(0.1)
 			dl_count = len(self.DL_ACTIVE)
-			if dl_count > 1:
-				log.info(f"Spider active downloads: {len(self.DL_ACTIVE)}")
-			elif dl_count == 1:
-				log.info(f"Spider active download: {list(self.DL_ACTIVE.keys())[0]}")
+			if not self.rich:
+				if dl_count > 1:
+					log.info(f"Spider active downloads: {len(self.DL_ACTIVE)}")
+				elif dl_count == 1:
+					log.info(f"Spider active download: {list(self.DL_ACTIVE.keys())[0]}")
+		self.progress.stop()
+		log.info("Status logger done.")
 
 	async def start_asyncio_tasks(self):
-		self.status_logger_task = asyncio.create_task(self.status_logger())
+		self.status_logger_task = asyncio.Task(self.status_logger())
 
-	def stop(self):
+	async def get_url_from_redirect(self, url):
+		"""
+		This function will take a URL that redirects and grab what it redirects to. This is useful
+		for /download URLs that redirect to a tarball 'foo-1.3.2.tar.xz' that you want to download,
+		when you want to grab the '1.3.2' without downloading the file (yet).
+		"""
+		request = FetchRequest(url=url)
+		logging.info(f"Getting redirect URL from {url}...")
+		client = await self.acquire_http_client(request)
+
+		try:
+			resp = await client.get(url=url, follow_redirects=False)
+			if resp.status_code == 302:
+				return resp.headers["location"]
+		except httpx.RequestError as e:
+			raise FetchError(url, f"Couldn't get_url_from_redirect due to exception {repr(e)}")
+
+	async def start(self):
+		if self.started:
+			return
+		# This turns on periodic logging of active downloads (to get rid of 'dots')
+		self.progress.start()
+		await self.start_asyncio_tasks()
+		self.transport = httpx.AsyncHTTPTransport(retries=3, limits=self.limits)
+
+	async def stop(self):
+		if not self.started:
+			return
 		self.keep_running = False
 		self.status_logger_task.cancel()
-		asyncio.gather(self.status_logger_task)
+		try:
+			await self.status_logger_task
+		except:
+			# This works around what is, from what I can tell, an asyncio bug. This, along with os._exit() in
+			# doit, prevents a traceback that looks like this on exit with python3.7
+			#
+			#   File "/usr/lib/python3.7/asyncio/selector_events.py", line 271, in _remove_reader
+			#     key = self._selector.get_key(fd)
+			#   File "/usr/lib/python3.7/selectors.py", line 190, in get_key
+			#     return mapping[fileobj]
+			#   File "/usr/lib/python3.7/selectors.py", line 71, in __getitem__
+			#     fd = self._selector._fileobj_lookup(fileobj)
+			#   File "/usr/lib/python3.7/selectors.py", line 225, in _fileobj_lookup
+			#     return _fileobj_to_fd(fileobj)
+			#   File "/usr/lib/python3.7/selectors.py", line 42, in _fileobj_to_fd
+			#     raise ValueError("Invalid file descriptor: {}".format(fd))
+			# ValueError: Invalid file descriptor: -1
+			pass
 
 	async def download(self, request: FetchRequest, completion_pipeline=None):
+		if not self.started:
+			await self.start()
 
 		"""
 		This method attempts to start a download. It is what users of the spider should call, and will take into
 		account any in-flight downloads for the same resource, which is most efficient and safe and will prevent
 		multiple requests for the same file.
 
 		The return value of this function varies depending on the value of ``completion_pipeline``. If
@@ -342,19 +461,22 @@
 		if os.path.exists(response.temp_path):
 			try:
 				os.unlink(response.temp_path)
 			except FileNotFoundError:
 				# FL-8301: address possible race condition
 				pass
 
-	async def acquire_host_semaphore(self, hostname):
-		semaphores = getattr(self.thread_ctx, "http_semaphores", None)
-		if semaphores is None:
-			semaphores = self.thread_ctx.http_semaphores = defaultdict(lambda: Semaphore(value=8))
-		return semaphores[hostname]
+	async def acquire_http_client(self, request):
+		log.debug(f"acquire_http_client: count: {len(self.http_clients)} (request for {request.hostname}) count: {self.fetch_count}")
+		if request.hostname not in self.http_clients:
+			headers, auth = self.get_headers_and_auth(request)
+			client = self.http_clients[request.hostname] = httpx.AsyncClient(transport=self.transport, http2=True, base_url=request.hostname, headers=headers, auth=auth, follow_redirects=True, timeout=8)
+			return client
+		else:
+			return self.http_clients[request.hostname]
 
 	def get_headers_and_auth(self, request):
 		headers = self.fetch_headers.copy()
 		if request.extra_headers:
 			headers.update(request.extra_headers)
 		else:
 			headers = self.fetch_headers
@@ -362,49 +484,96 @@
 			auth = (request.username, request.password)
 		else:
 			auth = None
 		return headers, auth
 
 	async def http_fetch(self, request: FetchRequest, is_json=False, encoding=None) -> str:
 		"""
+		UBER-NOTE:
+
 		This is a non-streaming HTTP fetcher that will properly convert the request to a Python string and return the entire
 		content as a string.
 
 		Use ``encoding`` if the HTTP resource does not have proper encoding and you have to set a specific encoding for string
 		conversion. Normally, the encoding will be auto-detected and decoded for you.
 
 		This method *will* return a FetchError if there was some kind of fetch failure, and this is used by the 'fetch cache'
 		so this is important.
-		"""
-		semi = await self.acquire_host_semaphore(request.hostname)
 
-		try:
-			async with semi:
-				async with httpx.AsyncClient() as client:
-					log.debug(f'Fetching data from {request.url}')
-					headers, auth = self.get_headers_and_auth(request)
-					response = await client.get(request.url, headers=headers, auth=auth, follow_redirects=True, timeout=8)
-					if response.status_code != 200:
-						if response.status_code in [400, 404, 410]:
-							# No need to retry as the server has just told us that the resource does not exist.
-							retry = False
-						else:
-							retry = True
-						log.error(f"Fetch failure for {request.url}: {response.status_code} {response.reason_phrase[:40]}")
-						raise FetchError(request, f"HTTP fetch Error: {request.url}: {response.status_code}: {response.reason_phrase[:40]}", retry=retry)
-					if is_json:
-						return response.json()
-					if encoding:
-						result = response.content.decode(encoding)
+		NEW IMPLEMENTATION of basic HTTP resource fetch:
+
+		We always want to store the "Last-Modified" response header, which contains a date to compare against.
+		We then want to always send "If-Modified-Since" with this date, when requesting the resource again, and if
+		we get a 304 back, we should just use the cached resource. If we get a 200, we should update the resource.
+		This means that for every request, we should intentionally look in our fetch cache first, and see if we have
+		a resource with a "Last-Modified" header. And if we do, we use this in our request, and potentially we return
+		the entry from our fetch cache.
+
+		ETag should also be used, which will use an "If-None-Match: "etag"" request header and similarly return a 304.
+
+		We should try to have our API hit the fetch cache only once.
+
+		In addition to this, metatools has its own built-in fetch_harness() which applies a level of caching, using
+		refresh_interval. Technically, this isn't a "cache" but just a default setting for how "fresh" we need something
+		to be for us to use it. By default, the refresh_interval is set to 15 minutes. (HOWEVER, IT LOOKS LIKE WE HAVE
+		A BUG WHERE THIS DEFAULTS to ZERO).
+
+		In addition to all this, we also have a 3-time-retry-the-fetch feature, which helps with flaky network and
+		intermittent Internet connectivity issues. Plus the ability to fall back to the cached resource if the fetch failed. In
+		this case, we are intentionally using a stale resource just for the sake of getting the autogen to work, and
+		we want this -- but we also currently don't really log these in a good way, and especially for production
+		tree regen, we would not see these unless we had a way to create a report that ran at the end of autogen.
+		I have a bug open to try to fix this.
+
+		It would be really good to implement something new to fix all these things.
+
+		New logic:
+
+		first, determine if we already have the resource and we are within our fetch cache interval. If so, let's
+		just use the resource.
+
+		if we don't have the resource, obviously we don't have a cached version to use, so we need to fetch the
+		resource.
+
+		If we have a resource already but are outside of our cached interval, we should attempt to update the
+		resource, using ETag and Modified-Since if we have those cached too. We should make several attempts
+		to update the resource (3) -- and if everything fails, we can fall back and use the stale resource.
+		But hopefully we have an updated or re-checked resource. When the resource is re-checked, even if it is
+		not actually updated, we should update our "refreshed" date so it remains inside our "refresh interval"
+		for longer.
+		"""
+		async with self.acquire_fetch_slot(request):
+			http_client = await self.acquire_http_client(request)
+			headers, auth = self.get_headers_and_auth(request)
+			# TODO: add code to explicitly close all clients, above:
+			try:
+				log.debug(f'http_fetch: GET {request.url}')
+				response = await http_client.get(request.url, headers=headers, auth=auth, follow_redirects=True, timeout=15)
+				if response.status_code != 200:
+					if response.status_code in [400, 404, 410]:
+						# No need to retry as the server has just told us that the resource does not exist.
+						retry = False
 					else:
-						result = response.text
-					log.info(f'Fetched {request.url} {len(result)} bytes')
-					return result
-		except httpx.RequestError as re:
-			raise FetchError(request, f"Could not connect to {request.url}: {repr(re)}", retry=False)
+						retry = True
+					try:
+						err_response = response.json()
+					except JSONDecodeError:
+						err_response = response.text
+					log.error(f"Fetch failure for {request.url}: {response.status_code} {response.reason_phrase} {err_response}")
+					raise FetchError(request, f"HTTP fetch Error: {request.url}: {response.status_code}: {response.reason_phrase} {err_response}", retry=retry)
+				if is_json:
+					return response.json()
+				if encoding:
+					result = response.content.decode(encoding)
+				else:
+					result = response.text
+				log.info(f'Fetched {request.url} {len(result)} bytes')
+				return result
+			except httpx.RequestError as re:
+				raise FetchError(request, f"Could not connect to {request.url}: {repr(re)}", retry=False)
 
 	@asynccontextmanager
 	async def acquire_download_slot(self):
 		"""
 		If you are inside this contextmanager, then it means you *have permission to start a download*.
 
 		This code originally tried to do this, but it would deadlock::
@@ -422,21 +591,38 @@
 		we wait.
 		"""
 		try:
 			while True:
 				success = self.DOWNLOAD_SLOT.acquire(blocking=False)
 				if not success:
 					await asyncio.sleep(0.1)
+					logging.info("WAITING ON SLOT")
 					continue
 				yield
 				break
 		finally:
 			self.DOWNLOAD_SLOT.release()
 
 	@asynccontextmanager
+	async def acquire_fetch_slot(self, request):
+		try:
+			while True:
+				success = self.FETCH_SLOT[request.hostname].acquire(blocking=False)
+				if not success:
+					await asyncio.sleep(0.1)
+					logging.info("WAITING ON SLOT")
+					continue
+				else:
+					self.fetch_count += 1
+				yield
+				break
+		finally:
+			self.FETCH_SLOT[request.hostname].release()
+
+	@asynccontextmanager
 	async def start_download(self, download):
 		"""
 		If you are inside the contextmanager, it means that you are ready to *start a download for a specific resource*.
 
 		Automatically record the download as being active, and remove from our list when complete.
 
 		While waiting for DL_ACTIVE_LOCK will FREEZE the current thread's ioloop, this is OK because we immediately release
@@ -453,13 +639,13 @@
 
 	def get_existing_download(self, request: FetchRequest):
 		"""
 		Get a download object for the file we're interested in if one is already being downloaded.
 		"""
 		with self.DL_ACTIVE_LOCK:
 			if request.url in self.DL_ACTIVE:
-				log.debug(f"WebSpider.get_existing_download:{threading.get_ident()} found active download for {request.url}")
+				log.warn(f"WebSpider.get_existing_download:{threading.get_ident()} found active download for {request.url}")
 
 				return self.DL_ACTIVE[request.url]
 
 			log.debug(f"WebSpider.get_existing_download:{threading.get_ident()} no active download for {request.url}")
 			return None
```

### Comparing `funtoo-metatools-1.1.1/metatools/fetch_cache.py` & `funtoo-metatools-1.2.0/metatools/fetch_cache.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.1.1/metatools/hashutils.py` & `funtoo-metatools-1.2.0/metatools/hashutils.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.1.1/metatools/kit.py` & `funtoo-metatools-1.2.0/metatools/kit.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,21 @@
 				eclass_path = os.path.join(eclass_scan_path, eclass)
 				eclass_name = eclass[:-7]
 				self.hashes[eclass_name] = get_md5(eclass_path)
 				scan_count += 1
 		model.log.debug(f"EclassHashCollection: Found {scan_count} eclasses in path {eclass_scan_path}.")
 
 
+class SimpleKitGenerator:
+	"""Our steps-based workflow requires a KitGenerator. If we want to use Steps, but don't have kits we're
+	working with, we can instead use this minimal implementation (used by bin/merge-gentoo-staging.)"""
+	def __init__(self, out_tree):
+		self.out_tree = out_tree
+
+
 class KitGenerator:
 	"""
 	This class represents the work associated with generating a Kit. A ``Kit`` (defined in metatools/files/release.py)
 	is passed to the constructor of this object to define settings, and stored within this object as ``self.kit``.
 
 	The KitGenerator takes care of creating or connecting to an existing Git tree that is used to house the results of
 	the kit generation, and this Git tree object is stored at ``self.out_tree``.
@@ -126,15 +133,15 @@
 			**model.git_kwargs
 		)
 		self.out_tree.initialize()
 		self.kit_cache = KitCache(name=kit.name, branch=kit.branch)
 
 	async def run(self, steps):
 		"""
-		This command runs ga series of steps. What I need to add is proper propagation of errors to caller.
+		This command runs a series of steps. What I need to add is proper propagation of errors to caller.
 		"""
 		for step in steps:
 			if step is not None:
 				model.log.info(f"Running step {step.__class__.__name__} for {self.out_tree.root}")
 				try:
 					await step.run(self)
 				except Exception as e:
@@ -219,16 +226,16 @@
 		cp_dir = ebuild_path[: ebuild_path.rfind("/")]
 		manifest_path = cp_dir + "/Manifest"
 
 		if not os.path.exists(manifest_path):
 			manifest_md5 = None
 		else:
 			# TODO: this is a potential area of performance improvement. Multiple ebuilds in a single catpkg
-			#       directory will result in get_md5() being called on the same Manifest file multiple times
-			#       during a run. Cache might be good here.
+			#		directory will result in get_md5() being called on the same Manifest file multiple times
+			#		during a run. Cache might be good here.
 			manifest_md5 = get_md5(manifest_path)
 
 		# Try to see if we already have this metadata in our kit metadata cache.
 		existing = self.kit_cache.get_atom(atom, ebuild_md5, manifest_md5, merged_eclasses)
 
 		if existing:
 			self.kit_cache.retrieved_atoms.add(atom)
@@ -376,23 +383,23 @@
 		"""
 		This function produces steps to recreate the contents of an autogenerated kit. This is typically run with a
 		destination kit that has been "emptied" and is ready to be regenerated from scratch:
 
 		1. First, look at ``packages.yaml`` and copy over any specified eclasses and files from source repositories.
 		2. Next, look at ``packages.yaml``, and copy over any specified ebuilds from any source repositories. Note
 		   that we do not run autogen for source repositories used in this way.
-	    3. Next, *remove* any files we specifically want to exclude from the destination kit.
+		3. Next, *remove* any files we specifically want to exclude from the destination kit.
 
-	    In the second phase, we then perform the following actions:
+		In the second phase, we then perform the following actions:
 
-	    4. Run autogen on the proper part of kit-fixups.
-	    5. Copy over all resultant ebuilds, eclasses, licenses, etc from kit-fixups that should be copied.
+		4. Run autogen on the proper part of kit-fixups.
+		5. Copy over all resultant ebuilds, eclasses, licenses, etc from kit-fixups that should be copied.
 
-	    This ensures that kit-fixups overrides whatever was in the source repositories. Once these steps are all done,
-	    the kit is ready for finalization (gencache, etc.) and a git commit which will contain the new changes.
+		This ensures that kit-fixups overrides whatever was in the source repositories. Once these steps are all done,
+		the kit is ready for finalization (gencache, etc.) and a git commit which will contain the new changes.
 		"""
 
 		await self.run(self.copy_eclasses_steps())
 		await self.run(self.packages_yaml_copy_ebuilds_steps())
 		await self.run([metatools.steps.RemoveFiles(self.kit.get_excludes())])
 
 		self.out_tree.gitAdd()
@@ -413,17 +420,17 @@
 				run_shell(f"cp {found} {self.out_tree.root}/licenses", logger=model.log)
 
 	async def distfile_scan(self):
 		self.kit_cache.load()
 		# We can now perform the steps in distfile-kit-fetch as we have access to the kit-cache.
 		# TODO: add code here
 		# TODO: add extra code here to log any issues. We should temp. hook into the log handler
-		#       to re-route any messages to an appropriate log file. This would actually be a good
-		#       general idea as we don't have this mechanism in the autogen process right now
-		#       (separated logs don't go to disk.) So maybe we want to implement this outside this
+		#		to re-route any messages to an appropriate log file. This would actually be a good
+		#		general idea as we don't have this mechanism in the autogen process right now
+		#		(separated logs don't go to disk.) So maybe we want to implement this outside this
 		#		method, in the KitJob.
 
 	async def reposcan(self):
 		self.fetch_kit()
 		self.gen_cache()
 		self.flush_kit()
 
@@ -435,17 +442,17 @@
 		Here is a basic overview of the process:
 
 		1. The to-be-updated kit is completely emptied of all files. (``CleanTree()``)
 		2. The basic metadata is created inside the kit to make it a valid, but empty overlay. (``GenerateRepoMetadata()``)
 		3. Depending on what type of kit it is -- autogenerated or sourced -- the steps will be executed to populate the kit
 		   with its updated contents.
 		4. Various miscellaneous tasks will be executed -- creating a global licensing information file, cleaning up of Manifests, etc.
-	    5. The Portage metadata cache will be updated and stored inside the kit.
-	    6. Auto-generation of Python USE settings will be performed. This optimizes the Python USE experience for Funtoo users.
-	    7. Licenses used by the ebuilds will be copied over to the ``licenses/`` directory.
+		5. The Portage metadata cache will be updated and stored inside the kit.
+		6. Auto-generation of Python USE settings will be performed. This optimizes the Python USE experience for Funtoo users.
+		7. Licenses used by the ebuilds will be copied over to the ``licenses/`` directory.
 		7. A new git commit within the kit will be created based on the result of these steps.
 		8. The HEAD SHA1 will be recorded so that we can record it later within the meta-repo metadata.
 		"""
 
 		# load on-disk JSON metadata cache into memory:
 
 		self.kit_cache.load()
@@ -508,15 +515,15 @@
 		# We can now run all the steps that require access to metadata:
 
 		# Funtoo and metatools has a feature where we will look at the configured Python kits for the release,
 		# and auto-generate optimal Python USE settings for each kit in the release. This ensures that things
 		# can be easily merged without weird Python USE errors. These settings are stored in the following
 		# location in each kit in the release::
 		#
-		# 	profiles/funtoo/kits/python-kit/<python-kit-branch>
+		#	profiles/funtoo/kits/python-kit/<python-kit-branch>
 		#
 		# When 'ego sync' runs, it will ensure that these settings are automatically enabled based upon what
 		# your currently-active python-kit is. This means that even if you have multiple python-kit branches
 		# defined in your release, switching between them is seamless and Python USE settings for all packages
 		# in the repository will auto-adapt to whatever Python kit is currently enabled.
 
 		await self.run([metatools.steps.GenPythonUse()])
@@ -639,15 +646,15 @@
 					steps += [metatools.steps.SyncFiles(model.kit_fixups.root, {readme_path: "README.rst"})]
 
 				# We now add a step to insert the fixups, and we want to record them as being copied so successive kits
 				# don't get this particular catpkg. Assume we may not have all these catpkgs listed in our package-set
 				# file...
 
 				# TODO: since we are running autogen in a for-loop, below, there is always the possibility of parallelizing this code further.
-				#       The only challenge is that we may be autogenning similar ebuilds, and thus we may be writing to the same Store() behind-the-scenes.
+				#		The only challenge is that we may be autogenning similar ebuilds, and thus we may be writing to the same Store() behind-the-scenes.
 
 				steps += [
 					metatools.steps.Autogen(model.kit_fixups, ebuildloc=fixup_path),
 					metatools.steps.InsertEbuilds(model.kit_fixups, ebuildloc=fixup_path, select="all", skip=None,
 												  replace=True)
 				]
 		return steps
```

### Comparing `funtoo-metatools-1.1.1/metatools/kit_cache.py` & `funtoo-metatools-1.2.0/metatools/kit_cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,16 +129,19 @@
 				model.log.error("THERE ARE EXTRA ATOMS THAT WERE RETRIEVED BUT NOT IN CACHE!")
 				model.log.error(f"{extra_atoms}")
 		outdata = {
 			"cache_data_version": CACHE_DATA_VERSION,
 			"atoms": self.json_data["atoms"],
 			"metadata_errors": self.metadata_errors,
 		}
-		model.log.warning(
-			f"Flushed {self.name}. {len(self.json_data['atoms'])} atoms. Removed {len(remove_keys)} keys. {len(self.metadata_errors)} errors.")
+		if len(self.metadata_errors):
+			log_out = model.log.warning
+		else:
+			log_out = model.log.debug
+		log_out(f"Flushed {self.name}. {len(self.json_data['atoms'])} atoms. Removed {len(remove_keys)} keys. {len(self.metadata_errors)} errors.")
 		os.makedirs(os.path.dirname(self.path), exist_ok=True)
 		with open(self.path, "w") as f:
 			f.write(json.dumps(outdata))
 		error_outpath = os.path.join(
 			model.temp_path, f"metadata-errors-{self.name}-{self.branch}.log"
 		)
 		if len(self.metadata_errors):
```

### Comparing `funtoo-metatools-1.1.1/metatools/metadata.py` & `funtoo-metatools-1.2.0/metatools/metadata.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.1.1/metatools/model.py` & `funtoo-metatools-1.2.0/metatools/model.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.1.1/metatools/pretty_logging.py` & `funtoo-metatools-1.2.0/metatools/pretty_logging.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.1.1/metatools/steps.py` & `funtoo-metatools-1.2.0/metatools/steps.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python3
-
+import asyncio
 import itertools
 import os
 import re
 import shutil
 import jinja2
 
 from metatools import metadata
@@ -13,14 +13,23 @@
 model = get_model("metatools.merge")
 
 
 def run_shell(cmd_list, abort_on_failure=True, chdir=None):
 	return metatools.tree.run_shell(cmd_list, abort_on_failure=abort_on_failure, chdir=chdir, logger=model.log)
 
 
+async def run_bg(cmd):
+	proc = await asyncio.create_subprocess_shell(cmd,
+	stdout=asyncio.subprocess.PIPE,
+	stderr=asyncio.subprocess.STDOUT)
+
+	stdout, stderr = await proc.communicate()
+	return proc, stdout
+
+
 class MergeStep:
 
 	# This is only used for Repository Steps:
 	collector = None
 
 	async def run(self, kit_gen):
 		pass
@@ -188,14 +197,16 @@
 
 	An assumption is made that we are copying regular files, so that we can properly create source directories
 	if they do not exist.
 
 	"""
 
 	def __init__(self, srctree, file_map_tuples):
+		if srctree is None:
+			raise ValueError("srctree can't be None")
 		self.srctree = srctree
 		self.file_map_tuples = file_map_tuples
 
 	async def run(self, kit_gen):
 		for src_path, dst_path in self.file_map_tuples:
 			f_src_path = os.path.join(self.srctree.root, src_path)
 			if not os.path.exists(f_src_path):
```

### Comparing `funtoo-metatools-1.1.1/metatools/store.py` & `funtoo-metatools-1.2.0/metatools/store.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.1.1/metatools/tree.py` & `funtoo-metatools-1.2.0/metatools/tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,15 +110,15 @@
 		if retcode != 0:
 			self.log.error(f"Command failure from merge-kits: {cmd_str}")
 			raise GitTreeError(f"failed autogen in {self.root} -- offset {src_offset}.")
 		self.autogenned = src_offset
 
 	def cleanTree(self):
 		self.log.info("Cleaning tree %s" % self.root)
-		self.run_shell("(cd %s &&  git reset --hard && git clean -fdx )" % self.root)
+		self.run_shell(f"(cd {self.root} && git reset --hard && git clean -fdx )")
 		self.autogenned = False
 
 	def getDepthOfCommit(self, sha1):
 		s, depth = subprocess.getstatusoutput("( cd %s && git rev-list HEAD ^%s --count)" % (self.root, sha1))
 		return int(depth) + 1
 
 	def localBranchExists(self, branch):
@@ -494,21 +494,27 @@
 			if self.head() != sha1:
 				raise GitTreeError("Not able to check out requested sha1: %s, got: %s" % (sha1, self.head()))
 		else:
 			if self.currentLocalBranch != branch:
 				self.run_shell("(cd %s && git fetch --verbose)" % self.root)
 				if self.localBranchExists(branch):
 					self.run_shell("(cd %s && git checkout %s)" % (self.root, branch))
+					self.cleanTree()
+					self.do_pull()
 				elif self.remoteBranchExists(branch):
 					# An AutoCreatedGitTree will automatically create branches as needed, as forks of master.
 					self.run_shell("(cd %s && git checkout -b %s --track origin/%s)" % (self.root, branch, branch))
-				else:
-					self.run_shell("(cd %s && git checkout -b %s)" % (self.root, branch))
-				self.cleanTree()
-				self.do_pull()
+					self.cleanTree()
+					self.do_pull()
+				elif self.create_branches:
+					self.run_shell(f"(cd {self.root} && git checkout -b {branch})")
+					self.run_shell(f"echo 'created by merge-kits.' > {self.root}/README")
+					self.run_shell(f"(cd {self.root} && git add README; git commit -a -m 'initial commit by merge-kits' )")
+					self.run_shell(f"(cd {self.root} && git push --set-upstream origin {branch})")
+					self.cleanTree()
 			else:
 				old_head = self.head()
 				self.do_pull()
 				new_head = self.head()
 				if old_head != new_head:
 					self.cleanTree()
 		if branch and self.currentLocalBranch != branch:
```

### Comparing `funtoo-metatools-1.1.1/metatools/yaml_util.py` & `funtoo-metatools-1.2.0/metatools/yaml_util.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.1.1/setup.py` & `funtoo-metatools-1.2.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 pkgr = Packager()
 
 with open("README.rst", "r") as fh:
 	long_description = fh.read()
 
 setuptools.setup(
 	name="funtoo-metatools",
-	version="1.1.1",
+	version="1.2.0",
 	author="Daniel Robbins",
 	author_email="drobbins@funtoo.org",
 	description="Funtoo framework for auto-creation of ebuilds.",
 	long_description=long_description,
 	long_description_content_type="text/x-rst",
 	url="https://code.funtoo.org/bitbucket/users/drobbins/repos/funtoo-metatools/browse",
 	scripts=["bin/doit", "bin/merge-kits"],
@@ -22,20 +22,21 @@
 		"Operating System :: POSIX :: Linux",
 	],
 	python_requires=">=3.7",
 	install_requires=[
 		"subpop >= 2.0.0",
 		"beautifulsoup4",
 		"dict_toolbox",
-		"httpx < 0.23.0",
+		"httpx[http2]",
 		"Jinja2 >= 3",
 		"packaging",
 		"psutil",
 		"pymongo",
 		"PyYAML",
+		"rich",
 		"toml",
 		"xmltodict",
 		"colorama",
 	],
 	packages=setuptools.find_packages(),
 	data_files=pkgr.generate_data_files(),
 	cmdclass={"install": SubPopSetupInstall},
```

