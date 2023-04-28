# Comparing `tmp/cyberdrop-dl-4.1.17.tar.gz` & `tmp/cyberdrop-dl-4.1.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyberdrop-dl-4.1.17.tar", last modified: Fri Apr 28 01:42:17 2023, max compression
+gzip compressed data, was "cyberdrop-dl-4.1.18.tar", last modified: Fri Apr 28 02:28:24 2023, max compression
```

## Comparing `cyberdrop-dl-4.1.17.tar` & `cyberdrop-dl-4.1.18.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:42:17.009539 cyberdrop-dl-4.1.17/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-04-28 01:42:17.009539 cyberdrop-dl-4.1.17/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16523 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:42:17.001539 cyberdrop-dl-4.1.17/cyberdrop_dl/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:42:17.005539 cyberdrop-dl-4.1.17/cyberdrop_dl/base_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/base_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/base_functions/base_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/base_functions/config_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/base_functions/config_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/base_functions/data_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/base_functions/error_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/base_functions/sorting_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12383 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/base_functions/sql_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:42:17.005539 cyberdrop-dl-4.1.17/cyberdrop_dl/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9523 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/client/rate_limiting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:42:17.009539 cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/Anonfiles_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     7493 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/Bunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/Coomeno_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    12064 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/CyberFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/EHentai_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/Erome_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/Fapello_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/Gfycat_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/GoFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/HGameCG_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/ImgBox_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/LoveFap_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/NSFWXXXCrawler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/PixelDrain_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/PostImg_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/Saint_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     8411 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/ShareX_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/XBunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    15025 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/Xenforo_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:42:17.009539 cyberdrop-dl-4.1.17/cyberdrop_dl/downloader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/downloader/downloader_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17390 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/downloader/downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    13871 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/downloader/old_downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/downloader/progress_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)    18626 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:42:17.009539 cyberdrop-dl-4.1.17/cyberdrop_dl/scraper/
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/scraper/JDownloader_Integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    20206 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/scraper/Scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/scraper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:42:17.001539 cyberdrop-dl-4.1.17/cyberdrop_dl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-04-28 01:42:16.000000 cyberdrop-dl-4.1.17/cyberdrop_dl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-28 01:42:16.000000 cyberdrop-dl-4.1.17/cyberdrop_dl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 01:42:16.000000 cyberdrop-dl-4.1.17/cyberdrop_dl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-28 01:42:16.000000 cyberdrop-dl-4.1.17/cyberdrop_dl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-28 01:42:16.000000 cyberdrop-dl-4.1.17/cyberdrop_dl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-28 01:42:16.000000 cyberdrop-dl-4.1.17/cyberdrop_dl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-28 01:42:17.009539 cyberdrop-dl-4.1.17/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:28:24.255931 cyberdrop-dl-4.1.18/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-28 02:28:12.000000 cyberdrop-dl-4.1.18/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-04-28 02:28:24.255931 cyberdrop-dl-4.1.18/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16523 2023-04-28 02:28:12.000000 cyberdrop-dl-4.1.18/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:28:24.251931 cyberdrop-dl-4.1.18/cyberdrop_dl/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-28 02:28:12.000000 cyberdrop-dl-4.1.18/cyberdrop_dl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:28:24.251931 cyberdrop-dl-4.1.18/cyberdrop_dl/base_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 02:28:12.000000 cyberdrop-dl-4.1.18/cyberdrop_dl/base_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-04-28 02:28:12.000000 cyberdrop-dl-4.1.18/cyberdrop_dl/base_functions/base_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-04-28 02:28:12.000000 cyberdrop-dl-4.1.18/cyberdrop_dl/base_functions/config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-04-28 02:28:12.000000 cyberdrop-dl-4.1.18/cyberdrop_dl/base_functions/config_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-04-28 02:28:12.000000 cyberdrop-dl-4.1.18/cyberdrop_dl/base_functions/data_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-28 02:28:12.000000 cyberdrop-dl-4.1.18/cyberdrop_dl/base_functions/error_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-04-28 02:28:12.000000 cyberdrop-dl-4.1.18/cyberdrop_dl/base_functions/sorting_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12383 2023-04-28 02:28:12.000000 cyberdrop-dl-4.1.18/cyberdrop_dl/base_functions/sql_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:28:24.251931 cyberdrop-dl-4.1.18/cyberdrop_dl/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 02:28:12.000000 cyberdrop-dl-4.1.18/cyberdrop_dl/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9523 2023-04-28 02:28:12.000000 cyberdrop-dl-4.1.18/cyberdrop_dl/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-04-28 02:28:12.000000 cyberdrop-dl-4.1.18/cyberdrop_dl/client/rate_limiting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:28:24.255931 cyberdrop-dl-4.1.18/cyberdrop_dl/crawlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-04-28 02:28:12.000000 cyberdrop-dl-4.1.18/cyberdrop_dl/crawlers/Anonfiles_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7493 2023-04-28 02:28:12.000000 cyberdrop-dl-4.1.18/cyberdrop_dl/crawlers/Bunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-04-28 02:28:12.000000 cyberdrop-dl-4.1.18/cyberdrop_dl/crawlers/Coomeno_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12064 2023-04-28 02:28:12.000000 cyberdrop-dl-4.1.18/cyberdrop_dl/crawlers/CyberFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-28 02:28:12.000000 cyberdrop-dl-4.1.18/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-04-28 02:28:12.000000 cyberdrop-dl-4.1.18/cyberdrop_dl/crawlers/EHentai_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-04-28 02:28:12.000000 cyberdrop-dl-4.1.18/cyberdrop_dl/crawlers/Erome_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-04-28 02:28:12.000000 cyberdrop-dl-4.1.18/cyberdrop_dl/crawlers/Fapello_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-04-28 02:28:12.000000 cyberdrop-dl-4.1.18/cyberdrop_dl/crawlers/Gfycat_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-04-28 02:28:12.000000 cyberdrop-dl-4.1.18/cyberdrop_dl/crawlers/GoFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-04-28 02:28:12.000000 cyberdrop-dl-4.1.18/cyberdrop_dl/crawlers/HGameCG_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-04-28 02:28:12.000000 cyberdrop-dl-4.1.18/cyberdrop_dl/crawlers/ImgBox_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-04-28 02:28:12.000000 cyberdrop-dl-4.1.18/cyberdrop_dl/crawlers/LoveFap_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-04-28 02:28:12.000000 cyberdrop-dl-4.1.18/cyberdrop_dl/crawlers/NSFWXXXCrawler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-04-28 02:28:12.000000 cyberdrop-dl-4.1.18/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-04-28 02:28:12.000000 cyberdrop-dl-4.1.18/cyberdrop_dl/crawlers/PixelDrain_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-04-28 02:28:12.000000 cyberdrop-dl-4.1.18/cyberdrop_dl/crawlers/PostImg_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-28 02:28:12.000000 cyberdrop-dl-4.1.18/cyberdrop_dl/crawlers/Saint_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8411 2023-04-28 02:28:12.000000 cyberdrop-dl-4.1.18/cyberdrop_dl/crawlers/ShareX_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-04-28 02:28:12.000000 cyberdrop-dl-4.1.18/cyberdrop_dl/crawlers/XBunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15025 2023-04-28 02:28:12.000000 cyberdrop-dl-4.1.18/cyberdrop_dl/crawlers/Xenforo_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 02:28:12.000000 cyberdrop-dl-4.1.18/cyberdrop_dl/crawlers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:28:24.255931 cyberdrop-dl-4.1.18/cyberdrop_dl/downloader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 02:28:12.000000 cyberdrop-dl-4.1.18/cyberdrop_dl/downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-04-28 02:28:12.000000 cyberdrop-dl-4.1.18/cyberdrop_dl/downloader/downloader_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17390 2023-04-28 02:28:12.000000 cyberdrop-dl-4.1.18/cyberdrop_dl/downloader/downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13871 2023-04-28 02:28:12.000000 cyberdrop-dl-4.1.18/cyberdrop_dl/downloader/old_downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-04-28 02:28:12.000000 cyberdrop-dl-4.1.18/cyberdrop_dl/downloader/progress_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18626 2023-04-28 02:28:12.000000 cyberdrop-dl-4.1.18/cyberdrop_dl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:28:24.255931 cyberdrop-dl-4.1.18/cyberdrop_dl/scraper/
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-04-28 02:28:12.000000 cyberdrop-dl-4.1.18/cyberdrop_dl/scraper/JDownloader_Integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20206 2023-04-28 02:28:12.000000 cyberdrop-dl-4.1.18/cyberdrop_dl/scraper/Scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 02:28:12.000000 cyberdrop-dl-4.1.18/cyberdrop_dl/scraper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 02:28:24.251931 cyberdrop-dl-4.1.18/cyberdrop_dl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-04-28 02:28:24.000000 cyberdrop-dl-4.1.18/cyberdrop_dl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-28 02:28:24.000000 cyberdrop-dl-4.1.18/cyberdrop_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 02:28:24.000000 cyberdrop-dl-4.1.18/cyberdrop_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-28 02:28:24.000000 cyberdrop-dl-4.1.18/cyberdrop_dl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-28 02:28:24.000000 cyberdrop-dl-4.1.18/cyberdrop_dl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-28 02:28:24.000000 cyberdrop-dl-4.1.18/cyberdrop_dl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-28 02:28:12.000000 cyberdrop-dl-4.1.18/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-28 02:28:24.255931 cyberdrop-dl-4.1.18/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 02:28:12.000000 cyberdrop-dl-4.1.18/setup.py
```

### Comparing `cyberdrop-dl-4.1.17/LICENSE` & `cyberdrop-dl-4.1.18/LICENSE`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.17/PKG-INFO` & `cyberdrop-dl-4.1.18/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.1.17
+Version: 4.1.18
 Summary: Bulk downloader for multiple file hosts and forum sites
 Home-page: https://github.com/Jules-WinnfieldX/CyberDropDownloader
 Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com
 Project-URL: Bug Tracker, https://github.com/Jules-WinnfieldX/CyberDropDownloader/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.1.17 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.1.18 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
```

### Comparing `cyberdrop-dl-4.1.17/README.md` & `cyberdrop-dl-4.1.18/README.md`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.17/cyberdrop_dl/base_functions/base_functions.py` & `cyberdrop-dl-4.1.18/cyberdrop_dl/base_functions/base_functions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.17/cyberdrop_dl/base_functions/config_manager.py` & `cyberdrop-dl-4.1.18/cyberdrop_dl/base_functions/config_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -76,14 +76,15 @@
 
 async def document_args(args: dict) -> None:
     """We document the runtime arguments for debugging and troubleshooting, redacting sensitive information"""
     print_args = copy.deepcopy(args)
     print_args['Authentication']['xbunker_password'] = '!REDACTED!' if args['Authentication']['xbunker_password'] is not None else None
     print_args['Authentication']['socialmediagirls_password'] = '!REDACTED!' if args['Authentication']['socialmediagirls_password'] is not None else None
     print_args['Authentication']['simpcity_password'] = '!REDACTED!' if args['Authentication']['simpcity_password'] is not None else None
+    print_args['Authentication']['nudostar_password'] = '!REDACTED!' if args['Authentication']['nudostar_password'] is not None else None
     print_args['Authentication']['pixeldrain_api_key'] = '!REDACTED!' if args['Authentication']['pixeldrain_api_key'] is not None else None
     print_args['JDownloader']['jdownloader_password'] = '!REDACTED!' if args['JDownloader']['jdownloader_password'] is not None else None
 
     log("Starting Cyberdrop-DL")
     log(f"Using authentication arguments: {print_args['Authentication']}", quiet=True)
     log(f"Using file arguments: {print_args['Files']}", quiet=True)
     log(f"Using forum option arguments: {print_args['Forum_Options']}", quiet=True)
```

### Comparing `cyberdrop-dl-4.1.17/cyberdrop_dl/base_functions/config_schema.py` & `cyberdrop-dl-4.1.18/cyberdrop_dl/base_functions/config_schema.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.17/cyberdrop_dl/base_functions/data_classes.py` & `cyberdrop-dl-4.1.18/cyberdrop_dl/base_functions/data_classes.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.17/cyberdrop_dl/base_functions/error_classes.py` & `cyberdrop-dl-4.1.18/cyberdrop_dl/base_functions/error_classes.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.17/cyberdrop_dl/base_functions/sorting_functions.py` & `cyberdrop-dl-4.1.18/cyberdrop_dl/base_functions/sorting_functions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.17/cyberdrop_dl/base_functions/sql_helper.py` & `cyberdrop-dl-4.1.18/cyberdrop_dl/base_functions/sql_helper.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.17/cyberdrop_dl/client/client.py` & `cyberdrop-dl-4.1.18/cyberdrop_dl/client/client.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.17/cyberdrop_dl/client/rate_limiting.py` & `cyberdrop-dl-4.1.18/cyberdrop_dl/client/rate_limiting.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/Anonfiles_Spider.py` & `cyberdrop-dl-4.1.18/cyberdrop_dl/crawlers/Anonfiles_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/Bunkr_Spider.py` & `cyberdrop-dl-4.1.18/cyberdrop_dl/crawlers/Bunkr_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/Coomeno_Spider.py` & `cyberdrop-dl-4.1.18/cyberdrop_dl/crawlers/Coomeno_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/CyberFile_Spider.py` & `cyberdrop-dl-4.1.18/cyberdrop_dl/crawlers/CyberFile_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/Cyberdrop_Spider.py` & `cyberdrop-dl-4.1.18/cyberdrop_dl/crawlers/Cyberdrop_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/EHentai_Spider.py` & `cyberdrop-dl-4.1.18/cyberdrop_dl/crawlers/EHentai_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/Erome_Spider.py` & `cyberdrop-dl-4.1.18/cyberdrop_dl/crawlers/Erome_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/Fapello_Spider.py` & `cyberdrop-dl-4.1.18/cyberdrop_dl/crawlers/Fapello_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/Gfycat_Spider.py` & `cyberdrop-dl-4.1.18/cyberdrop_dl/crawlers/Gfycat_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/GoFile_Spider.py` & `cyberdrop-dl-4.1.18/cyberdrop_dl/crawlers/GoFile_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/HGameCG_Spider.py` & `cyberdrop-dl-4.1.18/cyberdrop_dl/crawlers/HGameCG_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/ImgBox_Spider.py` & `cyberdrop-dl-4.1.18/cyberdrop_dl/crawlers/ImgBox_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/LoveFap_Spider.py` & `cyberdrop-dl-4.1.18/cyberdrop_dl/crawlers/LoveFap_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/NSFWXXXCrawler.py` & `cyberdrop-dl-4.1.18/cyberdrop_dl/crawlers/NSFWXXXCrawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/PimpAndHost_Spider.py` & `cyberdrop-dl-4.1.18/cyberdrop_dl/crawlers/PimpAndHost_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/PixelDrain_Spider.py` & `cyberdrop-dl-4.1.18/cyberdrop_dl/crawlers/PixelDrain_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/PostImg_Spider.py` & `cyberdrop-dl-4.1.18/cyberdrop_dl/crawlers/PostImg_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/Saint_Spider.py` & `cyberdrop-dl-4.1.18/cyberdrop_dl/crawlers/Saint_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/ShareX_Spider.py` & `cyberdrop-dl-4.1.18/cyberdrop_dl/crawlers/ShareX_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/XBunkr_Spider.py` & `cyberdrop-dl-4.1.18/cyberdrop_dl/crawlers/XBunkr_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/Xenforo_Spider.py` & `cyberdrop-dl-4.1.18/cyberdrop_dl/crawlers/Xenforo_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.17/cyberdrop_dl/downloader/downloader_utils.py` & `cyberdrop-dl-4.1.18/cyberdrop_dl/downloader/downloader_utils.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.17/cyberdrop_dl/downloader/downloaders.py` & `cyberdrop-dl-4.1.18/cyberdrop_dl/downloader/downloaders.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.17/cyberdrop_dl/downloader/old_downloaders.py` & `cyberdrop-dl-4.1.18/cyberdrop_dl/downloader/old_downloaders.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.17/cyberdrop_dl/downloader/progress_definitions.py` & `cyberdrop-dl-4.1.18/cyberdrop_dl/downloader/progress_definitions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.17/cyberdrop_dl/main.py` & `cyberdrop-dl-4.1.18/cyberdrop_dl/main.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.17/cyberdrop_dl/scraper/JDownloader_Integration.py` & `cyberdrop-dl-4.1.18/cyberdrop_dl/scraper/JDownloader_Integration.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.17/cyberdrop_dl/scraper/Scraper.py` & `cyberdrop-dl-4.1.18/cyberdrop_dl/scraper/Scraper.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.17/cyberdrop_dl.egg-info/PKG-INFO` & `cyberdrop-dl-4.1.18/cyberdrop_dl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.1.17
+Version: 4.1.18
 Summary: Bulk downloader for multiple file hosts and forum sites
 Home-page: https://github.com/Jules-WinnfieldX/CyberDropDownloader
 Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com
 Project-URL: Bug Tracker, https://github.com/Jules-WinnfieldX/CyberDropDownloader/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.1.17 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.1.18 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
```

### Comparing `cyberdrop-dl-4.1.17/cyberdrop_dl.egg-info/SOURCES.txt` & `cyberdrop-dl-4.1.18/cyberdrop_dl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.17/setup.cfg` & `cyberdrop-dl-4.1.18/setup.cfg`

 * *Files identical despite different names*

