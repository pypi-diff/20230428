# Comparing `tmp/ofscraper-1.81.tar.gz` & `tmp/ofscraper-1.82.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofscraper-1.81.tar", max compression
+gzip compressed data, was "ofscraper-1.82.tar", max compression
```

## Comparing `ofscraper-1.81.tar` & `ofscraper-1.82.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1067 2023-04-13 21:26:07.930007 ofscraper-1.81/LICENSE
--rw-r--r--   0        0        0     5679 2023-04-28 15:34:09.611256 ofscraper-1.81/README.md
--rw-r--r--   0        0        0     1235 2023-04-28 12:47:25.736908 ofscraper-1.81/pyproject.toml
--rw-r--r--   0        0        0      620 2023-04-06 15:33:38.742121 ofscraper-1.81/src/__init__.py
--rw-r--r--   0        0        0      733 2023-04-28 12:47:25.744908 ofscraper-1.81/src/__version__.py
--rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.81/src/api/__init__.py
--rw-r--r--   0        0        0     2169 2023-04-28 05:28:10.687970 ofscraper-1.81/src/api/highlights.py
--rw-r--r--   0        0        0      838 2023-04-28 05:28:10.687970 ofscraper-1.81/src/api/init.py
--rw-r--r--   0        0        0     1815 2023-04-06 15:33:38.742121 ofscraper-1.81/src/api/me.py
--rw-r--r--   0        0        0     3580 2023-04-28 05:28:10.687970 ofscraper-1.81/src/api/messages.py
--rw-r--r--   0        0        0     1788 2023-04-28 05:28:10.687970 ofscraper-1.81/src/api/paid.py
--rw-r--r--   0        0        0     7626 2023-04-28 11:23:57.457623 ofscraper-1.81/src/api/posts.py
--rw-r--r--   0        0        0     3247 2023-04-28 05:28:10.687970 ofscraper-1.81/src/api/profile.py
--rw-r--r--   0        0        0     2040 2023-04-06 15:33:38.742121 ofscraper-1.81/src/api/subscriptions.py
--rw-r--r--   0        0        0     5441 2023-04-28 05:28:10.687970 ofscraper-1.81/src/api/timeline.py
--rw-r--r--   0        0        0     4781 2023-04-28 11:23:57.457623 ofscraper-1.81/src/constants.py
--rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.81/src/db/__init__.py
--rw-r--r--   0        0        0    11266 2023-04-28 05:28:10.688970 ofscraper-1.81/src/db/operations.py
--rw-r--r--   0        0        0     3199 2023-04-06 17:48:03.239009 ofscraper-1.81/src/db/queries.py
--rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.81/src/interaction/__init__.py
--rw-r--r--   0        0        0     3169 2023-04-28 05:28:10.688970 ofscraper-1.81/src/interaction/like.py
--rw-r--r--   0        0        0     5080 2023-04-28 05:28:10.688970 ofscraper-1.81/src/prompts/prompt_functions.py
--rw-r--r--   0        0        0      359 2023-04-14 18:21:19.249081 ofscraper-1.81/src/prompts/prompt_strings.py
--rw-r--r--   0        0        0    17909 2023-04-28 11:23:57.457623 ofscraper-1.81/src/prompts/prompts.py
--rwxr-xr-x   0        0        0    19166 2023-04-28 14:14:09.709648 ofscraper-1.81/src/scraper.py
--rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.81/src/utils/__init__.py
--rw-r--r--   0        0        0     2726 2023-04-28 11:23:57.458623 ofscraper-1.81/src/utils/args.py
--rw-r--r--   0        0        0     8856 2023-04-28 05:28:10.689970 ofscraper-1.81/src/utils/auth.py
--rw-r--r--   0        0        0     8874 2023-04-28 11:59:24.168331 ofscraper-1.81/src/utils/config.py
--rw-r--r--   0        0        0      993 2023-04-07 16:49:03.190199 ofscraper-1.81/src/utils/dates.py
--rw-r--r--   0        0        0    10185 2023-04-28 12:26:51.606240 ofscraper-1.81/src/utils/download.py
--rw-r--r--   0        0        0      609 2023-04-06 15:33:38.743121 ofscraper-1.81/src/utils/encoding.py
--rw-r--r--   0        0        0     2937 2023-04-28 14:17:45.092813 ofscraper-1.81/src/utils/exit.py
--rw-r--r--   0        0        0     2795 2023-04-28 14:37:12.121950 ofscraper-1.81/src/utils/paths.py
--rw-r--r--   0        0        0     2998 2023-04-28 05:28:10.690970 ofscraper-1.81/src/utils/profiles.py
--rw-r--r--   0        0        0      779 2023-04-28 05:28:10.690970 ofscraper-1.81/src/utils/separate.py
--rw-r--r--   0        0        0     6888 1970-01-01 00:00:00.000000 ofscraper-1.81/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-13 21:26:07.930007 ofscraper-1.82/LICENSE
+-rw-r--r--   0        0        0     5679 2023-04-28 17:03:56.331089 ofscraper-1.82/README.md
+-rw-r--r--   0        0        0     1235 2023-04-28 17:03:56.331089 ofscraper-1.82/pyproject.toml
+-rw-r--r--   0        0        0      620 2023-04-06 15:33:38.742121 ofscraper-1.82/src/__init__.py
+-rw-r--r--   0        0        0      733 2023-04-28 17:03:56.331089 ofscraper-1.82/src/__version__.py
+-rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.82/src/api/__init__.py
+-rw-r--r--   0        0        0     2169 2023-04-28 05:28:10.687970 ofscraper-1.82/src/api/highlights.py
+-rw-r--r--   0        0        0      838 2023-04-28 05:28:10.687970 ofscraper-1.82/src/api/init.py
+-rw-r--r--   0        0        0     1815 2023-04-06 15:33:38.742121 ofscraper-1.82/src/api/me.py
+-rw-r--r--   0        0        0     3580 2023-04-28 05:28:10.687970 ofscraper-1.82/src/api/messages.py
+-rw-r--r--   0        0        0     1788 2023-04-28 05:28:10.687970 ofscraper-1.82/src/api/paid.py
+-rw-r--r--   0        0        0     7626 2023-04-28 11:23:57.457623 ofscraper-1.82/src/api/posts.py
+-rw-r--r--   0        0        0     3247 2023-04-28 05:28:10.687970 ofscraper-1.82/src/api/profile.py
+-rw-r--r--   0        0        0     2040 2023-04-06 15:33:38.742121 ofscraper-1.82/src/api/subscriptions.py
+-rw-r--r--   0        0        0     5441 2023-04-28 05:28:10.687970 ofscraper-1.82/src/api/timeline.py
+-rw-r--r--   0        0        0     4781 2023-04-28 11:23:57.457623 ofscraper-1.82/src/constants.py
+-rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.82/src/db/__init__.py
+-rw-r--r--   0        0        0    11266 2023-04-28 05:28:10.688970 ofscraper-1.82/src/db/operations.py
+-rw-r--r--   0        0        0     3199 2023-04-06 17:48:03.239009 ofscraper-1.82/src/db/queries.py
+-rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.82/src/interaction/__init__.py
+-rw-r--r--   0        0        0     3169 2023-04-28 05:28:10.688970 ofscraper-1.82/src/interaction/like.py
+-rw-r--r--   0        0        0     5080 2023-04-28 05:28:10.688970 ofscraper-1.82/src/prompts/prompt_functions.py
+-rw-r--r--   0        0        0      359 2023-04-14 18:21:19.249081 ofscraper-1.82/src/prompts/prompt_strings.py
+-rw-r--r--   0        0        0    17909 2023-04-28 11:23:57.457623 ofscraper-1.82/src/prompts/prompts.py
+-rwxr-xr-x   0        0        0    19166 2023-04-28 14:14:09.709648 ofscraper-1.82/src/scraper.py
+-rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.82/src/utils/__init__.py
+-rw-r--r--   0        0        0     2726 2023-04-28 11:23:57.458623 ofscraper-1.82/src/utils/args.py
+-rw-r--r--   0        0        0     8856 2023-04-28 05:28:10.689970 ofscraper-1.82/src/utils/auth.py
+-rw-r--r--   0        0        0     8874 2023-04-28 11:59:24.168331 ofscraper-1.82/src/utils/config.py
+-rw-r--r--   0        0        0      993 2023-04-07 16:49:03.190199 ofscraper-1.82/src/utils/dates.py
+-rw-r--r--   0        0        0    10235 2023-04-28 16:55:56.692036 ofscraper-1.82/src/utils/download.py
+-rw-r--r--   0        0        0      609 2023-04-06 15:33:38.743121 ofscraper-1.82/src/utils/encoding.py
+-rw-r--r--   0        0        0     2938 2023-04-28 16:51:38.491314 ofscraper-1.82/src/utils/exit.py
+-rw-r--r--   0        0        0     2795 2023-04-28 14:37:12.121950 ofscraper-1.82/src/utils/paths.py
+-rw-r--r--   0        0        0     2998 2023-04-28 05:28:10.690970 ofscraper-1.82/src/utils/profiles.py
+-rw-r--r--   0        0        0      779 2023-04-28 05:28:10.690970 ofscraper-1.82/src/utils/separate.py
+-rw-r--r--   0        0        0     6888 1970-01-01 00:00:00.000000 ofscraper-1.82/PKG-INFO
```

### Comparing `ofscraper-1.81/LICENSE` & `ofscraper-1.82/LICENSE`

 * *Files identical despite different names*

### Comparing `ofscraper-1.81/README.md` & `ofscraper-1.82/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     <li>
         This tool is not affiliated, associated, or partnered with OnlyFans in any way. We are not authorized, endorsed, or sponsored by OnlyFans. All OnlyFans trademarks remain the property of Fenix International Limited.
     </li>
     <li>
         This is a theoritical program only and is for educational purposes. If you choose to use it then it may or may not work. You solely accept full responsability and indemnify the creator, hostors, contributors and all other involved persons from any any all responsability.
     </li>
 
- ## 1.81 Changes:
+ ## 1.82 Changes:
  - sync keys names across config(old keys will still work)
   * change username to model_username in metadata
   * change site_name to sitename in metadata
  - remove --purchased args
  - add purchase and pinned as post types
  - add letter-count argument
    * This is for counting letters and not words for
```

### Comparing `ofscraper-1.81/pyproject.toml` & `ofscraper-1.82/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ofscraper"
-version = "1.81"
+version = "1.82"
 description = "automatically scrape onlyfans"
 authors = ["datawhores <datawhores@riseup.net>"]
 readme = "README.md"
 packages = [{include = "src"}]
 
 [tool.poetry.dependencies]
 python = ">=3.7.0,<4"
```

### Comparing `ofscraper-1.81/src/__init__.py` & `ofscraper-1.82/src/__init__.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.81/src/api/highlights.py` & `ofscraper-1.82/src/api/highlights.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.81/src/api/init.py` & `ofscraper-1.82/src/api/init.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.81/src/api/me.py` & `ofscraper-1.82/src/api/me.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.81/src/api/messages.py` & `ofscraper-1.82/src/api/messages.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.81/src/api/paid.py` & `ofscraper-1.82/src/api/paid.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.81/src/api/posts.py` & `ofscraper-1.82/src/api/posts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.81/src/api/profile.py` & `ofscraper-1.82/src/api/profile.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.81/src/api/subscriptions.py` & `ofscraper-1.82/src/api/subscriptions.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.81/src/api/timeline.py` & `ofscraper-1.82/src/api/timeline.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.81/src/constants.py` & `ofscraper-1.82/src/constants.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.81/src/db/operations.py` & `ofscraper-1.82/src/db/operations.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.81/src/db/queries.py` & `ofscraper-1.82/src/db/queries.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.81/src/interaction/like.py` & `ofscraper-1.82/src/interaction/like.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.81/src/prompts/prompt_functions.py` & `ofscraper-1.82/src/prompts/prompt_functions.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.81/src/prompts/prompts.py` & `ofscraper-1.82/src/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.81/src/scraper.py` & `ofscraper-1.82/src/scraper.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.81/src/utils/args.py` & `ofscraper-1.82/src/utils/args.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.81/src/utils/auth.py` & `ofscraper-1.82/src/utils/auth.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.81/src/utils/config.py` & `ofscraper-1.82/src/utils/config.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.81/src/utils/dates.py` & `ofscraper-1.82/src/utils/dates.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.81/src/utils/download.py` & `ofscraper-1.82/src/utils/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,16 +150,16 @@
                                     operations.write_media_table(ele,path_to_file,model_id,username)
                                 return media_type,total
                             else:
                                 return 'skipped', 1
                     else:
                         r.raise_for_status()
     except Exception as e:
-        if not r or r.status_code==200:
-            print(traceback.format_exc())
+        # if not r or r.status_code==200:
+        #     # print(traceback.format_exc())
         return 'skipped', 1
     finally:
         if bar:
             bar.close()
         if temp:
             pathlib.Path(temp).unlink(missing_ok=True)
         
@@ -185,15 +185,15 @@
     error_content = content.get('error', 'No error message available')
     try:
         return error_content.get('message', 'No error message available')
     except AttributeError:
         return error_content
 def createfilename(ele,username,model_id,ext):
     if ele.responsetype =="profile":
-        return ele.filename
+        return "{filename}.{ext}".format(ext=ext,filename=ele.filename)
     return (config.get('file_format') or FILE_FORMAT_DEFAULT).format(filename=ele.filename,sitename="Onlyfans",site_name="Onlyfans",post_id=ele.id_,media_id=ele.id,first_letter=username[0],mediatype=ele.mediatype,value=ele.value,text=ele.text_,date=arrow.get(ele.postdate).format(config.get('date') or DATE_DEFAULT),ext=ext,model_username=username,model_id=model_id,responsetype=ele.responsetype) 
 
 
 def trunicate(path):
     if platform.system() == 'Windows' and len(str(path))>256:
         return _windows_trunicateHelper(path)
     elif platform.system() == 'Linux':
```

### Comparing `ofscraper-1.81/src/utils/encoding.py` & `ofscraper-1.82/src/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.81/src/utils/exit.py` & `ofscraper-1.82/src/utils/exit.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     def __enter__(self):
         self._old_signal_handler_map = {
             sig: signal.signal(sig, self._handler)
             for sig, _ in SIGNAL_TRANSLATION_MAP.items()
         }
 
     def __exit__(self, exc_type, exc_val, exc_tb):
+
         for sig, handler in self._old_signal_handler_map.items():
             signal.signal(sig, handler)
         self.endprogram()
         if self._sig is None:
             return
         self._old_signal_handler_map[self._sig](self._sig, self._frame)
```

### Comparing `ofscraper-1.81/src/utils/paths.py` & `ofscraper-1.82/src/utils/paths.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.81/src/utils/profiles.py` & `ofscraper-1.82/src/utils/profiles.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.81/src/utils/separate.py` & `ofscraper-1.82/src/utils/separate.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.81/PKG-INFO` & `ofscraper-1.82/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofscraper
-Version: 1.81
+Version: 1.82
 Summary: automatically scrape onlyfans
 Author: datawhores
 Author-email: datawhores@riseup.net
 Requires-Python: >=3.7.0,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -40,15 +40,15 @@
     <li>
         This tool is not affiliated, associated, or partnered with OnlyFans in any way. We are not authorized, endorsed, or sponsored by OnlyFans. All OnlyFans trademarks remain the property of Fenix International Limited.
     </li>
     <li>
         This is a theoritical program only and is for educational purposes. If you choose to use it then it may or may not work. You solely accept full responsability and indemnify the creator, hostors, contributors and all other involved persons from any any all responsability.
     </li>
 
- ## 1.81 Changes:
+ ## 1.82 Changes:
  - sync keys names across config(old keys will still work)
   * change username to model_username in metadata
   * change site_name to sitename in metadata
  - remove --purchased args
  - add purchase and pinned as post types
  - add letter-count argument
    * This is for counting letters and not words for
```

