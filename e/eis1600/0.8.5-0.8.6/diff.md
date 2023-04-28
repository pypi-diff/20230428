# Comparing `tmp/eis1600-0.8.5.tar.gz` & `tmp/eis1600-0.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eis1600-0.8.5.tar", last modified: Thu Apr 20 10:02:52 2023, max compression
+gzip compressed data, was "eis1600-0.8.6.tar", last modified: Thu Apr 27 07:58:49 2023, max compression
```

## Comparing `eis1600-0.8.5.tar` & `eis1600-0.8.6.tar`

### file list

```diff
@@ -1,75 +1,76 @@
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-20 10:02:52.196050 eis1600-0.8.5/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1046 2022-09-21 09:22:30.000000 eis1600-0.8.5/LICENSE
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     7956 2023-04-20 10:02:52.196050 eis1600-0.8.5/PKG-INFO
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5895 2023-04-13 08:22:59.000000 eis1600-0.8.5/README.md
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-20 10:02:52.184050 eis1600-0.8.5/eis1600/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-09-19 09:55:48.000000 eis1600-0.8.5/eis1600/__init__.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-20 10:02:52.188050 eis1600-0.8.5/eis1600/dates/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      911 2023-04-05 11:10:16.000000 eis1600-0.8.5/eis1600/dates/Date.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-0.8.5/eis1600/dates/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5856 2023-04-06 11:34:18.000000 eis1600-0.8.5/eis1600/dates/date_patterns.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3924 2023-04-12 06:44:26.000000 eis1600-0.8.5/eis1600/dates/methods.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-20 10:02:52.188050 eis1600-0.8.5/eis1600/gazetteers/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4225 2023-04-14 12:34:00.000000 eis1600-0.8.5/eis1600/gazetteers/Onomastics.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3259 2023-04-12 08:40:27.000000 eis1600-0.8.5/eis1600/gazetteers/Toponyms.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-03-09 08:52:31.000000 eis1600-0.8.5/eis1600/gazetteers/__init__.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-20 10:02:52.188050 eis1600-0.8.5/eis1600/gazetteers/data/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-0.8.5/eis1600/gazetteers/data/__init__.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-20 10:02:52.192050 eis1600-0.8.5/eis1600/helper/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      712 2023-04-20 08:48:52.000000 eis1600-0.8.5/eis1600/helper/EntityTags.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1280 2023-04-06 10:45:49.000000 eis1600-0.8.5/eis1600/helper/Singleton.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-10-20 15:09:05.000000 eis1600-0.8.5/eis1600/helper/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1030 2023-04-06 13:50:26.000000 eis1600-0.8.5/eis1600/helper/ar_normalization.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-20 10:02:52.192050 eis1600-0.8.5/eis1600/helper/data/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-04-03 10:40:59.000000 eis1600-0.8.5/eis1600/helper/data/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1237 2023-04-12 06:44:26.000000 eis1600-0.8.5/eis1600/helper/fix_miu_annotation.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      365 2023-03-31 11:03:40.000000 eis1600-0.8.5/eis1600/helper/logging.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      637 2023-04-06 09:28:14.000000 eis1600-0.8.5/eis1600/helper/markdown_methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3739 2023-04-20 08:46:34.000000 eis1600-0.8.5/eis1600/helper/markdown_patterns.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     6461 2023-03-09 10:15:31.000000 eis1600-0.8.5/eis1600/helper/miu_random_revisions.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      370 2023-04-19 14:31:23.000000 eis1600-0.8.5/eis1600/helper/my_json_ecoder.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    10796 2023-04-05 11:18:46.000000 eis1600-0.8.5/eis1600/helper/repo.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1425 2023-04-20 09:45:05.000000 eis1600-0.8.5/eis1600/helper/yml_to_json.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-20 10:02:52.192050 eis1600-0.8.5/eis1600/markdown/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1822 2023-04-12 07:11:17.000000 eis1600-0.8.5/eis1600/markdown/UIDs.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-09-30 09:01:09.000000 eis1600-0.8.5/eis1600/markdown/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4794 2023-02-23 07:56:48.000000 eis1600-0.8.5/eis1600/markdown/convert_mARkdown_to_EIS1600TMP.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4574 2023-02-23 07:56:48.000000 eis1600-0.8.5/eis1600/markdown/insert_uids.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    13077 2023-04-19 15:21:14.000000 eis1600-0.8.5/eis1600/markdown/methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2856 2023-02-23 07:56:48.000000 eis1600-0.8.5/eis1600/markdown/update_uids.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5284 2023-04-05 08:21:34.000000 eis1600-0.8.5/eis1600/markdown/update_uids_old_process.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-20 10:02:52.192050 eis1600-0.8.5/eis1600/miu/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3484 2023-04-12 15:29:30.000000 eis1600-0.8.5/eis1600/miu/HeadingTracker.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     6164 2023-04-20 09:51:08.000000 eis1600-0.8.5/eis1600/miu/YAMLHandler.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-08 08:28:10.000000 eis1600-0.8.5/eis1600/miu/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2715 2023-02-23 07:39:16.000000 eis1600-0.8.5/eis1600/miu/disassemble_into_miu_files.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     8907 2023-04-12 06:50:23.000000 eis1600-0.8.5/eis1600/miu/methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2590 2022-11-21 11:57:36.000000 eis1600-0.8.5/eis1600/miu/reassemble_from_miu_files.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     6314 2023-04-20 09:52:40.000000 eis1600-0.8.5/eis1600/miu/yml_handling.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-20 10:02:52.192050 eis1600-0.8.5/eis1600/nlp/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-17 12:10:00.000000 eis1600-0.8.5/eis1600/nlp/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2017 2023-03-31 12:22:46.000000 eis1600-0.8.5/eis1600/nlp/cameltools.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3672 2023-03-31 11:52:32.000000 eis1600-0.8.5/eis1600/nlp/ner_annotate_mius.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2726 2023-04-05 11:18:46.000000 eis1600-0.8.5/eis1600/nlp/utils.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-20 10:02:52.192050 eis1600-0.8.5/eis1600/onomastics/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-03-02 09:23:30.000000 eis1600-0.8.5/eis1600/onomastics/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1410 2023-04-20 10:02:38.000000 eis1600-0.8.5/eis1600/onomastics/annotation.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    10301 2023-04-20 10:02:38.000000 eis1600-0.8.5/eis1600/onomastics/methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1966 2023-04-17 09:33:17.000000 eis1600-0.8.5/eis1600/onomastics/re_pattern.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-20 10:02:52.196050 eis1600-0.8.5/eis1600/processing/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-0.8.5/eis1600/processing/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4660 2023-04-12 08:23:03.000000 eis1600-0.8.5/eis1600/processing/postprocessing.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4604 2023-04-14 13:42:02.000000 eis1600-0.8.5/eis1600/processing/preprocessing.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-20 10:02:52.196050 eis1600-0.8.5/eis1600/stats/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-02-17 08:45:10.000000 eis1600-0.8.5/eis1600/stats/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      842 2023-02-17 15:06:29.000000 eis1600-0.8.5/eis1600/stats/methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1978 2023-02-17 15:05:56.000000 eis1600-0.8.5/eis1600/stats/miu_stats.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-20 10:02:52.188050 eis1600-0.8.5/eis1600.egg-info/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     7956 2023-04-20 10:02:52.000000 eis1600-0.8.5/eis1600.egg-info/PKG-INFO
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1748 2023-04-20 10:02:52.000000 eis1600-0.8.5/eis1600.egg-info/SOURCES.txt
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        1 2023-04-20 10:02:52.000000 eis1600-0.8.5/eis1600.egg-info/dependency_links.txt
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      746 2023-04-20 10:02:52.000000 eis1600-0.8.5/eis1600.egg-info/entry_points.txt
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)       72 2023-04-20 10:02:52.000000 eis1600-0.8.5/eis1600.egg-info/requires.txt
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        8 2023-04-20 10:02:52.000000 eis1600-0.8.5/eis1600.egg-info/top_level.txt
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)       38 2023-04-20 10:02:52.196050 eis1600-0.8.5/setup.cfg
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2253 2023-04-20 10:02:38.000000 eis1600-0.8.5/setup.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-27 07:58:49.504257 eis1600-0.8.6/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1046 2022-09-21 09:22:30.000000 eis1600-0.8.6/LICENSE
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     7956 2023-04-27 07:58:49.504257 eis1600-0.8.6/PKG-INFO
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5895 2023-04-13 08:22:59.000000 eis1600-0.8.6/README.md
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-27 07:58:49.496257 eis1600-0.8.6/eis1600/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-09-19 09:55:48.000000 eis1600-0.8.6/eis1600/__init__.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-27 07:58:49.496257 eis1600-0.8.6/eis1600/dates/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      911 2023-04-05 11:10:16.000000 eis1600-0.8.6/eis1600/dates/Date.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-0.8.6/eis1600/dates/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5856 2023-04-06 11:34:18.000000 eis1600-0.8.6/eis1600/dates/date_patterns.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3924 2023-04-12 06:44:26.000000 eis1600-0.8.6/eis1600/dates/methods.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-27 07:58:49.496257 eis1600-0.8.6/eis1600/gazetteers/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4225 2023-04-14 12:34:00.000000 eis1600-0.8.6/eis1600/gazetteers/Onomastics.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5529 2023-04-27 07:28:56.000000 eis1600-0.8.6/eis1600/gazetteers/Toponyms.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-03-09 08:52:31.000000 eis1600-0.8.6/eis1600/gazetteers/__init__.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-27 07:58:49.496257 eis1600-0.8.6/eis1600/gazetteers/data/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-0.8.6/eis1600/gazetteers/data/__init__.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-27 07:58:49.500257 eis1600-0.8.6/eis1600/helper/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      730 2023-04-27 07:54:20.000000 eis1600-0.8.6/eis1600/helper/EntityTags.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1280 2023-04-24 10:02:09.000000 eis1600-0.8.6/eis1600/helper/Singleton.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-10-20 15:09:05.000000 eis1600-0.8.6/eis1600/helper/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1030 2023-04-06 13:50:26.000000 eis1600-0.8.6/eis1600/helper/ar_normalization.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-27 07:58:49.500257 eis1600-0.8.6/eis1600/helper/data/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-04-03 10:40:59.000000 eis1600-0.8.6/eis1600/helper/data/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1237 2023-04-12 06:44:26.000000 eis1600-0.8.6/eis1600/helper/fix_miu_annotation.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      365 2023-03-31 11:03:40.000000 eis1600-0.8.6/eis1600/helper/logging.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      637 2023-04-06 09:28:14.000000 eis1600-0.8.6/eis1600/helper/markdown_methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3739 2023-04-20 08:46:34.000000 eis1600-0.8.6/eis1600/helper/markdown_patterns.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     6461 2023-03-09 10:15:31.000000 eis1600-0.8.6/eis1600/helper/miu_random_revisions.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      370 2023-04-26 15:08:00.000000 eis1600-0.8.6/eis1600/helper/my_json_ecoder.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    10796 2023-04-05 11:18:46.000000 eis1600-0.8.6/eis1600/helper/repo.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      598 2023-04-26 15:20:40.000000 eis1600-0.8.6/eis1600/helper/yml_methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1356 2023-04-24 07:56:45.000000 eis1600-0.8.6/eis1600/helper/yml_to_json.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-27 07:58:49.500257 eis1600-0.8.6/eis1600/markdown/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1822 2023-04-12 07:11:17.000000 eis1600-0.8.6/eis1600/markdown/UIDs.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-09-30 09:01:09.000000 eis1600-0.8.6/eis1600/markdown/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4794 2023-02-23 07:56:48.000000 eis1600-0.8.6/eis1600/markdown/convert_mARkdown_to_EIS1600TMP.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4574 2023-02-23 07:56:48.000000 eis1600-0.8.6/eis1600/markdown/insert_uids.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    13077 2023-04-19 15:21:14.000000 eis1600-0.8.6/eis1600/markdown/methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2856 2023-02-23 07:56:48.000000 eis1600-0.8.6/eis1600/markdown/update_uids.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5284 2023-04-05 08:21:34.000000 eis1600-0.8.6/eis1600/markdown/update_uids_old_process.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-27 07:58:49.500257 eis1600-0.8.6/eis1600/miu/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3484 2023-04-12 15:29:30.000000 eis1600-0.8.6/eis1600/miu/HeadingTracker.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     7477 2023-04-27 07:58:47.000000 eis1600-0.8.6/eis1600/miu/YAMLHandler.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-08 08:28:10.000000 eis1600-0.8.6/eis1600/miu/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2715 2023-02-23 07:39:16.000000 eis1600-0.8.6/eis1600/miu/disassemble_into_miu_files.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     8907 2023-04-12 06:50:23.000000 eis1600-0.8.6/eis1600/miu/methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2590 2022-11-21 11:57:36.000000 eis1600-0.8.6/eis1600/miu/reassemble_from_miu_files.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     7231 2023-04-27 07:35:56.000000 eis1600-0.8.6/eis1600/miu/yml_handling.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-27 07:58:49.500257 eis1600-0.8.6/eis1600/nlp/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-17 12:10:00.000000 eis1600-0.8.6/eis1600/nlp/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2017 2023-03-31 12:22:46.000000 eis1600-0.8.6/eis1600/nlp/cameltools.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3672 2023-03-31 11:52:32.000000 eis1600-0.8.6/eis1600/nlp/ner_annotate_mius.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2726 2023-04-05 11:18:46.000000 eis1600-0.8.6/eis1600/nlp/utils.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-27 07:58:49.504257 eis1600-0.8.6/eis1600/onomastics/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-03-02 09:23:30.000000 eis1600-0.8.6/eis1600/onomastics/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1596 2023-04-24 09:54:11.000000 eis1600-0.8.6/eis1600/onomastics/annotation.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    10535 2023-04-24 09:53:23.000000 eis1600-0.8.6/eis1600/onomastics/methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1966 2023-04-17 09:33:17.000000 eis1600-0.8.6/eis1600/onomastics/re_pattern.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-27 07:58:49.504257 eis1600-0.8.6/eis1600/processing/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-0.8.6/eis1600/processing/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4660 2023-04-12 08:23:03.000000 eis1600-0.8.6/eis1600/processing/postprocessing.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4604 2023-04-21 13:13:53.000000 eis1600-0.8.6/eis1600/processing/preprocessing.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-27 07:58:49.504257 eis1600-0.8.6/eis1600/stats/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-02-17 08:45:10.000000 eis1600-0.8.6/eis1600/stats/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      842 2023-02-17 15:06:29.000000 eis1600-0.8.6/eis1600/stats/methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1978 2023-02-17 15:05:56.000000 eis1600-0.8.6/eis1600/stats/miu_stats.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-04-27 07:58:49.496257 eis1600-0.8.6/eis1600.egg-info/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     7956 2023-04-27 07:58:49.000000 eis1600-0.8.6/eis1600.egg-info/PKG-INFO
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1778 2023-04-27 07:58:49.000000 eis1600-0.8.6/eis1600.egg-info/SOURCES.txt
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        1 2023-04-27 07:58:49.000000 eis1600-0.8.6/eis1600.egg-info/dependency_links.txt
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      746 2023-04-27 07:58:49.000000 eis1600-0.8.6/eis1600.egg-info/entry_points.txt
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)       72 2023-04-27 07:58:49.000000 eis1600-0.8.6/eis1600.egg-info/requires.txt
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        8 2023-04-27 07:58:49.000000 eis1600-0.8.6/eis1600.egg-info/top_level.txt
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)       38 2023-04-27 07:58:49.504257 eis1600-0.8.6/setup.cfg
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2253 2023-04-27 07:49:40.000000 eis1600-0.8.6/setup.py
```

### Comparing `eis1600-0.8.5/LICENSE` & `eis1600-0.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.5/PKG-INFO` & `eis1600-0.8.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eis1600
-Version: 0.8.5
+Version: 0.8.6
 Summary: EIS1600 project tools and utilities
 Home-page: https://github.com/EIS1600/eis1600-pkg
 Author: Lisa Mischer
 Author-email: mischer.lisa@gmail.com
 License: MIT License
 Description: # EIS1600 Tools
```

### Comparing `eis1600-0.8.5/README.md` & `eis1600-0.8.6/README.md`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.5/eis1600/dates/Date.py` & `eis1600-0.8.6/eis1600/dates/Date.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.5/eis1600/dates/date_patterns.py` & `eis1600-0.8.6/eis1600/dates/date_patterns.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.5/eis1600/dates/methods.py` & `eis1600-0.8.6/eis1600/dates/methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.5/eis1600/gazetteers/Onomastics.py` & `eis1600-0.8.6/eis1600/gazetteers/Onomastics.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.5/eis1600/helper/EntityTags.py` & `eis1600-0.8.6/eis1600/helper/EntityTags.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from importlib_resources import files
 from typing import List
 import pandas as pd
 from eis1600.helper.Singleton import Singleton
 
-path = files('eis1600.helper.data').joinpath('entity_tags.csv')
+entities_path = files('eis1600.helper.data').joinpath('entity_tags.csv')
 
 
 @Singleton
 class EntityTags:
     __entity_tags_df = None
     __tag_list = None
 
     def __init__(self) -> None:
-        entity_tags_df = pd.read_csv(path)
+        entity_tags_df = pd.read_csv(entities_path)
         EntityTags.__entity_tags_df = entity_tags_df
         EntityTags.__tag_list = entity_tags_df.loc[entity_tags_df['CATEGORY'].notna(), 'TAG'].to_list()
 
     @staticmethod
     def get_entity_tags_df() -> pd.DataFrame:
         return EntityTags.__entity_tags_df
```

### Comparing `eis1600-0.8.5/eis1600/helper/Singleton.py` & `eis1600-0.8.6/eis1600/helper/Singleton.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.5/eis1600/helper/ar_normalization.py` & `eis1600-0.8.6/eis1600/helper/ar_normalization.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.5/eis1600/helper/fix_miu_annotation.py` & `eis1600-0.8.6/eis1600/helper/fix_miu_annotation.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.5/eis1600/helper/markdown_methods.py` & `eis1600-0.8.6/eis1600/helper/markdown_methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.5/eis1600/helper/markdown_patterns.py` & `eis1600-0.8.6/eis1600/helper/markdown_patterns.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.5/eis1600/helper/miu_random_revisions.py` & `eis1600-0.8.6/eis1600/helper/miu_random_revisions.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.5/eis1600/helper/repo.py` & `eis1600-0.8.6/eis1600/helper/repo.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.5/eis1600/helper/yml_to_json.py` & `eis1600-0.8.6/eis1600/helper/yml_to_json.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,40 @@
 import json
 import sys
 from argparse import ArgumentParser, RawDescriptionHelpFormatter
-from glob import glob
 from pathlib import Path
 
 from eis1600.helper.my_json_ecoder import MyJSONEncoder
 from p_tqdm import p_uimap
 
 from eis1600.processing.preprocessing import get_yml
 
 
 def main():
     arg_parser = ArgumentParser(
             prog=sys.argv[0], formatter_class=RawDescriptionHelpFormatter,
             description='''Script to generate JSON from MIU YAMLHeaders.'''
     )
-    arg_parser.add_argument('-v', '--verbose', action='store_true')
+    arg_parser.add_argument('-D', '--debug', action='store_true')
     args = arg_parser.parse_args()
 
-    verbose = args.verbose
-    # TODO: infiles = glob('OpenITI_EIS1600_MIUs/data/**/MIUs/*.EIS1600')
+    debug = args.debug
     with open('OpenITI_EIS1600_MIUs/gold_standard.txt', 'r', encoding='utf-8') as fh:
         files_txt = fh.read().splitlines()
     infiles = ['OpenITI_EIS1600_MIUs/training_nasab/' + file for file in files_txt if Path(
             'OpenITI_EIS1600_MIUs/training_nasab/' + file
     ).exists()]
 
     res = []
-    res = p_uimap(get_yml, infiles)
-
-    # for file in infiles[:10]:
-    #     print(file)
-    #     res.append(get_yml(file))
+    if debug:
+        for file in infiles[:10]:
+            print(file)
+            res.append(get_yml(file))
+    else:
+        res = p_uimap(get_yml, infiles)
 
     yml_dict = {}
     for path, yml in res:
         yml_dict[path] = yml
 
     # TODO: Where shall that file be?
     with open('OpenITI_EIS1600_MIUs/gold_standard_yml.json', 'w', encoding='utf-8') as fh:
```

### Comparing `eis1600-0.8.5/eis1600/markdown/UIDs.py` & `eis1600-0.8.6/eis1600/markdown/UIDs.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.5/eis1600/markdown/convert_mARkdown_to_EIS1600TMP.py` & `eis1600-0.8.6/eis1600/markdown/convert_mARkdown_to_EIS1600TMP.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.5/eis1600/markdown/insert_uids.py` & `eis1600-0.8.6/eis1600/markdown/insert_uids.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.5/eis1600/markdown/methods.py` & `eis1600-0.8.6/eis1600/markdown/methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.5/eis1600/markdown/update_uids.py` & `eis1600-0.8.6/eis1600/markdown/update_uids.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.5/eis1600/markdown/update_uids_old_process.py` & `eis1600-0.8.6/eis1600/markdown/update_uids_old_process.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.5/eis1600/miu/HeadingTracker.py` & `eis1600-0.8.6/eis1600/miu/HeadingTracker.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.5/eis1600/miu/disassemble_into_miu_files.py` & `eis1600-0.8.6/eis1600/miu/disassemble_into_miu_files.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.5/eis1600/miu/methods.py` & `eis1600-0.8.6/eis1600/miu/methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.5/eis1600/miu/reassemble_from_miu_files.py` & `eis1600-0.8.6/eis1600/miu/reassemble_from_miu_files.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.5/eis1600/miu/yml_handling.py` & `eis1600-0.8.6/eis1600/miu/yml_handling.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from itertools import combinations
 from typing import Dict, List, Optional, Set, TextIO, Tuple, Union
 
-from eis1600.gazetteers.Toponyms import Toponyms
+from eis1600.gazetteers.Toponyms import Toponyms, YAMLToponym
 from eis1600.helper.markdown_methods import get_yrs_tag_value
 from eis1600.helper.EntityTags import EntityTags
 from eis1600.miu.HeadingTracker import HeadingTracker
 from eis1600.miu.YAMLHandler import YAMLHandler
 from eis1600.helper.markdown_patterns import ENTITY_TAGS_PATTERN, MIU_HEADER_PATTERN, NEWLINES_CROWD_PATTERN
 
 
@@ -56,15 +56,15 @@
             text = NEWLINES_CROWD_PATTERN.sub('\n\n', text)
 
     return miu_yml_header, text
 
 
 def add_to_entities_dict(
         entities_dict: Dict, cat: str,
-        entity: Union[str, Tuple[str, Union[int, str]], List[Tuple[str, str]], List[str], Tuple[int, str]],
+        entity: Union[str, Tuple[str, Union[int, str]], List[Tuple[str, str]], List[str], Tuple[int, str], Dict],
         tag: Optional[str] = None
 ) -> None:
     """Add a tagged entity to the respective list in the entities_dict.
 
     :param Dict entities_dict: Dict containing previous tagged entities.
     :param str cat: Category of the entity.
     :param Union[str|int] entity: Entity - might be int if entity is a date, otherwise str.
@@ -87,60 +87,83 @@
             entities_dict[cat][tag] = [entity]
         elif isinstance(entity, list):
             entities_dict[cat] = entity
         else:
             entities_dict[cat] = [entity]
 
 
+def toponyms_list_to_dict(t_list: List[YAMLToponym]) -> Dict:
+    t_dict = {}
+    for t in t_list:
+        t_dict[t.name] = t.geometry
+
+    return t_dict
+
+
 def add_annotated_entities_to_yml(text_with_tags: str, yml_handler: YAMLHandler, filename: str) -> None:
     """Populates YAMLHeader with annotated entities.
 
     :param str text_with_tags: Text with inserted tags of the MIU.
     :param YAMLHandler yml_handler: YAMLHandler of the MIU.
     :param str filename: Filename of the current MIU (used in error msg).
     """
     # We do not need to differentiate between automated and manual tags
     text_with_tags = text_with_tags.replace('Ü', '')
     entity_tags_df = EntityTags.instance().get_entity_tags_df()
     entities_dict = {}
-    toponyms_set: Set[str] = set()
-    provinces_set: Set[str] = set()
+    nas_dict = {}
+    toponyms_set: Set[YAMLToponym] = set()
+    provinces_set: Set[YAMLToponym] = set()
     nas_counter = 0
 
     m = ENTITY_TAGS_PATTERN.search(text_with_tags)
     while m:
         tag = m.group('entity')
         length = int(m.group('length'))
         entity = ' '.join(text_with_tags[m.end():].split(maxsplit=length)[:length])
 
         cat = entity_tags_df.loc[entity_tags_df['TAG'].str.fullmatch(tag), 'CATEGORY'].iloc[0]
         if cat == 'DATE' or cat == 'AGE':
             try:
                 val = get_yrs_tag_value(m.group(0))
-                add_to_entities_dict(entities_dict, cat, (entity, val))
+                add_to_entities_dict(entities_dict, cat, {'entity': entity, cat.lower(): val})
             except ValueError:
                 print(f'Tag is neither year nor age: {m.group(0)}\nCheck: {filename}')
                 return
         elif cat == 'TOPONYM':
             tg = Toponyms.instance()
             place, uri, list_of_uris, list_of_provinces = tg.look_up_entity(entity)
             if len(list_of_uris) > 1:
                 yml_handler.set_ambigious_toponyms()
             toponyms_set.update(list_of_uris)
             provinces_set.update(list_of_provinces)
-            add_to_entities_dict(entities_dict, cat, (place, uri))
+            add_to_entities_dict(entities_dict, cat, {'entity': place, 'URI': uri})
         elif cat == 'ONOMASTIC':
             if tag.startswith('SHR') and entity.startswith('ب'):
                 entity = entity[1:]
+                add_to_entities_dict(entities_dict, cat, entity, tag)
             elif tag.startswith('NAS'):
-                entity = (nas_counter, entity)
+                nas_dict['nas_' + str(nas_counter)] = entity
                 nas_counter += 1
             add_to_entities_dict(entities_dict, cat, entity, tag)
         else:
             add_to_entities_dict(entities_dict, cat, entity, tag)
 
         m = ENTITY_TAGS_PATTERN.search(text_with_tags, m.end())
 
-    add_to_entities_dict(entities_dict, 'edges_toponym', list(combinations(toponyms_set, 2)))
-    add_to_entities_dict(entities_dict, 'province', list(provinces_set))
-    add_to_entities_dict(entities_dict, 'edges_province', list(combinations(provinces_set, 2)))
+    if nas_dict != {}:
+        if 'onomastics' in entities_dict.keys():
+            entities_dict['onomastics']['nas'] = nas_dict
+        else:
+            entities_dict['onomastics'] = {'nas': nas_dict}
+
+    if 'onomastics' in entities_dict.keys():
+        # Sort dict by keys
+        entities_dict['onomastics'] = dict(sorted(entities_dict.get('onomastics').items()))
+
+    if toponyms_set:
+        entities_dict['places'] = toponyms_list_to_dict(list(toponyms_set))
+        entities_dict['edges_places'] = [[a.coords(), b.coords()] for a, b in combinations(toponyms_set, 2)]
+        provinces_set = set([tg.look_up_province(p) for p in provinces_set])
+        entities_dict['provinces'] = toponyms_list_to_dict(list(provinces_set))
+        entities_dict['edges_provinces'] = [[a.coords(), b.coords()] for a, b in combinations(provinces_set, 2)]
     yml_handler.add_tagged_entities(entities_dict)
```

### Comparing `eis1600-0.8.5/eis1600/nlp/cameltools.py` & `eis1600-0.8.6/eis1600/nlp/cameltools.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.5/eis1600/nlp/ner_annotate_mius.py` & `eis1600-0.8.6/eis1600/nlp/ner_annotate_mius.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.5/eis1600/nlp/utils.py` & `eis1600-0.8.6/eis1600/nlp/utils.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.5/eis1600/onomastics/annotation.py` & `eis1600-0.8.6/eis1600/onomastics/annotation.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,30 +12,35 @@
 
 
 def main():
     arg_parser = ArgumentParser(
             prog=sys.argv[0], formatter_class=RawDescriptionHelpFormatter,
             description='''Script to annotate onomastic information in gold-standard MIUs.'''
     )
+    arg_parser.add_argument('-D', '--debug', action='store_true')
+    arg_parser.add_argument('-T', '--test', action='store_true')
+
+    args = arg_parser.parse_args()
+    debug = args.debug
+    test = args.test
 
     with open('OpenITI_EIS1600_MIUs/gold_standard.txt', 'r', encoding='utf-8') as fh:
         files_txt = fh.read().splitlines()
-    # Uncomment to test on training_data
-    # infiles = ['OpenITI_EIS1600_MIUs/training_data/' + file for file in files_txt if Path(
-    #         'OpenITI_EIS1600_MIUs/training_data/' + file).exists()]
-
-    # test on new batch
-    infiles = glob('OpenITI_EIS1600_MIUs/training_data_nasab_ML2/*.EIS1600')
+    if test:
+        infiles = ['OpenITI_EIS1600_MIUs/training_data/' + file for file in files_txt if Path(
+                'OpenITI_EIS1600_MIUs/training_data/' + file).exists()]
+    else:
+        infiles = glob('OpenITI_EIS1600_MIUs/training_data_nasab_ML2/*.EIS1600')
 
     logger_nasab = setup_logger('nasab_unknown', 'OpenITI_EIS1600_MIUs/logs/nasab_unknown.log')
     res = []
-    res += p_uimap(partial(nasab_annotation, logger_nasab=logger_nasab), infiles)
-
-    # run serialized (nor parallelized)
-    # for file in infiles:
-    #     print(file)
-    #     res.append(nasab_annotation(file, logger_nasab))
+    if debug:
+        for file in infiles:
+            print(file)
+            res.append(nasab_annotation(file, logger_nasab, test))
+    else:
+        res += p_uimap(partial(nasab_annotation, logger_nasab=logger_nasab, test=test), infiles)
 
     with open('gazetteers/tagged.txt', 'w', encoding='utf-8') as fh:
         fh.write('\n\n'.join(res))
 
     print('Done')
```

### Comparing `eis1600-0.8.5/eis1600/onomastics/methods.py` & `eis1600-0.8.6/eis1600/onomastics/methods.py`

 * *Files 5% similar despite different names*

```diff
@@ -157,35 +157,41 @@
         text_updated = text_updated[:pos] + tag + text_updated[pos:]
 
         m = SPELLING.search(text_updated, m.end() + len(tag))
 
     return text_updated
 
 
-def nasab_annotate_miu(df: pd.DataFrame, yml_handler: YAMLHandler, file: str, logger_nasab: Optional[Logger]) -> \
-        Series:
+def nasab_annotate_miu(
+        df: pd.DataFrame, yml_handler: YAMLHandler, file: str, logger_nasab: Optional[Logger],
+        test: Optional[bool] = False
+) -> Series:
     """Onomastic analysis of the nasab part of the MIU.
 
     :param DataFrame df: DataFrame of the MIU.
     :param YAMLHandler yml_handler: YAMLHandler of the MIU.
     :param Path file: the MIU which was opened.
     :param Logger logger_nasab: logs unrecognized uni- and bi-grams to a log file, optional.
+    :param bool test: run on test data set, optional.
     :return Series: a series of the same length as the df containing the nasab tags corresponding to the tokens.
     """
     if not yml_handler.is_bio():
         return Series([nan] * len(df))
 
     s_notna = df['TAGS_LISTS'].loc[df['TAGS_LISTS'].notna()].apply(lambda tag_list: ','.join(tag_list))
     try:
-        # training_data batch uses old NASAB tag, not new ENASAB tag
-        # idx = s_notna.loc[s_notna.str.contains('NASAB')].index[0]
-        idx = s_notna.loc[s_notna.str.contains('ENASAB')].index[0]
+        if test:
+            # training_data batch uses old NASAB tag, not new ENASAB tag
+            idx = s_notna.loc[s_notna.str.contains('NASAB')].index[0]
+        else:
+            idx = s_notna.loc[s_notna.str.contains('ENASAB')].index[0]
     except IndexError:
         print(
-                f'MIU does not have a NASAB tag, most likely the MIU is not a biography but a cross reference. '
+                f'MIU does not have a ENASAB tag, most likely the MIU is not a biography but a cross reference and '
+                f'wrongly labeled. '
                 f'Check:\n{file}'
         )
         return Series([nan] * len(df))
 
     # The following blacklisted elements are considered noise in the text data and are therefore ignored but kept
     blacklist = ['(', ')', '[', ']', '"', "'", '.', '،', '؟', '!', ':', '؛', ',', ';', '?', '|']
     nasab_idx = df.loc[df['TOKENS'].notna() & ~df['TOKENS'].isin(blacklist) & df.index.isin(df.iloc[:idx].index)].index
@@ -216,33 +222,36 @@
     if idx != len(df):
         # TODO make NASAB stay on same line
         df.loc[idx - 1, 'NASAB_END'] = 'NASAB'
 
     return df['NASAB_TAGS'].to_list()
 
 
-def nasab_annotation(file: str, logger_nasab: Logger) -> str:
+def nasab_annotation(file: str, logger_nasab: Logger, test: bool) -> str:
     """Only used for onomastic_annotation cmdline script."""
     with open(file, 'r', encoding='utf-8') as miu_file_object:
         yml_handler, df = get_yml_and_miu_df(miu_file_object)
-    # Only used if run on training_data batch because this information is missing there
-    # if '$' not in df.iloc[0]['SECTIONS'] or '$$$' in df.iloc[0]['SECTIONS'] or not yml_handler.is_reviewed():
-    #     df['NASAB_TAGS'] = Series([nan] * len(df))
-    # else:
-    #     yml_handler.set_category('$')
-    #     df['NASAB_TAGS'] = nasab_annotate_miu(df, yml_handler, file, logger_nasab)
-
-    # Run on new data batch
-    df['NASAB_TAGS'] = nasab_annotate_miu(df, yml_handler, file, logger_nasab)
+    if test:
+        # Only used if run on training_data batch because this information is missing there
+        if '$' not in df.iloc[0]['SECTIONS'] or '$$$' in df.iloc[0]['SECTIONS'] or not yml_handler.is_reviewed():
+            df['NASAB_TAGS'] = Series([nan] * len(df))
+        else:
+            yml_handler.set_category('$')
+            df['NASAB_TAGS'] = nasab_annotate_miu(df, yml_handler, file, logger_nasab, test)
+    else:
+        # Run on new data batch
+        df['NASAB_TAGS'] = nasab_annotate_miu(df, yml_handler, file, logger_nasab, test)
     yml_handler.unset_reviewed()
 
     reconstructed_miu = reconstruct_miu_text_with_tags(df[['SECTIONS', 'TOKENS', 'NASAB_TAGS']])
 
-    # Outpath for training_data batch
-    # output_path = str(file).replace('training_data', 'training_nasab')
-    output_path = str(file)
+    if test:
+        output_path = str(file).replace('training_data', 'training_nasab')
+    else:
+        output_path = str(file)
+
     with open(output_path, 'w', encoding='utf-8') as out_file_object:
         write_updated_miu_to_file(
                 out_file_object, yml_handler, df[['SECTIONS', 'TOKENS', 'TAGS_LISTS', 'NASAB_TAGS']]
         )
 
     return f'{file}\n' + reconstructed_miu
```

### Comparing `eis1600-0.8.5/eis1600/onomastics/re_pattern.py` & `eis1600-0.8.6/eis1600/onomastics/re_pattern.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.5/eis1600/processing/postprocessing.py` & `eis1600-0.8.6/eis1600/processing/postprocessing.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.5/eis1600/processing/preprocessing.py` & `eis1600-0.8.6/eis1600/processing/preprocessing.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.5/eis1600/stats/methods.py` & `eis1600-0.8.6/eis1600/stats/methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.5/eis1600/stats/miu_stats.py` & `eis1600-0.8.6/eis1600/stats/miu_stats.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.5/eis1600.egg-info/PKG-INFO` & `eis1600-0.8.6/eis1600.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eis1600
-Version: 0.8.5
+Version: 0.8.6
 Summary: EIS1600 project tools and utilities
 Home-page: https://github.com/EIS1600/eis1600-pkg
 Author: Lisa Mischer
 Author-email: mischer.lisa@gmail.com
 License: MIT License
 Description: # EIS1600 Tools
```

### Comparing `eis1600-0.8.5/eis1600.egg-info/SOURCES.txt` & `eis1600-0.8.6/eis1600.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 eis1600/helper/fix_miu_annotation.py
 eis1600/helper/logging.py
 eis1600/helper/markdown_methods.py
 eis1600/helper/markdown_patterns.py
 eis1600/helper/miu_random_revisions.py
 eis1600/helper/my_json_ecoder.py
 eis1600/helper/repo.py
+eis1600/helper/yml_methods.py
 eis1600/helper/yml_to_json.py
 eis1600/helper/data/__init__.py
 eis1600/markdown/UIDs.py
 eis1600/markdown/__init__.py
 eis1600/markdown/convert_mARkdown_to_EIS1600TMP.py
 eis1600/markdown/insert_uids.py
 eis1600/markdown/methods.py
```

### Comparing `eis1600-0.8.5/eis1600.egg-info/entry_points.txt` & `eis1600-0.8.6/eis1600.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `eis1600-0.8.5/setup.py` & `eis1600-0.8.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name='eis1600',
-      version='0.8.5',
+      version='0.8.6',
       description='EIS1600 project tools and utilities',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url='https://github.com/EIS1600/eis1600-pkg',
       author='Lisa Mischer',
       author_email='mischer.lisa@gmail.com',
       license='MIT License',
```

