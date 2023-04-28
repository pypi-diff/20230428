# Comparing `tmp/ofscraper-1.80.tar.gz` & `tmp/ofscraper-1.81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofscraper-1.80.tar", max compression
+gzip compressed data, was "ofscraper-1.81.tar", max compression
```

## Comparing `ofscraper-1.80.tar` & `ofscraper-1.81.tar`

### file list

```diff
@@ -1,36 +1,37 @@
--rw-r--r--   0        0        0     1067 2023-04-13 21:26:07.930007 ofscraper-1.80/LICENSE
--rw-r--r--   0        0        0     5388 2023-04-28 11:30:45.292822 ofscraper-1.80/README.md
--rw-r--r--   0        0        0     1235 2023-04-28 11:23:57.457623 ofscraper-1.80/pyproject.toml
--rw-r--r--   0        0        0      620 2023-04-06 15:33:38.742121 ofscraper-1.80/src/__init__.py
--rw-r--r--   0        0        0      733 2023-04-28 05:28:10.687970 ofscraper-1.80/src/__version__.py
--rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.80/src/api/__init__.py
--rw-r--r--   0        0        0     2169 2023-04-28 05:28:10.687970 ofscraper-1.80/src/api/highlights.py
--rw-r--r--   0        0        0      838 2023-04-28 05:28:10.687970 ofscraper-1.80/src/api/init.py
--rw-r--r--   0        0        0     1815 2023-04-06 15:33:38.742121 ofscraper-1.80/src/api/me.py
--rw-r--r--   0        0        0     3580 2023-04-28 05:28:10.687970 ofscraper-1.80/src/api/messages.py
--rw-r--r--   0        0        0     1788 2023-04-28 05:28:10.687970 ofscraper-1.80/src/api/paid.py
--rw-r--r--   0        0        0     7626 2023-04-28 11:23:57.457623 ofscraper-1.80/src/api/posts.py
--rw-r--r--   0        0        0     3247 2023-04-28 05:28:10.687970 ofscraper-1.80/src/api/profile.py
--rw-r--r--   0        0        0     2040 2023-04-06 15:33:38.742121 ofscraper-1.80/src/api/subscriptions.py
--rw-r--r--   0        0        0     5441 2023-04-28 05:28:10.687970 ofscraper-1.80/src/api/timeline.py
--rw-r--r--   0        0        0     4781 2023-04-28 11:23:57.457623 ofscraper-1.80/src/constants.py
--rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.80/src/db/__init__.py
--rw-r--r--   0        0        0    11266 2023-04-28 05:28:10.688970 ofscraper-1.80/src/db/operations.py
--rw-r--r--   0        0        0     3199 2023-04-06 17:48:03.239009 ofscraper-1.80/src/db/queries.py
--rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.80/src/interaction/__init__.py
--rw-r--r--   0        0        0     3169 2023-04-28 05:28:10.688970 ofscraper-1.80/src/interaction/like.py
--rw-r--r--   0        0        0     5080 2023-04-28 05:28:10.688970 ofscraper-1.80/src/prompts/prompt_functions.py
--rw-r--r--   0        0        0      359 2023-04-14 18:21:19.249081 ofscraper-1.80/src/prompts/prompt_strings.py
--rw-r--r--   0        0        0    17909 2023-04-28 11:23:57.457623 ofscraper-1.80/src/prompts/prompts.py
--rwxr-xr-x   0        0        0    18814 2023-04-28 11:23:57.458623 ofscraper-1.80/src/scraper.py
--rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.80/src/utils/__init__.py
--rw-r--r--   0        0        0     2726 2023-04-28 11:23:57.458623 ofscraper-1.80/src/utils/args.py
--rw-r--r--   0        0        0     8856 2023-04-28 05:28:10.689970 ofscraper-1.80/src/utils/auth.py
--rw-r--r--   0        0        0     8874 2023-04-28 11:23:57.458623 ofscraper-1.80/src/utils/config.py
--rw-r--r--   0        0        0      993 2023-04-07 16:49:03.190199 ofscraper-1.80/src/utils/dates.py
--rw-r--r--   0        0        0    10373 2023-04-28 05:28:10.689970 ofscraper-1.80/src/utils/download.py
--rw-r--r--   0        0        0      609 2023-04-06 15:33:38.743121 ofscraper-1.80/src/utils/encoding.py
--rw-r--r--   0        0        0     2513 2023-04-28 05:28:10.690970 ofscraper-1.80/src/utils/paths.py
--rw-r--r--   0        0        0     2998 2023-04-28 05:28:10.690970 ofscraper-1.80/src/utils/profiles.py
--rw-r--r--   0        0        0      779 2023-04-28 05:28:10.690970 ofscraper-1.80/src/utils/separate.py
--rw-r--r--   0        0        0     6597 1970-01-01 00:00:00.000000 ofscraper-1.80/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-13 21:26:07.930007 ofscraper-1.81/LICENSE
+-rw-r--r--   0        0        0     5679 2023-04-28 15:34:09.611256 ofscraper-1.81/README.md
+-rw-r--r--   0        0        0     1235 2023-04-28 12:47:25.736908 ofscraper-1.81/pyproject.toml
+-rw-r--r--   0        0        0      620 2023-04-06 15:33:38.742121 ofscraper-1.81/src/__init__.py
+-rw-r--r--   0        0        0      733 2023-04-28 12:47:25.744908 ofscraper-1.81/src/__version__.py
+-rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.81/src/api/__init__.py
+-rw-r--r--   0        0        0     2169 2023-04-28 05:28:10.687970 ofscraper-1.81/src/api/highlights.py
+-rw-r--r--   0        0        0      838 2023-04-28 05:28:10.687970 ofscraper-1.81/src/api/init.py
+-rw-r--r--   0        0        0     1815 2023-04-06 15:33:38.742121 ofscraper-1.81/src/api/me.py
+-rw-r--r--   0        0        0     3580 2023-04-28 05:28:10.687970 ofscraper-1.81/src/api/messages.py
+-rw-r--r--   0        0        0     1788 2023-04-28 05:28:10.687970 ofscraper-1.81/src/api/paid.py
+-rw-r--r--   0        0        0     7626 2023-04-28 11:23:57.457623 ofscraper-1.81/src/api/posts.py
+-rw-r--r--   0        0        0     3247 2023-04-28 05:28:10.687970 ofscraper-1.81/src/api/profile.py
+-rw-r--r--   0        0        0     2040 2023-04-06 15:33:38.742121 ofscraper-1.81/src/api/subscriptions.py
+-rw-r--r--   0        0        0     5441 2023-04-28 05:28:10.687970 ofscraper-1.81/src/api/timeline.py
+-rw-r--r--   0        0        0     4781 2023-04-28 11:23:57.457623 ofscraper-1.81/src/constants.py
+-rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.81/src/db/__init__.py
+-rw-r--r--   0        0        0    11266 2023-04-28 05:28:10.688970 ofscraper-1.81/src/db/operations.py
+-rw-r--r--   0        0        0     3199 2023-04-06 17:48:03.239009 ofscraper-1.81/src/db/queries.py
+-rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.81/src/interaction/__init__.py
+-rw-r--r--   0        0        0     3169 2023-04-28 05:28:10.688970 ofscraper-1.81/src/interaction/like.py
+-rw-r--r--   0        0        0     5080 2023-04-28 05:28:10.688970 ofscraper-1.81/src/prompts/prompt_functions.py
+-rw-r--r--   0        0        0      359 2023-04-14 18:21:19.249081 ofscraper-1.81/src/prompts/prompt_strings.py
+-rw-r--r--   0        0        0    17909 2023-04-28 11:23:57.457623 ofscraper-1.81/src/prompts/prompts.py
+-rwxr-xr-x   0        0        0    19166 2023-04-28 14:14:09.709648 ofscraper-1.81/src/scraper.py
+-rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.81/src/utils/__init__.py
+-rw-r--r--   0        0        0     2726 2023-04-28 11:23:57.458623 ofscraper-1.81/src/utils/args.py
+-rw-r--r--   0        0        0     8856 2023-04-28 05:28:10.689970 ofscraper-1.81/src/utils/auth.py
+-rw-r--r--   0        0        0     8874 2023-04-28 11:59:24.168331 ofscraper-1.81/src/utils/config.py
+-rw-r--r--   0        0        0      993 2023-04-07 16:49:03.190199 ofscraper-1.81/src/utils/dates.py
+-rw-r--r--   0        0        0    10185 2023-04-28 12:26:51.606240 ofscraper-1.81/src/utils/download.py
+-rw-r--r--   0        0        0      609 2023-04-06 15:33:38.743121 ofscraper-1.81/src/utils/encoding.py
+-rw-r--r--   0        0        0     2937 2023-04-28 14:17:45.092813 ofscraper-1.81/src/utils/exit.py
+-rw-r--r--   0        0        0     2795 2023-04-28 14:37:12.121950 ofscraper-1.81/src/utils/paths.py
+-rw-r--r--   0        0        0     2998 2023-04-28 05:28:10.690970 ofscraper-1.81/src/utils/profiles.py
+-rw-r--r--   0        0        0      779 2023-04-28 05:28:10.690970 ofscraper-1.81/src/utils/separate.py
+-rw-r--r--   0        0        0     6888 1970-01-01 00:00:00.000000 ofscraper-1.81/PKG-INFO
```

### Comparing `ofscraper-1.80/LICENSE` & `ofscraper-1.81/LICENSE`

 * *Files identical despite different names*

### Comparing `ofscraper-1.80/README.md` & `ofscraper-1.81/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -9,29 +9,34 @@
     <li>
         This tool is not affiliated, associated, or partnered with OnlyFans in any way. We are not authorized, endorsed, or sponsored by OnlyFans. All OnlyFans trademarks remain the property of Fenix International Limited.
     </li>
     <li>
         This is a theoritical program only and is for educational purposes. If you choose to use it then it may or may not work. You solely accept full responsability and indemnify the creator, hostors, contributors and all other involved persons from any any all responsability.
     </li>
 
- ## 1.80 Changes:
+ ## 1.81 Changes:
  - sync keys names across config(old keys will still work)
   * change username to model_username in metadata
   * change site_name to sitename in metadata
  - remove --purchased args
  - add purchase and pinned as post types
  - add letter-count argument
-   * This is counting letters and not words for
+   * This is for counting letters and not words for
    textlength
  - added testing 
     * to install run poetry install --with test 
     * run with poetry run pytest
  - print path for each file
  - responsetype mapping in config
     * This is for example keeping all messages or paid post in same folder, but also allow long time users to keep their current structure
+ - added a Post class to serve as a 'single source of truth' for all responsetypes
+ - removed unused functions like download_paid that are no longer needed
+ - prompts and config functions have been revamped
+ - fixed bugs caused by duplicate uploads on pages
+ - additional bugs and fixes
 
   ## Description:
   command-line program to download media, and to process other batch operations such as liking and unliking posts.
     
 
 ![CopyQ nsUBdI](https://user-images.githubusercontent.com/67020411/227816586-fb685959-cd3f-45af-adea-14773b7154f9.png)
```

### Comparing `ofscraper-1.80/pyproject.toml` & `ofscraper-1.81/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ofscraper"
-version = "1.80"
+version = "1.81"
 description = "automatically scrape onlyfans"
 authors = ["datawhores <datawhores@riseup.net>"]
 readme = "README.md"
 packages = [{include = "src"}]
 
 [tool.poetry.dependencies]
 python = ">=3.7.0,<4"
```

### Comparing `ofscraper-1.80/src/__init__.py` & `ofscraper-1.81/src/__init__.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.80/src/__version__.py` & `ofscraper-1.81/src/__version__.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,14 @@
  /  _ \   __\/  ___// ___\_  __ \__  \  /  _ \_/ __ \_  __ \
 (  <_> )  |  \___ \\  \___|  | \// __ \(  <_> )  ___/|  | \/
  \____/|__| /____  >\___  >__|  (____  /\____/ \___  >__|   
                  \/     \/           \/            \/       
 """
 
 __title__ = 'ofscraper'
-__version__ = '1.80'
+__version__ = '1.81'
 __author__ = 'datawhores'
 __author_email__ = 'datawhores@riseup.net'
 __description__ = 'A command-line program to quickly download,like or unlike posts, and more'
 __url__ = 'https://github.com/datawhores/ofscraper'
 __license__ = 'GNU General Public License v3 or later (GPLv3+)'
 __copyright__ = 'Copyright 2023'
```

### Comparing `ofscraper-1.80/src/api/highlights.py` & `ofscraper-1.81/src/api/highlights.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.80/src/api/init.py` & `ofscraper-1.81/src/api/init.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.80/src/api/me.py` & `ofscraper-1.81/src/api/me.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.80/src/api/messages.py` & `ofscraper-1.81/src/api/messages.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.80/src/api/paid.py` & `ofscraper-1.81/src/api/paid.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.80/src/api/posts.py` & `ofscraper-1.81/src/api/posts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.80/src/api/profile.py` & `ofscraper-1.81/src/api/profile.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.80/src/api/subscriptions.py` & `ofscraper-1.81/src/api/subscriptions.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.80/src/api/timeline.py` & `ofscraper-1.81/src/api/timeline.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.80/src/constants.py` & `ofscraper-1.81/src/constants.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.80/src/db/operations.py` & `ofscraper-1.81/src/db/operations.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.80/src/db/queries.py` & `ofscraper-1.81/src/db/queries.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.80/src/interaction/like.py` & `ofscraper-1.81/src/interaction/like.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.80/src/prompts/prompt_functions.py` & `ofscraper-1.81/src/prompts/prompt_functions.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.80/src/prompts/prompts.py` & `ofscraper-1.81/src/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.80/src/scraper.py` & `ofscraper-1.81/src/scraper.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,28 +16,30 @@
 import schedule
 from contextlib import contextmanager
 import threading
 import queue
 from itertools import chain
 import re
 from rich.console import Console
+import traceback
 
 from .prompts import prompts
 console=Console()
 from .constants import donateEP
 from .api import init, highlights, me, messages, profile, subscriptions, paid, timeline
 from .db import operations
 from .interaction import like
 from .utils import auth, config, download, profiles
 import webbrowser
 from halo import Halo
 from .utils.config import read_config
 import src.api.posts as posts_
 import src.utils.args as args_
-
+import src.utils.paths as paths
+import src.utils.exit as exit
 
 
 
 @Halo(text='Getting messages...')
 def process_messages(headers, model_id,username):
     messages_ =asyncio.run(messages.get_messages(headers,  model_id,username)) 
     operations.save_messages_response(messages_,model_id,username)
@@ -492,14 +494,23 @@
             yield
         finally:
             sys.stdout = old_stdout
             sys.stderr = old_stderr
 
 args=args_.getargs()
 def main():
+    with exit.DelayedKeyboardInterrupt(paths.cleanup,False):
+        try:
+            scrapper()
+        except Exception as E:
+            None
+            # console.print(E)
+            # console.print(traceback.format_exc(), style="white")
+        quit()
+def scrapper():
     if platform.system == 'Windows':
         os.system('color')
     # try:
     #     webbrowser.open(donateEP)
     # except:
     #     pass
     global selectedusers
```

### Comparing `ofscraper-1.80/src/utils/args.py` & `ofscraper-1.81/src/utils/args.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.80/src/utils/auth.py` & `ofscraper-1.81/src/utils/auth.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.80/src/utils/config.py` & `ofscraper-1.81/src/utils/config.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.80/src/utils/dates.py` & `ofscraper-1.81/src/utils/dates.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.80/src/utils/download.py` & `ofscraper-1.81/src/utils/download.py`

 * *Files 4% similar despite different names*

```diff
@@ -127,29 +127,25 @@
                         rheaders=r.headers
                         total = int(rheaders['Content-Length'])
                         if file_size_limit and total > int(file_size_limit): 
                                 return 'skipped', 1       
                         content_type = rheaders.get("content-type").split('/')[-1]
                         filename=createfilename(ele,username,model_id,content_type)
                         path_to_file = trunicate(pathlib.Path(path,f"{filename}"))
-
-                        with set_directory(pathlib.Path(pathlib.Path.home(),configPath,get_current_profile(),".tempmedia")):
-                            temp=trunicate(f"{filename}")
-                            pathlib.Path(temp).unlink(missing_ok=True)
-                            with open(temp, 'wb') as f:
-                                pathstr=str(path_to_file)
-                                bar=tqdm(desc=(pathstr[:50] + '....') if len(pathstr) > 50 else pathstr ,total=total, unit_scale=True, unit_divisor=1024, unit='B', leave=False)
-                                num_bytes_downloaded = r.num_bytes_downloaded
-                                async for chunk in r.aiter_bytes(chunk_size=1024):
-                                    f.write(chunk)
-                                    bar.update(
-                                        r.num_bytes_downloaded - num_bytes_downloaded)
-                                    num_bytes_downloaded = r.num_bytes_downloaded
-                        
-                            
+                        temp=trunicate(f"{path_to_file}.part")
+                        pathlib.Path(temp).unlink(missing_ok=True)
+                        with open(temp, 'wb') as f:
+                            pathstr=str(path_to_file)
+                            bar=tqdm(desc=(pathstr[:50] + '....') if len(pathstr) > 50 else pathstr ,total=total, unit_scale=True, unit_divisor=1024, unit='B', leave=False)
+                            num_bytes_downloaded = r.num_bytes_downloaded
+                            async for chunk in r.aiter_bytes(chunk_size=1024):
+                                f.write(chunk)
+                                bar.update(
+                                    r.num_bytes_downloaded - num_bytes_downloaded)
+                                num_bytes_downloaded = r.num_bytes_downloaded                           
                             if pathlib.Path(temp).exists() and  abs(total-pathlib.Path(temp).stat().st_size)<=1000:
                                 shutil.move(temp,path_to_file)
                                 if ele.postdate:
                                     set_time(path_to_file, convert_local_time(ele.postdate))
                                 if id_:
                                     operations.write_media_table(ele,path_to_file,model_id,username)
                                 return media_type,total
```

### Comparing `ofscraper-1.80/src/utils/encoding.py` & `ofscraper-1.81/src/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.80/src/utils/paths.py` & `ofscraper-1.81/src/utils/paths.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from contextlib import contextmanager
 from pathlib import Path
 import pathlib
 import os
 import sys
+import re
 from rich.console import Console
 console=Console()
 import arrow
 
 from ..constants import configPath,DIR_FORMAT_DEFAULT,DATE_DEFAULT,SAVE_LOCATION_DEFAULT
 from ..utils import profiles
 from .config import read_config
 
+
 homeDir=pathlib.Path.home()
 config = read_config()['config']
 @contextmanager
 def set_directory(path: Path):
     """Sets the cwd within the context
 
         Args:``
@@ -60,7 +62,12 @@
 def archiveResponsePathHelper(model_id,username):
     profile = profiles.get_current_profile()
     return homeDir / configPath / profile / ".data"/f"{username}_{model_id}"/"archive.json"
 def pinnedResponsePathHelper(model_id,username):
     profile = profiles.get_current_profile()
     return homeDir / configPath / profile / ".data"/f"{username}_{model_id}"/"pinned.json"
 
+def cleanup():
+    console.print("Cleaning up .part files\n\n")
+    root= pathlib.Path((config.get('save_location') or SAVE_LOCATION_DEFAULT))
+    for file in list(filter(lambda x:re.search("\.part$",str(x))!=None,root.glob("**/*"))):
+        file.unlink(missing_ok=True)
```

### Comparing `ofscraper-1.80/src/utils/profiles.py` & `ofscraper-1.81/src/utils/profiles.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.80/src/utils/separate.py` & `ofscraper-1.81/src/utils/separate.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.80/PKG-INFO` & `ofscraper-1.81/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofscraper
-Version: 1.80
+Version: 1.81
 Summary: automatically scrape onlyfans
 Author: datawhores
 Author-email: datawhores@riseup.net
 Requires-Python: >=3.7.0,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -40,29 +40,34 @@
     <li>
         This tool is not affiliated, associated, or partnered with OnlyFans in any way. We are not authorized, endorsed, or sponsored by OnlyFans. All OnlyFans trademarks remain the property of Fenix International Limited.
     </li>
     <li>
         This is a theoritical program only and is for educational purposes. If you choose to use it then it may or may not work. You solely accept full responsability and indemnify the creator, hostors, contributors and all other involved persons from any any all responsability.
     </li>
 
- ## 1.80 Changes:
+ ## 1.81 Changes:
  - sync keys names across config(old keys will still work)
   * change username to model_username in metadata
   * change site_name to sitename in metadata
  - remove --purchased args
  - add purchase and pinned as post types
  - add letter-count argument
-   * This is counting letters and not words for
+   * This is for counting letters and not words for
    textlength
  - added testing 
     * to install run poetry install --with test 
     * run with poetry run pytest
  - print path for each file
  - responsetype mapping in config
     * This is for example keeping all messages or paid post in same folder, but also allow long time users to keep their current structure
+ - added a Post class to serve as a 'single source of truth' for all responsetypes
+ - removed unused functions like download_paid that are no longer needed
+ - prompts and config functions have been revamped
+ - fixed bugs caused by duplicate uploads on pages
+ - additional bugs and fixes
 
   ## Description:
   command-line program to download media, and to process other batch operations such as liking and unliking posts.
     
 
 ![CopyQ nsUBdI](https://user-images.githubusercontent.com/67020411/227816586-fb685959-cd3f-45af-adea-14773b7154f9.png)
```

