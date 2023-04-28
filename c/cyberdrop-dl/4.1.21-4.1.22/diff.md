# Comparing `tmp/cyberdrop-dl-4.1.21.tar.gz` & `tmp/cyberdrop-dl-4.1.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyberdrop-dl-4.1.21.tar", last modified: Fri Apr 28 04:50:01 2023, max compression
+gzip compressed data, was "cyberdrop-dl-4.1.22.tar", last modified: Fri Apr 28 04:52:40 2023, max compression
```

## Comparing `cyberdrop-dl-4.1.21.tar` & `cyberdrop-dl-4.1.22.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 04:50:01.149752 cyberdrop-dl-4.1.21/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-28 04:49:52.000000 cyberdrop-dl-4.1.21/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-04-28 04:50:01.149752 cyberdrop-dl-4.1.21/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16523 2023-04-28 04:49:52.000000 cyberdrop-dl-4.1.21/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 04:50:01.145752 cyberdrop-dl-4.1.21/cyberdrop_dl/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-28 04:49:52.000000 cyberdrop-dl-4.1.21/cyberdrop_dl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 04:50:01.145752 cyberdrop-dl-4.1.21/cyberdrop_dl/base_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 04:49:52.000000 cyberdrop-dl-4.1.21/cyberdrop_dl/base_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-04-28 04:49:52.000000 cyberdrop-dl-4.1.21/cyberdrop_dl/base_functions/base_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-04-28 04:49:52.000000 cyberdrop-dl-4.1.21/cyberdrop_dl/base_functions/config_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-04-28 04:49:52.000000 cyberdrop-dl-4.1.21/cyberdrop_dl/base_functions/config_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-04-28 04:49:52.000000 cyberdrop-dl-4.1.21/cyberdrop_dl/base_functions/data_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-28 04:49:52.000000 cyberdrop-dl-4.1.21/cyberdrop_dl/base_functions/error_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-04-28 04:49:52.000000 cyberdrop-dl-4.1.21/cyberdrop_dl/base_functions/sorting_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12383 2023-04-28 04:49:52.000000 cyberdrop-dl-4.1.21/cyberdrop_dl/base_functions/sql_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 04:50:01.145752 cyberdrop-dl-4.1.21/cyberdrop_dl/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 04:49:52.000000 cyberdrop-dl-4.1.21/cyberdrop_dl/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9523 2023-04-28 04:49:52.000000 cyberdrop-dl-4.1.21/cyberdrop_dl/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-04-28 04:49:52.000000 cyberdrop-dl-4.1.21/cyberdrop_dl/client/rate_limiting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 04:50:01.149752 cyberdrop-dl-4.1.21/cyberdrop_dl/crawlers/
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-04-28 04:49:52.000000 cyberdrop-dl-4.1.21/cyberdrop_dl/crawlers/Anonfiles_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     7493 2023-04-28 04:49:52.000000 cyberdrop-dl-4.1.21/cyberdrop_dl/crawlers/Bunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-04-28 04:49:52.000000 cyberdrop-dl-4.1.21/cyberdrop_dl/crawlers/Coomeno_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    12064 2023-04-28 04:49:52.000000 cyberdrop-dl-4.1.21/cyberdrop_dl/crawlers/CyberFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-28 04:49:52.000000 cyberdrop-dl-4.1.21/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-04-28 04:49:52.000000 cyberdrop-dl-4.1.21/cyberdrop_dl/crawlers/EHentai_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-04-28 04:49:52.000000 cyberdrop-dl-4.1.21/cyberdrop_dl/crawlers/Erome_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-04-28 04:49:52.000000 cyberdrop-dl-4.1.21/cyberdrop_dl/crawlers/Fapello_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-04-28 04:49:52.000000 cyberdrop-dl-4.1.21/cyberdrop_dl/crawlers/Gfycat_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-04-28 04:49:52.000000 cyberdrop-dl-4.1.21/cyberdrop_dl/crawlers/GoFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-04-28 04:49:52.000000 cyberdrop-dl-4.1.21/cyberdrop_dl/crawlers/HGameCG_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-04-28 04:49:52.000000 cyberdrop-dl-4.1.21/cyberdrop_dl/crawlers/ImgBox_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-04-28 04:49:52.000000 cyberdrop-dl-4.1.21/cyberdrop_dl/crawlers/LoveFap_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-04-28 04:49:52.000000 cyberdrop-dl-4.1.21/cyberdrop_dl/crawlers/NSFWXXXCrawler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-04-28 04:49:52.000000 cyberdrop-dl-4.1.21/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-04-28 04:49:52.000000 cyberdrop-dl-4.1.21/cyberdrop_dl/crawlers/PixelDrain_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-04-28 04:49:52.000000 cyberdrop-dl-4.1.21/cyberdrop_dl/crawlers/PostImg_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-28 04:49:52.000000 cyberdrop-dl-4.1.21/cyberdrop_dl/crawlers/Saint_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     8411 2023-04-28 04:49:52.000000 cyberdrop-dl-4.1.21/cyberdrop_dl/crawlers/ShareX_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-04-28 04:49:52.000000 cyberdrop-dl-4.1.21/cyberdrop_dl/crawlers/XBunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    15075 2023-04-28 04:49:52.000000 cyberdrop-dl-4.1.21/cyberdrop_dl/crawlers/Xenforo_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 04:49:52.000000 cyberdrop-dl-4.1.21/cyberdrop_dl/crawlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 04:50:01.149752 cyberdrop-dl-4.1.21/cyberdrop_dl/downloader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 04:49:52.000000 cyberdrop-dl-4.1.21/cyberdrop_dl/downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-04-28 04:49:52.000000 cyberdrop-dl-4.1.21/cyberdrop_dl/downloader/downloader_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17390 2023-04-28 04:49:52.000000 cyberdrop-dl-4.1.21/cyberdrop_dl/downloader/downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    13871 2023-04-28 04:49:52.000000 cyberdrop-dl-4.1.21/cyberdrop_dl/downloader/old_downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-04-28 04:49:52.000000 cyberdrop-dl-4.1.21/cyberdrop_dl/downloader/progress_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)    18626 2023-04-28 04:49:52.000000 cyberdrop-dl-4.1.21/cyberdrop_dl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 04:50:01.149752 cyberdrop-dl-4.1.21/cyberdrop_dl/scraper/
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-04-28 04:49:52.000000 cyberdrop-dl-4.1.21/cyberdrop_dl/scraper/JDownloader_Integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    20266 2023-04-28 04:49:52.000000 cyberdrop-dl-4.1.21/cyberdrop_dl/scraper/Scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 04:49:52.000000 cyberdrop-dl-4.1.21/cyberdrop_dl/scraper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 04:50:01.145752 cyberdrop-dl-4.1.21/cyberdrop_dl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-04-28 04:50:01.000000 cyberdrop-dl-4.1.21/cyberdrop_dl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-28 04:50:01.000000 cyberdrop-dl-4.1.21/cyberdrop_dl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 04:50:01.000000 cyberdrop-dl-4.1.21/cyberdrop_dl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-28 04:50:01.000000 cyberdrop-dl-4.1.21/cyberdrop_dl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-28 04:50:01.000000 cyberdrop-dl-4.1.21/cyberdrop_dl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-28 04:50:01.000000 cyberdrop-dl-4.1.21/cyberdrop_dl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-28 04:49:52.000000 cyberdrop-dl-4.1.21/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-28 04:50:01.149752 cyberdrop-dl-4.1.21/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 04:49:52.000000 cyberdrop-dl-4.1.21/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 04:52:40.635170 cyberdrop-dl-4.1.22/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-04-28 04:52:40.635170 cyberdrop-dl-4.1.22/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16523 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 04:52:40.623169 cyberdrop-dl-4.1.22/cyberdrop_dl/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 04:52:40.627169 cyberdrop-dl-4.1.22/cyberdrop_dl/base_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/base_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/base_functions/base_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/base_functions/config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/base_functions/config_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/base_functions/data_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/base_functions/error_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/base_functions/sorting_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12383 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/base_functions/sql_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 04:52:40.627169 cyberdrop-dl-4.1.22/cyberdrop_dl/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9523 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/client/rate_limiting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 04:52:40.635170 cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/Anonfiles_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7493 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/Bunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/Coomeno_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12064 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/CyberFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/EHentai_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/Erome_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/Fapello_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/Gfycat_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/GoFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/HGameCG_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/ImgBox_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/LoveFap_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/NSFWXXXCrawler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/PixelDrain_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/PostImg_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/Saint_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8411 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/ShareX_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/XBunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15075 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/Xenforo_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 04:52:40.635170 cyberdrop-dl-4.1.22/cyberdrop_dl/downloader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/downloader/downloader_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17390 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/downloader/downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13871 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/downloader/old_downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/downloader/progress_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18626 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 04:52:40.635170 cyberdrop-dl-4.1.22/cyberdrop_dl/scraper/
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/scraper/JDownloader_Integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20266 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/scraper/Scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/cyberdrop_dl/scraper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 04:52:40.627169 cyberdrop-dl-4.1.22/cyberdrop_dl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-04-28 04:52:40.000000 cyberdrop-dl-4.1.22/cyberdrop_dl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-28 04:52:40.000000 cyberdrop-dl-4.1.22/cyberdrop_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 04:52:40.000000 cyberdrop-dl-4.1.22/cyberdrop_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-28 04:52:40.000000 cyberdrop-dl-4.1.22/cyberdrop_dl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-28 04:52:40.000000 cyberdrop-dl-4.1.22/cyberdrop_dl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-28 04:52:40.000000 cyberdrop-dl-4.1.22/cyberdrop_dl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-28 04:52:40.635170 cyberdrop-dl-4.1.22/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 04:52:25.000000 cyberdrop-dl-4.1.22/setup.py
```

### Comparing `cyberdrop-dl-4.1.21/LICENSE` & `cyberdrop-dl-4.1.22/LICENSE`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.21/PKG-INFO` & `cyberdrop-dl-4.1.22/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.1.21
+Version: 4.1.22
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
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.1.21 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.1.22 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
```

### Comparing `cyberdrop-dl-4.1.21/README.md` & `cyberdrop-dl-4.1.22/README.md`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.21/cyberdrop_dl/base_functions/base_functions.py` & `cyberdrop-dl-4.1.22/cyberdrop_dl/base_functions/base_functions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.21/cyberdrop_dl/base_functions/config_manager.py` & `cyberdrop-dl-4.1.22/cyberdrop_dl/base_functions/config_manager.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.21/cyberdrop_dl/base_functions/config_schema.py` & `cyberdrop-dl-4.1.22/cyberdrop_dl/base_functions/config_schema.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.21/cyberdrop_dl/base_functions/data_classes.py` & `cyberdrop-dl-4.1.22/cyberdrop_dl/base_functions/data_classes.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.21/cyberdrop_dl/base_functions/error_classes.py` & `cyberdrop-dl-4.1.22/cyberdrop_dl/base_functions/error_classes.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.21/cyberdrop_dl/base_functions/sorting_functions.py` & `cyberdrop-dl-4.1.22/cyberdrop_dl/base_functions/sorting_functions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.21/cyberdrop_dl/base_functions/sql_helper.py` & `cyberdrop-dl-4.1.22/cyberdrop_dl/base_functions/sql_helper.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.21/cyberdrop_dl/client/client.py` & `cyberdrop-dl-4.1.22/cyberdrop_dl/client/client.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.21/cyberdrop_dl/client/rate_limiting.py` & `cyberdrop-dl-4.1.22/cyberdrop_dl/client/rate_limiting.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.21/cyberdrop_dl/crawlers/Anonfiles_Spider.py` & `cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/Anonfiles_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.21/cyberdrop_dl/crawlers/Bunkr_Spider.py` & `cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/Bunkr_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.21/cyberdrop_dl/crawlers/Coomeno_Spider.py` & `cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/Coomeno_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.21/cyberdrop_dl/crawlers/CyberFile_Spider.py` & `cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/CyberFile_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.21/cyberdrop_dl/crawlers/Cyberdrop_Spider.py` & `cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/Cyberdrop_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.21/cyberdrop_dl/crawlers/EHentai_Spider.py` & `cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/EHentai_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.21/cyberdrop_dl/crawlers/Erome_Spider.py` & `cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/Erome_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.21/cyberdrop_dl/crawlers/Fapello_Spider.py` & `cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/Fapello_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.21/cyberdrop_dl/crawlers/Gfycat_Spider.py` & `cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/Gfycat_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.21/cyberdrop_dl/crawlers/GoFile_Spider.py` & `cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/GoFile_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.21/cyberdrop_dl/crawlers/HGameCG_Spider.py` & `cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/HGameCG_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.21/cyberdrop_dl/crawlers/ImgBox_Spider.py` & `cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/ImgBox_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.21/cyberdrop_dl/crawlers/LoveFap_Spider.py` & `cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/LoveFap_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.21/cyberdrop_dl/crawlers/NSFWXXXCrawler.py` & `cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/NSFWXXXCrawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.21/cyberdrop_dl/crawlers/PimpAndHost_Spider.py` & `cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/PimpAndHost_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.21/cyberdrop_dl/crawlers/PixelDrain_Spider.py` & `cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/PixelDrain_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.21/cyberdrop_dl/crawlers/PostImg_Spider.py` & `cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/PostImg_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.21/cyberdrop_dl/crawlers/Saint_Spider.py` & `cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/Saint_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.21/cyberdrop_dl/crawlers/ShareX_Spider.py` & `cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/ShareX_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.21/cyberdrop_dl/crawlers/XBunkr_Spider.py` & `cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/XBunkr_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.21/cyberdrop_dl/crawlers/Xenforo_Spider.py` & `cyberdrop-dl-4.1.22/cyberdrop_dl/crawlers/Xenforo_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.21/cyberdrop_dl/downloader/downloader_utils.py` & `cyberdrop-dl-4.1.22/cyberdrop_dl/downloader/downloader_utils.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.21/cyberdrop_dl/downloader/downloaders.py` & `cyberdrop-dl-4.1.22/cyberdrop_dl/downloader/downloaders.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.21/cyberdrop_dl/downloader/old_downloaders.py` & `cyberdrop-dl-4.1.22/cyberdrop_dl/downloader/old_downloaders.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.21/cyberdrop_dl/downloader/progress_definitions.py` & `cyberdrop-dl-4.1.22/cyberdrop_dl/downloader/progress_definitions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.21/cyberdrop_dl/main.py` & `cyberdrop-dl-4.1.22/cyberdrop_dl/main.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.21/cyberdrop_dl/scraper/JDownloader_Integration.py` & `cyberdrop-dl-4.1.22/cyberdrop_dl/scraper/JDownloader_Integration.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.21/cyberdrop_dl/scraper/Scraper.py` & `cyberdrop-dl-4.1.22/cyberdrop_dl/scraper/Scraper.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
         self.include_id = args['Runtime']['include_id']
         self.remove_bunkr_id = args['Runtime']['remove_bunkr_identifier']
         self.separate_posts = args["Forum_Options"]["separate_posts"]
         self.quiet = quiet
         self.jdownloader = JDownloader(args['JDownloader'], quiet)
 
-        self.bunkr_limiter = AsyncRateLimiter(15)
+        self.bunkr_limiter = AsyncRateLimiter(10)
         self.coomer_limiter = AsyncRateLimiter(8)
         self.gofile_limiter = AsyncRateLimiter(max_calls=1, period=3)
         self.jpgfish_limiter = AsyncRateLimiter(10)
         self.kemono_limiter = AsyncRateLimiter(8)
 
         self.coomer_semaphore = asyncio.Semaphore(1)
         self.cyberfile_semaphore = asyncio.Semaphore(2)
```

### Comparing `cyberdrop-dl-4.1.21/cyberdrop_dl.egg-info/PKG-INFO` & `cyberdrop-dl-4.1.22/cyberdrop_dl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.1.21
+Version: 4.1.22
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
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.1.21 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.1.22 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
```

### Comparing `cyberdrop-dl-4.1.21/cyberdrop_dl.egg-info/SOURCES.txt` & `cyberdrop-dl-4.1.22/cyberdrop_dl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.1.21/setup.cfg` & `cyberdrop-dl-4.1.22/setup.cfg`

 * *Files identical despite different names*

