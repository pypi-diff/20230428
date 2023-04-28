# Comparing `tmp/cyberdrop-dl-4.1.16.tar.gz` & `tmp/cyberdrop-dl-4.1.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyberdrop-dl-4.1.16.tar", last modified: Thu Apr 27 18:21:56 2023, max compression
+gzip compressed data, was "cyberdrop-dl-4.1.17.tar", last modified: Fri Apr 28 01:42:17 2023, max compression
```

## Comparing `cyberdrop-dl-4.1.16.tar` & `cyberdrop-dl-4.1.17.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:21:56.152648 cyberdrop-dl-4.1.16/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16561 2023-04-27 18:21:56.152648 cyberdrop-dl-4.1.16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16126 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:21:56.144648 cyberdrop-dl-4.1.16/cyberdrop_dl/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:21:56.144648 cyberdrop-dl-4.1.16/cyberdrop_dl/base_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/base_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/base_functions/base_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/base_functions/config_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/base_functions/config_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     8085 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/base_functions/data_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/base_functions/error_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/base_functions/sorting_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12443 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/base_functions/sql_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:21:56.148648 cyberdrop-dl-4.1.16/cyberdrop_dl/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9081 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/client/rate_limiting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:21:56.148648 cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/Anonfiles_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     7449 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/Bunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/Coomeno_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    10888 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/CyberFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/EHentai_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/Erome_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/Fapello_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/Gfycat_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/GoFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/HGameCG_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/ImgBox_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/LoveFap_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/NSFWXXXCrawler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/PixelDrain_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/PostImg_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/Saint_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     8383 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/ShareX_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/XBunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    14912 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/Xenforo_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:21:56.148648 cyberdrop-dl-4.1.16/cyberdrop_dl/downloader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/downloader/downloader_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17378 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/downloader/downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    13749 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/downloader/old_downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/downloader/progress_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)    18719 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:21:56.152648 cyberdrop-dl-4.1.16/cyberdrop_dl/scraper/
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/scraper/JDownloader_Integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    19342 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/scraper/Scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/cyberdrop_dl/scraper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 18:21:56.144648 cyberdrop-dl-4.1.16/cyberdrop_dl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16561 2023-04-27 18:21:56.000000 cyberdrop-dl-4.1.16/cyberdrop_dl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-27 18:21:56.000000 cyberdrop-dl-4.1.16/cyberdrop_dl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 18:21:56.000000 cyberdrop-dl-4.1.16/cyberdrop_dl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-27 18:21:56.000000 cyberdrop-dl-4.1.16/cyberdrop_dl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-27 18:21:56.000000 cyberdrop-dl-4.1.16/cyberdrop_dl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-27 18:21:56.000000 cyberdrop-dl-4.1.16/cyberdrop_dl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-27 18:21:56.152648 cyberdrop-dl-4.1.16/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 18:21:45.000000 cyberdrop-dl-4.1.16/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:42:17.009539 cyberdrop-dl-4.1.17/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-04-28 01:42:17.009539 cyberdrop-dl-4.1.17/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16523 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:42:17.001539 cyberdrop-dl-4.1.17/cyberdrop_dl/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:42:17.005539 cyberdrop-dl-4.1.17/cyberdrop_dl/base_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/base_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/base_functions/base_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/base_functions/config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/base_functions/config_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/base_functions/data_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/base_functions/error_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/base_functions/sorting_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12383 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/base_functions/sql_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:42:17.005539 cyberdrop-dl-4.1.17/cyberdrop_dl/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9523 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/client/rate_limiting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:42:17.009539 cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/Anonfiles_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7493 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/Bunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/Coomeno_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12064 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/CyberFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/EHentai_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/Erome_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/Fapello_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/Gfycat_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/GoFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/HGameCG_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/ImgBox_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/LoveFap_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/NSFWXXXCrawler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/PixelDrain_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/PostImg_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/Saint_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8411 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/ShareX_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/XBunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15025 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/Xenforo_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:42:17.009539 cyberdrop-dl-4.1.17/cyberdrop_dl/downloader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/downloader/downloader_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17390 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/downloader/downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13871 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/downloader/old_downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/downloader/progress_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18626 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:42:17.009539 cyberdrop-dl-4.1.17/cyberdrop_dl/scraper/
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/scraper/JDownloader_Integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20206 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/scraper/Scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/cyberdrop_dl/scraper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:42:17.001539 cyberdrop-dl-4.1.17/cyberdrop_dl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-04-28 01:42:16.000000 cyberdrop-dl-4.1.17/cyberdrop_dl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-28 01:42:16.000000 cyberdrop-dl-4.1.17/cyberdrop_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 01:42:16.000000 cyberdrop-dl-4.1.17/cyberdrop_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-28 01:42:16.000000 cyberdrop-dl-4.1.17/cyberdrop_dl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-28 01:42:16.000000 cyberdrop-dl-4.1.17/cyberdrop_dl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-28 01:42:16.000000 cyberdrop-dl-4.1.17/cyberdrop_dl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-28 01:42:17.009539 cyberdrop-dl-4.1.17/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 01:42:07.000000 cyberdrop-dl-4.1.17/setup.py
```

### Comparing `cyberdrop-dl-4.1.16/LICENSE` & `cyberdrop-dl-4.1.17/LICENSE`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.16/PKG-INFO` & `cyberdrop-dl-4.1.17/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.1.16
+Version: 4.1.17
 Summary: Bulk downloader for multiple file hosts and forum sites
 Home-page: https://github.com/Jules-WinnfieldX/CyberDropDownloader
 Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com
 Project-URL: Bug Tracker, https://github.com/Jules-WinnfieldX/CyberDropDownloader/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -63,14 +63,15 @@
 | jpg.church<br/>jpg.fish | Albums: jpg.church/album/... <br> Direct Images: jpg.church/image/... <br> User Profile: jpg.church/#USER# <br> All User Albums: jpg.church/#USER#/albums                                                                              |
 | LoveFap                 | Albums: lovefap.com/a/... <br> Direct Images: s*.lovefap.com/content/photos/... <br> Videos: lovefap.com/video/...                                                                                                                     |
 | NSFW.XXX                | Profile: nsfw.xxx/user/... <br> Post: nsfw.xxx/post/...                                                                                                                                                                                |
 | PimpAndHost             | Albums: pimpandhost.com/album/... <br> Single Files: pimpandhost.com/image/...                                                                                                                                                         |
 | PixelDrain              | Albums: Pixeldrain.com/l/... <br> Single Files: Pixeldrain.com/u/...                                                                                                                                                                   |
 | Pixl                    | Albums: pixl.li/album/... <br> Direct Images: pixl.li/image/...  <br> User Profile: pixl.li/#USER# <br> All User Albums: pixl.li/#USER#/albums                                                                                         |
 | Postimg.cc              | Albums: postimg.cc/gallery/... <br> Direct Images: postimg.cc/...                                                                                                                                                                      |
+| NudoStar                | Thread: nudostar.com/forum/threads/...  <br> Continue from (will download this post and after): nudostar.com/forum/threads/...post-NUMBER                                                                                              |
 | SimpCity                | Thread: simpcity.st/threads/...  <br> Continue from (will download this post and after): simpcity.st/threads/...post-NUMBER                                                                                                            |
 | SocialMediaGirls        | Thread: forum.socialmediagirls.com/threads/...  <br> Continue from (will download this post and after): forum.socialmediagirls.com/threads/...post-NUMBER                                                                              |
 | XBunker                 | Thread: xbunker.nu/threads/...  <br> Continue from (will download this post and after): xbunker.nu/threads/...post-NUMBER                                                                                                              |
 | XBunkr                  | Album: xbunkr.com/a/... <br> Direct Links: media.xbunkr.com/...                                                                                                                                                                        |
 
 Reminder to leave the link full (include the https://)
 
@@ -168,14 +169,16 @@
 --throttle              this is a throttle between requests during the downloading phase, the number is in seconds
 
 --output-last-forum-post        outputs the last post of a forum scrape to use as a starting point for future runs
 --separate-posts                separates forum scraping into folders by post number
 
 --gofile-api-key                api key for premium gofile
 --pixeldrain-api-key            api key for premium pixeldrain
+--nudostar-username             username to login to nudostar
+--nudostar-password             password to login to nudostar
 --simpcity-username             username to login to simpcity
 --simpcity-password             password to login to simpcity
 --socialmediagirls-username     username to login to socialmediagirls
 --socialmediagirls-password     password to login to socialmediagirls
 --xbunker-username              username to login to xbunker
 --xbunker-password              password to login to xbunker
 
@@ -190,8 +193,8 @@
 --hide-thread-progress          removes thread progress section while downloading
 --hide-domain-progress          removes domain progress section while downloading
 --hide-album-progress           removes album progress section while downloading
 --hide-file-progress            removes file progress section while downloading
 --refresh-rate                  changes the refresh rate of the progress table
 ```
 
-`--only-hosts` and `--skip-hosts` can use: `"anonfiles", "bayfiles", "bunkr", "coomer.party", "cyberdrop", "cyberfile", "e-hentai", "erome", "fapello", "gfycat", "gallery.deltaporno.com", "gofile", "hgamecg", "img.kiwi", "imgbox", "jpg.church", "jpg.fish", "kemono.party", "lovefap", "nsfw.xxx", "pimpandhost", "pixeldrain", "pixl.li", "postimg", "saint", "simpcity", "socialmediagirls", "xbunker", "xbunkr"`
+`--only-hosts` and `--skip-hosts` can use: `"anonfiles", "bayfiles", "bunkr", "coomer.party", "cyberdrop", "cyberfile", "e-hentai", "erome", "fapello", "gfycat", "gallery.deltaporno.com", "gofile", "hgamecg", "img.kiwi", "imgbox", "jpg.church", "jpg.fish", "kemono.party", "lovefap", "nsfw.xxx", "nudostar", "pimpandhost", "pixeldrain", "pixl.li", "postimg", "saint", "simpcity", "socialmediagirls", "xbunker", "xbunkr"`
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.1.16 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.1.17 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
@@ -70,15 +70,18 @@
 Single Files: pimpandhost.com/image/... | | PixelDrain | Albums:
 Pixeldrain.com/l/...
 Single Files: Pixeldrain.com/u/... | | Pixl | Albums: pixl.li/album/...
 Direct Images: pixl.li/image/...
 User Profile: pixl.li/#USER#
 All User Albums: pixl.li/#USER#/albums | | Postimg.cc | Albums: postimg.cc/
 gallery/...
-Direct Images: postimg.cc/... | | SimpCity | Thread: simpcity.st/threads/...
+Direct Images: postimg.cc/... | | NudoStar | Thread: nudostar.com/forum/
+threads/...
+Continue from (will download this post and after): nudostar.com/forum/
+threads/...post-NUMBER | | SimpCity | Thread: simpcity.st/threads/...
 Continue from (will download this post and after): simpcity.st/threads/...post-
 NUMBER | | SocialMediaGirls | Thread: forum.socialmediagirls.com/threads/...
 Continue from (will download this post and after): forum.socialmediagirls.com/
 threads/...post-NUMBER | | XBunker | Thread: xbunker.nu/threads/...
 Continue from (will download this post and after): xbunker.nu/threads/...post-
 NUMBER | | XBunkr | Album: xbunkr.com/a/...
 Direct Links: media.xbunkr.com/... | Reminder to leave the link full (include
@@ -141,29 +144,31 @@
 wait attempting to connect to a URL during the downloading phase --ratelimit
 this applies to requests made in the program during scraping, the number you
 provide is in requests/seconds --throttle this is a throttle between requests
 during the downloading phase, the number is in seconds --output-last-forum-post
 outputs the last post of a forum scrape to use as a starting point for future
 runs --separate-posts separates forum scraping into folders by post number --
 gofile-api-key api key for premium gofile --pixeldrain-api-key api key for
-premium pixeldrain --simpcity-username username to login to simpcity --
-simpcity-password password to login to simpcity --socialmediagirls-username
-username to login to socialmediagirls --socialmediagirls-password password to
-login to socialmediagirls --xbunker-username username to login to xbunker --
-xbunker-password password to login to xbunker --apply-jdownloader enables
-sending unsupported URLs to a running jdownloader2 instance to download --
-jdownloader-username username to login to jdownloader --jdownloader-password
-password to login to jdownloader --jdownloader-device device name to login to
-for jdownloader --hide-new-progress disables the new rich progress entirely and
-uses older methods --hide-overall-progress removes overall progress section
-while downloading --hide-forum-progress removes forum progress section while
-downloading --hide-thread-progress removes thread progress section while
-downloading --hide-domain-progress removes domain progress section while
-downloading --hide-album-progress removes album progress section while
-downloading --hide-file-progress removes file progress section while
-downloading --refresh-rate changes the refresh rate of the progress table ```
-`--only-hosts` and `--skip-hosts` can use: `"anonfiles", "bayfiles", "bunkr",
-"coomer.party", "cyberdrop", "cyberfile", "e-hentai", "erome", "fapello",
-"gfycat", "gallery.deltaporno.com", "gofile", "hgamecg", "img.kiwi", "imgbox",
-"jpg.church", "jpg.fish", "kemono.party", "lovefap", "nsfw.xxx", "pimpandhost",
-"pixeldrain", "pixl.li", "postimg", "saint", "simpcity", "socialmediagirls",
-"xbunker", "xbunkr"`
+premium pixeldrain --nudostar-username username to login to nudostar --
+nudostar-password password to login to nudostar --simpcity-username username to
+login to simpcity --simpcity-password password to login to simpcity --
+socialmediagirls-username username to login to socialmediagirls --
+socialmediagirls-password password to login to socialmediagirls --xbunker-
+username username to login to xbunker --xbunker-password password to login to
+xbunker --apply-jdownloader enables sending unsupported URLs to a running
+jdownloader2 instance to download --jdownloader-username username to login to
+jdownloader --jdownloader-password password to login to jdownloader --
+jdownloader-device device name to login to for jdownloader --hide-new-progress
+disables the new rich progress entirely and uses older methods --hide-overall-
+progress removes overall progress section while downloading --hide-forum-
+progress removes forum progress section while downloading --hide-thread-
+progress removes thread progress section while downloading --hide-domain-
+progress removes domain progress section while downloading --hide-album-
+progress removes album progress section while downloading --hide-file-progress
+removes file progress section while downloading --refresh-rate changes the
+refresh rate of the progress table ``` `--only-hosts` and `--skip-hosts` can
+use: `"anonfiles", "bayfiles", "bunkr", "coomer.party", "cyberdrop",
+"cyberfile", "e-hentai", "erome", "fapello", "gfycat",
+"gallery.deltaporno.com", "gofile", "hgamecg", "img.kiwi", "imgbox",
+"jpg.church", "jpg.fish", "kemono.party", "lovefap", "nsfw.xxx", "nudostar",
+"pimpandhost", "pixeldrain", "pixl.li", "postimg", "saint", "simpcity",
+"socialmediagirls", "xbunker", "xbunkr"`
```

### Comparing `cyberdrop-dl-4.1.16/README.md` & `cyberdrop-dl-4.1.17/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 | jpg.church<br/>jpg.fish | Albums: jpg.church/album/... <br> Direct Images: jpg.church/image/... <br> User Profile: jpg.church/#USER# <br> All User Albums: jpg.church/#USER#/albums                                                                              |
 | LoveFap                 | Albums: lovefap.com/a/... <br> Direct Images: s*.lovefap.com/content/photos/... <br> Videos: lovefap.com/video/...                                                                                                                     |
 | NSFW.XXX                | Profile: nsfw.xxx/user/... <br> Post: nsfw.xxx/post/...                                                                                                                                                                                |
 | PimpAndHost             | Albums: pimpandhost.com/album/... <br> Single Files: pimpandhost.com/image/...                                                                                                                                                         |
 | PixelDrain              | Albums: Pixeldrain.com/l/... <br> Single Files: Pixeldrain.com/u/...                                                                                                                                                                   |
 | Pixl                    | Albums: pixl.li/album/... <br> Direct Images: pixl.li/image/...  <br> User Profile: pixl.li/#USER# <br> All User Albums: pixl.li/#USER#/albums                                                                                         |
 | Postimg.cc              | Albums: postimg.cc/gallery/... <br> Direct Images: postimg.cc/...                                                                                                                                                                      |
+| NudoStar                | Thread: nudostar.com/forum/threads/...  <br> Continue from (will download this post and after): nudostar.com/forum/threads/...post-NUMBER                                                                                              |
 | SimpCity                | Thread: simpcity.st/threads/...  <br> Continue from (will download this post and after): simpcity.st/threads/...post-NUMBER                                                                                                            |
 | SocialMediaGirls        | Thread: forum.socialmediagirls.com/threads/...  <br> Continue from (will download this post and after): forum.socialmediagirls.com/threads/...post-NUMBER                                                                              |
 | XBunker                 | Thread: xbunker.nu/threads/...  <br> Continue from (will download this post and after): xbunker.nu/threads/...post-NUMBER                                                                                                              |
 | XBunkr                  | Album: xbunkr.com/a/... <br> Direct Links: media.xbunkr.com/...                                                                                                                                                                        |
 
 Reminder to leave the link full (include the https://)
 
@@ -156,14 +157,16 @@
 --throttle              this is a throttle between requests during the downloading phase, the number is in seconds
 
 --output-last-forum-post        outputs the last post of a forum scrape to use as a starting point for future runs
 --separate-posts                separates forum scraping into folders by post number
 
 --gofile-api-key                api key for premium gofile
 --pixeldrain-api-key            api key for premium pixeldrain
+--nudostar-username             username to login to nudostar
+--nudostar-password             password to login to nudostar
 --simpcity-username             username to login to simpcity
 --simpcity-password             password to login to simpcity
 --socialmediagirls-username     username to login to socialmediagirls
 --socialmediagirls-password     password to login to socialmediagirls
 --xbunker-username              username to login to xbunker
 --xbunker-password              password to login to xbunker
 
@@ -178,8 +181,8 @@
 --hide-thread-progress          removes thread progress section while downloading
 --hide-domain-progress          removes domain progress section while downloading
 --hide-album-progress           removes album progress section while downloading
 --hide-file-progress            removes file progress section while downloading
 --refresh-rate                  changes the refresh rate of the progress table
 ```
 
-`--only-hosts` and `--skip-hosts` can use: `"anonfiles", "bayfiles", "bunkr", "coomer.party", "cyberdrop", "cyberfile", "e-hentai", "erome", "fapello", "gfycat", "gallery.deltaporno.com", "gofile", "hgamecg", "img.kiwi", "imgbox", "jpg.church", "jpg.fish", "kemono.party", "lovefap", "nsfw.xxx", "pimpandhost", "pixeldrain", "pixl.li", "postimg", "saint", "simpcity", "socialmediagirls", "xbunker", "xbunkr"`
+`--only-hosts` and `--skip-hosts` can use: `"anonfiles", "bayfiles", "bunkr", "coomer.party", "cyberdrop", "cyberfile", "e-hentai", "erome", "fapello", "gfycat", "gallery.deltaporno.com", "gofile", "hgamecg", "img.kiwi", "imgbox", "jpg.church", "jpg.fish", "kemono.party", "lovefap", "nsfw.xxx", "nudostar", "pimpandhost", "pixeldrain", "pixl.li", "postimg", "saint", "simpcity", "socialmediagirls", "xbunker", "xbunkr"`
```

#### html2text {}

```diff
@@ -64,15 +64,18 @@
 Single Files: pimpandhost.com/image/... | | PixelDrain | Albums:
 Pixeldrain.com/l/...
 Single Files: Pixeldrain.com/u/... | | Pixl | Albums: pixl.li/album/...
 Direct Images: pixl.li/image/...
 User Profile: pixl.li/#USER#
 All User Albums: pixl.li/#USER#/albums | | Postimg.cc | Albums: postimg.cc/
 gallery/...
-Direct Images: postimg.cc/... | | SimpCity | Thread: simpcity.st/threads/...
+Direct Images: postimg.cc/... | | NudoStar | Thread: nudostar.com/forum/
+threads/...
+Continue from (will download this post and after): nudostar.com/forum/
+threads/...post-NUMBER | | SimpCity | Thread: simpcity.st/threads/...
 Continue from (will download this post and after): simpcity.st/threads/...post-
 NUMBER | | SocialMediaGirls | Thread: forum.socialmediagirls.com/threads/...
 Continue from (will download this post and after): forum.socialmediagirls.com/
 threads/...post-NUMBER | | XBunker | Thread: xbunker.nu/threads/...
 Continue from (will download this post and after): xbunker.nu/threads/...post-
 NUMBER | | XBunkr | Album: xbunkr.com/a/...
 Direct Links: media.xbunkr.com/... | Reminder to leave the link full (include
@@ -135,29 +138,31 @@
 wait attempting to connect to a URL during the downloading phase --ratelimit
 this applies to requests made in the program during scraping, the number you
 provide is in requests/seconds --throttle this is a throttle between requests
 during the downloading phase, the number is in seconds --output-last-forum-post
 outputs the last post of a forum scrape to use as a starting point for future
 runs --separate-posts separates forum scraping into folders by post number --
 gofile-api-key api key for premium gofile --pixeldrain-api-key api key for
-premium pixeldrain --simpcity-username username to login to simpcity --
-simpcity-password password to login to simpcity --socialmediagirls-username
-username to login to socialmediagirls --socialmediagirls-password password to
-login to socialmediagirls --xbunker-username username to login to xbunker --
-xbunker-password password to login to xbunker --apply-jdownloader enables
-sending unsupported URLs to a running jdownloader2 instance to download --
-jdownloader-username username to login to jdownloader --jdownloader-password
-password to login to jdownloader --jdownloader-device device name to login to
-for jdownloader --hide-new-progress disables the new rich progress entirely and
-uses older methods --hide-overall-progress removes overall progress section
-while downloading --hide-forum-progress removes forum progress section while
-downloading --hide-thread-progress removes thread progress section while
-downloading --hide-domain-progress removes domain progress section while
-downloading --hide-album-progress removes album progress section while
-downloading --hide-file-progress removes file progress section while
-downloading --refresh-rate changes the refresh rate of the progress table ```
-`--only-hosts` and `--skip-hosts` can use: `"anonfiles", "bayfiles", "bunkr",
-"coomer.party", "cyberdrop", "cyberfile", "e-hentai", "erome", "fapello",
-"gfycat", "gallery.deltaporno.com", "gofile", "hgamecg", "img.kiwi", "imgbox",
-"jpg.church", "jpg.fish", "kemono.party", "lovefap", "nsfw.xxx", "pimpandhost",
-"pixeldrain", "pixl.li", "postimg", "saint", "simpcity", "socialmediagirls",
-"xbunker", "xbunkr"`
+premium pixeldrain --nudostar-username username to login to nudostar --
+nudostar-password password to login to nudostar --simpcity-username username to
+login to simpcity --simpcity-password password to login to simpcity --
+socialmediagirls-username username to login to socialmediagirls --
+socialmediagirls-password password to login to socialmediagirls --xbunker-
+username username to login to xbunker --xbunker-password password to login to
+xbunker --apply-jdownloader enables sending unsupported URLs to a running
+jdownloader2 instance to download --jdownloader-username username to login to
+jdownloader --jdownloader-password password to login to jdownloader --
+jdownloader-device device name to login to for jdownloader --hide-new-progress
+disables the new rich progress entirely and uses older methods --hide-overall-
+progress removes overall progress section while downloading --hide-forum-
+progress removes forum progress section while downloading --hide-thread-
+progress removes thread progress section while downloading --hide-domain-
+progress removes domain progress section while downloading --hide-album-
+progress removes album progress section while downloading --hide-file-progress
+removes file progress section while downloading --refresh-rate changes the
+refresh rate of the progress table ``` `--only-hosts` and `--skip-hosts` can
+use: `"anonfiles", "bayfiles", "bunkr", "coomer.party", "cyberdrop",
+"cyberfile", "e-hentai", "erome", "fapello", "gfycat",
+"gallery.deltaporno.com", "gofile", "hgamecg", "img.kiwi", "imgbox",
+"jpg.church", "jpg.fish", "kemono.party", "lovefap", "nsfw.xxx", "nudostar",
+"pimpandhost", "pixeldrain", "pixl.li", "postimg", "saint", "simpcity",
+"socialmediagirls", "xbunker", "xbunkr"`
```

### Comparing `cyberdrop-dl-4.1.16/cyberdrop_dl/base_functions/base_functions.py` & `cyberdrop-dl-4.1.17/cyberdrop_dl/base_functions/base_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
 
 async def clear() -> None:
     """Clears the terminal screen"""
     os.system('cls' if os.name == 'nt' else 'clear')
 
 
-async def log(text: str, quiet: bool = False, style: str = "") -> None:
+def log(text: str, quiet: bool = False, style: str = "") -> None:
     """Logs to the output log file and optionally (by default) prints to the terminal with given style"""
     logger.debug(text)
     if not quiet:
         if style:
             text = f"[{style}]{text}[/{style}]"
         rich.print(text)
 
@@ -84,23 +84,23 @@
     title = title.replace("\t", "").strip()
     title = re.sub(' +', ' ', title)
     title = re.sub(r'[\\*?:"<>|./]', "-", title)
     title = title[:60].strip()
     return title
 
 
-async def check_direct(url: URL):
+async def check_direct(url: URL) -> bool:
     """Checks whether the given url is a direct link to a content item"""
     mapping_direct = [r'i.pixl.li', r'i..pixl.li', r'img-...cyberdrop...', r'f.cyberdrop...',
                       r'fs-...cyberdrop...', r'jpg.church/images/...', r'simp..jpg.church', r's..putmega.com',
                       r's..putme.ga', r'images..imgbox.com', r's..lovefap...', r'img.kiwi/images/']
     return any(re.search(domain, str(url)) for domain in mapping_direct)
 
 
-async def get_filename_and_ext(filename, forum=False):
+async def get_filename_and_ext(filename: str, forum: bool = False) -> tuple[str, str]:
     """Returns the filename and extension of a given file, throws NoExtensionFailure if there is no extension"""
     filename_parts = filename.rsplit('.', 1)
     if len(filename_parts) == 1:
         raise NoExtensionFailure()
     if filename_parts[-1].isnumeric() and forum:
         filename_parts = filename_parts[0].rsplit('-', 1)
     ext = "." + filename_parts[-1].lower()
```

### Comparing `cyberdrop-dl-4.1.16/cyberdrop_dl/base_functions/config_manager.py` & `cyberdrop-dl-4.1.17/cyberdrop_dl/base_functions/config_manager.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from __future__ import annotations
 
 import copy
 from pathlib import Path
+from typing import Optional
 
 import yaml
 
 from cyberdrop_dl.base_functions.base_functions import log
 from cyberdrop_dl.base_functions.config_schema import config_default
 
 
 def _to_config_value(value):
     return str(value) if isinstance(value, Path) else value
 
 
-def _create_config(config: Path, passed_args: dict = None, enabled=False) -> dict:
+def _create_config(config: Path, passed_args: Optional[dict] = None, enabled=False) -> dict:
     """Creates the default config file, or remakes it with passed arguments"""
-    config_data = config_default
+    config_data: dict = config_default
     if passed_args:
         config_data["Apply_Config"] = enabled
         for group in config_data["Configuration"].values():
             for arg in group:
                 if arg in passed_args:
                     group[arg] = _to_config_value(passed_args[arg])
 
@@ -33,15 +34,15 @@
     """Validates the existing config file"""
     with open(config, "r") as yamlfile:
         config_data = yaml.load(yamlfile, Loader=yaml.FullLoader)
     try:
         data = config_data["Configuration"]
         enabled = config_data["Apply_Config"]
 
-        config_groups = config_default["Configuration"]
+        config_groups: dict = config_default["Configuration"]
         if all(set(group) <= set(data[group_name]) for group_name, group in config_groups.items()):
             return config_data
 
         config.unlink()
 
         args = {}
         for group_name in config_groups:
@@ -61,34 +62,34 @@
     if data['Apply_Config']:
         data = data["Configuration"]
         for file, path in data['Files'].items():
             data['Files'][file] = Path(path)
         data['Sorting']['sort_directory'] = Path(data['Sorting']['sort_directory'])
         return data
 
-    config_data = config_default["Configuration"]
+    config_data: dict = config_default["Configuration"]
     for group in config_data.values():
         for arg in group:
             if arg in cmd_arg:
                 group[arg] = cmd_arg[arg]
     return config_data
 
 
-async def document_args(args: dict):
+async def document_args(args: dict) -> None:
     """We document the runtime arguments for debugging and troubleshooting, redacting sensitive information"""
     print_args = copy.deepcopy(args)
     print_args['Authentication']['xbunker_password'] = '!REDACTED!' if args['Authentication']['xbunker_password'] is not None else None
     print_args['Authentication']['socialmediagirls_password'] = '!REDACTED!' if args['Authentication']['socialmediagirls_password'] is not None else None
     print_args['Authentication']['simpcity_password'] = '!REDACTED!' if args['Authentication']['simpcity_password'] is not None else None
     print_args['Authentication']['pixeldrain_api_key'] = '!REDACTED!' if args['Authentication']['pixeldrain_api_key'] is not None else None
     print_args['JDownloader']['jdownloader_password'] = '!REDACTED!' if args['JDownloader']['jdownloader_password'] is not None else None
 
-    await log("Starting Cyberdrop-DL")
-    await log(f"Using authentication arguments: {print_args['Authentication']}", quiet=True)
-    await log(f"Using file arguments: {print_args['Files']}", quiet=True)
-    await log(f"Using forum option arguments: {print_args['Forum_Options']}", quiet=True)
-    await log(f"Using ignore arguments: {print_args['Ignore']}", quiet=True)
-    await log(f"Using jdownloader arguments: {print_args['JDownloader']}", quiet=True)
-    await log(f"Using progress option arguments: {print_args['Progress_Options']}", quiet=True)
-    await log(f"Using ratelimiting arguments: {print_args['Ratelimiting']}", quiet=True)
-    await log(f"Using runtime arguments: {print_args['Runtime']}", quiet=True)
-    await log(f"Using sorting arguments: {print_args['Sorting']}", quiet=True)
+    log("Starting Cyberdrop-DL")
+    log(f"Using authentication arguments: {print_args['Authentication']}", quiet=True)
+    log(f"Using file arguments: {print_args['Files']}", quiet=True)
+    log(f"Using forum option arguments: {print_args['Forum_Options']}", quiet=True)
+    log(f"Using ignore arguments: {print_args['Ignore']}", quiet=True)
+    log(f"Using jdownloader arguments: {print_args['JDownloader']}", quiet=True)
+    log(f"Using progress option arguments: {print_args['Progress_Options']}", quiet=True)
+    log(f"Using ratelimiting arguments: {print_args['Ratelimiting']}", quiet=True)
+    log(f"Using runtime arguments: {print_args['Runtime']}", quiet=True)
+    log(f"Using sorting arguments: {print_args['Sorting']}", quiet=True)
```

### Comparing `cyberdrop-dl-4.1.16/cyberdrop_dl/base_functions/config_schema.py` & `cyberdrop-dl-4.1.17/cyberdrop_dl/base_functions/config_schema.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-config_default = {
+from __future__ import annotations
+
+config_default: dict = {
     "Apply_Config": False,
     "Configuration": {
         "Authentication": {
             "gofile_api_key": "",
             "pixeldrain_api_key": "",
             "nudostar_username": "",
             "nudostar_password": "",
```

### Comparing `cyberdrop-dl-4.1.16/cyberdrop_dl/base_functions/data_classes.py` & `cyberdrop-dl-4.1.17/cyberdrop_dl/base_functions/data_classes.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,160 +1,158 @@
 from __future__ import annotations
 
 import asyncio
-from dataclasses import dataclass
-from typing import TYPE_CHECKING, ClassVar, List, Tuple
+from dataclasses import dataclass, field
+from typing import TYPE_CHECKING, ClassVar
 
 if TYPE_CHECKING:
     from yarl import URL
 
 
 @dataclass
 class MediaItem:
     url: URL
     referer: URL
     complete: bool
     filename: str
     ext: str
     original_filename: str
 
-    async def is_complete(self):
+    async def is_complete(self) -> bool:
         return self.complete
 
-    async def mark_completed(self):
+    async def mark_completed(self) -> None:
         self.complete = True
 
 
 @dataclass
 class AlbumItem:
     """Class for keeping track of download links for each album"""
     title: str
-    media: List[MediaItem]
+    media: list[MediaItem]
 
-    async def add_media(self, media_item: MediaItem):
+    async def add_media(self, media_item: MediaItem) -> None:
         self.media.append(media_item)
 
-    async def set_new_title(self, new_title: str):
+    async def set_new_title(self, new_title: str) -> None:
         self.title = new_title
 
-    async def append_title(self, title):
+    async def append_title(self, title) -> None:
         new_title = title + '/' + self.title
         self.title = new_title
 
-    async def extend(self, album):
+    async def extend(self, album) -> None:
         self.media.extend(album.media)
 
-    async def is_empty(self):
-        if not self.media:
-            return True
-        return False
+    async def is_empty(self) -> bool:
+        return True if not self.media else False
 
 
 @dataclass
 class DomainItem:
     """Class for keeping track of albums for each scraper type"""
     domain: str
     albums: dict
 
-    async def add_to_album(self, title: str, media: MediaItem):
+    async def add_to_album(self, title: str, media: MediaItem) -> None:
         if title in self.albums:
             await self.albums[title].add_media(media)
         else:
             self.albums[title] = AlbumItem(title=title, media=[media])
 
-    async def add_media(self, title: str, media: MediaItem):
+    async def add_media(self, title: str, media: MediaItem) -> None:
         if title in self.albums:
             album = self.albums[title]
             await album.add_media(media)
         else:
             self.albums[title] = AlbumItem(title, [media])
 
-    async def add_album(self, title: str, album: AlbumItem):
+    async def add_album(self, title: str, album: AlbumItem) -> None:
         if title in self.albums:
             stored_album = self.albums[title]
             for media_item in album.media:
                 if media_item in stored_album.media:
                     continue
                 await stored_album.add_media(media_item)
         else:
             self.albums[title] = album
 
-    async def set_new_domain(self, domain: str):
+    async def set_new_domain(self, domain: str) -> None:
         self.domain = domain
 
-    async def extend(self, domain):
+    async def extend(self, domain) -> None:
         for title, album in domain.albums.items():
             await self.add_album(title, album)
 
-    async def append_title(self, title):
+    async def append_title(self, title) -> None:
         if not title:
             return
         new_albums = {}
         for album_str, album in self.albums.items():
-            new_title = title+'/'+album_str
+            new_title = title + '/' + album_str
             new_albums[new_title] = album
             album.title = new_title
         self.albums = new_albums
 
 
 @dataclass
 class CascadeItem:
     """Class for keeping track of domains for each scraper type"""
     domains: dict
 
-    async def add_albums(self, domain_item: DomainItem):
+    async def add_albums(self, domain_item: DomainItem) -> None:
         domain = domain_item.domain
         albums = domain_item.albums
         for title, album in albums.items():
             await self.add_album(domain, title, album)
 
-    async def add_to_album(self, domain: str, title: str, media_item: MediaItem):
+    async def add_to_album(self, domain: str, title: str, media_item: MediaItem) -> None:
         if domain in self.domains:
             await self.domains[domain].add_to_album(title, media_item)
         else:
             self.domains[domain] = DomainItem(domain, {title: AlbumItem(title, [media_item])})
 
-    async def add_album(self, domain: str, title: str, album: AlbumItem):
+    async def add_album(self, domain: str, title: str, album: AlbumItem) -> None:
         if domain in self.domains:
             await self.domains[domain].add_album(title, album)
         else:
             self.domains[domain] = DomainItem(domain, {title: album})
 
-    async def is_empty(self):
+    async def is_empty(self) -> bool:
         for domain in self.domains.values():
             for album in domain.albums.values():
                 if album.media:
                     return False
         return True
 
-    async def get_total(self):
+    async def get_total(self) -> int:
         total = 0
         for domain in self.domains.values():
             for album in domain.albums.values():
                 total += len(album.media)
         return total
 
-    async def append_title(self, title: str):
+    async def append_title(self, title: str) -> None:
         if not title:
             return
         for domain in self.domains.values():
             new_albums = {}
             for album_str, album in domain.albums.items():
-                new_title = title+'/'+album_str
+                new_title = title + '/' + album_str
                 new_albums[new_title] = album
                 album.title = new_title
             domain.albums = new_albums
 
-    async def extend(self, Cascade):
+    async def extend(self, Cascade) -> None:
         if Cascade and Cascade.domains:
             for domain_str, domain in Cascade.domains.items():
                 for album_str, album in domain.albums.items():
                     await self.add_album(domain_str, album_str, album)
 
-    async def dedupe(self):
+    async def dedupe(self) -> None:
         for domain in self.domains.values():
             for album in domain.albums.values():
                 check = []
                 allowed = []
                 for media_item in album.media:
                     if media_item.url in check:
                         continue
@@ -164,80 +162,82 @@
 
 
 @dataclass
 class ForumItem:
     """Class for keeping track of forum threads"""
     threads: dict
 
-    async def add_album_to_thread(self, title: str, domain: str, album: AlbumItem):
+    async def add_album_to_thread(self, title: str, domain: str, album: AlbumItem) -> None:
         if title not in self.threads:
             self.threads[title] = CascadeItem({domain: DomainItem(domain, {album.title: album})})
         else:
             await self.threads[title].add_album(domain, album.title, album)
 
-    async def add_thread(self, title: str, cascade: CascadeItem):
+    async def add_thread(self, title: str, cascade: CascadeItem) -> None:
         if title not in self.threads:
             self.threads[title] = cascade
         else:
             await self.threads[title].extend(cascade)
 
-    async def is_empty(self):
+    async def is_empty(self) -> bool:
         for Cascade in self.threads.values():
             for domain in Cascade.domains.values():
                 for album in domain.albums.values():
                     if album.media:
                         return False
         return True
 
-    async def get_total(self):
+    async def get_total(self) -> int:
         total = 0
         for Cascade in self.threads.values():
             for domain in Cascade.domains.values():
                 for album in domain.albums.values():
                     total += len(album.media)
         return total
 
-    async def dedupe(self):
+    async def dedupe(self) -> None:
         for Cascade in self.threads.values():
             for domain in Cascade.domains.values():
                 for album in domain.albums.values():
                     check = []
                     allowed = []
                     for media_item in album.media:
                         if media_item.url in check:
                             continue
                         check.append(media_item.url)
                         allowed.append(media_item)
                     album.media = allowed
 
-    async def extend_thread(self, title: str, cascade: CascadeItem):
+    async def extend_thread(self, title: str, cascade: CascadeItem) -> None:
         if title in self.threads:
             await self.threads[title].extend(cascade)
         else:
             self.threads[title] = cascade
 
+
 @dataclass
 class FileLock:
     """Rudimentary file lock system"""
-    locked_files = []
+    locked_files: list[str] = field(default_factory=list)
 
-    async def check_lock(self, filename):
+    async def check_lock(self, filename: str) -> bool:
         await asyncio.sleep(.1)
         return filename.lower() in self.locked_files
 
-    async def add_lock(self, filename):
+    async def add_lock(self, filename: str) -> None:
         self.locked_files.append(filename.lower())
 
-    async def remove_lock(self, filename):
+    async def remove_lock(self, filename: str) -> None:
         self.locked_files.remove(filename.lower())
 
 
 @dataclass
 class SkipData:
     """The allows optoins for domains to skip when scraping"""
-    supported_hosts: ClassVar[Tuple[str]] = ("anonfiles", "bayfiles", "bunkr", "coomer.party", "cyberdrop",
-                                             "cyberfile", "e-hentai", "erome", "fapello", "gfycat", "gofile",
-                                             "hgamecg", "img.kiwi", "imgbox", "jpg.church", "jpg.fish",
-                                             "gallery.deltaporno.com", "kemono.party",
-                                             "lovefap", "nsfw.xxx", "pimpandhost", "pixeldrain", "pixl.li", "postimg",
-                                             "saint", "nudostar", "simpcity", "socialmediagirls", "xbunker", "xbunkr")
-    sites: List[str]
+    supported_hosts: ClassVar[tuple[str, ...]] = ("anonfiles", "bayfiles", "bunkr", "coomer.party", "cyberdrop",
+                                                  "cyberfile", "e-hentai", "erome", "fapello", "gfycat", "gofile",
+                                                  "hgamecg", "img.kiwi", "imgbox", "jpg.church", "jpg.fish",
+                                                  "gallery.deltaporno.com", "kemono.party",
+                                                  "lovefap", "nsfw.xxx", "pimpandhost", "pixeldrain", "pixl.li",
+                                                  "postimg", "saint", "nudostar", "simpcity", "socialmediagirls",
+                                                  "xbunker", "xbunkr")
+    sites: list[str]
```

### Comparing `cyberdrop-dl-4.1.16/cyberdrop_dl/base_functions/error_classes.py` & `cyberdrop-dl-4.1.17/cyberdrop_dl/base_functions/error_classes.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 class JDownloaderFailure(Exception):
     """Basic failure template for JDownloader"""
-    def __init__(self, message="Something went wrong"):
+    def __init__(self, message: str = "Something went wrong"):
         self.message = message
         super().__init__(self.message)
 
 
 class NoExtensionFailure(Exception):
     """This error will be thrown when no extension is given for a file"""
-    def __init__(self, *, message="Extension missing for file"):
+    def __init__(self, *, message: str = "Extension missing for file"):
         self.message = message
         super().__init__(self.message)
 
 
 class FailedLoginFailure(Exception):
     """This error will be thrown when the login fails for a site"""
-    def __init__(self, *, message="Failed login."):
+    def __init__(self, *, message: str = "Failed login."):
         self.message = message
         super().__init__(self.message)
 
 
 class InvalidContentTypeFailure(Exception):
-    def __init__(self, *, message="Failed login."):
+    def __init__(self, *, message: str = "Failed login."):
         self.message = message
         super().__init__(self.message)
 
+
 class DownloadFailure(Exception):
     """This error will be thrown when a download fails"""
-    def __init__(self, code, message="Something went wrong"):
+    def __init__(self, code: int, message: str = "Something went wrong"):
         self.code = code
         self.message = message
         super().__init__(self.message)
         super().__init__(self.code)
```

### Comparing `cyberdrop-dl-4.1.16/cyberdrop_dl/base_functions/sorting_functions.py` & `cyberdrop-dl-4.1.17/cyberdrop_dl/base_functions/sorting_functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,24 +12,24 @@
         self.sorted_downloads = sorted_downloads
 
         self.audio_dir = audio_dir
         self.image_dir = image_dir
         self.video_dir = video_dir
         self.other_dir = other_dir
 
-    async def find_files_in_dir(self, directory: Path):
+    async def find_files_in_dir(self, directory: Path) -> list:
         file_list = []
         for x in directory.iterdir():
             if x.is_file():
                 file_list.append(x)
             elif x.is_dir():
                 file_list.extend(await self.find_files_in_dir(x))
         return file_list
 
-    async def sort(self):
+    async def sort(self) -> None:
         audio_count = 0
         image_count = 0
         video_count = 0
         other_count = 0
 
         for folder in self.download_dir.iterdir():
             if not folder.is_dir():
@@ -59,20 +59,21 @@
                     video_count += 1
                 else:
                     other_destination.mkdir(parents=True, exist_ok=True)
                     await self.move_cd(file, other_destination)
                     other_count += 1
         await asyncio.sleep(5)
         await purge_dir(self.download_dir)
-        await log(f"Organized: {audio_count} Audio Files", style="green")
-        await log(f"Organized: {image_count} Image Files", style="green")
-        await log(f"Organized: {video_count} Video Files", style="green")
-        await log(f"Organized: {other_count} Other Files", style="green")
 
-    async def move_cd(self, file: Path, dest: Path):
+        log(f"Organized: {audio_count} Audio Files", style="green")
+        log(f"Organized: {image_count} Image Files", style="green")
+        log(f"Organized: {video_count} Video Files", style="green")
+        log(f"Organized: {other_count} Other Files", style="green")
+
+    async def move_cd(self, file: Path, dest: Path) -> None:
         try:
             dest_file = dest / file.name
             file.rename(dest_file)
         except FileExistsError:
             if file.stat().st_size == dest_file.stat().st_size:
                 file.unlink()
                 return
```

### Comparing `cyberdrop-dl-4.1.16/cyberdrop_dl/base_functions/sql_helper.py` & `cyberdrop-dl-4.1.17/cyberdrop_dl/base_functions/sql_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from __future__ import annotations
 
 import atexit
 import logging
 import sqlite3
-from typing import TYPE_CHECKING, List, Optional
+from typing import TYPE_CHECKING, Optional
 
 if TYPE_CHECKING:
     from pathlib import Path
 
     from yarl import URL
 
     from cyberdrop_dl.base_functions.data_classes import (
         AlbumItem,
         CascadeItem,
         DomainItem,
         MediaItem,
     )
 
 
-async def get_db_path(url: URL, referer: str = None) -> str:
+async def get_db_path(url: URL, referer: str = "") -> str:
     """Gets the URL path to be put into the DB and checked from the DB"""
     url_path = url.path
 
     if url.host and ('anonfiles' in url.host or 'bayfiles' in url.host):
         url_parts = url_path.split('/')
         url_parts.pop(0)
         if len(url_parts) > 1:
@@ -37,28 +37,24 @@
 
 class SQLHelper:
     """This class is responsible for handling SQL operations"""
     def __init__(self, ignore_history: bool, ignore_cache: bool, download_history: str):
         self.ignore_history = ignore_history
         self.ignore_cache = ignore_cache
         self.download_history = download_history
-        self.conn = None
-        self.curs = None
+        self.conn = sqlite3.connect(self.download_history)
+        self.curs = self.conn.cursor()
 
         self.old_history = False
         # Close the sql connection when the program exits
         atexit.register(self._exit_handler)
 
     async def sql_initialize(self) -> None:
         """Initializes the SQL connection, and makes sure necessary tables exist"""
-        self.conn = sqlite3.connect(self.download_history)
-        self.curs = self.conn.cursor()
-
         await self._check_old_history()
-
         await self._pre_allocate()
         await self._create_media_history()
         await self._create_coomeno_history()
 
     async def _check_old_history(self) -> None:
         """Checks whether V3 history exists"""
         try:
@@ -120,15 +116,15 @@
             self.curs.execute(pre_alloc2)
             self.conn.commit()
             self.curs.execute(drop_pre)
             self.conn.commit()
 
     """Temp Table Operations"""
 
-    async def get_temp_names(self) -> List[str]:
+    async def get_temp_names(self) -> list[str]:
         """Gets the list of temp filenames"""
         self.curs.execute("SELECT downloaded_filename FROM downloads_temp;")
         filenames = self.curs.fetchall()
         return list(sum(filenames, ()))
 
     async def sql_insert_temp(self, downloaded_filename: str) -> None:
         """Inserts a temp filename into the downloads_temp table"""
```

### Comparing `cyberdrop-dl-4.1.16/cyberdrop_dl/client/client.py` & `cyberdrop-dl-4.1.17/cyberdrop_dl/client/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import asyncio
 import json
 import logging
 import ssl
 import time
 from http import HTTPStatus
-from typing import TYPE_CHECKING, Callable
+from typing import TYPE_CHECKING, Callable, Optional, Coroutine, Any
 
 import aiofiles
 import aiohttp
 import certifi
 from bs4 import BeautifulSoup
 from tqdm import tqdm
 from yarl import URL
@@ -38,15 +38,15 @@
                 return await func(self, *args, **kwargs)
 
     return wrapper
 
 
 class Client:
     """Creates a 'client' that can be referenced by scraping or download sessions"""
-    def __init__(self, ratelimit: int, throttle: int, secure: bool, connect_timeout: int, user_agent: str):
+    def __init__(self, ratelimit: int, throttle: float, secure: bool, connect_timeout: int, user_agent: str):
         self.connect_timeout = connect_timeout
         self.ratelimit = ratelimit
         self.throttle = throttle
         self.simultaneous_session_limit = asyncio.Semaphore(50)
         self.user_agent = user_agent
         self.verify_ssl = secure
         self.ssl_context = ssl.create_default_context(cafile=certifi.where()) if secure else False
@@ -56,103 +56,109 @@
 class ScrapeSession:
     """AIOHTTP operations for scraping"""
     def __init__(self, client: Client) -> None:
         self.client = client
         self.rate_limiter = AsyncRateLimiter(self.client.ratelimit)
         self.headers = {"user-agent": client.user_agent}
         self.timeouts = aiohttp.ClientTimeout(total=5 * 60, connect=self.client.connect_timeout, sock_read=30)
-        self.client_session = aiohttp.ClientSession(headers=self.headers, raise_for_status=True, cookie_jar=self.client.cookies, timeout=self.timeouts)
+        self.client_session = aiohttp.ClientSession(headers=self.headers, raise_for_status=True,
+                                                    cookie_jar=self.client.cookies, timeout=self.timeouts)
 
     @scrape_limit
-    async def get_BS4(self, url: URL):
+    async def get_BS4(self, url: URL) -> BeautifulSoup:
         async with self.client_session.get(url, ssl=self.client.ssl_context) as response:
             content_type = response.headers.get('Content-Type')
+            assert content_type is not None
             if not any(s in content_type.lower() for s in ("html", "text")):
                 raise InvalidContentTypeFailure(message=f"Received {content_type}, was expecting text")
             text = await response.text()
             return BeautifulSoup(text, 'html.parser')
 
     @scrape_limit
-    async def get_BS4_and_url(self, url: URL):
+    async def get_BS4_and_url(self, url: URL) -> tuple[BeautifulSoup, URL]:
         async with self.client_session.get(url, ssl=self.client.ssl_context) as response:
             text = await response.text()
             soup = BeautifulSoup(text, 'html.parser')
             return soup, URL(response.url)
 
     @scrape_limit
-    async def get_json(self, url: URL, params: dict = None):
+    async def get_json(self, url: URL, params: Optional[dict] = None) -> dict:
         async with self.client_session.get(url, ssl=self.client.ssl_context, params=params) as response:
             return json.loads(await response.content.read())
 
     @scrape_limit
-    async def get_text(self, url: URL):
+    async def get_text(self, url: URL) -> str:
         async with self.client_session.get(url, ssl=self.client.ssl_context) as response:
             return await response.text()
 
     @scrape_limit
-    async def post(self, url: URL, data: dict):
+    async def post(self, url: URL, data: dict) -> dict:
         async with self.client_session.post(url, data=data, headers=self.headers, ssl=self.client.ssl_context) as response:
             return json.loads(await response.content.read())
 
     @scrape_limit
-    async def get_no_resp(self, url: URL, headers: dict):
+    async def get_no_resp(self, url: URL, headers: dict) -> None:
         async with self.client_session.get(url, headers=headers, ssl=self.client.ssl_context):
             pass
 
     @scrape_limit
-    async def post_data_no_resp(self, url: URL, data: dict):
+    async def post_data_no_resp(self, url: URL, data: dict) -> None:
         async with self.client_session.post(url, data=data, headers=self.headers, ssl=self.client.ssl_context):
             pass
 
-    async def exit_handler(self):
+    async def exit_handler(self) -> None:
         try:
             await self.client_session.close()
         except Exception:
             logging.debug("Failed to close session.")
 
 
 class DownloadSession:
     """AIOHTTP operations for downloading"""
     def __init__(self, client: Client):
         self.client = client
         self.headers = {"user-agent": client.user_agent}
         self.timeouts = aiohttp.ClientTimeout(total=5 * 60, connect=self.client.connect_timeout)
         self.client_session = aiohttp.ClientSession(headers=self.headers, raise_for_status=True, cookie_jar=self.client.cookies, timeout=self.timeouts)
-        self.throttle_times = {}
+        self.throttle_times: dict[str, float] = {}
 
         self.bunkr_maintenance = [URL("https://bnkr.b-cdn.net/maintenance-vid.mp4"), URL("https://bnkr.b-cdn.net/maintenance.mp4")]
 
-    async def _append_content(self, file: Path, content: aiohttp.StreamReader, update_progress: Callable[[int], None]):
+    async def _append_content(self, file: Path, content: aiohttp.StreamReader,
+                              update_progress: Callable[[int], Optional[bool]]) -> None:
         file.parent.mkdir(parents=True, exist_ok=True)
         async with aiofiles.open(file, mode='ab') as f:
             async for chunk, _ in content.iter_chunks():
                 await asyncio.sleep(0)
                 await f.write(chunk)
                 update_progress(len(chunk))
 
-    async def _download(self, media: MediaItem, current_throttle: int, proxy: str, headers: dict,
-                        save_content: Callable[[aiohttp.StreamReader, int], None]) -> None:
+    async def _download(self, media: MediaItem, current_throttle: float, proxy: str, headers: dict,
+                        save_content: Callable[[aiohttp.StreamReader, int], Coroutine[Any, Any, None]]) -> None:
         headers['Referer'] = str(media.referer)
         headers['user-agent'] = self.client.user_agent
+
+        assert media.url.host is not None
         await self._throttle(current_throttle, media.url.host)
+
         async with self.client_session.get(media.url, headers=headers, ssl=self.client.ssl_context,
                                            raise_for_status=True, proxy=proxy) as resp:
             content_type = resp.headers.get('Content-Type')
             if not content_type:
                 raise DownloadFailure(code=CustomHTTPStatus.IM_A_TEAPOT, message="No content-type in response header")
             if resp.url in self.bunkr_maintenance:
                 raise DownloadFailure(code=HTTPStatus.SERVICE_UNAVAILABLE, message="Bunkr under maintenance")
             if any(s in content_type.lower() for s in ('html', 'text')):
                 logger.debug("Server for %s is experiencing issues, you are being ratelimited, or cookies have expired", str(media.url))
                 raise DownloadFailure(code=CustomHTTPStatus.IM_A_TEAPOT, message="Unexpectedly got text as response")
 
             size = int(resp.headers.get('Content-Length', '0'))
             await save_content(resp.content, size)
 
-    async def _throttle(self, delay: int, host: str) -> None:
+    async def _throttle(self, delay: float, host: str) -> None:
         """Throttles requests to domains by a parameter amount of time"""
         if delay is None or delay == 0:
             return
 
         key = f'throttle:{host}'
         while True:
             now = time.time()
@@ -162,40 +168,42 @@
             if elapsed >= delay:
                 self.throttle_times[key] = now
                 return
 
             remaining = delay - elapsed + 0.1
             await asyncio.sleep(remaining)
 
-    async def download_file(self, media: MediaItem, file: Path, current_throttle: int, resume_point: int,
-                            proxy: str, headers: dict, file_task: TaskID):
+    async def download_file(self, media: MediaItem, file: Path, current_throttle: float, resume_point: int,
+                            proxy: str, headers: dict, file_task: TaskID) -> None:
 
-        async def save_content(content: aiohttp.StreamReader, size: int):
+        async def save_content(content: aiohttp.StreamReader, size: int) -> None:
             file_progress.update(file_task, total=size + resume_point)
             file_progress.advance(file_task, resume_point)
             await self._append_content(file, content, lambda chunk_len: file_progress.advance(file_task, chunk_len))
 
         await self._download(media, current_throttle, proxy, headers, save_content)
 
-    async def old_download_file(self, media: MediaItem, file: Path, current_throttle: int, resume_point: int,
+    async def old_download_file(self, media: MediaItem, file: Path, current_throttle: float, resume_point: int,
                                 proxy: str, headers: dict):
 
-        async def save_content(content: aiohttp.StreamReader, size: int):
+        async def save_content(content: aiohttp.StreamReader, size: int) -> None:
             task_description = await adjust(f"{media.url.host}: {media.filename}")
             with tqdm(total=size + resume_point, unit_scale=True, unit='B', leave=False,
                       initial=resume_point, desc=task_description) as progress:
                 await self._append_content(file, content, lambda chunk_len: progress.update(chunk_len))
 
         await self._download(media, current_throttle, proxy, headers, save_content)
 
-    async def get_filesize(self, url: URL, referer: str, current_throttle: int):
+    async def get_filesize(self, url: URL, referer: str, current_throttle: int) -> int:
         headers = {'Referer': referer, 'user-agent': self.client.user_agent}
+
+        assert url.host is not None
         await self._throttle(current_throttle, url.host)
         async with self.client_session.get(url, headers=headers, ssl=self.client.ssl_context,
                                            raise_for_status=True) as resp:
             return int(resp.headers.get('Content-Length', str(0)))
 
-    async def exit_handler(self):
+    async def exit_handler(self) -> None:
         try:
             await self.client_session.close()
         except Exception:
             logging.debug("Failed to close session.")
```

### Comparing `cyberdrop-dl-4.1.16/cyberdrop_dl/client/rate_limiting.py` & `cyberdrop-dl-4.1.17/cyberdrop_dl/client/rate_limiting.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/Anonfiles_Spider.py` & `cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/Anonfiles_Spider.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,20 +16,21 @@
     def __init__(self, quiet: bool, SQL_Helper: SQLHelper):
         self.quiet = quiet
         self.SQL_Helper = SQL_Helper
         self.api_link = URL("https://api.anonfiles.com/v2/file")
 
     async def fetch(self, session: ScrapeSession, url: URL) -> AlbumItem:
         """Scraper for Anonfiles"""
+        assert url.host is not None
         if 'cdn' in url.host:
             url = URL("https://anonfiles.com") / url.parts[1]
 
         album_obj = AlbumItem("Loose Anon Files", [])
 
-        await log(f"Starting: {str(url)}", quiet=self.quiet, style="green")
+        log(f"Starting: {str(url)}", quiet=self.quiet, style="green")
 
         try:
             json = await session.get_json(self.api_link/url.parts[1]/"info")
             if json['status']:
                 soup = await session.get_BS4(url)
 
                 link = soup.select_one("a[id=download-url]")
@@ -39,17 +40,17 @@
 
                 filename, ext = await get_filename_and_ext(".".join(json['data']['file']['metadata']['name'].rsplit("_", 1)))
                 media_item = MediaItem(link, url, complete, filename, ext, filename)
                 await album_obj.add_media(media_item)
                 if not complete:
                     await self.SQL_Helper.insert_media("anonfiles", "", media_item)
             else:
-                await log(f"Dead: {str(url)}", quiet=self.quiet, style="red")
+                log(f"Dead: {str(url)}", quiet=self.quiet, style="red")
 
         except Exception as e:
             logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            await log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
             logger.debug(e)
             return album_obj
 
-        await log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
+        log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
         return album_obj
```

### Comparing `cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/Bunkr_Spider.py` & `cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/Bunkr_Spider.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,32 +25,32 @@
         self.quiet = quiet
         self.SQL_Helper = SQL_Helper
         self.remove_bunkr_id = remove_bunkr_id
 
     async def fetch(self, session: ScrapeSession, url: URL) -> AlbumItem:
         """Scraper for Bunkr"""
         album_obj = AlbumItem("Loose Bunkr Files", [])
-        await log(f"Starting: {str(url)}", quiet=self.quiet, style="green")
+        log(f"Starting: {str(url)}", quiet=self.quiet, style="green")
 
         if "v" in url.parts or "d" in url.parts:
             media = await self.get_file(session, url)
             if not media.filename:
                 return album_obj
             await album_obj.add_media(media)
-            await log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
+            log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
             if not media.complete:
                 await self.SQL_Helper.insert_media("bunkr", "", media)
             return album_obj
 
         if "a" in url.parts:
             album_obj = await self.get_album(session, url)
             await self.SQL_Helper.insert_album("bunkr", url, album_obj)
 
             if album_obj.media:
-                await log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
+                log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
             return album_obj
 
         cdn_possibilities = r"(?:cdn.bunkr...|cdn..bunkr...|cdn...bunkr...|media-files.bunkr...|media-files..bunkr...|media-files...bunkr...)"
         ext = '.' + url.parts[-1].split('.')[-1]
         if ext:
             ext = ext.lower()
         if ext in FILE_FORMATS['Images']:
@@ -68,28 +68,29 @@
                 referer = URL(re.sub(cdn_possibilities, "bunkr.la/v", str(url)))
             else:
                 referer = URL(re.sub(cdn_possibilities, "bunkr.la/d", str(url)))
             media_item = await self.get_file(session, referer)
             await album_obj.add_media(media_item)
 
         await self.SQL_Helper.insert_album("bunkr", url, album_obj)
-        await log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
+        log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
         return album_obj
 
     async def remove_id(self, filename: str, ext: str):
         """Removes the additional string bunkr adds to the end of every filename"""
         original_filename = filename
         if self.remove_bunkr_id:
             filename = filename.rsplit(ext, 1)[0]
             filename = filename.rsplit("-", 1)[0]
             if ext not in filename:
                 filename = filename + ext
         return original_filename, filename
 
     async def check_for_la(self, url: URL):
+        assert url.host is not None
         if "12" in url.host:
             url_host = url.host.replace(".su", ".la").replace(".ru", ".la")
             url = url.with_host(url_host)
         return url
 
     async def get_file(self, session: ScrapeSession, url: URL):
         """Gets the media item from the supplied url"""
@@ -119,15 +120,15 @@
 
             await self.SQL_Helper.fix_bunkr_entries(link, original_filename)
             complete = await self.SQL_Helper.check_complete_singular("bunkr", link)
             return MediaItem(link, url, complete, filename, ext, original_filename)
 
         except Exception as e:
             logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            await log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
             logger.debug(e)
             return MediaItem(url, url, False, "", "", "")
 
     async def get_album(self, session: ScrapeSession, url: URL):
         """Iterates through an album and creates the media items"""
 
         ### Temp Fix ###
@@ -141,14 +142,15 @@
                 elem.decompose()
             title = await make_title_safe(title.get_text())
             await album.set_new_title(title)
             for file in soup.select('a[class*="grid-images_box-link"]'):
                 link = file.get("href")
                 media_loc = file.select_one("img").get("src").split("//i")[-1].split(".bunkr.")[0]
 
+                assert url.host is not None
                 if link.startswith("/"):
                     link = URL("https://" + url.host + link)
                 link = URL(link)
 
                 try:
                     filename, ext = await get_filename_and_ext(link.name)
                 except NoExtensionFailure:
@@ -171,11 +173,11 @@
                 await self.SQL_Helper.fix_bunkr_entries(link, original_filename)
                 complete = await self.SQL_Helper.check_complete_singular("bunkr", link)
                 media = MediaItem(link, url, complete, filename, ext, original_filename)
                 await album.add_media(media)
 
         except Exception as e:
             logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            await log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
             logger.debug(e)
 
         return album
```

### Comparing `cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/Coomeno_Spider.py` & `cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/Coomeno_Spider.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import asyncio
 from dataclasses import dataclass, field
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Union
 
 from bs4 import BeautifulSoup
 from yarl import URL
 
 from ..base_functions.base_functions import create_media_item, log, logger, make_title_safe
 from ..base_functions.data_classes import CascadeItem
 
@@ -39,28 +39,29 @@
         self.quiet = quiet
         self.scraping_mapper = scraping_mapper
         self.separate_posts = separate_posts
         self.SQL_Helper = SQL_Helper
 
     async def fetch(self, session: ScrapeSession, url: URL):
         """Director for Coomer/Kemono scraping"""
-        await log(f"Starting: {str(url)}", quiet=self.quiet, style="green")
+        log(f"Starting: {str(url)}", quiet=self.quiet, style="green")
         cascade = CascadeItem({})
         title = None
         try:
+            assert url.host is not None
             domain = next((domain for domain in ("coomer", "kemono") if domain in url.host), None)
             if domain:
                 title = await self.handle_coomeno(session, url, domain, cascade)
         except Exception as e:
             logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            await log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
             logger.debug(e)
 
         await self.SQL_Helper.insert_cascade(cascade)
-        await log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
+        log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
         return cascade, title
 
     async def handle_coomeno(self, session: ScrapeSession, url: URL, domain: str, cascade: CascadeItem) -> str:
         """Coomer/Kemono director function"""
         title = f"Loose {domain.capitalize()} Files"
         if "thumbnail" in url.parts:
             parts = [x for x in url.parts if x not in ("thumbnail", "/")]
@@ -88,21 +89,22 @@
             link = URL(content.get('href'))
             tasks.append(asyncio.create_task(self.scraping_mapper.map_url(link, title, referer)))
         if tasks:
             await asyncio.wait(tasks)
 
     async def parse_profile(self, session: ScrapeSession, url: URL, spec: ParseSpec, cascade: CascadeItem) -> str:
         """Parses profiles with supplied selectors"""
-        title = None
+        title = ""
         try:
             soup = await session.get_BS4(url)
             title = await make_title_safe(soup.select_one("span[itemprop=name]").get_text())
             title = f"{title} ({url.host})"
 
             posts = []
+            assert url.host is not None
             for posts_selector in spec.posts_selectors:
                 posts += soup.select(posts_selector)
             for post in posts:
                 path = post.get('href')
                 if path:
                     post_link = URL("https://" + url.host + path)
                     await self.parse_post(session, post_link, spec.domain, cascade, title)
@@ -111,57 +113,65 @@
             if next_page:
                 next_page = next_page.get('href')
                 if next_page:
                     await self.parse_profile(session, URL("https://" + url.host + next_page), spec, cascade)
 
         except Exception as e:
             logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            await log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
             logger.debug(e)
 
         return title
 
-    async def parse_post(self, session: ScrapeSession, url: URL, domain: str, cascade: CascadeItem, title: str = None) -> str:
+    async def parse_post(self, session: ScrapeSession, url: URL, domain: str, cascade: CascadeItem,
+                         title: str = "") -> str:
         """Parses posts with supplied selectors"""
         try:
             text = await self.SQL_Helper.get_blob(url)
             if not text:
                 text = await session.get_text(url)
+                assert text is not None
                 await self.SQL_Helper.insert_blob(text, url)
             soup = BeautifulSoup(text, 'html.parser')
 
             if self.separate_posts:
-                post_title = soup.select_one("h1[class=post__title]").text.replace('\n', '').replace("..", "")
+                post_tag = soup.select_one("h1[class=post__title]")
+                assert post_tag is not None
+                post_title = post_tag.text.replace('\n', '').replace("..", "")
                 prefix = f"{str(url.parts[-1])} - " if self.include_id else ""
                 if title:
                     title = title + '/' + await make_title_safe(prefix + post_title)
                 else:
                     title = await make_title_safe(prefix + post_title)
             elif not title:
-                post_title = soup.select_one("h1[class=post__title]").text.replace('\n', '').replace("..", "")
+                post_tag = soup.select_one("h1[class=post__title]")
+                assert post_tag is not None
+                post_title = post_tag.text.replace('\n', '').replace("..", "")
                 title = await make_title_safe(post_title)
 
             images = soup.select('a[class="fileThumb"]')
             for image in images:
                 await self.parse_tag(image, url, domain, title, cascade)
 
             downloads = soup.select('a[class=post__attachment-link]')
             for download in downloads:
                 await self.parse_tag(download, url, domain, title, cascade)
 
             text_content = soup.select('div[class=post__content] a')
             await self.map_links(text_content, title, url)
         except Exception as e:
             logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            await log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
             logger.debug(e)
 
         return title
 
     async def parse_tag(self, tag: Tag, url: URL, domain: str, title: str, cascade: CascadeItem):
         """Convert link from tag to MediaItem and add it to cascade"""
-        href = tag.get('href')
+        href: Union[str, list[str], None] = tag.get('href')
+
+        assert url.host is not None and isinstance(href, str)
         if href.startswith("/"):
             href = "https://" + url.host + href
         link = URL(href)
         media_item = await create_media_item(link, url, self.SQL_Helper, domain)
         await cascade.add_to_album(domain, title, media_item)
```

### Comparing `cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/CyberFile_Spider.py` & `cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/CyberFile_Spider.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         self.quiet = quiet
         self.SQL_Helper = SQL_Helper
         self.load_files = URL('https://cyberfile.me/account/ajax/load_files')
         self.file_details = URL('https://cyberfile.me/account/ajax/file_details')
 
     async def fetch(self, session: ScrapeSession, url: URL) -> DomainItem:
         """Director for cyberfile scraping"""
-        await log(f"Starting: {str(url)}", quiet=self.quiet, style="green")
+        log(f"Starting: {str(url)}", quiet=self.quiet, style="green")
         domain_obj = DomainItem("cyberfile", {})
 
         download_links = []
         if 'folder' in url.parts:
             Folder_ID = await self.get_folder_id(session, url)
             Content_IDs = None
             if Folder_ID:
@@ -44,30 +44,30 @@
             Content_ID = await self.get_single_contentId(session, url)
             if Content_ID:
                 download_links = await self.get_download_links(session, url, [("Loose CyberFile Files", Content_ID)])
 
         for title, media_item in download_links:
             await domain_obj.add_media(title, media_item)
         await self.SQL_Helper.insert_domain("cyberfile", url, domain_obj)
-        await log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
+        log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
         return domain_obj
 
     async def get_folder_id(self, session: ScrapeSession, url: URL):
         """Gets the internal ID for a folder"""
         try:
             soup = await session.get_BS4(url)
             script_func = soup.select_one('div[class="page-container horizontal-menu with-sidebar fit-logo-with-sidebar logged-out clear-adblock"] script').text
             script_func = script_func.split('loadImages(')[-1]
             script_func = script_func.split(';')[0]
             nodeId = int(script_func.split(',')[1].replace("'", ""))
             return nodeId
 
         except Exception as e:
             logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            await log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
             logger.debug(e)
             return 0
 
     async def get_folder_content(self, session, url: URL, nodeId, page, title=None):
         """Gets the content id's encased in a folder"""
         data = {"pageType": "folder", "nodeId": nodeId, "pageStart": page, "perPage": 0, "filterOrderBy": ""}
         nodes = []
@@ -78,33 +78,40 @@
             original_title = title
             if title:
                 title = title + "/" + await make_title_safe(content['page_title'])
             else:
                 title = content['page_title']
                 title = await make_title_safe(title)
 
-
             soup = BeautifulSoup(text.replace("\\", ""), 'html.parser')
-            total_pages = int(soup.select("a[onclick*=loadImages]")[-1].get('onclick').split(',')[2])
+            pages_tag = soup.select("a[onclick*=loadImages]")[-1]
+            assert pages_tag is not None
+            pages_str = pages_tag.get('onclick')
+            assert isinstance(pages_str, str)
+            total_pages = int(pages_str.split(',')[2])
             listings = soup.select("div[class=fileListing] div")
             for listing in listings:
                 with contextlib.suppress(TypeError):
-                    nodes.append(int(listing.get('folderid')))
+                    folder_id = listing.get('folderid')
+                    assert isinstance(folder_id, str)
+                    nodes.append(int(folder_id))
 
                 with contextlib.suppress(TypeError):
-                    contents.append((title, int(listing.get('fileid'))))
+                    file_id = listing.get('fileid')
+                    assert isinstance(file_id, str)
+                    contents.append((title, int(file_id)))
 
             if page < total_pages:
                 contents.extend(await self.get_folder_content(session, url, nodeId, page+1, original_title))
             for node in nodes:
                 contents.extend(await self.get_folder_content(session, url, node, 1, title))
             return contents
 
         except Exception as e:
-            await log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
             logger.debug(e)
             return []
 
     async def get_single_contentId(self, session: ScrapeSession, url: URL):
         """Gets an individual content id"""
         try:
             soup = await session.get_BS4(url)
@@ -117,15 +124,15 @@
                     part_b = part_a.split(");")[0]
                     contentId = int(part_b)
                     return contentId
             return None
 
         except Exception as e:
             logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            await log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
             logger.debug(e)
             return 0
 
     async def get_shared_ids_and_content(self, session: ScrapeSession, url: URL, page):
         """Gets folder id's and content id's from shared links"""
         try:
             # Initial page load to tell server, this is what we want.
@@ -135,70 +142,91 @@
             data = {"pageType": "nonaccountshared", "nodeId": '', "pageStart": page, "perPage": 0, "filterOrderBy": ""}
             nodes = []
             contents = []
 
             content = await session.post(self.load_files, data)
             text = content['html']
             soup = BeautifulSoup(text.replace("\\", ""), 'html.parser')
-            total_pages = int(soup.select_one('input[id=rspTotalPages]').get('value'))
+            page_tag = soup.select_one('input[id=rspTotalPages]')
+            assert page_tag is not None
+            page_str = page_tag.get('value')
+            assert isinstance(page_str, str)
+            total_pages = int()
             listings = soup.select("div[class=fileListing] div")
             for listing in listings:
                 title = await make_title_safe(content['page_title'])
-                with contextlib.suppress(TypeError, AttributeError):
-                    title = title + '/' + await make_title_safe(listing.select_one('span[class=filename]').text)
-                    nodes.append((title, int(listing.get('folderid'))))
-
-                with contextlib.suppress(TypeError):
-                    contents.append((title, int(listing.get('fileid'))))
+                with contextlib.suppress(TypeError, AttributeError, AssertionError):
+                    folder_tag = listing.select_one('span[class=filename]')
+                    assert folder_tag is not None
+                    folder_name = folder_tag.text
+                    assert isinstance(folder_name, str)
+                    title = title + '/' + await make_title_safe(folder_name)
+                    folder_id = listing.get('folderid')
+                    assert isinstance(folder_id, str)
+                    nodes.append((title, int(folder_id)))
+
+                with contextlib.suppress(TypeError, AttributeError, AssertionError):
+                    file_id = listing.get('fileid')
+                    assert isinstance(file_id, str)
+                    contents.append((title, int(file_id)))
 
             if page < total_pages:
                 nodes_temp, content_temp = await self.get_shared_ids_and_content(session, url, page + 1)
                 nodes.extend(nodes_temp)
                 contents.extend(content_temp)
             return nodes, contents
 
         except Exception as e:
             logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            await log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
             logger.debug(e)
             return []
 
     async def get_shared_content(self, session, url: URL, nodeId, page, title=None):
         """Gets content from shared folders"""
         try:
             nodes = []
             contents = []
             data = {"pageType": "nonaccountshared", "nodeId": nodeId, "pageStart": page, "perPage": 0, "filterOrderBy": ""}
 
             content = await session.post(self.load_files, data)
             text = content['html']
 
             title = title if title else content['page_title']
-
             soup = BeautifulSoup(text.replace("\\", ""), 'html.parser')
-            total_pages = int(soup.select("a[onclick*=loadImages]")[-1].get('onclick').split(',')[2])
+
+            page_ref = soup.select("a[onclick*=loadImages]")[-1].get('onclick')
+            assert isinstance(page_ref, str)
+            total_pages = int(page_ref.split(',')[2])
+
             listings = soup.select("div[class=fileListing] div")
             for listing in listings:
                 with contextlib.suppress(TypeError, AttributeError):
                     filename = listing.select_one('span[class=filename]')
+                    assert filename is not None
                     temp_title = title + '/' + await make_title_safe(filename.text)
-                    nodes.append((temp_title, int(listing.get('folderid'))))
+
+                    folder_id = listing.get('folderid')
+                    assert isinstance(folder_id, str)
+                    nodes.append((temp_title, int(folder_id)))
 
                 with contextlib.suppress(TypeError):
-                    contents.append((title, int(listing.get('fileid'))))
+                    file_id = listing.get('fileid')
+                    assert isinstance(file_id, str)
+                    contents.append((title, int(file_id)))
 
             if page < total_pages:
                 contents.extend(await self.get_shared_content(session, url, nodeId, page + 1, title))
             for title, node in nodes:
                 contents.extend(await self.get_shared_content(session, url, node, 1, title))
             return contents
 
         except Exception as e:
             logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            await log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
             logger.debug(e)
             return []
 
     async def get_download_links(self, session, url, contentIds):
         """Obtains download links from content ids"""
         download_links = []
         try:
@@ -223,10 +251,10 @@
                     continue
 
                 download_links.append((title, media))
             return download_links
 
         except Exception as e:
             logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            await log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
             logger.debug(e)
             return []
```

### Comparing `cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/Cyberdrop_Spider.py` & `cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/Cyberdrop_Spider.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,30 +25,30 @@
         self.SQL_Helper = SQL_Helper
         self.quiet = quiet
 
     async def fetch(self, session: ScrapeSession, url: URL) -> AlbumItem:
         """Cyberdrop scraper"""
         album_obj = AlbumItem("Loose Cyberdrop Files", [])
 
-        await log(f"Starting: {str(url)}", quiet=self.quiet, style="green")
+        log(f"Starting: {str(url)}", quiet=self.quiet, style="green")
         if await check_direct(url):
             media = await create_media_item(url, url, self.SQL_Helper, "cyberdrop")
             await album_obj.add_media(media)
             await self.SQL_Helper.insert_album("cyberdrop", URL(""), album_obj)
-            await log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
+            log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
             return album_obj
 
         try:
             try:
                 soup = await session.get_BS4(url)
             except InvalidContentTypeFailure:
                 media = await create_media_item(url, url, self.SQL_Helper, "cyberdrop")
                 await album_obj.add_media(media)
                 await self.SQL_Helper.insert_album("cyberdrop", URL(""), album_obj)
-                await log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
+                log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
                 return album_obj
 
             title = soup.select_one("h1[id=title]").get_text()
             title = await make_title_safe(title)
             if title is None:
                 title = url.name
             elif self.include_id:
@@ -65,14 +65,14 @@
                     logger.debug("Couldn't get extension for %s", str(link))
                     continue
 
                 await album_obj.add_media(media)
 
         except Exception as e:
             logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            await log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
             logger.debug(e)
             return album_obj
 
         await self.SQL_Helper.insert_album("cyberdrop", url, album_obj)
-        await log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
+        log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
         return album_obj
```

### Comparing `cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/EHentai_Spider.py` & `cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/EHentai_Spider.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,20 +17,20 @@
         self.quiet = quiet
         self.SQL_Helper = SQL_Helper
 
     async def fetch(self, session: ScrapeSession, url: URL) -> AlbumItem:
         """Director for E-Hentai"""
         album_obj = AlbumItem("Loose EHentai Files", [])
 
-        await log(f"Starting: {str(url)}", quiet=self.quiet, style="green")
+        log(f"Starting: {str(url)}", quiet=self.quiet, style="green")
         if "g" in url.parts:
             await self.get_album(session, url, album_obj)
         elif "s" in url.parts:
             await self.get_image(session, url, album_obj)
-        await log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
+        log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
         await self.SQL_Helper.insert_album("e-hentai", url, album_obj)
         return album_obj
 
     async def get_album(self, session: ScrapeSession, url: URL, album_obj: AlbumItem):
         """Gets links from an album"""
         try:
             soup = await session.get_BS4(url)
@@ -52,24 +52,24 @@
             if next_page is not None:
                 next_page = next_page.get('href')
                 if next_page is not None:
                     await self.get_album(session, next_page, album_obj)
 
         except Exception as e:
             logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            await log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
             logger.debug(e)
 
     async def get_image(self, session: ScrapeSession, url: URL, album_obj: AlbumItem):
         """Gets media items from image links"""
         try:
             soup = await session.get_BS4(url)
             image = soup.select_one("img[id=img]")
             link = URL(image.get('src'))
 
             media_item = await create_media_item(link, url, self.SQL_Helper, "e-hentai")
             await album_obj.add_media(media_item)
         except Exception as e:
             logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            await log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
             logger.debug(e)
```

### Comparing `cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/Erome_Spider.py` & `cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/Erome_Spider.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,22 +17,22 @@
     def __init__(self, *, include_id: bool, quiet: bool, SQL_Helper: SQLHelper):
         self.include_id = include_id
         self.quiet = quiet
         self.SQL_Helper = SQL_Helper
 
     async def fetch(self, session: ScrapeSession, url: URL) -> DomainItem:
         """Director function for Erome scraping"""
-        await log(f"Starting: {str(url)}", quiet=self.quiet, style="green")
+        log(f"Starting: {str(url)}", quiet=self.quiet, style="green")
 
         if 'a' in url.parts:
             domain_obj = await self.handle_album(session, url)
         else:
             domain_obj = await self.handle_profile(session, url)
 
-        await log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
+        log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
 
         return domain_obj
 
     async def handle_album(self, session: ScrapeSession, url: URL) -> DomainItem:
         """Handler function for erome albums, adds media items to the domain item"""
         domain_obj = DomainItem("erome", {})
         try:
@@ -63,15 +63,15 @@
                     logger.debug("Couldn't get extension for %s", str(link))
                     continue
                 await domain_obj.add_media(title, media)
 
             await self.SQL_Helper.insert_domain("erome", url, domain_obj)
         except Exception as e:
             logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            await log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
             logger.debug(e)
 
         return domain_obj
 
     async def handle_profile(self, session: ScrapeSession, url: URL) -> DomainItem:
         """Handler for erome profiles, sends albums to handle_album"""
         domain_obj = DomainItem("erome", {})
@@ -93,11 +93,11 @@
             if next_page:
                 next_page = next_page.get("href").split("page=")[-1]
                 next_page = url.with_query(f"page={next_page}")
                 await domain_obj.extend(await self.handle_profile(session, next_page))
 
         except Exception as e:
             logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            await log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
             logger.debug(e)
 
         return domain_obj
```

### Comparing `cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/Fapello_Spider.py` & `cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/Fapello_Spider.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,22 +17,22 @@
 class FapelloCrawler:
     def __init__(self, *, quiet: bool, SQL_Helper: SQLHelper):
         self.quiet = quiet
         self.SQL_Helper = SQL_Helper
 
     async def fetch(self, session: ScrapeSession, url: URL) -> Optional[AlbumItem]:
         """Basic director for fapello"""
-        await log(f"Starting: {str(url)}", quiet=self.quiet, style="green")
+        log(f"Starting: {str(url)}", quiet=self.quiet, style="green")
 
         if not str(url).endswith("/"):
             url = url / ""
 
         album_obj = await self.parse_profile(session, url)
 
-        await log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
+        log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
         return album_obj
 
     async def parse_profile(self, session: ScrapeSession, url: URL) -> Optional[AlbumItem]:
         """Profile parser, passes posts to parse_post"""
         try:
             soup, returned_url = await session.get_BS4_and_url(url)
             title = soup.select_one('h2[class="font-semibold lg:text-2xl text-lg mb-2 mt-4"]').get_text()
@@ -60,15 +60,15 @@
                 if next_page:
                     await album_obj.extend(await self.parse_profile(session, URL(next_page)))
             await self.SQL_Helper.insert_album("fapello", url, album_obj)
             return album_obj
 
         except Exception as e:
             logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            await log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
             logger.debug(e)
             return None
 
     async def parse_post(self, session: ScrapeSession, url: URL) -> list[MediaItem]:
         """Parses posts, returns list of MediaItem"""
         results = []
         try:
@@ -93,11 +93,11 @@
                     media_item = await create_media_item(download_link, url, self.SQL_Helper, "fapello")
                 except NoExtensionFailure:
                     logger.debug("Couldn't get extension for %s", str(download_link))
                     continue
                 results.append(media_item)
         except Exception as e:
             logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            await log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
             logger.debug(e)
 
         return results
```

### Comparing `cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/Gfycat_Spider.py` & `cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/Gfycat_Spider.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,32 +17,33 @@
         self.quiet = quiet
         self.SQL_Helper = SQL_Helper
 
     async def fetch(self, session: ScrapeSession, url: URL) -> AlbumItem:
         """Basic scraper for gfycat"""
         album_obj = AlbumItem("Gfycat", [])
         try:
-            await log(f"Starting: {str(url)}", quiet=self.quiet, style="green")
+            log(f"Starting: {str(url)}", quiet=self.quiet, style="green")
             soup = await session.get_BS4(url)
 
             video = soup.select_one("video[class='video media']")
             video_srcs = video.select("source")
 
             video_link = None
             for src in video_srcs:
                 link = URL(src.get("src"))
+                assert link.host is not None
                 if "giant" in link.host:
                     video_link = link
                     break
             if video_link is None:
                 video_link = URL(video_srcs[0].get("src"))
 
             media_item = await create_media_item(video_link, url, self.SQL_Helper, "gfycat")
             await album_obj.add_media(media_item)
             await self.SQL_Helper.insert_album("gfycat", video_link, album_obj)
-            await log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
+            log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
         except Exception as e:
             logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            await log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
             logger.debug(e)
 
         return album_obj
```

### Comparing `cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/GoFile_Spider.py` & `cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/GoFile_Spider.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 class GoFileCrawler:
     def __init__(self, quiet: bool, SQL_Helper: SQLHelper):
         self.quiet = quiet
         self.SQL_Helper = SQL_Helper
 
         self.api_address = URL("https://api.gofile.io")
-        self.token = None
+        self.token = ""
 
     async def get_token(self, session: ScrapeSession, api_token=None):
         """Creates an anon gofile account to use."""
         if self.token:
             return
 
         if api_token:
@@ -37,75 +37,82 @@
             if json_obj["status"] == "ok":
                 self.token = json_obj["data"]["token"]
                 await self.set_cookie(session)
             else:
                 raise
         except Exception as e:
             logger.debug("Error encountered while getting GoFile token", exc_info=True)
-            await log("Error: Couldn't generate GoFile token", quiet=self.quiet, style="red")
+            log("Error: Couldn't generate GoFile token", quiet=self.quiet, style="red")
             logger.debug(e)
 
     async def set_cookie(self, session: ScrapeSession):
         """Sets the given token as a cookie into the session (and client)"""
         client_token = self.token
-        morsel = http.cookies.Morsel()
+        morsel: http.cookies.Morsel = http.cookies.Morsel()
         morsel['domain'] = 'gofile.io'
         morsel.set('accountToken', client_token, client_token)
         session.client_session.cookie_jar.update_cookies({'gofile.io': morsel})
 
     async def fetch(self, session: ScrapeSession, url: URL) -> DomainItem:
         """Basic director for actual scraping"""
         domain_obj = DomainItem("gofile", {})
         try:
-            await log(f"Starting: {str(url)}", quiet=self.quiet, style="green")
+            log(f"Starting: {str(url)}", quiet=self.quiet, style="green")
             content_id = url.name
             results = await self.get_links(session, url, content_id, None)
             for title, media_item in results:
                 await domain_obj.add_media(title, media_item)
 
             await self.SQL_Helper.insert_domain("gofile", url, domain_obj)
-            await log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
+            log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
         except Exception as e:
             logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            await log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
             logger.debug(e)
 
         return domain_obj
 
-    async def get_links(self, session: ScrapeSession, url: URL, content_id: str, title=None):
+    async def get_links(self, session: ScrapeSession, url: URL, content_id: str, title=None) -> list[list]:
         """Gets links from the given url, creates media_items"""
-        results = []
+        results: list[list] = []
         params = {
             "token": self.token,
             "contentId": content_id,
             "websiteToken": "12345",
         }
         content = await session.get_json(self.api_address / "getContent", params)
         if content["status"] != "ok":
-            logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            await log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            logger.debug("Error encountered while handling %s", str(url))
+            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
             return results
 
         content = content['data']
         if title:
             title = title + "/" + await make_title_safe(content["name"])
         else:
             title = await make_title_safe(content["name"])
 
         contents: dict[str, dict[str, Union[str, int]]] = content["contents"]
         sub_folders = []
         for val in contents.values():
             if val["type"] == "folder":
                 sub_folders.append(val['code'])
             else:
-                link = URL(val["link"]) if val["link"] != "overloaded" else URL(val["directLink"])
+                assert isinstance(val['name'], str)
+                if val["link"] == "overloaded":
+                    assert isinstance(val["directLink"], str)
+                    link = URL(val["directLink"])
+                else:
+                    assert isinstance(val["link"], str)
+                    link = URL(val["link"])
                 try:
                     filename, ext = await get_filename_and_ext(val['name'])
                 except NoExtensionFailure:
                     logger.debug("Couldn't get extension for %s", str(link))
                     continue
                 complete = await self.SQL_Helper.check_complete_singular("gofile", link)
                 media_item = MediaItem(link, url, complete, filename, ext, filename)
                 results.append([title, media_item])
         for sub_folder in sub_folders:
+            assert isinstance(sub_folder, str)
             results.extend(await self.get_links(session, url, sub_folder, title))
         return results
```

### Comparing `cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/HGameCG_Spider.py` & `cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/PimpAndHost_Spider.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,59 +8,64 @@
 from ..base_functions.data_classes import AlbumItem
 
 if TYPE_CHECKING:
     from ..base_functions.sql_helper import SQLHelper
     from ..client.client import ScrapeSession
 
 
-class HGameCGCrawler:
+class PimpAndHostCrawler:
     def __init__(self, quiet: bool, SQL_Helper: SQLHelper):
         self.quiet = quiet
         self.SQL_Helper = SQL_Helper
 
     async def fetch(self, session: ScrapeSession, url: URL) -> AlbumItem:
-        """Basic director for HGameCG"""
-        album_obj = AlbumItem("Loose HGamesCG Files", [])
+        """Director for pimpandhost scraping"""
+        log(f"Starting: {str(url)}", quiet=self.quiet, style="green")
+        album_obj = AlbumItem("Loose Pixeldrain Files", [])
 
-        await log(f"Starting: {str(url)}", quiet=self.quiet, style="green")
-        await self.get_album(session, url, album_obj)
-        await log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
-        await self.SQL_Helper.insert_album("hgamecg", url, album_obj)
+        if url.parts[1] == 'album':
+            media_items, title = await self.get_listings(session, url)
+            await album_obj.set_new_title(title)
+            if media_items:
+                for media_item in media_items:
+                    await album_obj.add_media(media_item)
+        else:
+            media_item = await self.get_singular(session, url)
+            await album_obj.add_media(media_item)
+
+        await self.SQL_Helper.insert_album("pimpandhost", url, album_obj)
+        log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
         return album_obj
 
-    async def get_album(self, session: ScrapeSession, url: URL, album_obj: AlbumItem):
-        """Handles album scraping, adds media items to the album_obj"""
+    async def get_listings(self, session: ScrapeSession, url: URL):
+        """Handles album media"""
+        media_items = []
         try:
             soup = await session.get_BS4(url)
-            title = await make_title_safe(soup.select_one("div[class=navbar] h1").get_text())
-            await album_obj.set_new_title(title)
-
-            images = soup.select("div[class=image] a")
-            for image in images:
-                image = image.get('href')
-                image = URL("https://" + url.host + image)
-                link = await self.get_image(session, image)
-
-                media_item = await create_media_item(link, image, self.SQL_Helper, "hgamecg")
-                await album_obj.add_media(media_item)
-
-            next_page = soup.find("a", text="Next Page")
-            if next_page is not None:
-                next_page = next_page.get('href')
-                if next_page is not None:
-                    next_page = URL("https://" + url.host + next_page)
-                    await self.get_album(session, next_page, album_obj)
+            title = soup.select_one("div[class=image-header]")
+            user_link = title.select_one("span[class=details]")
+            user_link.decompose()
+            title = await make_title_safe(title.get_text())
+
+            for file in soup.select('a[class*="image-wrapper center-cropped im-wr"]'):
+                link = file.get("href")
+                media_items.append(await self.get_singular(session, link))
+            return media_items, title
 
         except Exception as e:
             logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            await log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
             logger.debug(e)
 
-    async def get_image(self, session: ScrapeSession, url: URL):
-        """Gets image link from the given url."""
+    async def get_singular(self, session: ScrapeSession, url: URL):
+        """Handles singular files"""
         try:
             soup = await session.get_BS4(url)
-            image = soup.select_one("div[class=hgamecgimage] img")
-            image = URL(image.get('src'))
-            return image
-        except Exception:
-            await log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            img = soup.select_one("a img")
+            img = img.get("src")
+            if img.startswith("//"):
+                img = URL("https:" + img)
+            return await create_media_item(img, url, self.SQL_Helper, "pimpandhost")
+        except Exception as e:
+            logger.debug("Error encountered while handling %s", str(url), exc_info=True)
+            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            logger.debug(e)
```

### Comparing `cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/ImgBox_Spider.py` & `cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/ImgBox_Spider.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     def __init__(self, *, quiet: bool, SQL_Helper: SQLHelper):
         self.quiet = quiet
         self.SQL_Helper = SQL_Helper
 
     async def fetch(self, session: ScrapeSession, url: URL) -> AlbumItem:
         """Director func for ImgBox scraping"""
         album_obj = AlbumItem("Loose ImgBox Files", [])
-        await log(f"Starting: {str(url)}", quiet=self.quiet, style="green")
+        log(f"Starting: {str(url)}", quiet=self.quiet, style="green")
 
         try:
             if await check_direct(url):
                 media_item = await create_media_item(url, url, self.SQL_Helper, "imgbox")
                 await album_obj.add_media(media_item)
 
             elif "g" in url.parts:
@@ -50,19 +50,19 @@
             else:
                 img = await self.singular(session, url)
                 media_item = await create_media_item(img, url, self.SQL_Helper, "imgbox")
                 await album_obj.add_media(media_item)
 
         except Exception as e:
             logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            await log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
             logger.debug(e)
 
         await self.SQL_Helper.insert_album("imgbox", url, album_obj)
-        await log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
+        log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
         return album_obj
 
     async def folder(self, session: ScrapeSession, url: URL):
         """Gets links from a folder"""
         soup = await session.get_BS4(url)
         output = []
         title = soup.select_one("div[id=gallery-view] h1").get_text()
```

### Comparing `cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/LoveFap_Spider.py` & `cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/LoveFap_Spider.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,36 +24,36 @@
         self.SQL_Helper = SQL_Helper
         self.quiet = quiet
 
     async def fetch(self, session: ScrapeSession, url: URL) -> AlbumItem:
         """Director for lovefap scraping"""
         album_obj = AlbumItem("Loose LoveFap Files", [])
 
-        await log(f"Starting: {str(url)}", quiet=self.quiet, style="green")
+        log(f"Starting: {str(url)}", quiet=self.quiet, style="green")
         if await check_direct(url):
             media = await create_media_item(url, url, self.SQL_Helper, "lovefap")
             await album_obj.add_media(media)
             await self.SQL_Helper.insert_album("lovefap", URL(""), album_obj)
-            await log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
+            log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
             return album_obj
 
         try:
             if "video" in url.parts:
                 await self.fetch_video(session, url, album_obj)
             else:
                 await self.fetch_album(session, url, album_obj)
 
         except Exception as e:
             logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            await log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
             logger.debug(e)
             return album_obj
 
         await self.SQL_Helper.insert_album("lovefap", url, album_obj)
-        await log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
+        log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
         return album_obj
 
     async def fetch_album(self, session: ScrapeSession, url: URL, album_obj: AlbumItem):
         """Gets media_items for albums, and adds them to the Album_obj"""
         soup = await session.get_BS4(url)
 
         title = soup.select_one('div[class=albums-content-header] span[style*="float: left"]').get_text()
```

### Comparing `cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/NSFWXXXCrawler.py` & `cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/NSFWXXXCrawler.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,29 +20,29 @@
         self.separate_posts = separate_posts
         self.SQL_Helper = SQL_Helper
 
     async def fetch(self, session: ScrapeSession, url: URL) -> DomainItem:
         """Director for NSFW.XXX scraping"""
         domain_obj = DomainItem("nsfw.xxx", {})
 
-        await log(f"Starting: {str(url)}", quiet=self.quiet, style="green")
+        log(f"Starting: {str(url)}", quiet=self.quiet, style="green")
         if "user" in url.parts:
             await self.get_user(session, url, domain_obj)
         else:
             await self.get_post(session, url, domain_obj)
         await self.SQL_Helper.insert_domain("nsfw.xxx", url, domain_obj)
         return domain_obj
 
     async def get_user(self, session: ScrapeSession, url: URL, domain_obj: DomainItem):
         """Gets posts for a user profile"""
         try:
             model = url.name + " (NSFW.XXX)"
             for page in itertools.count(1):
-                model_name = url.path.split("/")
-                model_name = list(filter(None, model_name))[-1]
+                model_name_parts = url.path.split("/")
+                model_name = list(filter(None, model_name_parts))[-1]
                 page_url = URL(f"https://nsfw.xxx/page/{page}?nsfw[]=0&types[]=image&types[]=video&types[]=gallery&slider=1&jsload=1&user={model_name}")
                 page_soup = await session.get_BS4(page_url)
 
                 posts = page_soup.select('div[class="sh-section__image grid-item"] a[class=slider_init_href]')
                 posts.extend(page_soup.select('div[class="sh-video__player"] a[class=slider_init_href]'))
                 posts.extend(page_soup.select('div[class="sh-section__images row"] div a'))
 
@@ -51,15 +51,15 @@
 
                 posts = await self.get_post_hrefs(posts)
                 for post in posts:
                     await self.get_post(session, post, domain_obj, model)
 
         except Exception as e:
             logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            await log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
             logger.debug(e)
 
     async def get_post_hrefs(self, posts):
         """Gets links from post objects"""
         posts_links = []
         for post in posts:
             url = URL(post.get("href"))
@@ -90,9 +90,9 @@
                     continue
 
                 title = f"{model}/{post_name}" if self.separate_posts else model
                 await domain_obj.add_media(title, media)
 
         except Exception as e:
             logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            await log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
             logger.debug(e)
```

### Comparing `cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/PimpAndHost_Spider.py` & `cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/XBunkr_Spider.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,70 +2,52 @@
 
 from typing import TYPE_CHECKING
 
 from yarl import URL
 
 from ..base_functions.base_functions import create_media_item, log, logger, make_title_safe
 from ..base_functions.data_classes import AlbumItem
+from ..base_functions.error_classes import NoExtensionFailure
 
 if TYPE_CHECKING:
     from ..base_functions.sql_helper import SQLHelper
     from ..client.client import ScrapeSession
 
 
-class PimpAndHostCrawler:
+class XBunkrCrawler:
     def __init__(self, quiet: bool, SQL_Helper: SQLHelper):
         self.quiet = quiet
         self.SQL_Helper = SQL_Helper
 
     async def fetch(self, session: ScrapeSession, url: URL) -> AlbumItem:
-        """Director for pimpandhost scraping"""
-        await log(f"Starting: {str(url)}", quiet=self.quiet, style="green")
-        album_obj = AlbumItem("Loose Pixeldrain Files", [])
-
-        if url.parts[1] == 'album':
-            media_items, title = await self.get_listings(session, url)
-            await album_obj.set_new_title(title)
-            if media_items:
-                for media_item in media_items:
-                    await album_obj.add_media(media_item)
-        else:
-            media_item = await self.get_singular(session, url)
-            await album_obj.add_media(media_item)
-
-        await self.SQL_Helper.insert_album("pimpandhost", url, album_obj)
-        await log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
-        return album_obj
+        """Director for XBunkr scraping"""
+        album_obj = AlbumItem("Loose XBunkr Files", [])
 
-    async def get_listings(self, session: ScrapeSession, url: URL):
-        """Handles album media"""
-        media_items = []
         try:
-            soup = await session.get_BS4(url)
-            title = soup.select_one("div[class=image-header]")
-            user_link = title.select_one("span[class=details]")
-            user_link.decompose()
-            title = await make_title_safe(title.get_text())
-
-            for file in soup.select('a[class*="image-wrapper center-cropped im-wr"]'):
-                link = file.get("href")
-                media_items.append(await self.get_singular(session, link))
-            return media_items, title
+            assert url.host is not None
+            if "media" in url.host:
+                media_item = await create_media_item(url, url, self.SQL_Helper, "xbunkr")
+                await album_obj.add_media(media_item)
+
+            else:
+                soup = await session.get_BS4(url)
+                links = soup.select("a[class=image]")
+                title = await make_title_safe(soup.select_one("h1[id=title]").text)
+                title = title.strip()
+                await album_obj.set_new_title(title)
+                for link in links:
+                    link = URL(link.get('href'))
+                    try:
+                        media_item = await create_media_item(link, url, self.SQL_Helper, "xbunkr")
+                    except NoExtensionFailure:
+                        logger.debug("Couldn't get extension for %s", str(link))
+                        continue
+                    await album_obj.add_media(media_item)
 
         except Exception as e:
             logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            await log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            log("Error scraping " + str(url), quiet=self.quiet)
             logger.debug(e)
 
-    async def get_singular(self, session: ScrapeSession, url: URL):
-        """Handles singular files"""
-        try:
-            soup = await session.get_BS4(url)
-            img = soup.select_one("a img")
-            img = img.get("src")
-            if img.startswith("//"):
-                img = URL("https:" + img)
-            return await create_media_item(img, url, self.SQL_Helper, "pimpandhost")
-        except Exception as e:
-            logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            await log(f"Error: {str(url)}", quiet=self.quiet, style="red")
-            logger.debug(e)
+        await self.SQL_Helper.insert_album("xbunkr", URL(""), album_obj)
+        log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
+        return album_obj
```

### Comparing `cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/PixelDrain_Spider.py` & `cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/PixelDrain_Spider.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     def __init__(self, quiet: bool, SQL_Helper: SQLHelper):
         self.quiet = quiet
         self.SQL_Helper = SQL_Helper
         self.api = URL('https://pixeldrain.com/api/')
 
     async def fetch(self, session: ScrapeSession, url: URL) -> AlbumItem:
         """Director for pixeldrain scraping"""
-        await log(f"Starting: {str(url)}", quiet=self.quiet, style="green")
+        log(f"Starting: {str(url)}", quiet=self.quiet, style="green")
         album_obj = AlbumItem("Loose Pixeldrain Files", [])
 
         identifier = str(url).split('/')[-1]
         if url.parts[1] == 'l':
             await album_obj.set_new_title(url.name)
             media_items = await self.get_listings(session, identifier, url)
             for media_item in media_items:
@@ -34,15 +34,15 @@
             link = await self.create_download_link(identifier)
             complete = await self.SQL_Helper.check_complete_singular("pixeldrain", link)
             filename, ext = await get_filename_and_ext(await self.get_file_name(session, identifier))
             media_item = MediaItem(link, url, complete, filename, ext, filename)
             await album_obj.add_media(media_item)
 
         await self.SQL_Helper.insert_album("pixeldrain", url, album_obj)
-        await log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
+        log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
         return album_obj
 
     async def get_listings(self, session: ScrapeSession, identifier: str, url: URL) -> list[MediaItem]:
         """Handles album scraping"""
         media_items = []
         try:
             content = await session.get_json(self.api / "list" / identifier)
@@ -54,15 +54,15 @@
                     logger.debug("Couldn't get extension for %s", str(link))
                     continue
                 complete = await self.SQL_Helper.check_complete_singular("pixeldrain", link)
                 media_item = MediaItem(link, url, complete, filename, ext, filename)
                 media_items.append(media_item)
         except Exception as e:
             logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            await log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
             logger.debug(e)
 
         return media_items
 
     async def get_file_name(self, session: ScrapeSession, identifier: str) -> str:
         """Gets filename for the given file identifier"""
         content = await session.get_json(self.api / 'file' / identifier / 'info')
```

### Comparing `cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/PostImg_Spider.py` & `cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/PostImg_Spider.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,38 +19,38 @@
     def __init__(self, quiet: bool, SQL_Helper: SQLHelper):
         self.quiet = quiet
         self.SQL_Helper = SQL_Helper
 
     async def fetch(self, session: ScrapeSession, url: URL) -> AlbumItem:
         """Director for PostImg scraping"""
         album_obj = AlbumItem("Loose PostImg Files", [])
-        await log(f"Starting: {str(url)}", quiet=self.quiet, style="green")
+        log(f"Starting: {str(url)}", quiet=self.quiet, style="green")
 
         try:
             if "gallery" in url.parts:
                 content = await self.get_folder(session, url)
                 for media_item in content:
                     await album_obj.add_media(media_item)
             else:
                 media_item = await self.get_singular(session, url)
                 await album_obj.add_media(media_item)
 
         except Exception as e:
             logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            await log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
             logger.debug(e)
 
         await self.SQL_Helper.insert_album("postimg", url, album_obj)
-        await log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
+        log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
         return album_obj
 
     async def get_folder(self, session: ScrapeSession, url: URL):
         """Handles folder scraping"""
         album = url.raw_name
-        data = {"action": "list", "album": album}
+        data = {"action": "list", "album": album, "page": 0}
         content = []
         for i in itertools.count(1):
             data["page"] = i
             data_out = await session.post(URL("https://postimg.cc/json"), data)
             if data_out['status_code'] != HTTPStatus.OK or not data_out['images']:
                 break
             for item in data_out['images']:
```

### Comparing `cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/Saint_Spider.py` & `cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/Saint_Spider.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,23 +16,23 @@
     def __init__(self, quiet: bool, SQL_Helper: SQLHelper):
         self.quiet = quiet
         self.SQL_Helper = SQL_Helper
 
     async def fetch(self, session: ScrapeSession, url: URL) -> AlbumItem:
         """Basic director for saint scraping"""
         album_obj = AlbumItem("Loose Saint Files", [])
-        await log(f"Starting: {str(url)}", quiet=self.quiet, style="green")
+        log(f"Starting: {str(url)}", quiet=self.quiet, style="green")
 
         try:
             soup = await session.get_BS4(url)
             link = URL(soup.select_one('video[id=main-video] source').get('src'))
             media_item = await create_media_item(link, url, self.SQL_Helper, "saint")
             await album_obj.add_media(media_item)
             await self.SQL_Helper.insert_album("saint", link, album_obj)
 
         except Exception as e:
             logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            await log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
             logger.debug(e)
 
-        await log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
+        log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
         return album_obj
```

### Comparing `cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/ShareX_Spider.py` & `cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/ShareX_Spider.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,17 +25,18 @@
     def __init__(self, *, include_id=False, quiet: bool, SQL_Helper: SQLHelper):
         self.include_id = include_id
         self.quiet = quiet
         self.SQL_Helper = SQL_Helper
 
     async def fetch(self, session: ScrapeSession, url: URL) -> DomainItem:
         """Director for ShareX scraper"""
+        assert url.host is not None
         domain_obj = DomainItem(url.host.lower(), {})
 
-        await log(f"Starting: {str(url)}", quiet=self.quiet, style="green")
+        log(f"Starting: {str(url)}", quiet=self.quiet, style="green")
 
         if await check_direct(url):
             url = url.with_name(url.name.replace('.md.', '.').replace('.th.', '.'))
             url = await self.jpg_fish_from_church(url)
             media_item = await create_media_item(url, url, self.SQL_Helper, "sharex")
             await domain_obj.add_media("Loose ShareX Files", media_item)
         elif "album" in url.parts or "a" in url.parts:
@@ -44,15 +45,15 @@
             await self.get_albums(session, url, domain_obj)
         elif 'image' in url.parts or 'img' in url.parts or 'images' in url.parts:
             await self.get_singular(session, url, domain_obj)
         else:
             await self.parse_profile(session, url, domain_obj)
 
         await self.SQL_Helper.insert_domain("sharex", url, domain_obj)
-        await log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
+        log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
         return domain_obj
 
     async def jpg_fish_from_church(self, url: URL) -> URL:
         pattern = r"simp([1-5])\.jpg\.church/"
         return URL(re.sub(pattern, r'simp\1.jpg.fish/', str(url)))
 
     async def get_albums(self, session: ScrapeSession, url: URL, domain_obj: DomainItem):
@@ -71,15 +72,15 @@
                 next_page = next_page.get('href')
                 if next_page is not None:
                     next_page = URL(next_page)
                     await self.get_albums(session, next_page, domain_obj)
 
         except Exception as e:
             logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            await log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
             logger.debug(e)
 
     async def get_singular(self, session: ScrapeSession, url: URL, domain_obj: DomainItem):
         """Handles scraping for singular files"""
         await asyncio.sleep(1)
         try:
             soup = await session.get_BS4(url)
@@ -87,29 +88,29 @@
             link = link.with_name(link.name.replace('.md.', '.').replace('.th.', '.'))
             link = await self.jpg_fish_from_church(link)
 
             media_item = await create_media_item(link, url, self.SQL_Helper, "sharex")
             await domain_obj.add_media("Loose ShareX Files", media_item)
         except Exception as e:
             logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            await log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
             logger.debug(e)
 
     async def get_sub_album_links(self, session: ScrapeSession, url: URL, og_title: str, domain_obj: DomainItem):
         try:
             soup = await session.get_BS4(url)
             albums = soup.select("div[class=pad-content-listing] div")
             for album in albums:
                 album_url = album.get('data-url-short')
                 if album_url is not None:
                     album_url = URL(album_url)
                     await self.parse(session=session, url=album_url, og_title=og_title, domain_obj=domain_obj)
         except Exception as e:
             logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            await log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
             logger.debug(e)
 
     async def parse_profile(self, session: ScrapeSession, url: URL, domain_obj: DomainItem):
         """Handles scraping for profiles"""
         try:
             soup = await session.get_BS4(url)
             title = soup.select_one("div[class=header] h1 strong").get_text()
@@ -119,21 +120,22 @@
                 titlep2 = url.name
                 title = title + " - " + titlep2
             title = await make_title_safe(title.replace(r"\n", "").strip())
             await self.get_list_links(session, url, title, domain_obj)
 
         except Exception as e:
             logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            await log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
             logger.debug(e)
 
     async def get_list_links(self, session: ScrapeSession, url: URL, title: str, domain_obj: DomainItem):
         """Gets final links and adds to domain_obj"""
         try:
             soup = await session.get_BS4(url)
+            assert url.host is not None
             if 'jpg.fish' in url.host or 'jpg.church' in url.host:
                 links = soup.select("a[href*=img] img")
             else:
                 links = soup.select("a[href*=image] img")
             for link in links:
                 link = URL(link.get('src'))
                 link = link.with_name(link.name.replace('.md.', '.').replace('.th.', '.'))
@@ -152,15 +154,15 @@
             if next_page is not None:
                 next_page = next_page.get('href')
                 if next_page is not None:
                     next_page = URL(next_page)
                     await self.get_list_links(session, next_page, title, domain_obj)
         except Exception as e:
             logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            await log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
             logger.debug(e)
 
     async def parse(self, *, session: ScrapeSession, url: URL, og_title=None, domain_obj: DomainItem):
         try:
             soup = await session.get_BS4(url)
 
             title = soup.select_one("a[data-text=album-name]").get_text()
@@ -179,9 +181,9 @@
                 await self.get_sub_album_links(session, sub_albums, title, domain_obj)
             finally:
                 list_recent = URL(soup.select_one("a[id=list-most-recent-link]").get("href"))
                 await self.get_list_links(session, list_recent, title, domain_obj)
 
         except Exception as e:
             logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            await log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
             logger.debug(e)
```

### Comparing `cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/XBunkr_Spider.py` & `cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/HGameCG_Spider.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,51 +2,67 @@
 
 from typing import TYPE_CHECKING
 
 from yarl import URL
 
 from ..base_functions.base_functions import create_media_item, log, logger, make_title_safe
 from ..base_functions.data_classes import AlbumItem
-from ..base_functions.error_classes import NoExtensionFailure
 
 if TYPE_CHECKING:
     from ..base_functions.sql_helper import SQLHelper
     from ..client.client import ScrapeSession
 
 
-class XBunkrCrawler:
+class HGameCGCrawler:
     def __init__(self, quiet: bool, SQL_Helper: SQLHelper):
         self.quiet = quiet
         self.SQL_Helper = SQL_Helper
 
     async def fetch(self, session: ScrapeSession, url: URL) -> AlbumItem:
-        """Director for XBunkr scraping"""
-        album_obj = AlbumItem("Loose XBunkr Files", [])
+        """Basic director for HGameCG"""
+        album_obj = AlbumItem("Loose HGamesCG Files", [])
 
+        log(f"Starting: {str(url)}", quiet=self.quiet, style="green")
+        await self.get_album(session, url, album_obj)
+        log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
+        await self.SQL_Helper.insert_album("hgamecg", url, album_obj)
+        return album_obj
+
+    async def get_album(self, session: ScrapeSession, url: URL, album_obj: AlbumItem):
+        """Handles album scraping, adds media items to the album_obj"""
         try:
-            if "media" in url.host:
-                media_item = await create_media_item(url, url, self.SQL_Helper, "xbunkr")
+            soup = await session.get_BS4(url)
+            title = await make_title_safe(soup.select_one("div[class=navbar] h1").get_text())
+            await album_obj.set_new_title(title)
+
+            images = soup.select("div[class=image] a")
+            for image in images:
+                image = image.get('href')
+                assert url.host is not None
+                image = URL("https://" + url.host + image)
+                link = await self.get_image(session, image)
+
+                media_item = await create_media_item(link, image, self.SQL_Helper, "hgamecg")
                 await album_obj.add_media(media_item)
 
-            else:
-                soup = await session.get_BS4(url)
-                links = soup.select("a[class=image]")
-                title = await make_title_safe(soup.select_one("h1[id=title]").text)
-                title = title.strip()
-                await album_obj.set_new_title(title)
-                for link in links:
-                    link = URL(link.get('href'))
-                    try:
-                        media_item = await create_media_item(link, url, self.SQL_Helper, "xbunkr")
-                    except NoExtensionFailure:
-                        logger.debug("Couldn't get extension for %s", str(link))
-                        continue
-                    await album_obj.add_media(media_item)
+            next_page = soup.find("a", text="Next Page")
+            if next_page is not None:
+                next_page = next_page.get('href')
+                if next_page is not None:
+                    assert url.host is not None
+                    next_page = URL("https://" + url.host + next_page)
+                    await self.get_album(session, next_page, album_obj)
 
         except Exception as e:
             logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            await log("Error scraping " + str(url), quiet=self.quiet)
+            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
             logger.debug(e)
 
-        await self.SQL_Helper.insert_album("xbunkr", URL(""), album_obj)
-        await log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
-        return album_obj
+    async def get_image(self, session: ScrapeSession, url: URL):
+        """Gets image link from the given url."""
+        try:
+            soup = await session.get_BS4(url)
+            image = soup.select_one("div[class=hgamecgimage] img")
+            image = URL(image.get('src'))
+            return image
+        except Exception:
+            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
```

### Comparing `cyberdrop-dl-4.1.16/cyberdrop_dl/crawlers/Xenforo_Spider.py` & `cyberdrop-dl-4.1.17/cyberdrop_dl/crawlers/Xenforo_Spider.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,92 +23,96 @@
     from ..client.client import ScrapeSession
 
 
 @dataclass
 class ParseSpec:
     """Class for specific selectors of supported domains"""
     domain: str
-    title_block_element: str = "h1[class=p-title-value]"
-    title_clutter_element: str = field(init=False)
+    
+    title_block_tag: str = "h1[class=p-title-value]"
+    title_clutter_tag: str = field(init=False)
 
-    posts_block_element: str = "div[class*=message-main]"
-    posts_number_element: str = field(init=False)
+    posts_block_tag: str = "div[class*=message-main]"
+    posts_number_tag: str = field(init=False)
     posts_number_attribute: str = "href"
 
-    post_content_element: str = "div[class=bbWrapper]"
-    block_quote_element: str = "blockquote"
+    post_content_tag: str = "div[class=bbWrapper]"
+    block_quote_tag: str = "blockquote"
 
-    links_element: str = "a"
+    links_tag: str = "a"
     links_attribute: str = "href"
 
-    images_element: str = field(init=False)
+    images_tag: str = field(init=False)
     images_attribute: str = field(init=False)
 
-    video_element: str = "video source"
+    video_tag: str = "video source"
     video_attribute: str = "src"
-    saint_iframe_element: str = "iframe[class=saint-iframe]"
+    saint_iframe_tag: str = "iframe[class=saint-iframe]"
     saint_iframe_attribute: str = "src"
 
-    embedded_content_element: str = "span[data-s9e-mediaembed-iframe]"
+    embedded_content_tag: str = "span[data-s9e-mediaembed-iframe]"
     embedded_content_attribute: str = "data-s9e-mediaembed-iframe"
 
-    attachment_block_element: str = "section[class=message-attachments]"
-    attachment_element: str = "a"
+    attachment_block_tag: str = "section[class=message-attachments]"
+    attachment_tag: str = "a"
     attachment_attribute: str = "href"
 
-    next_page_element: str = 'a[class="pageNav-jump pageNav-jump--next"]'
+    next_page_tag: str = 'a[class="pageNav-jump pageNav-jump--next"]'
     next_page_attribute: str = "href"
 
     def __post_init__(self):
         if self.domain in ("simpcity", "xbunker", "socialmediagirls"):
-            self.title_clutter_element = "a" if self.domain in ("simpcity", "xbunker") else "span"
-            self.posts_number_element = "li[class=u-concealed] a"
-            self.images_element = "div[class*=bbImage]"
+            self.title_clutter_tag = "a" if self.domain in ("simpcity", "xbunker") else "span"
+            self.posts_number_tag = "li[class=u-concealed] a"
+            self.images_tag = "div[class*=bbImage]"
             self.images_attribute = "data-src"
 
         elif self.domain == "nudostar":
-            self.title_clutter_element = "span"
-            self.posts_number_element = "a[class=u-concealed]"
-            self.images_element = "img[class*=bbImage]"
+            self.title_clutter_tag = "span"
+            self.posts_number_tag = "a[class=u-concealed]"
+            self.images_tag = "img[class*=bbImage]"
             self.images_attribute = "src"
 
 
 class ForumLogin:
     def __init__(self, name: str, username: str, password: str):
         self.name = name
         self.logged_in = False
         self.username = username
         self.password = password
 
     async def login(self, session: ScrapeSession, url: URL, quiet: bool):
         """Handles forum logging in"""
         if not self.username or not self.password:
-            await log(f"Login wasn't provided for {self.name}", quiet=quiet, style="red")
+            log(f"Login wasn't provided for {self.name}", quiet=quiet, style="red")
             raise FailedLoginFailure()
         attempt = 0
         while True:
             try:
                 if self.logged_in:
                     return
                 if attempt == 5:
                     raise FailedLoginFailure()
 
+                assert url.host is not None
                 domain = URL("https://" + url.host) / "forum/login" if "nudostar" in url.host else \
                     URL("https://" + url.host) / "login"
 
                 text = await session.get_text(domain)
                 await asyncio.sleep(5)
                 soup = BeautifulSoup(text, 'html.parser')
 
                 inputs = soup.select('form input')
                 data = {
                     elem['name']: elem['value']
                     for elem in inputs
                     if elem.get('name') and elem.get('value')
                 }
+
+                assert url.host is not None
                 data.update({
                     "login": self.username,
                     "password": self.password,
                     "_xfRedirect": str(URL("https://" + url.host))
                 })
                 await session.post_data_no_resp(domain / "login", data=data)
                 await asyncio.sleep(5)
@@ -147,42 +151,43 @@
         self.xbunker = ForumLogin("XBunker",
                                   args["Authentication"]["xbunker_username"],
                                   args["Authentication"]["xbunker_password"])
 
         self.scraping_mapper = scraping_mapper
         self.SQL_Helper = SQL_Helper
 
-    async def fetch(self, session: ScrapeSession, url: URL):
+    async def fetch(self, session: ScrapeSession, url: URL) -> tuple[CascadeItem, str]:
         """Xenforo forum director"""
-        await log(f"Starting: {str(url)}", quiet=self.quiet, style="green")
+        log(f"Starting: {str(url)}", quiet=self.quiet, style="green")
         cascade = CascadeItem({})
 
         scrape_url, post_num = await self.get_thread_url_and_post_num(url)
-        title = None
+        title = ""
         try:
+            assert url.host is not None
             if "simpcity" in url.host:
                 await self.simpcity.login(session, url, self.quiet)
             elif "socialmediagirls" in url.host:
                 await self.socialmediagirls.login(session, url, self.quiet)
             elif "xbunker" in url.host:
                 await self.xbunker.login(session, url, self.quiet)
             elif "nudostar" in url.host:
                 await self.nudostar.login(session, url, self.quiet)
 
             domain = next((domain for domain in self.domains if domain in url.host), None)
             if domain:
                 title = await self.parse_forum(session, scrape_url, ParseSpec(domain), cascade, "", post_num)
         except Exception as e:
             logger.debug("Error encountered while handling %s", str(url), exc_info=True)
-            await log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            log(f"Error: {str(url)}", quiet=self.quiet, style="red")
             logger.debug(e)
             return cascade, ""
 
         await self.SQL_Helper.insert_cascade(cascade)
-        await log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
+        log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
         return cascade, title
 
     async def get_thread_url_and_post_num(self, url: URL):
         """Splits the thread url and returns the url and post number if provided"""
         post_number = 0
         if "post-" in str(url):
             post_number_parts = str(url).rsplit("post-", 1)
@@ -230,14 +235,15 @@
                 embed_url = URL(embed_url.group(0).replace("www.", ""))
                 found_links.append([embed_url, temp_title])
         return found_links
 
     async def filter_content_links(self, cascade: CascadeItem, content_links: list, url: URL, domain: str):
         """Splits given links into direct links and external links,
         returns external links, adds internal to the cascade"""
+        assert url.host is not None
         forum_direct_urls = [x for x in content_links if x[0].host.replace(".st", ".su") in url.host]
         forum_direct_urls.extend([x for x in content_links if url.host in x[0].host.replace(".st", ".su")])
         forum_direct_urls.extend([x for x in content_links if "smgmedia" in x[0].host])
         content_links = [x for x in content_links if x not in forum_direct_urls]
         for link_title_bundle in forum_direct_urls:
             link, temp_title = link_title_bundle
             in_prog_title = temp_title + "/Attachments"
@@ -264,78 +270,80 @@
             await asyncio.wait(tasks)
 
     async def parse_forum(self, session: ScrapeSession, url: URL, spec: ParseSpec, cascade: CascadeItem,
                           title: str, post_number: int):
         """Parses forum threads"""
         soup = await session.get_BS4(url)
 
+        assert url.host is not None
         domain = URL("https://" + url.host)
-        post_num_str = None
+        post_num_str = ""
         content_links = []
 
-        title_block = soup.select_one(spec.title_block_element)
-        for elem in title_block.find_all(spec.title_clutter_element):
+        title_block = soup.select_one(spec.title_block_tag)
+        for elem in title_block.find_all(spec.title_clutter_tag):
             elem.decompose()
 
         if title:
             pass
         else:
             title = title_block.text
             title = await make_title_safe(title.replace("\n", "").strip())
 
-        posts = soup.select(spec.posts_block_element)
+        posts = soup.select(spec.posts_block_tag)
 
         for post in posts:
-            post_num_str = post.select_one(spec.posts_number_element).get(spec.posts_number_attribute).split('/')[-1]
+            post_num_str = post.select_one(spec.posts_number_tag).get(spec.posts_number_attribute).split('/')[-1]
             post_num_int = int(post_num_str.split('post-')[-1])
             if post_number > post_num_int:
                 continue
 
             temp_title = title + "/" + post_num_str if self.separate_posts else title
 
-            for elem in post.find_all(spec.block_quote_element):
+            for elem in post.find_all(spec.block_quote_tag):
                 elem.decompose()
-            post_content = post.select_one(spec.post_content_element)
+            post_content = post.select_one(spec.post_content_tag)
 
             # Get Links
-            content_links.extend(await self.get_links(post_content, spec.links_element, spec.links_attribute, domain,
+            content_links.extend(await self.get_links(post_content, spec.links_tag, spec.links_attribute, domain,
                                                       temp_title))
 
             # Get Images
-            content_links.extend(await self.get_links(post_content, spec.images_element, spec.images_attribute, domain,
+            content_links.extend(await self.get_links(post_content, spec.images_tag, spec.images_attribute, domain,
                                                       temp_title))
 
             # Get Videos:
-            content_links.extend(await self.get_links(post_content, spec.video_element, spec.video_attribute, domain,
+            content_links.extend(await self.get_links(post_content, spec.video_tag, spec.video_attribute, domain,
                                                       temp_title))
-            content_links.extend(await self.get_links(post_content, spec.saint_iframe_element,
+            content_links.extend(await self.get_links(post_content, spec.saint_iframe_tag,
                                                       spec.saint_iframe_attribute, domain, temp_title))
 
             # Get Other Embedded Content
-            content_links.extend(await self.get_embedded(post_content, spec.embedded_content_element,
+            content_links.extend(await self.get_embedded(post_content, spec.embedded_content_tag,
                                                          spec.embedded_content_attribute, temp_title))
 
             # Get Attachments
-            attachments_block = post.select_one(spec.attachment_block_element)
-            content_links.extend(await self.get_links(attachments_block, spec.attachment_element,
+            attachments_block = post.select_one(spec.attachment_block_tag)
+            content_links.extend(await self.get_links(attachments_block, spec.attachment_tag,
                                                       spec.attachment_attribute, domain, temp_title))
 
         # Handle links
         content_links = await self.filter_content_links(cascade, content_links, url, spec.domain)
         await self.handle_external_links(content_links, url)
 
-        next_page = soup.select_one(spec.next_page_element)
+        next_page = soup.select_one(spec.next_page_tag)
         if next_page is not None:
             next_page = next_page.get(spec.next_page_attribute)
             if next_page is not None:
                 if next_page.startswith('/'):
                     next_page = domain / next_page[1:]
                 next_page = URL(next_page)
                 await self.parse_forum(session, next_page, spec, cascade, title, post_number)
         elif self.output_last:
+            assert url.raw_name is not None
             if 'page-' in url.raw_name or 'post-' in url.raw_name:
                 last_post_url = url.parent / post_num_str
             else:
                 last_post_url = url / post_num_str
             async with aiofiles.open(self.output_last_file, mode='a') as f:
                 await f.write(f'{last_post_url}\n')
         return title
```

### Comparing `cyberdrop-dl-4.1.16/cyberdrop_dl/downloader/downloader_utils.py` & `cyberdrop-dl-4.1.17/cyberdrop_dl/downloader/downloader_utils.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.16/cyberdrop_dl/downloader/downloaders.py` & `cyberdrop-dl-4.1.17/cyberdrop_dl/downloader/downloaders.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,18 +97,18 @@
         self.domain_obj = domain_obj
 
         self.errored_output = args['Runtime']['output_errored_urls']
         self.errored_file = args['Files']['errored_urls_file']
 
         self.files = files
 
-        self.current_attempt = {}
+        self.current_attempt: dict[str, int] = {}
         max_workers = get_threads_number(args, domain)
         self._semaphore = asyncio.Semaphore(max_workers)
-        self.delay = {'cyberfile': 1, 'anonfiles': 1, "coomer": 0.2, "kemono": 0.2}
+        self.delay = {'cyberfile': 1.0, 'anonfiles': 1.0, "coomer": 0.2, "kemono": 0.2}
 
         self.pixeldrain_api_key = args["Authentication"]["pixeldrain_api_key"]
 
         self.exclude_audio = args["Ignore"]["exclude_audio"]
         self.exclude_images = args["Ignore"]["exclude_images"]
         self.exclude_videos = args["Ignore"]["exclude_videos"]
         self.exclude_other = args["Ignore"]["exclude_other"]
@@ -144,34 +144,34 @@
         await asyncio.gather(*download_tasks)
         album_progress.update(album_task, visible=False)
         domain_progress.advance(domain_task, 1)
 
     async def start_file(self, album_task: TaskID, album: str, media: MediaItem):
         """Handler for files and the progress bars for it"""
         if media.complete or await self.SQL_Helper.check_complete_singular(self.domain, media.url):
-            await log(f"Previously Downloaded: {media.filename}", quiet=True)
+            log(f"Previously Downloaded: {media.filename}", quiet=True)
             await self.files.add_skipped()
             album_progress.advance(album_task, 1)
             return
         async with self._semaphore:
             url_path = await get_db_path(media.url, self.domain)
             await self.download_file(album, media, url_path, album_task)
 
     @retry
     async def download_file(self, album: str, media: MediaItem, url_path: str, album_task: TaskID) -> None:
         """File downloader"""
         if not await check_free_space(self.required_free_space, self.download_dir):
-            await log("We've run out of free space.", quiet=True)
+            log("We've run out of free space.", quiet=True)
             await self.files.add_skipped()
             album_progress.advance(album_task, 1)
             return
 
         if not await allowed_filetype(media, self.exclude_images, self.exclude_videos, self.exclude_audio,
                                       self.exclude_other):
-            await log(f"Blocked by file extension: {media.filename}", quiet=True)
+            log(f"Blocked by file extension: {media.filename}", quiet=True)
             await self.files.add_skipped()
             album_progress.advance(album_task, 1)
             return
 
         if self.block_sub_folders:
             album = album.split('/')[0]
 
@@ -206,14 +206,15 @@
             resume_point = 0
             await self.SQL_Helper.sql_insert_temp(str(partial_file))
             range_num = None
             if partial_file.exists():
                 resume_point = partial_file.stat().st_size
                 range_num = f'bytes={resume_point}-'
 
+            assert media.url.host is not None
             for key, value in self.delay.items():
                 if key in media.url.host:
                     current_throttle = value
 
             headers = {"Authorization": await basic_auth("Cyberdrop-DL", self.pixeldrain_api_key)} \
                 if (self.pixeldrain_api_key and "pixeldrain" in media.url.host) else {}
             if range_num:
@@ -229,22 +230,22 @@
                 partial_file.rename(complete_file)
 
             await self.SQL_Helper.mark_complete(url_path, original_filename)
             if media.url.parts[-1] in self.current_attempt:
                 self.current_attempt.pop(media.url.parts[-1])
 
             if fake_download:
-                await log(f"Already Downloaded: {media.filename} from {media.referer}", quiet=True)
+                log(f"Already Downloaded: {media.filename} from {media.referer}", quiet=True)
                 await self.files.add_skipped()
             else:
                 await self.files.add_completed()
             album_progress.advance(album_task, 1)
             file_progress.update(file_task, visible=False)
 
-            await log(f"Completed Download: {media.filename} from {media.referer}", quiet=True)
+            log(f"Completed Download: {media.filename} from {media.referer}", quiet=True)
             await self.File_Lock.remove_lock(filename)
             return
 
         except (aiohttp.client_exceptions.ClientPayloadError, aiohttp.client_exceptions.ClientOSError,
                 aiohttp.client_exceptions.ServerDisconnectedError, asyncio.TimeoutError,
                 aiohttp.client_exceptions.ClientResponseError, aiohttp.client_exceptions.ServerTimeoutError,
                 DownloadFailure, FileNotFoundError, PermissionError) as e:
@@ -256,27 +257,27 @@
 
             if hasattr(e, "message"):
                 logging.debug(f"\n{media.url} ({e.message})")
 
             if hasattr(e, "code"):
                 if await is_4xx_client_error(e.code) and e.code != HTTPStatus.TOO_MANY_REQUESTS:
                     logger.debug("We ran into a 400 level error: %s", str(e.code))
-                    await log(f"Failed Download: {media.filename}", quiet=True)
+                    log(f"Failed Download: {media.filename}", quiet=True)
                     await self.files.add_failed()
                     if url_path in self.current_attempt:
                         self.current_attempt.pop(url_path)
                     await self.output_failed(media, e)
                     return
                 if e.code == HTTPStatus.SERVICE_UNAVAILABLE or e.code == HTTPStatus.BAD_GATEWAY \
                         or e.code == CustomHTTPStatus.WEB_SERVER_IS_DOWN:
                     if hasattr(e, "message"):
                         if not e.message:
                             e.message = "Web server is down"
                         logging.debug(f"\n{media.url} ({e.message})")
-                    await log(f"Failed Download: {media.filename}", quiet=True)
+                    log(f"Failed Download: {media.filename}", quiet=True)
                     await self.files.add_failed()
                     if url_path in self.current_attempt:
                         self.current_attempt.pop(url_path)
                     await self.output_failed(media, e)
                     return
 
                 logger.debug("Error status code: " + str(e.code))
@@ -355,15 +356,15 @@
         await asyncio.gather(*tasks)
 
         cascade_progress.update(cascade_task, visible=False)
 
     await files.hide()
 
     await clear()
-    await log(f"| [green]Files Complete: {files.completed_files}[/green] - [yellow]Files Skipped: "
+    log(f"| [green]Files Complete: {files.completed_files}[/green] - [yellow]Files Skipped: "
               f"{files.skipped_files}[/yellow] - [red]Files Failed: {files.failed_files}[/red] |")
 
 
 async def download_forums(args: dict, Forums: ForumItem, SQL_Helper: SQLHelper, client: Client) -> None:
     """Handler for forum threads and the progress bars for it"""
     progress_table = await get_forum_table(args["Progress_Options"])
     total_files = await Forums.get_total()
@@ -379,9 +380,9 @@
                 tasks.append(downloader.start_domain(cascade_task))
             await asyncio.gather(*tasks)
 
             cascade_progress.update(cascade_task, visible=False)
             forum_progress.advance(forum_task, 1)
 
     await clear()
-    await log(f"| [green]Files Complete: {files.completed_files}[/green] - [yellow]Files Skipped: "
+    log(f"| [green]Files Complete: {files.completed_files}[/green] - [yellow]Files Skipped: "
               f"{files.skipped_files}[/yellow] - [red]Files Failed: {files.failed_files}[/red] |")
```

### Comparing `cyberdrop-dl-4.1.16/cyberdrop_dl/downloader/old_downloaders.py` & `cyberdrop-dl-4.1.17/cyberdrop_dl/downloader/old_downloaders.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import asyncio
 import itertools
 import logging
 from http import HTTPStatus
+from pathlib import Path
 from random import gauss
 
 import aiofiles
 import aiohttp.client_exceptions
 from tqdm import tqdm
 
 from cyberdrop_dl.base_functions.base_functions import (
@@ -36,23 +37,23 @@
 
     def __init__(self, progress: tqdm):
         self.progress = progress
         self.completed_files = 0
         self.skipped_files = 0
         self.failed_files = 0
 
-    async def add_completed(self):
+    async def add_completed(self) -> None:
         self.completed_files += 1
         self.progress.update(1)
 
-    async def add_skipped(self):
+    async def add_skipped(self) -> None:
         self.skipped_files += 1
         self.progress.update(1)
 
-    async def add_failed(self):
+    async def add_failed(self) -> None:
         self.failed_files += 1
         self.progress.update(1)
 
 
 class Old_Downloader:
     """Downloader class, directs downloading for domain objects"""
 
@@ -67,15 +68,15 @@
         self.domain_obj = domain_obj
 
         self.errored_output = args['Runtime']['output_errored_urls']
         self.errored_file = args['Files']['errored_urls_file']
 
         self.files = files
 
-        self.current_attempt = {}
+        self.current_attempt: dict[str, int] = {}
         max_workers = get_threads_number(args, domain)
         self._semaphore = asyncio.Semaphore(max_workers)
         self.delay = {'cyberfile': 1, 'anonfiles': 1, "coomer": 0.2, "kemono": 0.2}
 
         self.pixeldrain_api_key = args["Authentication"]["pixeldrain_api_key"]
 
         self.exclude_audio = args["Ignore"]["exclude_audio"]
@@ -87,50 +88,50 @@
         self.allowed_attempts = args["Runtime"]["attempts"]
         self.disable_attempt_limit = args["Runtime"]["disable_attempt_limit"]
         self.download_dir = args["Files"]["output_folder"]
         self.mark_downloaded = args["Runtime"]["skip_download_mark_completed"]
         self.proxy = args["Runtime"]["proxy"]
         self.required_free_space = args["Runtime"]["required_free_space"]
 
-    async def start_domain(self):
+    async def start_domain(self) -> None:
         """Handler for domains and the progress bars for it"""
         for album, album_obj in self.domain_obj.albums.items():
             await self.start_album(album, album_obj)
         await self.download_session.exit_handler()
 
-    async def start_album(self, album: str, album_obj: AlbumItem):
+    async def start_album(self, album: str, album_obj: AlbumItem) -> None:
         """Handler for albums and the progress bars for it"""
         if await album_obj.is_empty():
             return
         download_tasks = []
         for media in album_obj.media:
             download_tasks.append(self.start_file(album, media))
         await asyncio.gather(*download_tasks)
 
-    async def start_file(self, album: str, media: MediaItem):
+    async def start_file(self, album: str, media: MediaItem) -> None:
         """Handler for files and the progress bars for it"""
         if media.complete or await self.SQL_Helper.check_complete_singular(self.domain, media.url):
-            await log(f"Previously Downloaded: {media.filename}", quiet=True)
+            log(f"Previously Downloaded: {media.filename}", quiet=True)
             await self.files.add_skipped()
             return
         async with self._semaphore:
             url_path = await get_db_path(media.url, self.domain)
             await self.download_file(album, media, url_path)
 
     @retry
     async def download_file(self, album: str, media: MediaItem, url_path: str) -> None:
         """File downloader"""
         if not await check_free_space(self.required_free_space, self.download_dir):
-            await log("We've run out of free space.", quiet=True)
+            log("We've run out of free space.", quiet=True)
             await self.files.add_skipped()
             return
 
         if not await allowed_filetype(media, self.exclude_images, self.exclude_videos, self.exclude_audio,
                                       self.exclude_other):
-            await log(f"Blocked by file extension: {media.filename}", quiet=True)
+            log(f"Blocked by file extension: {media.filename}", quiet=True)
             await self.files.add_skipped()
             return
 
         if self.block_sub_folders:
             album = album.split('/')[0]
 
         try:
@@ -162,14 +163,15 @@
             resume_point = 0
             await self.SQL_Helper.sql_insert_temp(str(partial_file))
             range_num = None
             if partial_file.exists():
                 resume_point = partial_file.stat().st_size
                 range_num = f'bytes={resume_point}-'
 
+            assert media.url.host is not None
             for key, value in self.delay.items():
                 if key in media.url.host:
                     current_throttle = value
 
             headers = {"Authorization": await basic_auth("Cyberdrop-DL", self.pixeldrain_api_key)} \
                 if (self.pixeldrain_api_key and "pixeldrain" in media.url.host) else {}
             if range_num:
@@ -185,15 +187,15 @@
                 self.current_attempt.pop(media.url.parts[-1])
 
             if fake_download:
                 await self.files.add_skipped()
             else:
                 await self.files.add_completed()
 
-            await log(f"Completed Download: {media.filename} from {media.referer}", quiet=True)
+            log(f"Completed Download: {media.filename} from {media.referer}", quiet=True)
             await self.File_Lock.remove_lock(original_filename)
             return
 
         except (aiohttp.client_exceptions.ClientPayloadError, aiohttp.client_exceptions.ClientOSError,
                 aiohttp.client_exceptions.ServerDisconnectedError, asyncio.TimeoutError,
                 aiohttp.client_exceptions.ClientResponseError, aiohttp.client_exceptions.ServerTimeoutError,
                 DownloadFailure, PermissionError) as e:
@@ -202,42 +204,42 @@
 
             if hasattr(e, "message"):
                 logging.debug(f"\n{media.url} ({e.message})")
 
             if hasattr(e, "code"):
                 if await is_4xx_client_error(e.code) and e.code != HTTPStatus.TOO_MANY_REQUESTS:
                     logger.debug("We ran into a 400 level error: %s", str(e.code))
-                    await log(f"Failed Download: {media.filename}", quiet=True)
+                    log(f"Failed Download: {media.filename}", quiet=True)
                     await self.files.add_failed()
                     if url_path in self.current_attempt:
                         self.current_attempt.pop(url_path)
                     await self.output_failed(media, e)
                     return
                 if e.code == HTTPStatus.SERVICE_UNAVAILABLE or e.code == CustomHTTPStatus.WEB_SERVER_IS_DOWN:
                     if hasattr(e, "message"):
                         if not e.message:
                             e.message = "Web server is down"
                         logging.debug(f"\n{media.url} ({e.message})")
-                    await log(f"Failed Download: {media.filename}", quiet=True)
+                    log(f"Failed Download: {media.filename}", quiet=True)
                     await self.files.add_failed()
                     if url_path in self.current_attempt:
                         self.current_attempt.pop(url_path)
                     await self.output_failed(media, e)
                     return
                 logger.debug("Error status code: " + str(e.code))
 
             raise DownloadFailure(code=getattr(e, "code", 1), message=repr(e))
 
-    async def output_failed(self, media, e):
+    async def output_failed(self, media, e) -> None:
         if self.errored_output:
             async with aiofiles.open(self.errored_file, mode='a') as file:
                 await file.write(f"{media.url},{media.referer},{e.message}\n")
 
     async def check_file_exists(self, complete_file, partial_file, media, album, url_path, original_filename,
-                                current_throttle):
+                                current_throttle) -> tuple[Path, Path, bool]:
         """Complicated checker for if a file already exists, and was already downloaded"""
         expected_size = None
         proceed = True
         while True:
             if not complete_file.exists() and not partial_file.exists():
                 break
 
@@ -284,15 +286,15 @@
         tasks = []
         for domain, domain_obj in Cascade.domains.items():
             downloader = Old_Downloader(args, client, SQL_Helper, domain, domain_obj, files)
             tasks.append(downloader.start_domain())
         await asyncio.gather(*tasks)
 
     await clear()
-    await log(f"| [green]Files Complete: {files.completed_files}[/green] - [yellow]Files Skipped: "
+    log(f"| [green]Files Complete: {files.completed_files}[/green] - [yellow]Files Skipped: "
               f"{files.skipped_files}[/yellow] - [red]Files Failed: {files.failed_files}[/red] |")
 
 
 async def old_download_forums(args: dict, Forums: ForumItem, SQL_Helper: SQLHelper, client: Client) -> None:
     """Handler for forum threads and the progress bars for it"""
     total_files = await Forums.get_total()
     with tqdm(total=total_files, unit_scale=True, unit='Files', leave=True, initial=0,
@@ -302,9 +304,9 @@
             tasks = []
             for domain, domain_obj in Cascade.domains.items():
                 downloader = Old_Downloader(args, client, SQL_Helper, domain, domain_obj, files)
                 tasks.append(downloader.start_domain())
             await asyncio.gather(*tasks)
 
     await clear()
-    await log(f"| [green]Files Complete: {files.completed_files}[/green] - [yellow]Files Skipped: "
+    log(f"| [green]Files Complete: {files.completed_files}[/green] - [yellow]Files Skipped: "
               f"{files.skipped_files}[/yellow] - [red]Files Failed: {files.failed_files}[/red] |")
```

### Comparing `cyberdrop-dl-4.1.16/cyberdrop_dl/downloader/progress_definitions.py` & `cyberdrop-dl-4.1.17/cyberdrop_dl/downloader/progress_definitions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from __future__ import annotations
 
 from rich.panel import Panel
 from rich.progress import Progress, BarColumn, SpinnerColumn, TransferSpeedColumn, DownloadColumn, TimeRemainingColumn
 from rich.table import Table
 
 forum_progress = Progress("[progress.description]{task.description}",
-                         BarColumn(bar_width=None),
-                         "[progress.percentage]{task.percentage:>3.2f}%",
-                         "{task.completed} of {task.total} Threads Completed")
+                          BarColumn(bar_width=None),
+                          "[progress.percentage]{task.percentage:>3.2f}%",
+                          "{task.completed} of {task.total} Threads Completed")
 
 cascade_progress = Progress("[progress.description]{task.description}",
                             BarColumn(bar_width=None),
                             "[progress.percentage]{task.percentage:>3.2f}%",
                             "{task.completed} of {task.total} Domains Completed")
 
 domain_progress = Progress("[progress.description]{task.description}",
@@ -37,39 +37,49 @@
                          DownloadColumn(),
                          "━",
                          TransferSpeedColumn(),
                          "━",
                          TimeRemainingColumn())
 
 
-async def get_forum_table(progress_options: dict):
+async def get_forum_table(progress_options: dict) -> Table:
     """Table creator for forum threads"""
     progress_table = Table.grid(expand=True)
     if not progress_options['hide_overall_progress']:
-        progress_table.add_row(Panel.fit(overall_file_progress, title="Overall Progress", border_style="green", padding=(1, 1)))
+        progress_table.add_row(
+            Panel.fit(overall_file_progress, title="Overall Progress", border_style="green", padding=(1, 1)))
     if not progress_options['hide_forum_progress']:
         progress_table.add_row(Panel.fit(forum_progress, title="Total Thread", border_style="green", padding=(1, 1)))
     if not progress_options['hide_thread_progress']:
-        progress_table.add_row(Panel.fit(cascade_progress, title="Current Thread", border_style="green", padding=(1, 1)))
+        progress_table.add_row(
+            Panel.fit(cascade_progress, title="Current Thread", border_style="green", padding=(1, 1)))
     if not progress_options['hide_domain_progress']:
-        progress_table.add_row(Panel.fit(domain_progress, title="Domains Being Downloaded", border_style="green", padding=(1, 1)))
+        progress_table.add_row(
+            Panel.fit(domain_progress, title="Domains Being Downloaded", border_style="green", padding=(1, 1)))
     if not progress_options['hide_album_progress']:
-        progress_table.add_row(Panel.fit(album_progress, title="Albums Being Downloaded", border_style="green", padding=(1, 1)))
+        progress_table.add_row(
+            Panel.fit(album_progress, title="Albums Being Downloaded", border_style="green", padding=(1, 1)))
     if not progress_options['hide_file_progress']:
-        progress_table.add_row(Panel.fit(file_progress, title="[b]Files Being Downloaded", border_style="green", padding=(1, 1)))
+        progress_table.add_row(
+            Panel.fit(file_progress, title="[b]Files Being Downloaded", border_style="green", padding=(1, 1)))
     return progress_table
 
 
-async def get_cascade_table(progress_options: dict):
+async def get_cascade_table(progress_options: dict) -> Table:
     """Table creator for cascade objects"""
     progress_table = Table.grid(expand=True)
     if not progress_options['hide_overall_progress']:
-        progress_table.add_row(Panel.fit(overall_file_progress, title="Overall Progress", border_style="green", padding=(1, 1)))
+        progress_table.add_row(
+            Panel.fit(overall_file_progress, title="Overall Progress", border_style="green", padding=(1, 1)))
     if not progress_options['hide_thread_progress']:
-        progress_table.add_row(Panel.fit(cascade_progress, title="Current Thread", border_style="green", padding=(1, 1)))
+        progress_table.add_row(
+            Panel.fit(cascade_progress, title="Current Thread", border_style="green", padding=(1, 1)))
     if not progress_options['hide_domain_progress']:
-        progress_table.add_row(Panel.fit(domain_progress, title="Domains Being Downloaded", border_style="green", padding=(1, 1)))
+        progress_table.add_row(
+            Panel.fit(domain_progress, title="Domains Being Downloaded", border_style="green", padding=(1, 1)))
     if not progress_options['hide_album_progress']:
-        progress_table.add_row(Panel.fit(album_progress, title="Albums Being Downloaded", border_style="green", padding=(1, 1)))
+        progress_table.add_row(
+            Panel.fit(album_progress, title="Albums Being Downloaded", border_style="green", padding=(1, 1)))
     if not progress_options['hide_file_progress']:
-        progress_table.add_row(Panel.fit(file_progress, title="[b]Files Being Downloaded", border_style="green", padding=(1, 1)))
+        progress_table.add_row(
+            Panel.fit(file_progress, title="[b]Files Being Downloaded", border_style="green", padding=(1, 1)))
     return progress_table
```

### Comparing `cyberdrop-dl-4.1.16/cyberdrop_dl/main.py` & `cyberdrop-dl-4.1.17/cyberdrop_dl/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from cyberdrop_dl.client.client import Client
 from cyberdrop_dl.downloader.downloader_utils import check_free_space
 from cyberdrop_dl.downloader.downloaders import download_cascade, download_forums
 from cyberdrop_dl.downloader.old_downloaders import old_download_cascade, old_download_forums
 from cyberdrop_dl.scraper.Scraper import ScrapeMapper
 
 from . import __version__ as VERSION
-from .base_functions.data_classes import CascadeItem, SkipData
+from .base_functions.data_classes import CascadeItem, ForumItem, SkipData
 
 
 def parse_args() -> argparse.Namespace:
     """Parses the command line arguments passed into the program"""
     parser = argparse.ArgumentParser(description="Bulk downloader for multiple file hosts")
     parser.add_argument("-V", "--version", action="version", version=f"%(prog)s {VERSION}")
 
@@ -193,46 +193,46 @@
     links = list(map(URL, links))
     if args["Files"]["input_file"].is_file():
         with open(args["Files"]["input_file"], "r", encoding="utf8") as f:
             links += await regex_links([line.rstrip() for line in f])
     links = list(filter(None, links))
 
     if not links:
-        await log("No valid links found.", style="red")
+        log("No valid links found.", style="red")
     return links
 
 
-async def scrape_links(scraper: ScrapeMapper, links: list, quiet=False) -> CascadeItem:
+async def scrape_links(scraper: ScrapeMapper, links: list, quiet=False) -> tuple[CascadeItem, ForumItem]:
     """Maps links from URLs.txt or command to the scraper class"""
-    await log("Starting Scrape", quiet=quiet, style="green")
+    log("Starting Scrape", quiet=quiet, style="green")
     tasks = []
 
     for link in links:
         tasks.append(asyncio.create_task(scraper.map_url(link)))
     await asyncio.wait(tasks)
 
     Cascade = scraper.Cascade
     await Cascade.dedupe()
     Forums = scraper.Forums
     await Forums.dedupe()
 
-    await log("", quiet=quiet)
-    await log("Finished Scrape", quiet=quiet, style="green")
+    log("", quiet=quiet)
+    log("Finished Scrape", quiet=quiet, style="green")
     return Cascade, Forums
 
 
 async def director(args: dict, links: list) -> None:
     """This is the overarching director coordinator for CDL."""
     await clear()
     await document_args(args)
     await file_management(args, links)
-    await log(f"We are running version {VERSION} of Cyberdrop Downloader")
+    log(f"We are running version {VERSION} of Cyberdrop Downloader")
 
     if not await check_free_space(args['Runtime']['required_free_space'], args['Files']['output_folder']):
-        await log("Not enough free space to continue. You can change the required space required using --required-free-space.", style="red")
+        log("Not enough free space to continue. You can change the required space required using --required-free-space.", style="red")
         exit(1)
 
     links = await consolidate_links(args, links)
     client = Client(args['Ratelimiting']['ratelimit'], args['Ratelimiting']['throttle'],
                     args['Runtime']['allow_insecure_connections'], args["Ratelimiting"]["connection_timeout"],
                     args['Runtime']['user_agent'])
     SQL_Helper = SQLHelper(args['Ignore']['ignore_history'], args['Ignore']['ignore_cache'], args['Files']['db_file'])
@@ -254,37 +254,37 @@
             if not await Cascade.is_empty():
                 await download_cascade(args, Cascade, SQL_Helper, client)
             if not await Forums.is_empty():
                 await download_forums(args, Forums, SQL_Helper, client)
 
     if args['Files']['output_folder'].is_dir():
         if args['Sorting']['sort_downloads']:
-            await log("")
-            await log("Sorting Downloads")
+            log("")
+            log("Sorting Downloads")
             sorter = Sorter(args['Files']['output_folder'], args['Sorting']['sort_directory'],
                             args['Sorting']['sorted_audio'], args['Sorting']['sorted_images'],
                             args['Sorting']['sorted_videos'], args['Sorting']['sorted_others'],)
             await sorter.sort()
 
-        await log("")
-        await log("Checking for incomplete downloads")
-        partial_downloads = [str(f) for f in args['Files']['output_folder'].rglob("*.part") if f.is_file()]
-        temp_downloads_check = [str(f) for f in await SQL_Helper.get_temp_names() if Path(f).is_file()]
+        log("")
+        log("Checking for incomplete downloads")
+        partial_downloads = any(f.is_file() for f in args['Files']['output_folder'].rglob("*.part"))
+        temp_downloads = any(Path(f).is_file() for f in await SQL_Helper.get_temp_names())
 
-        await log('Purging empty directories')
+        log('Purging empty directories')
         await purge_dir(args['Files']['output_folder'])
 
-        await log('Finished downloading. Enjoy :)')
+        log('Finished downloading. Enjoy :)')
         if partial_downloads:
-            await log('There are partial downloads in the downloads folder.', style="yellow")
-        if temp_downloads_check:
-            await log('There are partial downloads from this run, please re-run the program.', style="yellow")
+            log('There are partial downloads in the downloads folder.', style="yellow")
+        if temp_downloads:
+            log('There are partial downloads from this run, please re-run the program.', style="yellow")
 
-    await log('')
-    await log("If you enjoy using this program, please consider buying the developer a coffee :)\nhttps://www.buymeacoffee.com/juleswinnft", style="green")
+    log('')
+    log("If you enjoy using this program, please consider buying the developer a coffee :)\nhttps://www.buymeacoffee.com/juleswinnft", style="green")
 
 
 def main(args=None):
     if not args:
         args = parse_args()
 
     links = args.links
```

### Comparing `cyberdrop-dl-4.1.16/cyberdrop_dl/scraper/JDownloader_Integration.py` & `cyberdrop-dl-4.1.17/cyberdrop_dl/scraper/JDownloader_Integration.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 import logging
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Optional
 
 from myjdapi import myjdapi
 
 from cyberdrop_dl.base_functions.base_functions import log
 from cyberdrop_dl.base_functions.error_classes import JDownloaderFailure
 
 if TYPE_CHECKING:
@@ -14,44 +14,46 @@
 
 class JDownloader:
     """Class that handles connecting and passing links to JDownloader"""
     def __init__(self, jdownloader_args: dict, quiet: bool):
         self.jdownloader_device = jdownloader_args['jdownloader_device']
         self.jdownloader_username = jdownloader_args['jdownloader_username']
         self.jdownloader_password = jdownloader_args['jdownloader_password']
-
         self.jdownloader_enable = jdownloader_args['apply_jdownloader']
-        self.jdownloader_agent = None
         self.quiet = quiet
+        self.jdownloader_agent = self.jdownloader_setup()
 
-    async def jdownloader_setup(self):
+    def jdownloader_setup(self) -> Optional[myjdapi.Jddevice]:
         """Setup function for JDownloader"""
+        if not self.jdownloader_enable:
+            return None
+
         try:
             if not self.jdownloader_username or not self.jdownloader_password or not self.jdownloader_device:
                 raise JDownloaderFailure("jdownloader credentials were not provided.")
             jd = myjdapi.Myjdapi()
             jd.set_app_key("CYBERDROP-DL")
             jd.connect(self.jdownloader_username, self.jdownloader_password)
-            self.jdownloader_agent = jd.get_device(self.jdownloader_device)
+            return jd.get_device(self.jdownloader_device)
         except JDownloaderFailure:
-            await log("Failed JDownloader setup", quiet=self.quiet, style="red")
+            log("Failed JDownloader setup", quiet=self.quiet, style="red")
             self.jdownloader_enable = False
+            return None
 
-    async def direct_unsupported_to_jdownloader(self, url: URL, title: str):
+    async def direct_unsupported_to_jdownloader(self, url: URL, title: str) -> None:
         """Sends links to JDownloader"""
         if self.jdownloader_enable:
-            if not self.jdownloader_agent:
-                await self.jdownloader_setup()
             try:
+                assert url.host is not None
                 if "facebook" in url.host.lower() or "instagram" in url.host.lower():
                     raise JDownloaderFailure("Blacklisted META")
-
+                assert self.jdownloader_agent is not None
                 self.jdownloader_agent.linkgrabber.add_links([{
                     "autostart": False,
                     "links": str(url),
                     "packageName": title if title else "Cyberdrop-DL",
                     "overwritePackagizerRules": True
                     }])
 
-            except JDownloaderFailure as e:
+            except (JDownloaderFailure, AssertionError) as e:
                 logging.debug(e)
-                await log(f"Failed to send {str(url)} to JDownloader", quiet=self.quiet, style="red")
+                log(f"Failed to send {str(url)} to JDownloader", quiet=self.quiet, style="red")
```

### Comparing `cyberdrop-dl-4.1.16/cyberdrop_dl/scraper/Scraper.py` & `cyberdrop-dl-4.1.17/cyberdrop_dl/scraper/Scraper.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 import asyncio
-from typing import TYPE_CHECKING, Dict
+from typing import TYPE_CHECKING, Optional
 
 import aiofiles
 from yarl import URL
 
 from cyberdrop_dl.base_functions.base_functions import log
 from cyberdrop_dl.base_functions.data_classes import AlbumItem, CascadeItem, DomainItem, ForumItem, SkipData
 from cyberdrop_dl.client.client import Client, ScrapeSession
@@ -35,64 +35,65 @@
 
 if TYPE_CHECKING:
     from cyberdrop_dl.base_functions.sql_helper import SQLHelper
 
 
 class ScrapeMapper:
     """This class maps links to their respective handlers, or JDownloader if they are unsupported"""
-    def __init__(self, args: Dict, client: Client, SQL_Helper: SQLHelper, quiet: bool):
+    def __init__(self, args: dict, client: Client, SQL_Helper: SQLHelper, quiet: bool):
         self.args = args
         self.client = client
         self.SQL_Helper = SQL_Helper
         self.Cascade = CascadeItem({})
         self.Forums = ForumItem({})
         self.skip_data = SkipData(args['Ignore']['skip_hosts'])
         self.only_data = SkipData(args['Ignore']['only_hosts'])
 
         self.unsupported_file = args["Files"]["unsupported_urls_file"]
         self.unsupported_output = args['Runtime']['output_unsupported_urls']
 
-        self.anonfiles_crawler = None
-        self.bunkr_crawler = None
-        self.cyberdrop_crawler = None
-        self.coomeno_crawler = None
-        self.cyberfile_crawler = None
-        self.ehentai_crawler = None
-        self.erome_crawler = None
-        self.fapello_crawler = None
-        self.gfycat_crawler = None
-        self.gofile_crawler = None
-        self.hgamecg_crawler = None
-        self.imgbox_crawler = None
-        self.lovefap_crawler = None
-        self.nsfwxxx_crawler = None
-        self.pimpandhost_crawler = None
-        self.pixeldrain_crawler = None
-        self.postimg_crawler = None
-        self.redgifs_crawler = None
-        self.rule34_crawler = None
-        self.saint_crawler = None
-        self.sharex_crawler = None
-        self.xbunkr_crawler = None
-        self.xenforo_crawler = None
+        self.anonfiles_crawler: Optional[AnonfilesCrawler] = None
+        self.bunkr_crawler: Optional[BunkrCrawler] = None
+        self.cyberdrop_crawler: Optional[CyberdropCrawler] = None
+        self.coomeno_crawler: Optional[CoomenoCrawler] = None
+        self.cyberfile_crawler: Optional[CyberFileCrawler] = None
+        self.ehentai_crawler: Optional[EHentaiCrawler] = None
+        self.erome_crawler: Optional[EromeCrawler] = None
+        self.fapello_crawler: Optional[FapelloCrawler] = None
+        self.gfycat_crawler: Optional[GfycatCrawler] = None
+        self.gofile_crawler: Optional[GoFileCrawler] = None
+        self.hgamecg_crawler: Optional[HGameCGCrawler] = None
+        self.imgbox_crawler: Optional[ImgBoxCrawler] = None
+        self.lovefap_crawler: Optional[LoveFapCrawler] = None
+        self.nsfwxxx_crawler: Optional[NSFWXXXCrawler] = None
+        self.pimpandhost_crawler: Optional[PimpAndHostCrawler] = None
+        self.pixeldrain_crawler: Optional[PixelDrainCrawler] = None
+        self.postimg_crawler: Optional[PostImgCrawler] = None
+        self.saint_crawler: Optional[SaintCrawler] = None
+        self.sharex_crawler: Optional[ShareXCrawler] = None
+        self.xbunkr_crawler: Optional[XBunkrCrawler] = None
+        self.xenforo_crawler: Optional[XenforoCrawler] = None
 
         self.include_id = args['Runtime']['include_id']
         self.remove_bunkr_id = args['Runtime']['remove_bunkr_identifier']
         self.separate_posts = args["Forum_Options"]["separate_posts"]
         self.quiet = quiet
         self.jdownloader = JDownloader(args['JDownloader'], quiet)
 
-        self.jpgfish_limiter = AsyncRateLimiter(10)
         self.bunkr_limiter = AsyncRateLimiter(15)
-        self.coomeno_limiter = AsyncRateLimiter(6)
+        self.coomer_limiter = AsyncRateLimiter(8)
         self.gofile_limiter = AsyncRateLimiter(max_calls=1, period=2)
+        self.jpgfish_limiter = AsyncRateLimiter(10)
+        self.kemono_limiter = AsyncRateLimiter(8)
 
+        self.coomer_semaphore = asyncio.Semaphore(1)
+        self.cyberfile_semaphore = asyncio.Semaphore(2)
         self.gofile_semaphore = asyncio.Semaphore(1)
         self.jpgfish_semaphore = asyncio.Semaphore(5)
-        self.cyberfile_semaphore = asyncio.Semaphore(2)
+        self.kemono_semaphore = asyncio.Semaphore(1)
         self.nudostar_semaphore = asyncio.Semaphore(1)
         self.simpcity_semaphore = asyncio.Semaphore(1)
         self.socialmediagirls_semaphore = asyncio.Semaphore(1)
         self.xbunker_semaphore = asyncio.Semaphore(1)
 
         self.mapping = {"anonfiles": self.Anonfiles, "bayfiles": self.Anonfiles, "xbunkr": self.XBunkr,
                         "bunkr": self.Bunkr, "cyberdrop": self.Cyberdrop, "cyberfile": self.CyberFile,
@@ -298,16 +299,23 @@
 
     async def Coomeno(self, url: URL, title=None):
         coomeno_session = ScrapeSession(self.client)
         if not self.coomeno_crawler:
             self.coomeno_crawler = CoomenoCrawler(include_id=self.include_id, scraping_mapper=self,
                                                   separate_posts=self.separate_posts, SQL_Helper=self.SQL_Helper,
                                                   quiet=self.quiet)
-        async with self.coomeno_limiter:
-            cascade, new_title = await self.coomeno_crawler.fetch(coomeno_session, url)
+        assert url.host is not None
+        if "coomer" in url.host:
+            async with self.coomer_semaphore:
+                async with self.coomer_limiter:
+                    cascade, new_title = await self.coomeno_crawler.fetch(coomeno_session, url)
+        elif "kemono" in url.host:
+            async with self.kemono_semaphore:
+                async with self.kemono_limiter:
+                    cascade, new_title = await self.coomeno_crawler.fetch(coomeno_session, url)
         if not new_title or await cascade.is_empty():
             await coomeno_session.exit_handler()
             return
         if title:
             await cascade.append_title(title)
             await self.Forums.extend_thread(title, cascade)
         else:
@@ -320,62 +328,62 @@
         xenforo_session = ScrapeSession(self.client)
         if not self.xenforo_crawler:
             self.xenforo_crawler = XenforoCrawler(scraping_mapper=self, args=self.args, SQL_Helper=self.SQL_Helper,
                                                   quiet=self.quiet)
         title = None
         cascade = None
 
+        assert self.xenforo_crawler is not None and url.host is not None
         if "simpcity" in url.host:
             async with self.simpcity_semaphore:
                 cascade, title = await self.xenforo_crawler.fetch(xenforo_session, url)
         elif "socialmediagirls" in url.host:
             async with self.socialmediagirls_semaphore:
                 cascade, title = await self.xenforo_crawler.fetch(xenforo_session, url)
         elif "xbunker" in url.host:
             async with self.xbunker_semaphore:
                 cascade, title = await self.xenforo_crawler.fetch(xenforo_session, url)
         elif "nudostar" in url.host:
             async with self.nudostar_semaphore:
                 cascade, title = await self.xenforo_crawler.fetch(xenforo_session, url)
+
+        assert cascade is not None
         if not title or await cascade.is_empty():
             await xenforo_session.exit_handler()
             return
+
         await self.Forums.add_thread(title, cascade)
         await xenforo_session.exit_handler()
 
     """URL to Function Mapper"""
 
     async def is_skip_host(self, host: str) -> bool:
         if self.only_data.sites:
             return not any(site in host for site in self.only_data.sites)
         return any(site in host for site in self.skip_data.sites)
 
     async def map_url(self, url_to_map: URL, title=None, referer=None):
         if not url_to_map:
             return
         if not url_to_map.host:
-            await log(f"Not Supported: {str(url_to_map)}", quiet=self.quiet, style="yellow")
+            log(f"Not Supported: {str(url_to_map)}", quiet=self.quiet, style="yellow")
             return
 
         key = next((key for key in self.mapping if key in url_to_map.host), None)
         if key:
             if await self.is_skip_host(key):
-                await log(f"Skipping: {str(url_to_map)}", quiet=self.quiet, style="yellow")
+                log(f"Skipping: {str(url_to_map)}", quiet=self.quiet, style="yellow")
             else:
                 handler = self.mapping[key]
                 await handler(url=url_to_map, title=title)
             return
 
         if self.jdownloader.jdownloader_enable:
-            async with asyncio.Semaphore(1):
-                self.jdownloader.quiet = self.quiet
-                if not self.jdownloader.jdownloader_agent:
-                    await self.jdownloader.jdownloader_setup()
             await self.jdownloader.direct_unsupported_to_jdownloader(url_to_map, title)
 
         else:
-            await log(f"Not Supported: {str(url_to_map)}", quiet=self.quiet, style="yellow")
+            log(f"Not Supported: {str(url_to_map)}", quiet=self.quiet, style="yellow")
             if self.unsupported_output:
                 title = title.encode("ascii", "ignore")
                 title = title.decode().strip()
                 async with aiofiles.open(self.unsupported_file, mode='a') as f:
                     await f.write(f"{str(url_to_map)},{str(referer)},{title}\n")
```

### Comparing `cyberdrop-dl-4.1.16/cyberdrop_dl.egg-info/PKG-INFO` & `cyberdrop-dl-4.1.17/cyberdrop_dl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.1.16
+Version: 4.1.17
 Summary: Bulk downloader for multiple file hosts and forum sites
 Home-page: https://github.com/Jules-WinnfieldX/CyberDropDownloader
 Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com
 Project-URL: Bug Tracker, https://github.com/Jules-WinnfieldX/CyberDropDownloader/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -63,14 +63,15 @@
 | jpg.church<br/>jpg.fish | Albums: jpg.church/album/... <br> Direct Images: jpg.church/image/... <br> User Profile: jpg.church/#USER# <br> All User Albums: jpg.church/#USER#/albums                                                                              |
 | LoveFap                 | Albums: lovefap.com/a/... <br> Direct Images: s*.lovefap.com/content/photos/... <br> Videos: lovefap.com/video/...                                                                                                                     |
 | NSFW.XXX                | Profile: nsfw.xxx/user/... <br> Post: nsfw.xxx/post/...                                                                                                                                                                                |
 | PimpAndHost             | Albums: pimpandhost.com/album/... <br> Single Files: pimpandhost.com/image/...                                                                                                                                                         |
 | PixelDrain              | Albums: Pixeldrain.com/l/... <br> Single Files: Pixeldrain.com/u/...                                                                                                                                                                   |
 | Pixl                    | Albums: pixl.li/album/... <br> Direct Images: pixl.li/image/...  <br> User Profile: pixl.li/#USER# <br> All User Albums: pixl.li/#USER#/albums                                                                                         |
 | Postimg.cc              | Albums: postimg.cc/gallery/... <br> Direct Images: postimg.cc/...                                                                                                                                                                      |
+| NudoStar                | Thread: nudostar.com/forum/threads/...  <br> Continue from (will download this post and after): nudostar.com/forum/threads/...post-NUMBER                                                                                              |
 | SimpCity                | Thread: simpcity.st/threads/...  <br> Continue from (will download this post and after): simpcity.st/threads/...post-NUMBER                                                                                                            |
 | SocialMediaGirls        | Thread: forum.socialmediagirls.com/threads/...  <br> Continue from (will download this post and after): forum.socialmediagirls.com/threads/...post-NUMBER                                                                              |
 | XBunker                 | Thread: xbunker.nu/threads/...  <br> Continue from (will download this post and after): xbunker.nu/threads/...post-NUMBER                                                                                                              |
 | XBunkr                  | Album: xbunkr.com/a/... <br> Direct Links: media.xbunkr.com/...                                                                                                                                                                        |
 
 Reminder to leave the link full (include the https://)
 
@@ -168,14 +169,16 @@
 --throttle              this is a throttle between requests during the downloading phase, the number is in seconds
 
 --output-last-forum-post        outputs the last post of a forum scrape to use as a starting point for future runs
 --separate-posts                separates forum scraping into folders by post number
 
 --gofile-api-key                api key for premium gofile
 --pixeldrain-api-key            api key for premium pixeldrain
+--nudostar-username             username to login to nudostar
+--nudostar-password             password to login to nudostar
 --simpcity-username             username to login to simpcity
 --simpcity-password             password to login to simpcity
 --socialmediagirls-username     username to login to socialmediagirls
 --socialmediagirls-password     password to login to socialmediagirls
 --xbunker-username              username to login to xbunker
 --xbunker-password              password to login to xbunker
 
@@ -190,8 +193,8 @@
 --hide-thread-progress          removes thread progress section while downloading
 --hide-domain-progress          removes domain progress section while downloading
 --hide-album-progress           removes album progress section while downloading
 --hide-file-progress            removes file progress section while downloading
 --refresh-rate                  changes the refresh rate of the progress table
 ```
 
-`--only-hosts` and `--skip-hosts` can use: `"anonfiles", "bayfiles", "bunkr", "coomer.party", "cyberdrop", "cyberfile", "e-hentai", "erome", "fapello", "gfycat", "gallery.deltaporno.com", "gofile", "hgamecg", "img.kiwi", "imgbox", "jpg.church", "jpg.fish", "kemono.party", "lovefap", "nsfw.xxx", "pimpandhost", "pixeldrain", "pixl.li", "postimg", "saint", "simpcity", "socialmediagirls", "xbunker", "xbunkr"`
+`--only-hosts` and `--skip-hosts` can use: `"anonfiles", "bayfiles", "bunkr", "coomer.party", "cyberdrop", "cyberfile", "e-hentai", "erome", "fapello", "gfycat", "gallery.deltaporno.com", "gofile", "hgamecg", "img.kiwi", "imgbox", "jpg.church", "jpg.fish", "kemono.party", "lovefap", "nsfw.xxx", "nudostar", "pimpandhost", "pixeldrain", "pixl.li", "postimg", "saint", "simpcity", "socialmediagirls", "xbunker", "xbunkr"`
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.1.16 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.1.17 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
@@ -70,15 +70,18 @@
 Single Files: pimpandhost.com/image/... | | PixelDrain | Albums:
 Pixeldrain.com/l/...
 Single Files: Pixeldrain.com/u/... | | Pixl | Albums: pixl.li/album/...
 Direct Images: pixl.li/image/...
 User Profile: pixl.li/#USER#
 All User Albums: pixl.li/#USER#/albums | | Postimg.cc | Albums: postimg.cc/
 gallery/...
-Direct Images: postimg.cc/... | | SimpCity | Thread: simpcity.st/threads/...
+Direct Images: postimg.cc/... | | NudoStar | Thread: nudostar.com/forum/
+threads/...
+Continue from (will download this post and after): nudostar.com/forum/
+threads/...post-NUMBER | | SimpCity | Thread: simpcity.st/threads/...
 Continue from (will download this post and after): simpcity.st/threads/...post-
 NUMBER | | SocialMediaGirls | Thread: forum.socialmediagirls.com/threads/...
 Continue from (will download this post and after): forum.socialmediagirls.com/
 threads/...post-NUMBER | | XBunker | Thread: xbunker.nu/threads/...
 Continue from (will download this post and after): xbunker.nu/threads/...post-
 NUMBER | | XBunkr | Album: xbunkr.com/a/...
 Direct Links: media.xbunkr.com/... | Reminder to leave the link full (include
@@ -141,29 +144,31 @@
 wait attempting to connect to a URL during the downloading phase --ratelimit
 this applies to requests made in the program during scraping, the number you
 provide is in requests/seconds --throttle this is a throttle between requests
 during the downloading phase, the number is in seconds --output-last-forum-post
 outputs the last post of a forum scrape to use as a starting point for future
 runs --separate-posts separates forum scraping into folders by post number --
 gofile-api-key api key for premium gofile --pixeldrain-api-key api key for
-premium pixeldrain --simpcity-username username to login to simpcity --
-simpcity-password password to login to simpcity --socialmediagirls-username
-username to login to socialmediagirls --socialmediagirls-password password to
-login to socialmediagirls --xbunker-username username to login to xbunker --
-xbunker-password password to login to xbunker --apply-jdownloader enables
-sending unsupported URLs to a running jdownloader2 instance to download --
-jdownloader-username username to login to jdownloader --jdownloader-password
-password to login to jdownloader --jdownloader-device device name to login to
-for jdownloader --hide-new-progress disables the new rich progress entirely and
-uses older methods --hide-overall-progress removes overall progress section
-while downloading --hide-forum-progress removes forum progress section while
-downloading --hide-thread-progress removes thread progress section while
-downloading --hide-domain-progress removes domain progress section while
-downloading --hide-album-progress removes album progress section while
-downloading --hide-file-progress removes file progress section while
-downloading --refresh-rate changes the refresh rate of the progress table ```
-`--only-hosts` and `--skip-hosts` can use: `"anonfiles", "bayfiles", "bunkr",
-"coomer.party", "cyberdrop", "cyberfile", "e-hentai", "erome", "fapello",
-"gfycat", "gallery.deltaporno.com", "gofile", "hgamecg", "img.kiwi", "imgbox",
-"jpg.church", "jpg.fish", "kemono.party", "lovefap", "nsfw.xxx", "pimpandhost",
-"pixeldrain", "pixl.li", "postimg", "saint", "simpcity", "socialmediagirls",
-"xbunker", "xbunkr"`
+premium pixeldrain --nudostar-username username to login to nudostar --
+nudostar-password password to login to nudostar --simpcity-username username to
+login to simpcity --simpcity-password password to login to simpcity --
+socialmediagirls-username username to login to socialmediagirls --
+socialmediagirls-password password to login to socialmediagirls --xbunker-
+username username to login to xbunker --xbunker-password password to login to
+xbunker --apply-jdownloader enables sending unsupported URLs to a running
+jdownloader2 instance to download --jdownloader-username username to login to
+jdownloader --jdownloader-password password to login to jdownloader --
+jdownloader-device device name to login to for jdownloader --hide-new-progress
+disables the new rich progress entirely and uses older methods --hide-overall-
+progress removes overall progress section while downloading --hide-forum-
+progress removes forum progress section while downloading --hide-thread-
+progress removes thread progress section while downloading --hide-domain-
+progress removes domain progress section while downloading --hide-album-
+progress removes album progress section while downloading --hide-file-progress
+removes file progress section while downloading --refresh-rate changes the
+refresh rate of the progress table ``` `--only-hosts` and `--skip-hosts` can
+use: `"anonfiles", "bayfiles", "bunkr", "coomer.party", "cyberdrop",
+"cyberfile", "e-hentai", "erome", "fapello", "gfycat",
+"gallery.deltaporno.com", "gofile", "hgamecg", "img.kiwi", "imgbox",
+"jpg.church", "jpg.fish", "kemono.party", "lovefap", "nsfw.xxx", "nudostar",
+"pimpandhost", "pixeldrain", "pixl.li", "postimg", "saint", "simpcity",
+"socialmediagirls", "xbunker", "xbunkr"`
```

### Comparing `cyberdrop-dl-4.1.16/cyberdrop_dl.egg-info/SOURCES.txt` & `cyberdrop-dl-4.1.17/cyberdrop_dl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.16/setup.cfg` & `cyberdrop-dl-4.1.17/setup.cfg`

 * *Files identical despite different names*

