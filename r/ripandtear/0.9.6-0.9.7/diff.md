# Comparing `tmp/ripandtear-0.9.6.tar.gz` & `tmp/ripandtear-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ripandtear-0.9.6.tar", last modified: Sat Apr 22 18:42:07 2023, max compression
+gzip compressed data, was "ripandtear-0.9.7.tar", last modified: Fri Apr 28 18:06:58 2023, max compression
```

## Comparing `ripandtear-0.9.6.tar` & `ripandtear-0.9.7.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxr-x   0 beard     (1000) beard     (1000)        0 2023-04-22 18:42:07.639579 ripandtear-0.9.6/
--rw-rw-r--   0 beard     (1000) beard     (1000)    35064 2023-02-18 23:42:30.000000 ripandtear-0.9.6/LICENSE
--rw-rw-r--   0 beard     (1000) beard     (1000)    17411 2023-04-22 18:42:07.639579 ripandtear-0.9.6/PKG-INFO
--rw-rw-r--   0 beard     (1000) beard     (1000)    17021 2023-04-22 18:41:05.000000 ripandtear-0.9.6/README.md
--rw-rw-r--   0 beard     (1000) beard     (1000)       90 2023-02-20 00:52:42.000000 ripandtear-0.9.6/pyproject.toml
-drwxrwxr-x   0 beard     (1000) beard     (1000)        0 2023-04-22 18:42:07.631579 ripandtear-0.9.6/ripandtear/
--rw-rw-r--   0 beard     (1000) beard     (1000)       22 2023-04-22 18:41:05.000000 ripandtear-0.9.6/ripandtear/__init__.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     8025 2023-04-22 18:41:05.000000 ripandtear-0.9.6/ripandtear/__main__.py
-drwxrwxr-x   0 beard     (1000) beard     (1000)        0 2023-04-22 18:42:07.635579 ripandtear-0.9.6/ripandtear/extractors/
--rw-rw-r--   0 beard     (1000) beard     (1000)        0 2023-02-19 22:50:13.000000 ripandtear-0.9.6/ripandtear/extractors/__init__.py
--rw-rw-r--   0 beard     (1000) beard     (1000)    13425 2023-04-11 15:19:35.000000 ripandtear-0.9.6/ripandtear/extractors/bunkr.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     8646 2023-02-28 02:57:32.000000 ripandtear-0.9.6/ripandtear/extractors/common.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     6740 2023-04-11 15:19:35.000000 ripandtear-0.9.6/ripandtear/extractors/coomer.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     5143 2023-04-11 15:19:35.000000 ripandtear-0.9.6/ripandtear/extractors/cyberdrop.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     2451 2023-04-11 15:19:35.000000 ripandtear-0.9.6/ripandtear/extractors/gfycat.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     5370 2023-04-11 15:19:35.000000 ripandtear-0.9.6/ripandtear/extractors/gofile.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     7926 2023-04-11 15:19:35.000000 ripandtear-0.9.6/ripandtear/extractors/imgur.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     8128 2023-04-11 15:19:35.000000 ripandtear-0.9.6/ripandtear/extractors/jpg.py
--rw-rw-r--   0 beard     (1000) beard     (1000)    18471 2023-04-11 15:19:35.000000 ripandtear-0.9.6/ripandtear/extractors/reddit.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     9382 2023-04-22 18:41:05.000000 ripandtear-0.9.6/ripandtear/extractors/redgifs.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     6065 2023-04-11 15:19:35.000000 ripandtear-0.9.6/ripandtear/extractors/tiktits.py
-drwxrwxr-x   0 beard     (1000) beard     (1000)        0 2023-04-22 18:42:07.639579 ripandtear-0.9.6/ripandtear/utils/
--rw-rw-r--   0 beard     (1000) beard     (1000)        0 2023-02-19 04:04:14.000000 ripandtear-0.9.6/ripandtear/utils/__init__.py
--rw-rw-r--   0 beard     (1000) beard     (1000)    10060 2023-02-28 02:57:32.000000 ripandtear-0.9.6/ripandtear/utils/cli_arguments.py
--rw-rw-r--   0 beard     (1000) beard     (1000)      708 2023-02-27 19:25:42.000000 ripandtear-0.9.6/ripandtear/utils/color.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     6767 2023-04-11 15:19:35.000000 ripandtear-0.9.6/ripandtear/utils/conductor.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     7198 2023-04-22 18:41:05.000000 ripandtear-0.9.6/ripandtear/utils/content_finder.py
--rw-rw-r--   0 beard     (1000) beard     (1000)      870 2023-02-27 19:25:42.000000 ripandtear-0.9.6/ripandtear/utils/custom_types.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     8474 2023-04-11 15:19:35.000000 ripandtear-0.9.6/ripandtear/utils/downloader.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     2847 2023-02-20 00:52:42.000000 ripandtear-0.9.6/ripandtear/utils/file_hasher.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     2369 2023-04-11 15:19:35.000000 ripandtear-0.9.6/ripandtear/utils/file_sorter.py
--rw-rw-r--   0 beard     (1000) beard     (1000)      467 2023-02-27 19:25:42.000000 ripandtear-0.9.6/ripandtear/utils/logger.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     2196 2023-02-27 19:25:42.000000 ripandtear-0.9.6/ripandtear/utils/progress.py
--rw-rw-r--   0 beard     (1000) beard     (1000)    11036 2023-02-28 02:58:35.000000 ripandtear-0.9.6/ripandtear/utils/rat_info.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     4775 2023-02-27 19:25:42.000000 ripandtear-0.9.6/ripandtear/utils/rat_interaction.py
--rw-rw-r--   0 beard     (1000) beard     (1000)     4961 2023-04-11 15:19:35.000000 ripandtear-0.9.6/ripandtear/utils/tracker.py
-drwxrwxr-x   0 beard     (1000) beard     (1000)        0 2023-04-22 18:42:07.635579 ripandtear-0.9.6/ripandtear.egg-info/
--rw-rw-r--   0 beard     (1000) beard     (1000)    17411 2023-04-22 18:42:07.000000 ripandtear-0.9.6/ripandtear.egg-info/PKG-INFO
--rw-rw-r--   0 beard     (1000) beard     (1000)     1111 2023-04-22 18:42:07.000000 ripandtear-0.9.6/ripandtear.egg-info/SOURCES.txt
--rw-rw-r--   0 beard     (1000) beard     (1000)        1 2023-04-22 18:42:07.000000 ripandtear-0.9.6/ripandtear.egg-info/dependency_links.txt
--rw-rw-r--   0 beard     (1000) beard     (1000)       58 2023-04-22 18:42:07.000000 ripandtear-0.9.6/ripandtear.egg-info/entry_points.txt
--rw-rw-r--   0 beard     (1000) beard     (1000)      405 2023-04-22 18:42:07.000000 ripandtear-0.9.6/ripandtear.egg-info/requires.txt
--rw-rw-r--   0 beard     (1000) beard     (1000)       11 2023-04-22 18:42:07.000000 ripandtear-0.9.6/ripandtear.egg-info/top_level.txt
--rw-rw-r--   0 beard     (1000) beard     (1000)     1058 2023-04-22 18:42:07.639579 ripandtear-0.9.6/setup.cfg
+drwxrwxr-x   0 beard     (1000) beard     (1000)        0 2023-04-28 18:06:58.711943 ripandtear-0.9.7/
+-rw-rw-r--   0 beard     (1000) beard     (1000)    35064 2023-02-18 23:42:30.000000 ripandtear-0.9.7/LICENSE
+-rw-rw-r--   0 beard     (1000) beard     (1000)    17411 2023-04-28 18:06:58.711943 ripandtear-0.9.7/PKG-INFO
+-rw-rw-r--   0 beard     (1000) beard     (1000)    17021 2023-04-22 18:41:05.000000 ripandtear-0.9.7/README.md
+-rw-rw-r--   0 beard     (1000) beard     (1000)       90 2023-02-20 00:52:42.000000 ripandtear-0.9.7/pyproject.toml
+drwxrwxr-x   0 beard     (1000) beard     (1000)        0 2023-04-28 18:06:58.679944 ripandtear-0.9.7/ripandtear/
+-rw-rw-r--   0 beard     (1000) beard     (1000)       22 2023-04-28 18:05:18.000000 ripandtear-0.9.7/ripandtear/__init__.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     8025 2023-04-28 17:48:44.000000 ripandtear-0.9.7/ripandtear/__main__.py
+drwxrwxr-x   0 beard     (1000) beard     (1000)        0 2023-04-28 18:06:58.691944 ripandtear-0.9.7/ripandtear/extractors/
+-rw-rw-r--   0 beard     (1000) beard     (1000)        0 2023-02-19 22:50:13.000000 ripandtear-0.9.7/ripandtear/extractors/__init__.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)    13598 2023-04-28 18:05:18.000000 ripandtear-0.9.7/ripandtear/extractors/bunkr.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     8646 2023-02-28 02:57:32.000000 ripandtear-0.9.7/ripandtear/extractors/common.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     6740 2023-04-11 15:19:35.000000 ripandtear-0.9.7/ripandtear/extractors/coomer.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     5143 2023-04-11 15:19:35.000000 ripandtear-0.9.7/ripandtear/extractors/cyberdrop.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     2451 2023-04-11 15:19:35.000000 ripandtear-0.9.7/ripandtear/extractors/gfycat.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     5370 2023-04-11 15:19:35.000000 ripandtear-0.9.7/ripandtear/extractors/gofile.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     7926 2023-04-11 15:19:35.000000 ripandtear-0.9.7/ripandtear/extractors/imgur.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     8128 2023-04-11 15:19:35.000000 ripandtear-0.9.7/ripandtear/extractors/jpg.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)    18471 2023-04-11 15:19:35.000000 ripandtear-0.9.7/ripandtear/extractors/reddit.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     9382 2023-04-22 18:41:05.000000 ripandtear-0.9.7/ripandtear/extractors/redgifs.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     6065 2023-04-11 15:19:35.000000 ripandtear-0.9.7/ripandtear/extractors/tiktits.py
+drwxrwxr-x   0 beard     (1000) beard     (1000)        0 2023-04-28 18:06:58.707943 ripandtear-0.9.7/ripandtear/utils/
+-rw-rw-r--   0 beard     (1000) beard     (1000)        0 2023-02-19 04:04:14.000000 ripandtear-0.9.7/ripandtear/utils/__init__.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)    10060 2023-02-28 02:57:32.000000 ripandtear-0.9.7/ripandtear/utils/cli_arguments.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)      708 2023-02-27 19:25:42.000000 ripandtear-0.9.7/ripandtear/utils/color.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     6767 2023-04-11 15:19:35.000000 ripandtear-0.9.7/ripandtear/utils/conductor.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     7198 2023-04-22 18:41:05.000000 ripandtear-0.9.7/ripandtear/utils/content_finder.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)      870 2023-02-27 19:25:42.000000 ripandtear-0.9.7/ripandtear/utils/custom_types.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     8474 2023-04-11 15:19:35.000000 ripandtear-0.9.7/ripandtear/utils/downloader.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     2847 2023-02-20 00:52:42.000000 ripandtear-0.9.7/ripandtear/utils/file_hasher.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     2369 2023-04-11 15:19:35.000000 ripandtear-0.9.7/ripandtear/utils/file_sorter.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)      467 2023-02-27 19:25:42.000000 ripandtear-0.9.7/ripandtear/utils/logger.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     2196 2023-02-27 19:25:42.000000 ripandtear-0.9.7/ripandtear/utils/progress.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)    11036 2023-02-28 02:58:35.000000 ripandtear-0.9.7/ripandtear/utils/rat_info.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     4775 2023-02-27 19:25:42.000000 ripandtear-0.9.7/ripandtear/utils/rat_interaction.py
+-rw-rw-r--   0 beard     (1000) beard     (1000)     4961 2023-04-11 15:19:35.000000 ripandtear-0.9.7/ripandtear/utils/tracker.py
+drwxrwxr-x   0 beard     (1000) beard     (1000)        0 2023-04-28 18:06:58.683944 ripandtear-0.9.7/ripandtear.egg-info/
+-rw-rw-r--   0 beard     (1000) beard     (1000)    17411 2023-04-28 18:06:58.000000 ripandtear-0.9.7/ripandtear.egg-info/PKG-INFO
+-rw-rw-r--   0 beard     (1000) beard     (1000)     1111 2023-04-28 18:06:58.000000 ripandtear-0.9.7/ripandtear.egg-info/SOURCES.txt
+-rw-rw-r--   0 beard     (1000) beard     (1000)        1 2023-04-28 18:06:58.000000 ripandtear-0.9.7/ripandtear.egg-info/dependency_links.txt
+-rw-rw-r--   0 beard     (1000) beard     (1000)       58 2023-04-28 18:06:58.000000 ripandtear-0.9.7/ripandtear.egg-info/entry_points.txt
+-rw-rw-r--   0 beard     (1000) beard     (1000)      405 2023-04-28 18:06:58.000000 ripandtear-0.9.7/ripandtear.egg-info/requires.txt
+-rw-rw-r--   0 beard     (1000) beard     (1000)       11 2023-04-28 18:06:58.000000 ripandtear-0.9.7/ripandtear.egg-info/top_level.txt
+-rw-rw-r--   0 beard     (1000) beard     (1000)     1058 2023-04-28 18:06:58.711943 ripandtear-0.9.7/setup.cfg
```

### Comparing `ripandtear-0.9.6/LICENSE` & `ripandtear-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.6/PKG-INFO` & `ripandtear-0.9.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ripandtear
-Version: 0.9.6
+Version: 0.9.7
 Summary: An asynchronous file archival program
 Home-page: https://gitlab.com/johnny_barracuda/ripandtear/
 Author: Johnny-Barracuda
 Author-email: johnny_barracuda@protonmail.ch
 Project-URL: Bug Tracker, https://gitlab.com/johnny_barracuda/ripandtear/
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `ripandtear-0.9.6/README.md` & `ripandtear-0.9.7/README.md`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.6/ripandtear/__main__.py` & `ripandtear-0.9.7/ripandtear/__main__.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.6/ripandtear/extractors/bunkr.py` & `ripandtear-0.9.7/ripandtear/extractors/bunkr.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,15 +188,22 @@
             return
 
         url_dictionary['name'] = re_bunkr_single.match(
             url_dictionary['url']).group(6)
 
         url_dictionary['url_to_download'] = str(response.url)
 
-        url_dictionary['file_size'] = response.headers['Content-Length']
+        try:
+            url_dictionary['file_size'] = response.headers['Content-Length']
+
+        except KeyError:
+            log.info(
+                f"No 'Content-Length' found for {response.url}. Link is probably dead")
+            return
+
         url_dictionary['extension'] = response.headers['Content-Type']
         url_dictionary['filename'] = self.common_filename_creator(
             url_dictionary.copy())
 
         log.debug("Url dictionary built. Sending to tracker")
         # print(url_dictionary)
         # return
```

### Comparing `ripandtear-0.9.6/ripandtear/extractors/common.py` & `ripandtear-0.9.7/ripandtear/extractors/common.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.6/ripandtear/extractors/coomer.py` & `ripandtear-0.9.7/ripandtear/extractors/coomer.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.6/ripandtear/extractors/cyberdrop.py` & `ripandtear-0.9.7/ripandtear/extractors/cyberdrop.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.6/ripandtear/extractors/gfycat.py` & `ripandtear-0.9.7/ripandtear/extractors/gfycat.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.6/ripandtear/extractors/gofile.py` & `ripandtear-0.9.7/ripandtear/extractors/gofile.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.6/ripandtear/extractors/imgur.py` & `ripandtear-0.9.7/ripandtear/extractors/imgur.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.6/ripandtear/extractors/jpg.py` & `ripandtear-0.9.7/ripandtear/extractors/jpg.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.6/ripandtear/extractors/reddit.py` & `ripandtear-0.9.7/ripandtear/extractors/reddit.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.6/ripandtear/extractors/redgifs.py` & `ripandtear-0.9.7/ripandtear/extractors/redgifs.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.6/ripandtear/extractors/tiktits.py` & `ripandtear-0.9.7/ripandtear/extractors/tiktits.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.6/ripandtear/utils/cli_arguments.py` & `ripandtear-0.9.7/ripandtear/utils/cli_arguments.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.6/ripandtear/utils/color.py` & `ripandtear-0.9.7/ripandtear/utils/color.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.6/ripandtear/utils/conductor.py` & `ripandtear-0.9.7/ripandtear/utils/conductor.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.6/ripandtear/utils/content_finder.py` & `ripandtear-0.9.7/ripandtear/utils/content_finder.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.6/ripandtear/utils/custom_types.py` & `ripandtear-0.9.7/ripandtear/utils/custom_types.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.6/ripandtear/utils/downloader.py` & `ripandtear-0.9.7/ripandtear/utils/downloader.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.6/ripandtear/utils/file_hasher.py` & `ripandtear-0.9.7/ripandtear/utils/file_hasher.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.6/ripandtear/utils/file_sorter.py` & `ripandtear-0.9.7/ripandtear/utils/file_sorter.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.6/ripandtear/utils/progress.py` & `ripandtear-0.9.7/ripandtear/utils/progress.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.6/ripandtear/utils/rat_info.py` & `ripandtear-0.9.7/ripandtear/utils/rat_info.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.6/ripandtear/utils/rat_interaction.py` & `ripandtear-0.9.7/ripandtear/utils/rat_interaction.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.6/ripandtear/utils/tracker.py` & `ripandtear-0.9.7/ripandtear/utils/tracker.py`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.6/ripandtear.egg-info/PKG-INFO` & `ripandtear-0.9.7/ripandtear.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ripandtear
-Version: 0.9.6
+Version: 0.9.7
 Summary: An asynchronous file archival program
 Home-page: https://gitlab.com/johnny_barracuda/ripandtear/
 Author: Johnny-Barracuda
 Author-email: johnny_barracuda@protonmail.ch
 Project-URL: Bug Tracker, https://gitlab.com/johnny_barracuda/ripandtear/
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `ripandtear-0.9.6/ripandtear.egg-info/SOURCES.txt` & `ripandtear-0.9.7/ripandtear.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ripandtear-0.9.6/setup.cfg` & `ripandtear-0.9.7/setup.cfg`

 * *Files identical despite different names*

