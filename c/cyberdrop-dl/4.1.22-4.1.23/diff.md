# Comparing `tmp/cyberdrop-dl-4.1.22.tar.gz` & `tmp/cyberdrop-dl-4.1.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyberdrop-dl-4.1.22.tar", last modified: Fri Apr 28 04:52:40 2023, max compression
+gzip compressed data, was "cyberdrop-dl-4.1.23.tar", last modified: Fri Apr 28 17:40:27 2023, max compression
```

## Comparing `cyberdrop-dl-4.1.22.tar` & `cyberdrop-dl-4.1.23.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 04:52:40.635170 cyberdrop-dl-4.1.22/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-04-28 04:52:40.635170 cyberdrop-dl-4.1.22/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16523 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 04:52:40.623169 cyberdrop-dl-4.1.22/cyberdrop_dl/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 04:52:40.627169 cyberdrop-dl-4.1.22/cyberdrop_dl/base_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/base_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/base_functions/base_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/base_functions/config_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/base_functions/config_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/base_functions/data_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/base_functions/error_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/base_functions/sorting_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12383 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/base_functions/sql_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 04:52:40.627169 cyberdrop-dl-4.1.22/cyberdrop_dl/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9523 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/client/rate_limiting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 04:52:40.635170 cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/Anonfiles_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     7493 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/Bunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/Coomeno_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    12064 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/CyberFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/EHentai_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/Erome_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/Fapello_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/Gfycat_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/GoFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/HGameCG_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/ImgBox_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/LoveFap_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/NSFWXXXCrawler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/PixelDrain_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/PostImg_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/Saint_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     8411 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/ShareX_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/XBunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    15075 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/Xenforo_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 04:52:40.635170 cyberdrop-dl-4.1.22/cyberdrop_dl/downloader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/downloader/downloader_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17390 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/downloader/downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    13871 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/downloader/old_downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/downloader/progress_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)    18626 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 04:52:40.635170 cyberdrop-dl-4.1.22/cyberdrop_dl/scraper/
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/scraper/JDownloader_Integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    20266 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/scraper/Scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/scraper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 04:52:40.627169 cyberdrop-dl-4.1.22/cyberdrop_dl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-04-28 04:52:40.000000 cyberdrop-dl-4.1.22/cyberdrop_dl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-28 04:52:40.000000 cyberdrop-dl-4.1.22/cyberdrop_dl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 04:52:40.000000 cyberdrop-dl-4.1.22/cyberdrop_dl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-28 04:52:40.000000 cyberdrop-dl-4.1.22/cyberdrop_dl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-28 04:52:40.000000 cyberdrop-dl-4.1.22/cyberdrop_dl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-28 04:52:40.000000 cyberdrop-dl-4.1.22/cyberdrop_dl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-28 04:52:40.635170 cyberdrop-dl-4.1.22/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:40:26.997600 cyberdrop-dl-4.1.23/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-04-28 17:40:26.997600 cyberdrop-dl-4.1.23/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16523 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:40:26.985599 cyberdrop-dl-4.1.23/cyberdrop_dl/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:40:26.989600 cyberdrop-dl-4.1.23/cyberdrop_dl/base_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/base_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/base_functions/base_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/base_functions/config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/base_functions/config_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/base_functions/data_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/base_functions/error_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/base_functions/sorting_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12389 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/base_functions/sql_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:40:26.989600 cyberdrop-dl-4.1.23/cyberdrop_dl/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9675 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/client/rate_limiting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:40:26.997600 cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/Anonfiles_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7493 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/Bunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/Coomeno_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12367 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/CyberFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/EHentai_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/Erome_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/Fapello_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/Gfycat_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/GoFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/HGameCG_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/ImgBox_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/LoveFap_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/NSFWXXXCrawler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/PixelDrain_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/PostImg_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/Saint_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8493 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/ShareX_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/XBunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15304 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/Xenforo_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:40:26.997600 cyberdrop-dl-4.1.23/cyberdrop_dl/downloader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/downloader/downloader_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17579 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/downloader/downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13993 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/downloader/old_downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/downloader/progress_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18663 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:40:26.997600 cyberdrop-dl-4.1.23/cyberdrop_dl/scraper/
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/scraper/JDownloader_Integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20272 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/scraper/Scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/cyberdrop_dl/scraper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:40:26.989600 cyberdrop-dl-4.1.23/cyberdrop_dl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-04-28 17:40:26.000000 cyberdrop-dl-4.1.23/cyberdrop_dl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-28 17:40:26.000000 cyberdrop-dl-4.1.23/cyberdrop_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 17:40:26.000000 cyberdrop-dl-4.1.23/cyberdrop_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-28 17:40:26.000000 cyberdrop-dl-4.1.23/cyberdrop_dl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-28 17:40:26.000000 cyberdrop-dl-4.1.23/cyberdrop_dl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-28 17:40:26.000000 cyberdrop-dl-4.1.23/cyberdrop_dl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-28 17:40:26.997600 cyberdrop-dl-4.1.23/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 17:40:16.000000 cyberdrop-dl-4.1.23/setup.py
```

### Comparing `cyberdrop-dl-4.1.22/LICENSE` & `cyberdrop-dl-4.1.23/LICENSE`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.22/PKG-INFO` & `cyberdrop-dl-4.1.23/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.1.22
+Version: 4.1.23
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
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.1.22 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.1.23 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
```

### Comparing `cyberdrop-dl-4.1.22/README.md` & `cyberdrop-dl-4.1.23/README.md`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.22/cyberdrop_dl/base_functions/base_functions.py` & `cyberdrop-dl-4.1.23/cyberdrop_dl/base_functions/base_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import logging
 import os
 import re
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Tuple
 
 import rich
 
 from cyberdrop_dl.base_functions.data_classes import MediaItem
 from cyberdrop_dl.base_functions.error_classes import NoExtensionFailure
 
 if TYPE_CHECKING:
@@ -92,15 +92,15 @@
     """Checks whether the given url is a direct link to a content item"""
     mapping_direct = [r'i.pixl.li', r'i..pixl.li', r'img-...cyberdrop...', r'f.cyberdrop...',
                       r'fs-...cyberdrop...', r'jpg.church/images/...', r'simp..jpg.church', r's..putmega.com',
                       r's..putme.ga', r'images..imgbox.com', r's..lovefap...', r'img.kiwi/images/']
     return any(re.search(domain, str(url)) for domain in mapping_direct)
 
 
-async def get_filename_and_ext(filename: str, forum: bool = False) -> tuple[str, str]:
+async def get_filename_and_ext(filename: str, forum: bool = False) -> Tuple[str, str]:
     """Returns the filename and extension of a given file, throws NoExtensionFailure if there is no extension"""
     filename_parts = filename.rsplit('.', 1)
     if len(filename_parts) == 1:
         raise NoExtensionFailure()
     if filename_parts[-1].isnumeric() and forum:
         filename_parts = filename_parts[0].rsplit('-', 1)
     ext = "." + filename_parts[-1].lower()
```

### Comparing `cyberdrop-dl-4.1.22/cyberdrop_dl/base_functions/config_manager.py` & `cyberdrop-dl-4.1.23/cyberdrop_dl/base_functions/config_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 from __future__ import annotations
 
 import copy
 from pathlib import Path
-from typing import Optional
+from typing import Optional, Union, Dict
 
 import yaml
 
 from cyberdrop_dl.base_functions.base_functions import log
 from cyberdrop_dl.base_functions.config_schema import config_default
 
 
-def _to_config_value(value):
+def _to_config_value(value) -> Union[str, int]:
     return str(value) if isinstance(value, Path) else value
 
 
-def _create_config(config: Path, passed_args: Optional[dict] = None, enabled=False) -> dict:
+def _create_config(config: Path, passed_args: Optional[dict] = None, enabled=False) -> Dict:
     """Creates the default config file, or remakes it with passed arguments"""
-    config_data: dict = config_default
+    config_data: Dict = config_default
     if passed_args:
         config_data["Apply_Config"] = enabled
         for group in config_data["Configuration"].values():
             for arg in group:
                 if arg in passed_args:
                     group[arg] = _to_config_value(passed_args[arg])
 
     with open(config, 'w') as yamlfile:
         yaml.dump(config_data, yamlfile)
 
     return config_data
 
 
-def _validate_config(config: Path) -> dict:
+def _validate_config(config: Path) -> Dict:
     """Validates the existing config file"""
     with open(config, "r") as yamlfile:
         config_data = yaml.load(yamlfile, Loader=yaml.FullLoader)
     try:
         data = config_data["Configuration"]
         enabled = config_data["Apply_Config"]
 
-        config_groups: dict = config_default["Configuration"]
+        config_groups: Dict = config_default["Configuration"]
         if all(set(group) <= set(data[group_name]) for group_name, group in config_groups.items()):
             return config_data
 
         config.unlink()
 
         args = {}
         for group_name in config_groups:
@@ -52,33 +52,33 @@
     except (KeyError, TypeError):
         config.unlink()
         config_data = _create_config(config)
 
     return config_data
 
 
-def run_args(config: Path, cmd_arg: dict) -> dict:
+def run_args(config: Path, cmd_arg: Dict) -> Dict:
     """Returns the proper runtime arguments based on the config and command line arguments"""
     data = _validate_config(config) if config.is_file() else _create_config(config, cmd_arg)
     if data['Apply_Config']:
         data = data["Configuration"]
         for file, path in data['Files'].items():
             data['Files'][file] = Path(path)
         data['Sorting']['sort_directory'] = Path(data['Sorting']['sort_directory'])
         return data
 
-    config_data: dict = config_default["Configuration"]
+    config_data: Dict = config_default["Configuration"]
     for group in config_data.values():
         for arg in group:
             if arg in cmd_arg:
                 group[arg] = cmd_arg[arg]
     return config_data
 
 
-async def document_args(args: dict) -> None:
+async def document_args(args: Dict) -> None:
     """We document the runtime arguments for debugging and troubleshooting, redacting sensitive information"""
     print_args = copy.deepcopy(args)
     print_args['Authentication']['xbunker_password'] = '!REDACTED!' if args['Authentication']['xbunker_password'] is not None else None
     print_args['Authentication']['socialmediagirls_password'] = '!REDACTED!' if args['Authentication']['socialmediagirls_password'] is not None else None
     print_args['Authentication']['simpcity_password'] = '!REDACTED!' if args['Authentication']['simpcity_password'] is not None else None
     print_args['Authentication']['nudostar_password'] = '!REDACTED!' if args['Authentication']['nudostar_password'] is not None else None
     print_args['Authentication']['pixeldrain_api_key'] = '!REDACTED!' if args['Authentication']['pixeldrain_api_key'] is not None else None
```

### Comparing `cyberdrop-dl-4.1.22/cyberdrop_dl/base_functions/config_schema.py` & `cyberdrop-dl-4.1.23/cyberdrop_dl/base_functions/config_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from __future__ import annotations
 
-config_default: dict = {
+from typing import Dict
+
+config_default: Dict = {
     "Apply_Config": False,
     "Configuration": {
         "Authentication": {
             "gofile_api_key": "",
             "pixeldrain_api_key": "",
             "nudostar_username": "",
             "nudostar_password": "",
```

### Comparing `cyberdrop-dl-4.1.22/cyberdrop_dl/base_functions/data_classes.py` & `cyberdrop-dl-4.1.23/cyberdrop_dl/base_functions/data_classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import asyncio
 from dataclasses import dataclass, field
-from typing import TYPE_CHECKING, ClassVar
+from typing import TYPE_CHECKING, ClassVar, List, Dict, Tuple
 
 if TYPE_CHECKING:
     from yarl import URL
 
 
 @dataclass
 class MediaItem:
@@ -24,15 +24,15 @@
         self.complete = True
 
 
 @dataclass
 class AlbumItem:
     """Class for keeping track of download links for each album"""
     title: str
-    media: list[MediaItem]
+    media: List[MediaItem]
 
     async def add_media(self, media_item: MediaItem) -> None:
         self.media.append(media_item)
 
     async def set_new_title(self, new_title: str) -> None:
         self.title = new_title
 
@@ -47,15 +47,15 @@
         return True if not self.media else False
 
 
 @dataclass
 class DomainItem:
     """Class for keeping track of albums for each scraper type"""
     domain: str
-    albums: dict
+    albums: Dict
 
     async def add_to_album(self, title: str, media: MediaItem) -> None:
         if title in self.albums:
             await self.albums[title].add_media(media)
         else:
             self.albums[title] = AlbumItem(title=title, media=[media])
 
@@ -93,15 +93,15 @@
             album.title = new_title
         self.albums = new_albums
 
 
 @dataclass
 class CascadeItem:
     """Class for keeping track of domains for each scraper type"""
-    domains: dict
+    domains: Dict
 
     async def add_albums(self, domain_item: DomainItem) -> None:
         domain = domain_item.domain
         albums = domain_item.albums
         for title, album in albums.items():
             await self.add_album(domain, title, album)
 
@@ -160,15 +160,15 @@
                     allowed.append(media_item)
                 album.media = allowed
 
 
 @dataclass
 class ForumItem:
     """Class for keeping track of forum threads"""
-    threads: dict
+    threads: Dict
 
     async def add_album_to_thread(self, title: str, domain: str, album: AlbumItem) -> None:
         if title not in self.threads:
             self.threads[title] = CascadeItem({domain: DomainItem(domain, {album.title: album})})
         else:
             await self.threads[title].add_album(domain, album.title, album)
 
@@ -213,15 +213,15 @@
         else:
             self.threads[title] = cascade
 
 
 @dataclass
 class FileLock:
     """Rudimentary file lock system"""
-    locked_files: list[str] = field(default_factory=list)
+    locked_files: List[str] = field(default_factory=list)
 
     async def check_lock(self, filename: str) -> bool:
         await asyncio.sleep(.1)
         return filename.lower() in self.locked_files
 
     async def add_lock(self, filename: str) -> None:
         self.locked_files.append(filename.lower())
@@ -229,15 +229,15 @@
     async def remove_lock(self, filename: str) -> None:
         self.locked_files.remove(filename.lower())
 
 
 @dataclass
 class SkipData:
     """The allows optoins for domains to skip when scraping"""
-    supported_hosts: ClassVar[tuple[str, ...]] = ("anonfiles", "bayfiles", "bunkr", "coomer.party", "cyberdrop",
+    supported_hosts: ClassVar[Tuple[str, ...]] = ("anonfiles", "bayfiles", "bunkr", "coomer.party", "cyberdrop",
                                                   "cyberfile", "e-hentai", "erome", "fapello", "gfycat", "gofile",
                                                   "hgamecg", "img.kiwi", "imgbox", "jpg.church", "jpg.fish",
                                                   "gallery.deltaporno.com", "kemono.party",
                                                   "lovefap", "nsfw.xxx", "pimpandhost", "pixeldrain", "pixl.li",
                                                   "postimg", "saint", "nudostar", "simpcity", "socialmediagirls",
                                                   "xbunker", "xbunkr")
-    sites: list[str]
+    sites: List[str]
```

### Comparing `cyberdrop-dl-4.1.22/cyberdrop_dl/base_functions/error_classes.py` & `cyberdrop-dl-4.1.23/cyberdrop_dl/base_functions/error_classes.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.22/cyberdrop_dl/base_functions/sorting_functions.py` & `cyberdrop-dl-4.1.23/cyberdrop_dl/base_functions/sorting_functions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.22/cyberdrop_dl/base_functions/sql_helper.py` & `cyberdrop-dl-4.1.23/cyberdrop_dl/base_functions/sql_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import atexit
 import logging
 import sqlite3
-from typing import TYPE_CHECKING, Optional
+from typing import TYPE_CHECKING, Optional, List
 
 if TYPE_CHECKING:
     from pathlib import Path
 
     from yarl import URL
 
     from cyberdrop_dl.base_functions.data_classes import (
@@ -116,15 +116,15 @@
             self.curs.execute(pre_alloc2)
             self.conn.commit()
             self.curs.execute(drop_pre)
             self.conn.commit()
 
     """Temp Table Operations"""
 
-    async def get_temp_names(self) -> list[str]:
+    async def get_temp_names(self) -> List[str]:
         """Gets the list of temp filenames"""
         self.curs.execute("SELECT downloaded_filename FROM downloads_temp;")
         filenames = self.curs.fetchall()
         return list(sum(filenames, ()))
 
     async def sql_insert_temp(self, downloaded_filename: str) -> None:
         """Inserts a temp filename into the downloads_temp table"""
```

### Comparing `cyberdrop-dl-4.1.22/cyberdrop_dl/client/client.py` & `cyberdrop-dl-4.1.23/cyberdrop_dl/client/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import asyncio
 import json
 import logging
 import ssl
 import time
 from http import HTTPStatus
-from typing import TYPE_CHECKING, Callable, Optional, Coroutine, Any
+from typing import TYPE_CHECKING, Callable, Optional, Coroutine, Any, Tuple, Dict
 
 import aiofiles
 import aiohttp
 import certifi
 from bs4 import BeautifulSoup
 from tqdm import tqdm
 from yarl import URL
@@ -55,57 +55,58 @@
 
 class ScrapeSession:
     """AIOHTTP operations for scraping"""
     def __init__(self, client: Client) -> None:
         self.client = client
         self.rate_limiter = AsyncRateLimiter(self.client.ratelimit)
         self.headers = {"user-agent": client.user_agent}
-        self.timeouts = aiohttp.ClientTimeout(total=5 * 60, connect=self.client.connect_timeout, sock_read=30)
+        self.timeouts = aiohttp.ClientTimeout(total=self.client.connect_timeout + 45,
+                                              connect=self.client.connect_timeout, sock_read=45)
         self.client_session = aiohttp.ClientSession(headers=self.headers, raise_for_status=True,
                                                     cookie_jar=self.client.cookies, timeout=self.timeouts)
 
     @scrape_limit
     async def get_BS4(self, url: URL) -> BeautifulSoup:
         async with self.client_session.get(url, ssl=self.client.ssl_context) as response:
             content_type = response.headers.get('Content-Type')
             assert content_type is not None
             if not any(s in content_type.lower() for s in ("html", "text")):
                 raise InvalidContentTypeFailure(message=f"Received {content_type}, was expecting text")
             text = await response.text()
             return BeautifulSoup(text, 'html.parser')
 
     @scrape_limit
-    async def get_BS4_and_url(self, url: URL) -> tuple[BeautifulSoup, URL]:
+    async def get_BS4_and_url(self, url: URL) -> Tuple[BeautifulSoup, URL]:
         async with self.client_session.get(url, ssl=self.client.ssl_context) as response:
             text = await response.text()
             soup = BeautifulSoup(text, 'html.parser')
             return soup, URL(response.url)
 
     @scrape_limit
-    async def get_json(self, url: URL, params: Optional[dict] = None) -> dict:
+    async def get_json(self, url: URL, params: Optional[Dict] = None) -> Dict:
         async with self.client_session.get(url, ssl=self.client.ssl_context, params=params) as response:
             return json.loads(await response.content.read())
 
     @scrape_limit
     async def get_text(self, url: URL) -> str:
         async with self.client_session.get(url, ssl=self.client.ssl_context) as response:
             return await response.text()
 
     @scrape_limit
-    async def post(self, url: URL, data: dict) -> dict:
+    async def post(self, url: URL, data: Dict) -> Dict:
         async with self.client_session.post(url, data=data, headers=self.headers, ssl=self.client.ssl_context) as response:
             return json.loads(await response.content.read())
 
     @scrape_limit
-    async def get_no_resp(self, url: URL, headers: dict) -> None:
+    async def get_no_resp(self, url: URL, headers: Dict) -> None:
         async with self.client_session.get(url, headers=headers, ssl=self.client.ssl_context):
             pass
 
     @scrape_limit
-    async def post_data_no_resp(self, url: URL, data: dict) -> None:
+    async def post_data_no_resp(self, url: URL, data: Dict) -> None:
         async with self.client_session.post(url, data=data, headers=self.headers, ssl=self.client.ssl_context):
             pass
 
     async def exit_handler(self) -> None:
         try:
             await self.client_session.close()
         except Exception:
@@ -113,30 +114,30 @@
 
 
 class DownloadSession:
     """AIOHTTP operations for downloading"""
     def __init__(self, client: Client):
         self.client = client
         self.headers = {"user-agent": client.user_agent}
-        self.timeouts = aiohttp.ClientTimeout(total=5 * 60, connect=self.client.connect_timeout)
-        self.client_session = aiohttp.ClientSession(headers=self.headers, raise_for_status=True, cookie_jar=self.client.cookies, timeout=self.timeouts)
-        self.throttle_times: dict[str, float] = {}
-
+        self.timeouts = aiohttp.ClientTimeout(total=None, connect=self.client.connect_timeout, sock_read=None)
+        self.client_session = aiohttp.ClientSession(headers=self.headers, raise_for_status=True,
+                                                    cookie_jar=self.client.cookies, timeout=self.timeouts)
+        self.throttle_times: Dict[str, float] = {}
         self.bunkr_maintenance = [URL("https://bnkr.b-cdn.net/maintenance-vid.mp4"), URL("https://bnkr.b-cdn.net/maintenance.mp4")]
 
     async def _append_content(self, file: Path, content: aiohttp.StreamReader,
                               update_progress: Callable[[int], Optional[bool]]) -> None:
         file.parent.mkdir(parents=True, exist_ok=True)
         async with aiofiles.open(file, mode='ab') as f:
             async for chunk, _ in content.iter_chunks():
                 await asyncio.sleep(0)
                 await f.write(chunk)
                 update_progress(len(chunk))
 
-    async def _download(self, media: MediaItem, current_throttle: float, proxy: str, headers: dict,
+    async def _download(self, media: MediaItem, current_throttle: float, proxy: str, headers: Dict,
                         save_content: Callable[[aiohttp.StreamReader, int], Coroutine[Any, Any, None]]) -> None:
         headers['Referer'] = str(media.referer)
         headers['user-agent'] = self.client.user_agent
 
         assert media.url.host is not None
         await self._throttle(current_throttle, media.url.host)
 
@@ -169,35 +170,35 @@
                 self.throttle_times[key] = now
                 return
 
             remaining = delay - elapsed + 0.1
             await asyncio.sleep(remaining)
 
     async def download_file(self, media: MediaItem, file: Path, current_throttle: float, resume_point: int,
-                            proxy: str, headers: dict, file_task: TaskID) -> None:
+                            proxy: str, headers: Dict, file_task: TaskID) -> None:
 
         async def save_content(content: aiohttp.StreamReader, size: int) -> None:
             file_progress.update(file_task, total=size + resume_point)
             file_progress.advance(file_task, resume_point)
             await self._append_content(file, content, lambda chunk_len: file_progress.advance(file_task, chunk_len))
 
         await self._download(media, current_throttle, proxy, headers, save_content)
 
     async def old_download_file(self, media: MediaItem, file: Path, current_throttle: float, resume_point: int,
-                                proxy: str, headers: dict):
+                                proxy: str, headers: Dict):
 
         async def save_content(content: aiohttp.StreamReader, size: int) -> None:
             task_description = await adjust(f"{media.url.host}: {media.filename}")
             with tqdm(total=size + resume_point, unit_scale=True, unit='B', leave=False,
                       initial=resume_point, desc=task_description) as progress:
                 await self._append_content(file, content, lambda chunk_len: progress.update(chunk_len))
 
         await self._download(media, current_throttle, proxy, headers, save_content)
 
-    async def get_filesize(self, url: URL, referer: str, current_throttle: int) -> int:
+    async def get_filesize(self, url: URL, referer: str, current_throttle: float) -> int:
         headers = {'Referer': referer, 'user-agent': self.client.user_agent}
 
         assert url.host is not None
         await self._throttle(current_throttle, url.host)
         async with self.client_session.get(url, headers=headers, ssl=self.client.ssl_context,
                                            raise_for_status=True) as resp:
             return int(resp.headers.get('Content-Length', str(0)))
```

### Comparing `cyberdrop-dl-4.1.22/cyberdrop_dl/client/rate_limiting.py` & `cyberdrop-dl-4.1.23/cyberdrop_dl/client/rate_limiting.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/Anonfiles_Spider.py` & `cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/Anonfiles_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/Bunkr_Spider.py` & `cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/Bunkr_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/Coomeno_Spider.py` & `cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/Coomeno_Spider.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import asyncio
 from dataclasses import dataclass, field
-from typing import TYPE_CHECKING, Union
+from typing import TYPE_CHECKING, Union, List
 
 from bs4 import BeautifulSoup
 from yarl import URL
 
 from ..base_functions.base_functions import create_media_item, log, logger, make_title_safe
 from ..base_functions.data_classes import CascadeItem
 
@@ -17,15 +17,15 @@
     from ..client.client import ScrapeSession
 
 
 @dataclass
 class ParseSpec:
     """Class for specific selectors of supported domains"""
     domain: str
-    posts_selectors: list[str] = field(init=False)
+    posts_selectors: List[str] = field(init=False)
     next_page_selector: str = field(init=False)
 
     def __post_init__(self):
         if self.domain == "coomer":
             self.posts_selectors = ['h2[class=post-card__heading] a']
             self.next_page_selector = 'a[title="Next page"]'
         elif self.domain == "kemono":
@@ -78,15 +78,15 @@
             title = await self.parse_post(session, url, domain, cascade)
 
         else:
             title = await self.parse_profile(session, url, ParseSpec(domain), cascade)
 
         return title
 
-    async def map_links(self, text_content: list, title: str, referer: URL):
+    async def map_links(self, text_content: List, title: str, referer: URL):
         """Maps external links to other scrapers"""
         tasks = []
         for content in text_content:
             link = URL(content.get('href'))
             tasks.append(asyncio.create_task(self.scraping_mapper.map_url(link, title, referer)))
         if tasks:
             await asyncio.wait(tasks)
@@ -163,15 +163,15 @@
             log(f"Error: {str(url)}", quiet=self.quiet, style="red")
             logger.debug(e)
 
         return title
 
     async def parse_tag(self, tag: Tag, url: URL, domain: str, title: str, cascade: CascadeItem):
         """Convert link from tag to MediaItem and add it to cascade"""
-        href: Union[str, list[str], None] = tag.get('href')
+        href: Union[str, List[str], None] = tag.get('href')
 
         assert url.host is not None and isinstance(href, str)
         if href.startswith("/"):
             href = "https://" + url.host + href
         link = URL(href)
         media_item = await create_media_item(link, url, self.SQL_Helper, domain)
         await cascade.add_to_album(domain, title, media_item)
```

### Comparing `cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/CyberFile_Spider.py` & `cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/CyberFile_Spider.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 import contextlib
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Optional, Tuple, List
 
 from bs4 import BeautifulSoup
 from yarl import URL
 
 from ..base_functions.base_functions import create_media_item, log, logger, make_title_safe
 from ..base_functions.data_classes import DomainItem
 from ..base_functions.error_classes import NoExtensionFailure
@@ -47,15 +47,15 @@
 
         for title, media_item in download_links:
             await domain_obj.add_media(title, media_item)
         await self.SQL_Helper.insert_domain("cyberfile", url, domain_obj)
         log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
         return domain_obj
 
-    async def get_folder_id(self, session: ScrapeSession, url: URL):
+    async def get_folder_id(self, session: ScrapeSession, url: URL) -> int:
         """Gets the internal ID for a folder"""
         try:
             soup = await session.get_BS4(url)
             script_func = soup.select_one('div[class="page-container horizontal-menu with-sidebar fit-logo-with-sidebar logged-out clear-adblock"] script').text
             script_func = script_func.split('loadImages(')[-1]
             script_func = script_func.split(';')[0]
             nodeId = int(script_func.split(',')[1].replace("'", ""))
@@ -63,15 +63,15 @@
 
         except Exception as e:
             logger.debug("Error encountered while handling %s", str(url), exc_info=True)
             log(f"Error: {str(url)}", quiet=self.quiet, style="red")
             logger.debug(e)
             return 0
 
-    async def get_folder_content(self, session, url: URL, nodeId, page, title=None):
+    async def get_folder_content(self, session: ScrapeSession, url: URL, nodeId: int, page: int, title=None):
         """Gets the content id's encased in a folder"""
         data = {"pageType": "folder", "nodeId": nodeId, "pageStart": page, "perPage": 0, "filterOrderBy": ""}
         nodes = []
         contents = []
         try:
             content = await session.post(self.load_files, data)
             text = content['html']
@@ -88,55 +88,60 @@
             pages_str = pages_tag.get('onclick')
             assert isinstance(pages_str, str)
             total_pages = int(pages_str.split(',')[2])
             listings = soup.select("div[class=fileListing] div")
             for listing in listings:
                 with contextlib.suppress(TypeError):
                     folder_id = listing.get('folderid')
+                    if not folder_id:
+                        continue
                     assert isinstance(folder_id, str)
                     nodes.append(int(folder_id))
 
+            for listing in listings:
                 with contextlib.suppress(TypeError):
                     file_id = listing.get('fileid')
+                    if not file_id:
+                        continue
                     assert isinstance(file_id, str)
                     contents.append((title, int(file_id)))
 
             if page < total_pages:
                 contents.extend(await self.get_folder_content(session, url, nodeId, page+1, original_title))
             for node in nodes:
                 contents.extend(await self.get_folder_content(session, url, node, 1, title))
             return contents
 
         except Exception as e:
             log(f"Error: {str(url)}", quiet=self.quiet, style="red")
             logger.debug(e)
             return []
 
-    async def get_single_contentId(self, session: ScrapeSession, url: URL):
+    async def get_single_contentId(self, session: ScrapeSession, url: URL) -> int:
         """Gets an individual content id"""
         try:
             soup = await session.get_BS4(url)
             script_funcs = soup.select('script')
             for script in script_funcs:
                 script_text = script.text
                 if script_text and "showFileInformation" in script_text:
                     part_a = script_text.split("showFileInformation(")
                     part_a = [x for x in part_a if x[0].isdigit()][0]
                     part_b = part_a.split(");")[0]
                     contentId = int(part_b)
                     return contentId
-            return None
+            return 0
 
         except Exception as e:
             logger.debug("Error encountered while handling %s", str(url), exc_info=True)
             log(f"Error: {str(url)}", quiet=self.quiet, style="red")
             logger.debug(e)
             return 0
 
-    async def get_shared_ids_and_content(self, session: ScrapeSession, url: URL, page):
+    async def get_shared_ids_and_content(self, session: ScrapeSession, url: URL, page: int) -> Tuple[List, List]:
         """Gets folder id's and content id's from shared links"""
         try:
             # Initial page load to tell server, this is what we want.
             await session.get_no_resp(url, {'referer': str(url), "user-agent": session.client.user_agent})
 
             # get the content listings
             data = {"pageType": "nonaccountshared", "nodeId": '', "pageStart": page, "perPage": 0, "filterOrderBy": ""}
@@ -175,17 +180,17 @@
                 contents.extend(content_temp)
             return nodes, contents
 
         except Exception as e:
             logger.debug("Error encountered while handling %s", str(url), exc_info=True)
             log(f"Error: {str(url)}", quiet=self.quiet, style="red")
             logger.debug(e)
-            return []
+            return [], []
 
-    async def get_shared_content(self, session, url: URL, nodeId, page, title=None):
+    async def get_shared_content(self, session, url: URL, nodeId: int, page: int, title=None) -> List:
         """Gets content from shared folders"""
         try:
             nodes = []
             contents = []
             data = {"pageType": "nonaccountshared", "nodeId": nodeId, "pageStart": page, "perPage": 0, "filterOrderBy": ""}
 
             content = await session.post(self.load_files, data)
@@ -222,32 +227,33 @@
 
         except Exception as e:
             logger.debug("Error encountered while handling %s", str(url), exc_info=True)
             log(f"Error: {str(url)}", quiet=self.quiet, style="red")
             logger.debug(e)
             return []
 
-    async def get_download_links(self, session, url, contentIds):
+    async def get_download_links(self, session: ScrapeSession, url: URL, contentIds: List) -> List:
         """Obtains download links from content ids"""
         download_links = []
         try:
             for title, contentId in contentIds:
                 data = {"u": contentId}
                 content = await session.post(self.file_details, data)
                 text = content['html']
                 soup = BeautifulSoup(text.replace("\\", ""), 'html.parser')
                 menu = soup.select_one('ul[class="dropdown-menu dropdown-info account-dropdown-resize-menu"] li a')
                 button = soup.select_one('div[class="btn-group responsiveMobileMargin"] button')
 
                 if menu:
                     html_download_text = menu.get("onclick")
-                    link = URL(html_download_text.replace("openUrl('", "").replace("'); return false;", ""))
-                elif button:
+                else:
+                    assert button is not None
                     html_download_text = button.get("onclick")
-                    link = URL(html_download_text.replace("openUrl('", "").replace("'); return false;", ""))
+                assert isinstance(html_download_text, str)
+                link = URL(html_download_text.replace("openUrl('", "").replace("'); return false;", ""))
                 try:
                     media = await create_media_item(link, url, self.SQL_Helper, "cyberfile")
                 except NoExtensionFailure:
                     logger.debug("Couldn't get extension for %s", str(link))
                     continue
 
                 download_links.append((title, media))
```

### Comparing `cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/Cyberdrop_Spider.py` & `cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/Cyberdrop_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/EHentai_Spider.py` & `cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/EHentai_Spider.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
             next_page_opts = soup.select('td[onclick="document.location=this.firstChild.href"]')
             next_page = None
             for maybe_next in next_page_opts:
                 if maybe_next.get_text() == ">":
                     next_page = maybe_next.select_one('a')
                     break
             if next_page is not None:
-                next_page = next_page.get('href')
+                next_page = URL(next_page.get('href'))
                 if next_page is not None:
                     await self.get_album(session, next_page, album_obj)
 
         except Exception as e:
             logger.debug("Error encountered while handling %s", str(url), exc_info=True)
             log(f"Error: {str(url)}", quiet=self.quiet, style="red")
             logger.debug(e)
```

### Comparing `cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/Erome_Spider.py` & `cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/Erome_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/Fapello_Spider.py` & `cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/Fapello_Spider.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
             # Fapello does circular looped paging
             if returned_url != url:
                 return album_obj
 
             content_section = soup.select_one("div[id=content]")
             posts = content_section.select("a")
             for post in posts:
-                link = post.get('href')
+                link = URL(post.get('href'))
                 if link:
                     media_items = await self.parse_post(session, link)
                     for media in media_items:
                         await album_obj.add_media(media)
 
             next_page = soup.select_one('div[id="next_page"] a')
             if next_page:
```

### Comparing `cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/Gfycat_Spider.py` & `cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/Gfycat_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/GoFile_Spider.py` & `cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/GoFile_Spider.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 import http
-from typing import TYPE_CHECKING, Union
+from typing import TYPE_CHECKING, Union, List, Dict
 
 from yarl import URL
 
 from ..base_functions.base_functions import log, logger, make_title_safe, get_filename_and_ext
 from ..base_functions.data_classes import DomainItem, MediaItem
 from ..base_functions.error_classes import NoExtensionFailure
 
@@ -67,17 +67,17 @@
         except Exception as e:
             logger.debug("Error encountered while handling %s", str(url), exc_info=True)
             log(f"Error: {str(url)}", quiet=self.quiet, style="red")
             logger.debug(e)
 
         return domain_obj
 
-    async def get_links(self, session: ScrapeSession, url: URL, content_id: str, title=None) -> list[list]:
+    async def get_links(self, session: ScrapeSession, url: URL, content_id: str, title=None) -> List[List]:
         """Gets links from the given url, creates media_items"""
-        results: list[list] = []
+        results: List[List] = []
         params = {
             "token": self.token,
             "contentId": content_id,
             "websiteToken": "12345",
         }
         content = await session.get_json(self.api_address / "getContent", params)
         if content["status"] != "ok":
@@ -87,15 +87,15 @@
 
         content = content['data']
         if title:
             title = title + "/" + await make_title_safe(content["name"])
         else:
             title = await make_title_safe(content["name"])
 
-        contents: dict[str, dict[str, Union[str, int]]] = content["contents"]
+        contents: Dict[str, Dict[str, Union[str, int]]] = content["contents"]
         sub_folders = []
         for val in contents.values():
             if val["type"] == "folder":
                 sub_folders.append(val['code'])
             else:
                 assert isinstance(val['name'], str)
                 if val["link"] == "overloaded":
```

### Comparing `cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/HGameCG_Spider.py` & `cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/HGameCG_Spider.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
         log(f"Starting: {str(url)}", quiet=self.quiet, style="green")
         await self.get_album(session, url, album_obj)
         log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
         await self.SQL_Helper.insert_album("hgamecg", url, album_obj)
         return album_obj
 
-    async def get_album(self, session: ScrapeSession, url: URL, album_obj: AlbumItem):
+    async def get_album(self, session: ScrapeSession, url: URL, album_obj: AlbumItem) -> None:
         """Handles album scraping, adds media items to the album_obj"""
         try:
             soup = await session.get_BS4(url)
             title = await make_title_safe(soup.select_one("div[class=navbar] h1").get_text())
             await album_obj.set_new_title(title)
 
             images = soup.select("div[class=image] a")
@@ -53,16 +53,17 @@
                     await self.get_album(session, next_page, album_obj)
 
         except Exception as e:
             logger.debug("Error encountered while handling %s", str(url), exc_info=True)
             log(f"Error: {str(url)}", quiet=self.quiet, style="red")
             logger.debug(e)
 
-    async def get_image(self, session: ScrapeSession, url: URL):
+    async def get_image(self, session: ScrapeSession, url: URL) -> URL:
         """Gets image link from the given url."""
         try:
             soup = await session.get_BS4(url)
             image = soup.select_one("div[class=hgamecgimage] img")
             image = URL(image.get('src'))
             return image
         except Exception:
             log(f"Error: {str(url)}", quiet=self.quiet, style="red")
+            return URL()
```

### Comparing `cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/ImgBox_Spider.py` & `cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/ImgBox_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/LoveFap_Spider.py` & `cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/LoveFap_Spider.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,15 @@
             logger.debug(e)
             return album_obj
 
         await self.SQL_Helper.insert_album("lovefap", url, album_obj)
         log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
         return album_obj
 
-    async def fetch_album(self, session: ScrapeSession, url: URL, album_obj: AlbumItem):
+    async def fetch_album(self, session: ScrapeSession, url: URL, album_obj: AlbumItem) -> None:
         """Gets media_items for albums, and adds them to the Album_obj"""
         soup = await session.get_BS4(url)
 
         title = soup.select_one('div[class=albums-content-header] span[style*="float: left"]').get_text()
         if title is None:
             title = url.name
         title = await make_title_safe(title)
@@ -76,15 +76,15 @@
                     media = await create_media_item(link, url, self.SQL_Helper, "lovefap")
                 except NoExtensionFailure:
                     logger.debug("Couldn't get extension for %s", str(link))
                     continue
 
                 await album_obj.add_media(media)
 
-    async def fetch_video(self, session: ScrapeSession, url: URL, album_obj: AlbumItem):
+    async def fetch_video(self, session: ScrapeSession, url: URL, album_obj: AlbumItem) -> None:
         """Gets media_items for video links"""
         soup = await session.get_BS4(url)
         video = soup.select_one("video[id=main-video] source")
         if video:
             link = URL(video.get("src"))
             try:
                 media = await create_media_item(link, url, self.SQL_Helper, "lovefap")
```

### Comparing `cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/NSFWXXXCrawler.py` & `cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/NSFWXXXCrawler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 import itertools
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, List
 
 from yarl import URL
 
 from ..base_functions.base_functions import create_media_item, log, logger, make_title_safe
 from ..base_functions.data_classes import DomainItem
 from ..base_functions.error_classes import NoExtensionFailure
 
@@ -28,15 +28,15 @@
         if "user" in url.parts:
             await self.get_user(session, url, domain_obj)
         else:
             await self.get_post(session, url, domain_obj)
         await self.SQL_Helper.insert_domain("nsfw.xxx", url, domain_obj)
         return domain_obj
 
-    async def get_user(self, session: ScrapeSession, url: URL, domain_obj: DomainItem):
+    async def get_user(self, session: ScrapeSession, url: URL, domain_obj: DomainItem) -> None:
         """Gets posts for a user profile"""
         try:
             model = url.name + " (NSFW.XXX)"
             for page in itertools.count(1):
                 model_name_parts = url.path.split("/")
                 model_name = list(filter(None, model_name_parts))[-1]
                 page_url = URL(f"https://nsfw.xxx/page/{page}?nsfw[]=0&types[]=image&types[]=video&types[]=gallery&slider=1&jsload=1&user={model_name}")
@@ -54,24 +54,24 @@
                     await self.get_post(session, post, domain_obj, model)
 
         except Exception as e:
             logger.debug("Error encountered while handling %s", str(url), exc_info=True)
             log(f"Error: {str(url)}", quiet=self.quiet, style="red")
             logger.debug(e)
 
-    async def get_post_hrefs(self, posts):
+    async def get_post_hrefs(self, posts) -> List:
         """Gets links from post objects"""
         posts_links = []
         for post in posts:
             url = URL(post.get("href"))
             if url not in posts_links:
                 posts_links.append(url)
         return posts_links
 
-    async def get_post(self, session: ScrapeSession, url: URL, domain_obj: DomainItem, model=None):
+    async def get_post(self, session: ScrapeSession, url: URL, domain_obj: DomainItem, model=None) -> None:
         """Gets content for a given post url"""
         try:
             soup = await session.get_BS4(url)
             if not model:
                 model = await make_title_safe(soup.select_one("a[class=sh-section__name]").get_text()) + " (NSFW.XXX)"
             post_name = await make_title_safe(soup.select_one("div[class=sh-section__content] p").get_text())
```

### Comparing `cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/PimpAndHost_Spider.py` & `cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/PimpAndHost_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/PixelDrain_Spider.py` & `cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/PixelDrain_Spider.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, List
 
 from yarl import URL
 
 from ..base_functions.base_functions import get_filename_and_ext, log, logger
 from ..base_functions.data_classes import AlbumItem, MediaItem
 from ..base_functions.error_classes import NoExtensionFailure
 
@@ -37,15 +37,15 @@
             media_item = MediaItem(link, url, complete, filename, ext, filename)
             await album_obj.add_media(media_item)
 
         await self.SQL_Helper.insert_album("pixeldrain", url, album_obj)
         log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
         return album_obj
 
-    async def get_listings(self, session: ScrapeSession, identifier: str, url: URL) -> list[MediaItem]:
+    async def get_listings(self, session: ScrapeSession, identifier: str, url: URL) -> List[MediaItem]:
         """Handles album scraping"""
         media_items = []
         try:
             content = await session.get_json(self.api / "list" / identifier)
             for file in content['files']:
                 link = await self.create_download_link(file['id'])
                 try:
```

### Comparing `cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/PostImg_Spider.py` & `cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/PostImg_Spider.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import itertools
 from http import HTTPStatus
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, List
 
 from yarl import URL
 
 from ..base_functions.base_functions import create_media_item, log, logger
 from ..base_functions.data_classes import AlbumItem, MediaItem
 from ..base_functions.error_classes import NoExtensionFailure
 
@@ -39,15 +39,15 @@
             log(f"Error: {str(url)}", quiet=self.quiet, style="red")
             logger.debug(e)
 
         await self.SQL_Helper.insert_album("postimg", url, album_obj)
         log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
         return album_obj
 
-    async def get_folder(self, session: ScrapeSession, url: URL):
+    async def get_folder(self, session: ScrapeSession, url: URL) -> List:
         """Handles folder scraping"""
         album = url.raw_name
         data = {"action": "list", "album": album, "page": 0}
         content = []
         for i in itertools.count(1):
             data["page"] = i
             data_out = await session.post(URL("https://postimg.cc/json"), data)
```

### Comparing `cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/Saint_Spider.py` & `cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/Saint_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/ShareX_Spider.py` & `cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/ShareX_Spider.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         log(f"Finished: {str(url)}", quiet=self.quiet, style="green")
         return domain_obj
 
     async def jpg_fish_from_church(self, url: URL) -> URL:
         pattern = r"simp([1-5])\.jpg\.church/"
         return URL(re.sub(pattern, r'simp\1.jpg.fish/', str(url)))
 
-    async def get_albums(self, session: ScrapeSession, url: URL, domain_obj: DomainItem):
+    async def get_albums(self, session: ScrapeSession, url: URL, domain_obj: DomainItem) -> None:
         """Handles scraping for Albums"""
         try:
             soup = await session.get_BS4(url)
             albums = soup.select("a[class='image-container --media']")
             for album in albums:
                 album_url = URL(album.get('href'))
                 await self.parse(session=session, url=album_url, domain_obj=domain_obj)
@@ -75,15 +75,15 @@
                     await self.get_albums(session, next_page, domain_obj)
 
         except Exception as e:
             logger.debug("Error encountered while handling %s", str(url), exc_info=True)
             log(f"Error: {str(url)}", quiet=self.quiet, style="red")
             logger.debug(e)
 
-    async def get_singular(self, session: ScrapeSession, url: URL, domain_obj: DomainItem):
+    async def get_singular(self, session: ScrapeSession, url: URL, domain_obj: DomainItem) -> None:
         """Handles scraping for singular files"""
         await asyncio.sleep(1)
         try:
             soup = await session.get_BS4(url)
             link = URL(soup.select_one("input[id=embed-code-2]").get('value'))
             link = link.with_name(link.name.replace('.md.', '.').replace('.th.', '.'))
             link = await self.jpg_fish_from_church(link)
@@ -91,29 +91,30 @@
             media_item = await create_media_item(link, url, self.SQL_Helper, "sharex")
             await domain_obj.add_media("Loose ShareX Files", media_item)
         except Exception as e:
             logger.debug("Error encountered while handling %s", str(url), exc_info=True)
             log(f"Error: {str(url)}", quiet=self.quiet, style="red")
             logger.debug(e)
 
-    async def get_sub_album_links(self, session: ScrapeSession, url: URL, og_title: str, domain_obj: DomainItem):
+    async def get_sub_album_links(self, session: ScrapeSession, url: URL, og_title: str,
+                                  domain_obj: DomainItem) -> None:
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
             log(f"Error: {str(url)}", quiet=self.quiet, style="red")
             logger.debug(e)
 
-    async def parse_profile(self, session: ScrapeSession, url: URL, domain_obj: DomainItem):
+    async def parse_profile(self, session: ScrapeSession, url: URL, domain_obj: DomainItem) -> None:
         """Handles scraping for profiles"""
         try:
             soup = await session.get_BS4(url)
             title = soup.select_one("div[class=header] h1 strong").get_text()
             if title is None:
                 title = url.name
             elif self.include_id:
@@ -123,15 +124,15 @@
             await self.get_list_links(session, url, title, domain_obj)
 
         except Exception as e:
             logger.debug("Error encountered while handling %s", str(url), exc_info=True)
             log(f"Error: {str(url)}", quiet=self.quiet, style="red")
             logger.debug(e)
 
-    async def get_list_links(self, session: ScrapeSession, url: URL, title: str, domain_obj: DomainItem):
+    async def get_list_links(self, session: ScrapeSession, url: URL, title: str, domain_obj: DomainItem) -> None:
         """Gets final links and adds to domain_obj"""
         try:
             soup = await session.get_BS4(url)
             assert url.host is not None
             if 'jpg.fish' in url.host or 'jpg.church' in url.host:
                 links = soup.select("a[href*=img] img")
             else:
@@ -157,15 +158,15 @@
                     next_page = URL(next_page)
                     await self.get_list_links(session, next_page, title, domain_obj)
         except Exception as e:
             logger.debug("Error encountered while handling %s", str(url), exc_info=True)
             log(f"Error: {str(url)}", quiet=self.quiet, style="red")
             logger.debug(e)
 
-    async def parse(self, *, session: ScrapeSession, url: URL, og_title=None, domain_obj: DomainItem):
+    async def parse(self, *, session: ScrapeSession, url: URL, og_title=None, domain_obj: DomainItem) -> None:
         try:
             soup = await session.get_BS4(url)
 
             title = soup.select_one("a[data-text=album-name]").get_text()
             if title is None:
                 title = url.name
             elif self.include_id:
```

### Comparing `cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/XBunkr_Spider.py` & `cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/XBunkr_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/Xenforo_Spider.py` & `cyberdrop-dl-4.1.23/cyberdrop_dl/crawlers/Xenforo_Spider.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from __future__ import annotations
 
 import asyncio
 import re
 from dataclasses import dataclass, field
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Dict, Tuple, List
 
 import aiofiles
+import bs4
 from bs4 import BeautifulSoup
 from yarl import URL
 
 from ..base_functions.base_functions import (
     get_filename_and_ext,
     log,
     logger,
@@ -76,15 +77,15 @@
 class ForumLogin:
     def __init__(self, name: str, username: str, password: str):
         self.name = name
         self.logged_in = False
         self.username = username
         self.password = password
 
-    async def login(self, session: ScrapeSession, url: URL, quiet: bool):
+    async def login(self, session: ScrapeSession, url: URL, quiet: bool) -> None:
         """Handles forum logging in"""
         if not self.username or not self.password:
             log(f"Login wasn't provided for {self.name}", quiet=quiet, style="red")
             raise FailedLoginFailure()
         attempt = 0
         while True:
             try:
@@ -125,15 +126,15 @@
                 attempt += 1
                 continue
 
 
 class XenforoCrawler:
     domains = ("nudostar", "simpcity", "socialmediagirls", "xbunker")
 
-    def __init__(self, *, scraping_mapper, args: dict, SQL_Helper: SQLHelper, quiet: bool):
+    def __init__(self, *, scraping_mapper, args: Dict, SQL_Helper: SQLHelper, quiet: bool):
         self.include_id = args["Runtime"]["include_id"]
         self.quiet = quiet
         self.separate_posts = args["Forum_Options"]["separate_posts"]
         self.output_last = args["Forum_Options"]["output_last_forum_post"]
         self.output_last_file = args["Files"]["output_last_forum_post_file"]
 
         self.nudostar = ForumLogin("NudoStar",
@@ -151,15 +152,15 @@
         self.xbunker = ForumLogin("XBunker",
                                   args["Authentication"]["xbunker_username"],
                                   args["Authentication"]["xbunker_password"])
 
         self.scraping_mapper = scraping_mapper
         self.SQL_Helper = SQL_Helper
 
-    async def fetch(self, session: ScrapeSession, url: URL) -> tuple[CascadeItem, str]:
+    async def fetch(self, session: ScrapeSession, url: URL) -> Tuple[CascadeItem, str]:
         """Xenforo forum director"""
         log(f"Starting: {str(url)}", quiet=self.quiet, style="green")
         cascade = CascadeItem({})
 
         scrape_url, post_num = await self.get_thread_url_and_post_num(url)
         title = ""
         try:
@@ -191,58 +192,61 @@
         post_number = 0
         if "post-" in str(url):
             post_number_parts = str(url).rsplit("post-", 1)
             post_number = int(post_number_parts[-1].strip("/")) if len(post_number_parts) == 2 else 0
             url = URL(post_number_parts[0].rstrip("#"))
         return url, post_number
 
-    async def get_links(self, post_content, selector, attribute, domain, temp_title):
+    async def get_links(self, post_content: bs4.Tag, selector: str, attribute: str, domain: URL,
+                        temp_title: str) -> List:
         """Grabs links from the post content based on the given selector and attribute"""
-        found_links = []
+        found_links: List = []
         if not post_content:
             return found_links
         links = post_content.select(selector)
-        for link in links:
-            link = link.get(attribute)
+        for link_tag in links:
+            link = link_tag.get(attribute)
             if not link:
                 continue
+            assert isinstance(link, str)
             if link.endswith("/"):
                 link = link[:-1]
             if link.startswith('//'):
                 link = "https:" + link
             elif link.startswith('/'):
-                link = domain / link[1:]
+                link = str(domain / link[1:])
             found_links.append([URL(link), temp_title])
         return found_links
 
-    async def get_embedded(self, post_content, selector, attribute, temp_title):
+    async def get_embedded(self, post_content: bs4.Tag, selector: str, attribute: str, temp_title: str) -> List:
         """Gets embedded media from post content based on selector and attribute provided"""
         found_links = []
         links = post_content.select(selector)
         for link in links:
             embed_data = link.get(attribute)
+            assert isinstance(embed_data, str)
             embed_data = embed_data.replace("\/\/", "https://www.")
             embed_data = embed_data.replace("\\", "")
 
-            embed_url = re.search(
+            embed = re.search(
                 r"https?:\/\/(www\.)?[-a-zA-Z0-9@:%._\+~#=]{2,256}\.[a-z]{2,4}\\b([-a-zA-Z0-9@:%_\+.~#?&//=]*)",
                 embed_data)
-            if embed_url:
-                embed_url = URL(embed_url.group(0).replace("www.", ""))
+            if embed:
+                embed_url = URL(embed.group(0).replace("www.", ""))
                 found_links.append([embed_url, temp_title])
 
-            embed_url = re.search(
+            embed = re.search(
                 r"https?:\/\/(www\.)?[-a-zA-Z0-9@:%._\+~#=]{2,256}\.[a-z]{2,4}\/[-a-zA-Z0-9@:%._\+~#=]*\/[-a-zA-Z0-9@:?&%._\+~#=]*",
                 embed_data)
-            if embed_url:
-                embed_url = URL(embed_url.group(0).replace("www.", ""))
+            if embed:
+                embed_url = URL(embed.group(0).replace("www.", ""))
                 found_links.append([embed_url, temp_title])
         return found_links
 
-    async def filter_content_links(self, cascade: CascadeItem, content_links: list, url: URL, domain: str):
+    async def filter_content_links(self, cascade: CascadeItem, content_links: List, url: URL, domain: str):
         """Splits given links into direct links and external links,
         returns external links, adds internal to the cascade"""
         assert url.host is not None
         forum_direct_urls = [x for x in content_links if x[0].host.replace(".st", ".su") in url.host]
         forum_direct_urls.extend([x for x in content_links if url.host in x[0].host.replace(".st", ".su")])
         forum_direct_urls.extend([x for x in content_links if "smgmedia" in x[0].host])
         content_links = [x for x in content_links if x not in forum_direct_urls]
@@ -257,26 +261,26 @@
                     filename, ext = await get_filename_and_ext(link.name, True)
                 except NoExtensionFailure:
                     continue
                 media = MediaItem(link, url, completed, filename, ext, filename)
                 await cascade.add_to_album(domain, in_prog_title, media)
         return content_links
 
-    async def handle_external_links(self, content_links: list, referer: URL):
+    async def handle_external_links(self, content_links: List, referer: URL) -> None:
         """Maps external links to the scraper class"""
         tasks = []
         for link_title_bundle in content_links:
             link = link_title_bundle[0]
             temp_title = link_title_bundle[1]
             tasks.append(asyncio.create_task(self.scraping_mapper.map_url(link, temp_title, referer)))
         if tasks:
             await asyncio.wait(tasks)
 
     async def parse_forum(self, session: ScrapeSession, url: URL, spec: ParseSpec, cascade: CascadeItem,
-                          title: str, post_number: int):
+                          title: str, post_number: int) -> str:
         """Parses forum threads"""
         soup = await session.get_BS4(url)
 
         assert url.host is not None
         domain = URL("https://" + url.host)
         post_num_str = ""
         content_links = []
```

### Comparing `cyberdrop-dl-4.1.22/cyberdrop_dl/downloader/downloader_utils.py` & `cyberdrop-dl-4.1.23/cyberdrop_dl/downloader/downloader_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import multiprocessing
 import shutil
 from base64 import b64encode
 from enum import IntEnum
 from functools import wraps
 from http import HTTPStatus
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Dict
 
 from cyberdrop_dl.base_functions.base_functions import FILE_FORMATS, logger
 from cyberdrop_dl.base_functions.error_classes import DownloadFailure
 
 if TYPE_CHECKING:
     from pathlib import Path
 
@@ -18,15 +18,16 @@
 
 
 class CustomHTTPStatus(IntEnum):
     WEB_SERVER_IS_DOWN = 521
     IM_A_TEAPOT = 418
 
 
-async def allowed_filetype(media: MediaItem, block_images: bool, block_video: bool, block_audio: bool, block_other: bool):
+async def allowed_filetype(media: MediaItem, block_images: bool, block_video: bool, block_audio: bool,
+                           block_other: bool):
     """Checks whether the enclosed file is allowed to be downloaded"""
     ext = media.ext
     if block_images and ext in FILE_FORMATS["Images"]:
         return False
     if block_video and ext in FILE_FORMATS["Videos"]:
         return False
     if block_audio and ext in FILE_FORMATS["Audio"]:
@@ -44,15 +45,15 @@
 async def check_free_space(required_space_gb: int, download_directory: Path) -> bool:
     """Checks if there is enough free space on the drive to continue operating"""
     free_space = shutil.disk_usage(download_directory.parent).free
     free_space_gb = free_space / 1024 ** 3
     return free_space_gb >= required_space_gb
 
 
-def get_threads_number(args: dict, domain: str) -> int:
+def get_threads_number(args: Dict, domain: str) -> int:
     threads = args["Runtime"]["simultaneous_downloads_per_domain"] or multiprocessing.cpu_count()
     if any(s in domain for s in ('anonfiles', 'bunkr', 'pixeldrain')):
         return min(threads, 2)
     return threads
 
 
 async def is_4xx_client_error(status_code: int) -> bool:
```

### Comparing `cyberdrop-dl-4.1.22/cyberdrop_dl/downloader/downloaders.py` & `cyberdrop-dl-4.1.23/cyberdrop_dl/downloader/downloaders.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from __future__ import annotations
 
 import asyncio
 import contextlib
 import itertools
 import logging
 from http import HTTPStatus
+from pathlib import Path
 from random import gauss
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Dict, Any, Tuple, Optional
 
 import aiofiles
 import aiohttp.client_exceptions
 from rich.live import Live
 
 from cyberdrop_dl.base_functions.base_functions import (
     adjust,
@@ -82,30 +83,30 @@
         overall_file_progress.update(self.skipped_files_task_id, visible=False)
         overall_file_progress.update(self.failed_files_task_id, visible=False)
 
 
 class Downloader:
     """Downloader class, directs downloading for domain objects"""
 
-    def __init__(self, args: dict, client: Client, SQL_Helper: SQLHelper,
+    def __init__(self, args: Dict, client: Client, SQL_Helper: SQLHelper,
                  domain: str, domain_obj: DomainItem, files: Files):
         self.client = client
         self.download_session = DownloadSession(client)
         self.File_Lock = FileLock()
         self.SQL_Helper = SQL_Helper
 
         self.domain = domain
         self.domain_obj = domain_obj
 
         self.errored_output = args['Runtime']['output_errored_urls']
         self.errored_file = args['Files']['errored_urls_file']
 
         self.files = files
 
-        self.current_attempt: dict[str, int] = {}
+        self.current_attempt: Dict[str, int] = {}
         max_workers = get_threads_number(args, domain)
         self._semaphore = asyncio.Semaphore(max_workers)
         self.delay = {'cyberfile': 1.0, 'anonfiles': 1.0, "coomer": 0.2, "kemono": 0.2}
 
         self.pixeldrain_api_key = args["Authentication"]["pixeldrain_api_key"]
 
         self.exclude_audio = args["Ignore"]["exclude_audio"]
@@ -117,39 +118,39 @@
         self.allowed_attempts = args["Runtime"]["attempts"]
         self.disable_attempt_limit = args["Runtime"]["disable_attempt_limit"]
         self.download_dir = args["Files"]["output_folder"]
         self.mark_downloaded = args["Runtime"]["skip_download_mark_completed"]
         self.proxy = args["Runtime"]["proxy"]
         self.required_free_space = args["Runtime"]["required_free_space"]
 
-    async def start_domain(self, cascade_task: TaskID):
+    async def start_domain(self, cascade_task: TaskID) -> None:
         """Handler for domains and the progress bars for it"""
         domain_task = domain_progress.add_task("[light_pink3]" + self.domain.upper(), total=len(self.domain_obj.albums))
         for album, album_obj in self.domain_obj.albums.items():
             await self.start_album(domain_task, album, album_obj)
         cascade_progress.advance(cascade_task, 1)
         domain_progress.update(domain_task, visible=False)
         await self.download_session.exit_handler()
 
-    async def start_album(self, domain_task: TaskID, album: str, album_obj: AlbumItem):
+    async def start_album(self, domain_task: TaskID, album: str, album_obj: AlbumItem) -> None:
         """Handler for albums and the progress bars for it"""
         if await album_obj.is_empty():
             return
         task_description = album.split('/')[-1]
         task_description = task_description.encode("ascii", "ignore").decode().strip()
         task_description = await adjust(task_description)
         album_task = album_progress.add_task("[pink3]" + task_description.upper(), total=len(album_obj.media))
         download_tasks = []
         for media in album_obj.media:
             download_tasks.append(self.start_file(album_task, album, media))
         await asyncio.gather(*download_tasks)
         album_progress.update(album_task, visible=False)
         domain_progress.advance(domain_task, 1)
 
-    async def start_file(self, album_task: TaskID, album: str, media: MediaItem):
+    async def start_file(self, album_task: TaskID, album: str, media: MediaItem) -> None:
         """Handler for files and the progress bars for it"""
         if media.complete or await self.SQL_Helper.check_complete_singular(self.domain, media.url):
             log(f"Previously Downloaded: {media.filename}", quiet=True)
             await self.files.add_skipped()
             album_progress.advance(album_task, 1)
             return
         async with self._semaphore:
@@ -280,21 +281,21 @@
                     await self.output_failed(media, e)
                     return
 
                 logger.debug("Error status code: " + str(e.code))
 
             raise DownloadFailure(code=getattr(e, "code", 1), message=repr(e))
 
-    async def output_failed(self, media, e):
+    async def output_failed(self, media: MediaItem, e: Any) -> None:
         if self.errored_output:
             async with aiofiles.open(self.errored_file, mode='a') as file:
                 await file.write(f"{media.url},{media.referer},{e.message}\n")
 
-    async def check_file_exists(self, complete_file, partial_file, media, album, url_path, original_filename,
-                                current_throttle):
+    async def check_file_exists(self, complete_file: Path, partial_file: Path, media: MediaItem, album: str,
+                                url_path: str, original_filename: str, current_throttle: float):
         """Complicated checker for if a file already exists, and was already downloaded"""
         expected_size = None
         proceed = True
         while True:
             if not complete_file.exists() and not partial_file.exists():
                 break
 
@@ -324,27 +325,27 @@
 
             media.filename = downloaded_filename
             complete_file = (self.download_dir / album / media.filename)
             partial_file = complete_file.with_suffix(complete_file.suffix + '.part')
 
         return complete_file, partial_file, proceed
 
-    async def iterate_filename(self, complete_file, media, album):
+    async def iterate_filename(self, complete_file: Path, media: MediaItem, album: str) -> Tuple[Path, Path]:
         for iterations in itertools.count(1):
             filename = f"{complete_file.stem} ({iterations}){media.ext}"
             temp_complete_file = (self.download_dir / album / filename)
             if not temp_complete_file.exists() and not await self.SQL_Helper.check_filename(filename):
                 media.filename = filename
                 complete_file = (self.download_dir / album / media.filename)
                 partial_file = complete_file.with_suffix(complete_file.suffix + '.part')
                 break
         return complete_file, partial_file
 
 
-async def download_cascade(args: dict, Cascade: CascadeItem, SQL_Helper: SQLHelper, client: Client) -> None:
+async def download_cascade(args: Dict, Cascade: CascadeItem, SQL_Helper: SQLHelper, client: Client) -> None:
     """Handler for cascades and the progress bars for it"""
     progress_table = await get_cascade_table(args["Progress_Options"])
     total_files = await Cascade.get_total()
     files = Files(total_files)
     with Live(progress_table, refresh_per_second=args["Progress_Options"]["refresh_rate"]):
         cascade_task = cascade_progress.add_task("[light_salmon3]Domains", progress_type="cascade",
                                                  total=len(Cascade.domains))
@@ -360,15 +361,15 @@
     await files.hide()
 
     await clear()
     log(f"| [green]Files Complete: {files.completed_files}[/green] - [yellow]Files Skipped: "
               f"{files.skipped_files}[/yellow] - [red]Files Failed: {files.failed_files}[/red] |")
 
 
-async def download_forums(args: dict, Forums: ForumItem, SQL_Helper: SQLHelper, client: Client) -> None:
+async def download_forums(args: Dict, Forums: ForumItem, SQL_Helper: SQLHelper, client: Client) -> None:
     """Handler for forum threads and the progress bars for it"""
     progress_table = await get_forum_table(args["Progress_Options"])
     total_files = await Forums.get_total()
     files = Files(total_files)
     with Live(progress_table, refresh_per_second=args["Progress_Options"]["refresh_rate"]):
         forum_task = forum_progress.add_task("[orange3]FORUM THREADS", total=len(Forums.threads))
         for title, Cascade in Forums.threads.items():
```

### Comparing `cyberdrop-dl-4.1.22/cyberdrop_dl/downloader/old_downloaders.py` & `cyberdrop-dl-4.1.23/cyberdrop_dl/downloader/old_downloaders.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import asyncio
 import itertools
 import logging
 from http import HTTPStatus
 from pathlib import Path
 from random import gauss
+from typing import Dict, Any
 
 import aiofiles
 import aiohttp.client_exceptions
 from tqdm import tqdm
 
 from cyberdrop_dl.base_functions.base_functions import (
     clear,
@@ -53,30 +54,30 @@
         self.failed_files += 1
         self.progress.update(1)
 
 
 class Old_Downloader:
     """Downloader class, directs downloading for domain objects"""
 
-    def __init__(self, args: dict, client: Client, SQL_Helper: SQLHelper,
+    def __init__(self, args: Dict, client: Client, SQL_Helper: SQLHelper,
                  domain: str, domain_obj: DomainItem, files: Files):
         self.client = client
         self.download_session = DownloadSession(client)
         self.File_Lock = FileLock()
         self.SQL_Helper = SQL_Helper
 
         self.domain = domain
         self.domain_obj = domain_obj
 
         self.errored_output = args['Runtime']['output_errored_urls']
         self.errored_file = args['Files']['errored_urls_file']
 
         self.files = files
 
-        self.current_attempt: dict[str, int] = {}
+        self.current_attempt: Dict[str, int] = {}
         max_workers = get_threads_number(args, domain)
         self._semaphore = asyncio.Semaphore(max_workers)
         self.delay = {'cyberfile': 1, 'anonfiles': 1, "coomer": 0.2, "kemono": 0.2}
 
         self.pixeldrain_api_key = args["Authentication"]["pixeldrain_api_key"]
 
         self.exclude_audio = args["Ignore"]["exclude_audio"]
@@ -225,21 +226,22 @@
                         self.current_attempt.pop(url_path)
                     await self.output_failed(media, e)
                     return
                 logger.debug("Error status code: " + str(e.code))
 
             raise DownloadFailure(code=getattr(e, "code", 1), message=repr(e))
 
-    async def output_failed(self, media, e) -> None:
+    async def output_failed(self, media: MediaItem, e: Any) -> None:
         if self.errored_output:
             async with aiofiles.open(self.errored_file, mode='a') as file:
                 await file.write(f"{media.url},{media.referer},{e.message}\n")
 
-    async def check_file_exists(self, complete_file, partial_file, media, album, url_path, original_filename,
-                                current_throttle) -> tuple[Path, Path, bool]:
+    async def check_file_exists(self, complete_file: Path, partial_file: Path, media: MediaItem, album: str,
+                                url_path: str, original_filename: str,
+                                current_throttle: float) -> tuple[Path, Path, bool]:
         """Complicated checker for if a file already exists, and was already downloaded"""
         expected_size = None
         proceed = True
         while True:
             if not complete_file.exists() and not partial_file.exists():
                 break
 
@@ -290,15 +292,15 @@
         await asyncio.gather(*tasks)
 
     await clear()
     log(f"| [green]Files Complete: {files.completed_files}[/green] - [yellow]Files Skipped: "
               f"{files.skipped_files}[/yellow] - [red]Files Failed: {files.failed_files}[/red] |")
 
 
-async def old_download_forums(args: dict, Forums: ForumItem, SQL_Helper: SQLHelper, client: Client) -> None:
+async def old_download_forums(args: Dict, Forums: ForumItem, SQL_Helper: SQLHelper, client: Client) -> None:
     """Handler for forum threads and the progress bars for it"""
     total_files = await Forums.get_total()
     with tqdm(total=total_files, unit_scale=True, unit='Files', leave=True, initial=0,
               desc="Files Downloaded") as progress:
         files = Files(progress)
         for title, Cascade in Forums.threads.items():
             tasks = []
```

### Comparing `cyberdrop-dl-4.1.22/cyberdrop_dl/downloader/progress_definitions.py` & `cyberdrop-dl-4.1.23/cyberdrop_dl/downloader/progress_definitions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from __future__ import annotations
 
+from typing import Dict
+
 from rich.panel import Panel
 from rich.progress import Progress, BarColumn, SpinnerColumn, TransferSpeedColumn, DownloadColumn, TimeRemainingColumn
 from rich.table import Table
 
 forum_progress = Progress("[progress.description]{task.description}",
                           BarColumn(bar_width=None),
                           "[progress.percentage]{task.percentage:>3.2f}%",
@@ -37,15 +39,15 @@
                          DownloadColumn(),
                          "━",
                          TransferSpeedColumn(),
                          "━",
                          TimeRemainingColumn())
 
 
-async def get_forum_table(progress_options: dict) -> Table:
+async def get_forum_table(progress_options: Dict) -> Table:
     """Table creator for forum threads"""
     progress_table = Table.grid(expand=True)
     if not progress_options['hide_overall_progress']:
         progress_table.add_row(
             Panel.fit(overall_file_progress, title="Overall Progress", border_style="green", padding=(1, 1)))
     if not progress_options['hide_forum_progress']:
         progress_table.add_row(Panel.fit(forum_progress, title="Total Thread", border_style="green", padding=(1, 1)))
@@ -60,15 +62,15 @@
             Panel.fit(album_progress, title="Albums Being Downloaded", border_style="green", padding=(1, 1)))
     if not progress_options['hide_file_progress']:
         progress_table.add_row(
             Panel.fit(file_progress, title="[b]Files Being Downloaded", border_style="green", padding=(1, 1)))
     return progress_table
 
 
-async def get_cascade_table(progress_options: dict) -> Table:
+async def get_cascade_table(progress_options: Dict) -> Table:
     """Table creator for cascade objects"""
     progress_table = Table.grid(expand=True)
     if not progress_options['hide_overall_progress']:
         progress_table.add_row(
             Panel.fit(overall_file_progress, title="Overall Progress", border_style="green", padding=(1, 1)))
     if not progress_options['hide_thread_progress']:
         progress_table.add_row(
```

### Comparing `cyberdrop-dl-4.1.22/cyberdrop_dl/main.py` & `cyberdrop-dl-4.1.23/cyberdrop_dl/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import argparse
 import asyncio
 import contextlib
 import logging
 import re
 from pathlib import Path
+from typing import Dict, List, Tuple
 
 import aiofiles
 from yarl import URL
 
 from cyberdrop_dl.base_functions.base_functions import clear, log, purge_dir
 from cyberdrop_dl.base_functions.config_manager import document_args, run_args
 from cyberdrop_dl.base_functions.config_schema import config_default
@@ -138,15 +139,15 @@
     progress_opts.add_argument("--refresh-rate", type=int, help="refresh rate for the progress table (default: %(default)s)", default=config_group["refresh_rate"])
 
     # Links
     parser.add_argument("links", metavar="link", nargs="*", help="link to content to download (passing multiple links is supported)", default=[])
     return parser.parse_args()
 
 
-async def file_management(args: dict, links: list) -> None:
+async def file_management(args: Dict, links: List) -> None:
     """We handle file defaults here (resetting and creation)"""
     input_file = args['Files']['input_file']
     if not input_file.is_file() and not links:
         input_file.touch()
 
     Path(args['Files']['output_folder']).mkdir(parents=True, exist_ok=True)
 
@@ -169,43 +170,43 @@
         if errored_urls.exists():
             errored_urls.unlink()
             errored_urls.touch()
             async with aiofiles.open(errored_urls, mode='w') as f:
                 await f.write("URL,REFERER,REASON\n")
 
 
-async def regex_links(urls: list) -> list:
+async def regex_links(urls: List) -> List:
     """Regex grab the links from the URLs.txt file"""
     """This allows code blocks or full paragraphs to be copy and pasted into the URLs.txt"""
     yarl_links = []
     for line in urls:
         if line.lstrip().startswith('#'):
             continue
 
         all_links = [x.group().replace(".md.", ".") for x in re.finditer(
             r"(?:http.*?)(?=($|\n|\r\n|\r|\s|\"|\[/URL]|]\[|\[/img]))", line)]
         for link in all_links:
             yarl_links.append(URL(link))
     return yarl_links
 
 
-async def consolidate_links(args: dict, links: list) -> list:
+async def consolidate_links(args: Dict, links: List) -> List:
     """We consolidate links from command line and from URLs.txt into a singular list"""
     links = list(map(URL, links))
     if args["Files"]["input_file"].is_file():
         with open(args["Files"]["input_file"], "r", encoding="utf8") as f:
             links += await regex_links([line.rstrip() for line in f])
     links = list(filter(None, links))
 
     if not links:
         log("No valid links found.", style="red")
     return links
 
 
-async def scrape_links(scraper: ScrapeMapper, links: list, quiet=False) -> tuple[CascadeItem, ForumItem]:
+async def scrape_links(scraper: ScrapeMapper, links: List, quiet=False) -> Tuple[CascadeItem, ForumItem]:
     """Maps links from URLs.txt or command to the scraper class"""
     log("Starting Scrape", quiet=quiet, style="green")
     tasks = []
 
     for link in links:
         tasks.append(asyncio.create_task(scraper.map_url(link)))
     await asyncio.wait(tasks)
@@ -216,15 +217,15 @@
     await Forums.dedupe()
 
     log("", quiet=quiet)
     log("Finished Scrape", quiet=quiet, style="green")
     return Cascade, Forums
 
 
-async def director(args: dict, links: list) -> None:
+async def director(args: Dict, links: List) -> None:
     """This is the overarching director coordinator for CDL."""
     await clear()
     await document_args(args)
     await file_management(args, links)
     log(f"We are running version {VERSION} of Cyberdrop Downloader")
 
     if not await check_free_space(args['Runtime']['required_free_space'], args['Files']['output_folder']):
```

### Comparing `cyberdrop-dl-4.1.22/cyberdrop_dl/scraper/JDownloader_Integration.py` & `cyberdrop-dl-4.1.23/cyberdrop_dl/scraper/JDownloader_Integration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from __future__ import annotations
 
 import logging
-from typing import TYPE_CHECKING, Optional
+from typing import TYPE_CHECKING, Optional, Dict
 
 from myjdapi import myjdapi
 
 from cyberdrop_dl.base_functions.base_functions import log
 from cyberdrop_dl.base_functions.error_classes import JDownloaderFailure
 
 if TYPE_CHECKING:
     from yarl import URL
 
 
 class JDownloader:
     """Class that handles connecting and passing links to JDownloader"""
-    def __init__(self, jdownloader_args: dict, quiet: bool):
+    def __init__(self, jdownloader_args: Dict, quiet: bool):
         self.jdownloader_device = jdownloader_args['jdownloader_device']
         self.jdownloader_username = jdownloader_args['jdownloader_username']
         self.jdownloader_password = jdownloader_args['jdownloader_password']
         self.jdownloader_enable = jdownloader_args['apply_jdownloader']
         self.quiet = quiet
         self.jdownloader_agent = self.jdownloader_setup()
```

### Comparing `cyberdrop-dl-4.1.22/cyberdrop_dl/scraper/Scraper.py` & `cyberdrop-dl-4.1.23/cyberdrop_dl/scraper/Scraper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 import asyncio
-from typing import TYPE_CHECKING, Optional
+from typing import TYPE_CHECKING, Optional, Dict
 
 import aiofiles
 from yarl import URL
 
 from cyberdrop_dl.base_functions.base_functions import log
 from cyberdrop_dl.base_functions.data_classes import AlbumItem, CascadeItem, DomainItem, ForumItem, SkipData
 from cyberdrop_dl.client.client import Client, ScrapeSession
@@ -35,15 +35,15 @@
 
 if TYPE_CHECKING:
     from cyberdrop_dl.base_functions.sql_helper import SQLHelper
 
 
 class ScrapeMapper:
     """This class maps links to their respective handlers, or JDownloader if they are unsupported"""
-    def __init__(self, args: dict, client: Client, SQL_Helper: SQLHelper, quiet: bool):
+    def __init__(self, args: Dict, client: Client, SQL_Helper: SQLHelper, quiet: bool):
         self.args = args
         self.client = client
         self.SQL_Helper = SQL_Helper
         self.Cascade = CascadeItem({})
         self.Forums = ForumItem({})
         self.skip_data = SkipData(args['Ignore']['skip_hosts'])
         self.only_data = SkipData(args['Ignore']['only_hosts'])
```

### Comparing `cyberdrop-dl-4.1.22/cyberdrop_dl.egg-info/PKG-INFO` & `cyberdrop-dl-4.1.23/cyberdrop_dl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.1.22
+Version: 4.1.23
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
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.1.22 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.1.23 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
```

### Comparing `cyberdrop-dl-4.1.22/cyberdrop_dl.egg-info/SOURCES.txt` & `cyberdrop-dl-4.1.23/cyberdrop_dl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.22/setup.cfg` & `cyberdrop-dl-4.1.23/setup.cfg`

 * *Files identical despite different names*

