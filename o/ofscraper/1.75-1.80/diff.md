# Comparing `tmp/ofscraper-1.75.tar.gz` & `tmp/ofscraper-1.80.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofscraper-1.75.tar", max compression
+gzip compressed data, was "ofscraper-1.80.tar", max compression
```

## Comparing `ofscraper-1.75.tar` & `ofscraper-1.80.tar`

### file list

```diff
@@ -1,37 +1,36 @@
--rw-r--r--   0        0        0     1073 2023-04-06 15:33:38.736121 ofscraper-1.75/LICENSE
--rw-r--r--   0        0        0     4533 2023-04-09 16:26:59.278005 ofscraper-1.75/README.md
--rw-r--r--   0        0        0      822 2023-04-09 16:28:46.830053 ofscraper-1.75/pyproject.toml
--rw-r--r--   0        0        0      620 2023-04-06 15:33:38.742121 ofscraper-1.75/src/__init__.py
--rw-r--r--   0        0        0      751 2023-04-09 16:28:46.830053 ofscraper-1.75/src/__version__.py
--rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.75/src/api/__init__.py
--rw-r--r--   0        0        0     3418 2023-04-07 18:59:01.727222 ofscraper-1.75/src/api/highlights.py
--rw-r--r--   0        0        0      755 2023-04-06 15:33:38.742121 ofscraper-1.75/src/api/init.py
--rw-r--r--   0        0        0     1815 2023-04-06 15:33:38.742121 ofscraper-1.75/src/api/me.py
--rw-r--r--   0        0        0     4276 2023-04-08 02:39:37.314542 ofscraper-1.75/src/api/messages.py
--rw-r--r--   0        0        0     2286 2023-04-07 21:33:04.201250 ofscraper-1.75/src/api/paid.py
--rw-r--r--   0        0        0     6006 2023-04-08 02:39:58.242747 ofscraper-1.75/src/api/posts.py
--rw-r--r--   0        0        0     3166 2023-04-06 15:33:38.742121 ofscraper-1.75/src/api/profile.py
--rw-r--r--   0        0        0     2040 2023-04-06 15:33:38.742121 ofscraper-1.75/src/api/subscriptions.py
--rw-r--r--   0        0        0     4069 2023-04-08 17:31:23.478866 ofscraper-1.75/src/constants.py
--rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.75/src/db/__init__.py
--rw-r--r--   0        0        0    11481 2023-04-06 19:59:30.276880 ofscraper-1.75/src/db/operations.py
--rw-r--r--   0        0        0     3199 2023-04-06 17:48:03.239009 ofscraper-1.75/src/db/queries.py
--rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.75/src/interaction/__init__.py
--rw-r--r--   0        0        0     3246 2023-04-07 16:11:58.382914 ofscraper-1.75/src/interaction/like.py
--rwxr-xr-x   0        0        0    21163 2023-04-09 15:49:18.249866 ofscraper-1.75/src/scraper.py
--rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.75/src/utils/__init__.py
--rw-r--r--   0        0        0     8902 2023-04-07 07:23:51.927470 ofscraper-1.75/src/utils/auth.py
--rw-r--r--   0        0        0      694 2023-04-06 15:33:38.742121 ofscraper-1.75/src/utils/browser.py
--rw-r--r--   0        0        0     5025 2023-04-09 12:25:36.153843 ofscraper-1.75/src/utils/config.py
--rw-r--r--   0        0        0      993 2023-04-07 16:49:03.190199 ofscraper-1.75/src/utils/dates.py
--rw-r--r--   0        0        0      372 2023-04-06 15:33:38.742121 ofscraper-1.75/src/utils/decorators.py
--rw-r--r--   0        0        0    17435 2023-04-09 16:19:51.649835 ofscraper-1.75/src/utils/download.py
--rw-r--r--   0        0        0      609 2023-04-06 15:33:38.743121 ofscraper-1.75/src/utils/encoding.py
--rw-r--r--   0        0        0       28 2023-04-06 15:33:38.743121 ofscraper-1.75/src/utils/login.py
--rw-r--r--   0        0        0      418 2023-04-06 15:33:38.743121 ofscraper-1.75/src/utils/nap.py
--rw-r--r--   0        0        0     3160 2023-04-06 15:33:38.743121 ofscraper-1.75/src/utils/old_nap.py
--rw-r--r--   0        0        0     1901 2023-04-06 20:01:03.901832 ofscraper-1.75/src/utils/paths.py
--rw-r--r--   0        0        0     3891 2023-04-07 04:32:57.160701 ofscraper-1.75/src/utils/profiles.py
--rw-r--r--   0        0        0    16171 2023-04-09 12:26:19.702268 ofscraper-1.75/src/utils/prompts.py
--rw-r--r--   0        0        0      750 2023-04-06 15:33:38.743121 ofscraper-1.75/src/utils/separate.py
--rw-r--r--   0        0        0     5676 1970-01-01 00:00:00.000000 ofscraper-1.75/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-13 21:26:07.930007 ofscraper-1.80/LICENSE
+-rw-r--r--   0        0        0     5388 2023-04-28 11:30:45.292822 ofscraper-1.80/README.md
+-rw-r--r--   0        0        0     1235 2023-04-28 11:23:57.457623 ofscraper-1.80/pyproject.toml
+-rw-r--r--   0        0        0      620 2023-04-06 15:33:38.742121 ofscraper-1.80/src/__init__.py
+-rw-r--r--   0        0        0      733 2023-04-28 05:28:10.687970 ofscraper-1.80/src/__version__.py
+-rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.80/src/api/__init__.py
+-rw-r--r--   0        0        0     2169 2023-04-28 05:28:10.687970 ofscraper-1.80/src/api/highlights.py
+-rw-r--r--   0        0        0      838 2023-04-28 05:28:10.687970 ofscraper-1.80/src/api/init.py
+-rw-r--r--   0        0        0     1815 2023-04-06 15:33:38.742121 ofscraper-1.80/src/api/me.py
+-rw-r--r--   0        0        0     3580 2023-04-28 05:28:10.687970 ofscraper-1.80/src/api/messages.py
+-rw-r--r--   0        0        0     1788 2023-04-28 05:28:10.687970 ofscraper-1.80/src/api/paid.py
+-rw-r--r--   0        0        0     7626 2023-04-28 11:23:57.457623 ofscraper-1.80/src/api/posts.py
+-rw-r--r--   0        0        0     3247 2023-04-28 05:28:10.687970 ofscraper-1.80/src/api/profile.py
+-rw-r--r--   0        0        0     2040 2023-04-06 15:33:38.742121 ofscraper-1.80/src/api/subscriptions.py
+-rw-r--r--   0        0        0     5441 2023-04-28 05:28:10.687970 ofscraper-1.80/src/api/timeline.py
+-rw-r--r--   0        0        0     4781 2023-04-28 11:23:57.457623 ofscraper-1.80/src/constants.py
+-rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.80/src/db/__init__.py
+-rw-r--r--   0        0        0    11266 2023-04-28 05:28:10.688970 ofscraper-1.80/src/db/operations.py
+-rw-r--r--   0        0        0     3199 2023-04-06 17:48:03.239009 ofscraper-1.80/src/db/queries.py
+-rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.80/src/interaction/__init__.py
+-rw-r--r--   0        0        0     3169 2023-04-28 05:28:10.688970 ofscraper-1.80/src/interaction/like.py
+-rw-r--r--   0        0        0     5080 2023-04-28 05:28:10.688970 ofscraper-1.80/src/prompts/prompt_functions.py
+-rw-r--r--   0        0        0      359 2023-04-14 18:21:19.249081 ofscraper-1.80/src/prompts/prompt_strings.py
+-rw-r--r--   0        0        0    17909 2023-04-28 11:23:57.457623 ofscraper-1.80/src/prompts/prompts.py
+-rwxr-xr-x   0        0        0    18814 2023-04-28 11:23:57.458623 ofscraper-1.80/src/scraper.py
+-rw-r--r--   0        0        0        1 2023-04-06 15:33:38.742121 ofscraper-1.80/src/utils/__init__.py
+-rw-r--r--   0        0        0     2726 2023-04-28 11:23:57.458623 ofscraper-1.80/src/utils/args.py
+-rw-r--r--   0        0        0     8856 2023-04-28 05:28:10.689970 ofscraper-1.80/src/utils/auth.py
+-rw-r--r--   0        0        0     8874 2023-04-28 11:23:57.458623 ofscraper-1.80/src/utils/config.py
+-rw-r--r--   0        0        0      993 2023-04-07 16:49:03.190199 ofscraper-1.80/src/utils/dates.py
+-rw-r--r--   0        0        0    10373 2023-04-28 05:28:10.689970 ofscraper-1.80/src/utils/download.py
+-rw-r--r--   0        0        0      609 2023-04-06 15:33:38.743121 ofscraper-1.80/src/utils/encoding.py
+-rw-r--r--   0        0        0     2513 2023-04-28 05:28:10.690970 ofscraper-1.80/src/utils/paths.py
+-rw-r--r--   0        0        0     2998 2023-04-28 05:28:10.690970 ofscraper-1.80/src/utils/profiles.py
+-rw-r--r--   0        0        0      779 2023-04-28 05:28:10.690970 ofscraper-1.80/src/utils/separate.py
+-rw-r--r--   0        0        0     6597 1970-01-01 00:00:00.000000 ofscraper-1.80/PKG-INFO
```

### Comparing `ofscraper-1.75/LICENSE` & `ofscraper-1.80/LICENSE`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 excludedBittern8
+Copyright (c) 2023 datawhores
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `ofscraper-1.75/README.md` & `ofscraper-1.80/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,37 @@
 A fork of onlyfans-scraper. It has been optimized to make it more feature complete with dc's onlyfans script.
 A matter of fact with the right settings transitioning between the two scripts should be a easy enough process
 
 In addition there are numerous filtering features to control exactly which type of content you want to scrape.
-https://github.com/excludedBittern8/ofscraper/blob/main/CHANGES.md
+https://github.com/datawhores/ofscraper/blob/main/CHANGES.md
 
 <h3>DISCLAIMERS:</h3>
 <ol>
     <li>
         This tool is not affiliated, associated, or partnered with OnlyFans in any way. We are not authorized, endorsed, or sponsored by OnlyFans. All OnlyFans trademarks remain the property of Fenix International Limited.
     </li>
     <li>
         This is a theoritical program only and is for educational purposes. If you choose to use it then it may or may not work. You solely accept full responsability and indemnify the creator, hostors, contributors and all other involved persons from any any all responsability.
     </li>
 
+ ## 1.80 Changes:
+ - sync keys names across config(old keys will still work)
+  * change username to model_username in metadata
+  * change site_name to sitename in metadata
+ - remove --purchased args
+ - add purchase and pinned as post types
+ - add letter-count argument
+   * This is counting letters and not words for
+   textlength
+ - added testing 
+    * to install run poetry install --with test 
+    * run with poetry run pytest
+ - print path for each file
+ - responsetype mapping in config
+    * This is for example keeping all messages or paid post in same folder, but also allow long time users to keep their current structure
 
   ## Description:
   command-line program to download media, and to process other batch operations such as liking and unliking posts.
     
 
 ![CopyQ nsUBdI](https://user-images.githubusercontent.com/67020411/227816586-fb685959-cd3f-45af-adea-14773b7154f9.png)
 
@@ -30,31 +45,31 @@
 # Windows: 
 ```
 pip install ofscraper
 ```
 or 
 
 ```
-pip install git+https://github.com/excludedBittern8/ofscraper.git 
+pip install git+https://github.com/datawhores/ofscraper.git 
 ```
 
 #  macOS/Linux
 ```
 pip3 install ofscraper
 ```
 or
 ```
-pip3 install git+https://github.com/excludedBittern8/ofscraper.git 
+pip3 install git+https://github.com/datawhores/ofscraper.git 
 ```
 
 ## Authentication
 
 You'll need to retrive your auth information 
     
-https://github.com/excludedBittern8/ofscraper/wiki/Auth
+https://github.com/datawhores/ofscraper/wiki/Auth
 
 
 
 # Usage
 
 Whenever you want to run the program, all you need to do is type `ofscraper` in your terminal:
 
@@ -75,37 +90,38 @@
 
 ![image](https://user-images.githubusercontent.com/67020411/230735256-2d8aa788-53dc-49ee-ada8-5ddf5546851c.png)
 
 ## Selecting specific users
 
 The fuzzy search system can be a little confusing see
     
-https://github.com/excludedBittern8/ofscraper/wiki/Fuzzy-Search 
+https://github.com/datawhores/ofscraper/wiki/Fuzzy-Search 
     
 ## Other menu options    
   
- See: https://github.com/excludedBittern8/ofscraper/wiki/Menu-Options 
+ See: https://github.com/datawhores/ofscraper/wiki/Menu-Options 
  
  # commandline
  While the menu is easy to use, and convient. You may want more automation.
  
  The best way to do this is through the commandline system. This will allow you to skip the menu, and for example scrape a provided list of accounts
  
-  https://github.com/excludedBittern8/ofscraper/wiki/command-line-args
+  https://github.com/datawhores/ofscraper/wiki/command-line-args
  
  # Customazation
     
-https://github.com/excludedBittern8/ofscraper/wiki/Customizing-save-path
-https://github.com/excludedBittern8/ofscraper/wiki/Config-Options
+https://github.com/datawhores/ofscraper/wiki/Customizing-save-path
+https://github.com/datawhores/ofscraper/wiki/Config-Options
 
   
 # Issues
 Open a issue in this repo, or you can mention your issue in the discord
 
-https://discord.gg/zRXgb5Nv
+https://discord.gg/wN7uxEVHRK
+    
     
 ## Common
 ### Status Down
       
 This typically means that your auth information is not correct, or onlyfans signed you out.
 ### 404 Issue 
     
@@ -123,30 +139,35 @@
 
 You will need to change the settings so that the metadata option is compatible with your current folders
 Additionally you might want to set the save_path, dir_path, and filename so they output similar outputs
 
 The metadata path from dc's script is used for duplicate check so as long as your set the right path.
 Files won't download a second time
 
-https://github.com/excludedBittern8/ofscraper/wiki/Migrating-from-DC-script
-https://github.com/excludedBittern8/ofscraper/wiki/Config-Options
-https://github.com/excludedBittern8/ofscraper/wiki/Customizing-save-path
+https://github.com/datawhores/ofscraper/wiki/Migrating-from-DC-script
+https://github.com/datawhores/ofscraper/wiki/Config-Options
+https://github.com/datawhores/ofscraper/wiki/Customizing-save-path
 
 Ask in the discord or open an issue if you need help with what to change to accomplish this
 
 
 
 # Discord
 
-https://discord.gg/zRXgb5Nv
+https://discord.gg/wN7uxEVHRK
     
+# Support
+buymeacoffee.com/datawhores
     
-
-  
+BTC: bc1qcnnetrgmtr86rmqvukl2e24f5upghpcsqqsy87
     
+ETH: 0x1d427a6E336edF6D95e589C16cb740A1372F6609
+
+
+[![codecov](https://codecov.io/github/datawhores/ofscraper/branch/main/graph/badge.svg?token=U1F1PQ7LGM)](https://codecov.io/github/datawhores/ofscraper)
```

### Comparing `ofscraper-1.75/src/__init__.py` & `ofscraper-1.80/src/__init__.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.75/src/__version__.py` & `ofscraper-1.80/src/__version__.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,14 +4,14 @@
  /  _ \   __\/  ___// ___\_  __ \__  \  /  _ \_/ __ \_  __ \
 (  <_> )  |  \___ \\  \___|  | \// __ \(  <_> )  ___/|  | \/
  \____/|__| /____  >\___  >__|  (____  /\____/ \___  >__|   
                  \/     \/           \/            \/       
 """
 
 __title__ = 'ofscraper'
-__version__ = '1.75'
-__author__ = 'excludedBittern8'
-__author_email__ = 'excludedBittern8@riseup.net'
+__version__ = '1.80'
+__author__ = 'datawhores'
+__author_email__ = 'datawhores@riseup.net'
 __description__ = 'A command-line program to quickly download,like or unlike posts, and more'
-__url__ = 'https://github.com/excludedBittern8/ofscraper'
+__url__ = 'https://github.com/datawhores/ofscraper'
 __license__ = 'GNU General Public License v3 or later (GPLv3+)'
 __copyright__ = 'Copyright 2023'
```

### Comparing `ofscraper-1.75/src/api/highlights.py` & `ofscraper-1.80/src/api/highlights.py`

 * *Files 24% similar despite different names*

```diff
@@ -46,29 +46,15 @@
 
 
     
 
 
 
 
-def parse_highlights(highlights: list) -> list:
-    #This needs further work but will work for now. I was thinking of adding full recurssive ability until all conditions are met.
-    #This means that whenever onlyfans changes the name of the list containing the highlights it wont matter because the name is variable.
-    #To break this they would have to change the conditions or in this release the layers.
-    ids= [highlight['id'] for highlight in highlights]
-    results=asyncio.run(process_highlights_ids(auth.make_headers(auth.read_auth()),ids))
-    return parse_stories(results)
-    
-async def process_highlights_ids(headers, ids: list) -> list:
-    if not ids:
-        return []
-
-    tasks = [scrape_story(headers, id_) for id_ in ids]
-    results = await asyncio.gather(*tasks)
-    return list(chain.from_iterable(results))
+
 
 
 @retry(stop=stop_after_attempt(5),wait=wait_random(min=5, max=20),reraise=True)   
 async def scrape_story(headers, story_id: int) -> list:
     async with httpx.AsyncClient(http2=True, headers=headers) as c:
         url = storyEP.format(story_id)
 
@@ -77,15 +63,8 @@
 
         r = await c.get(url, timeout=None)
         if not r.is_error:
             return r.json()['stories']
         r.raise_for_status()
 
 
-def parse_stories(stories: list):
-    output=[]
-    for story in stories:
-        for count, media in enumerate(story["media"]):
-            output.append({"url":media["files"]["source"]["url"],"id":media["id"],"date":media["createdAt"],"responsetype":"stories","count":count+1,"text":None,"mediatype":media["type"],"postid":story["id"],"data":media,"postdate":story['createdAt'],"value":"free"})
-    return output
-
```

### Comparing `ofscraper-1.75/src/api/init.py` & `ofscraper-1.80/src/api/init.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,15 +8,20 @@
                  \/     \/           \/            \/         
 """
 
 from . import me
 from rich.console import Console
 console=Console()
 def print_sign_status(headers):
+    status=getstatus(headers)
+    if status=="UP":
+         print('Status - \033[32mUP\033[0m')
+    else:
+        print('Status - \033[31mDOWN\033[0m')
+
+
+def getstatus(headers):
     try:
         resp = me.scrape_user(headers)
-        print('Status - \033[32mUP\033[0m')
         return "UP"
     except Exception as e:
-        print('Status - \033[31mDOWN\033[0m')
-        return "DOWN"
-       
+        return "DOWN"
```

### Comparing `ofscraper-1.75/src/api/me.py` & `ofscraper-1.80/src/api/me.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.75/src/api/messages.py` & `ofscraper-1.80/src/api/messages.py`

 * *Files 14% similar despite different names*

```diff
@@ -82,18 +82,8 @@
                     return messages
                 global tasks
                 tasks.append(asyncio.create_task(scrape_messages(headers, user_id, recursive=True,message_id=messages[-1]['id'])))
                 return messages
             r.raise_for_status()
 
 
-def parse_messages(messages: list, user_id):
-    messages_with_media =list(filter(lambda message:message['fromUser']['id'] == user_id and message['media'] ,messages))
 
-    messages_urls = []
-    for message in messages_with_media:
-        for count,media in enumerate(list(filter(lambda x:x["canView"]==True,message["media"]))):
-                messages_urls.append({"url":media["source"]["source"],"id":media["id"],"count":count+1,"mediatype":media["type"],
-        "text":message["text"],'responsetype':"messages","date":message["createdAt"],"value":"free" if message["price"]==0 else "paid","postid":message["id"],"postdate":message["createdAt"],"data":message})
-
-    return messages_urls
-
```

### Comparing `ofscraper-1.75/src/api/paid.py` & `ofscraper-1.80/src/api/paid.py`

 * *Files 14% similar despite different names*

```diff
@@ -43,25 +43,20 @@
             headers = auth.make_headers(auth.read_auth())
             auth.add_cookies(c)
             url = purchased_contentEP.format(offset,username)
             offset += 10
             c.headers.update(auth.create_sign(url, headers))
             r = c.get(url, timeout=None)
             if not r.is_error:
-                console.print(f"Scraping, Scraping isn't frozen. It takes time.\nScraped Page: {count}")
+                console.print(f"Scraping paid content, Scraping isn't frozen. It takes time.\nScraped Page: {count}")
                 if "hasMore" in r.json():
                     hasMore = r.json()['hasMore']
                     count=count+1
                 media_to_download.extend(list(filter(lambda x:isinstance(x,list),r.json().values()))[0])
     return media_to_download
 
-def parse_paid(paid):
-    media_to_download=[]
-    for item in paid:
-        for count,media in enumerate(list(filter(lambda x:x.get("source"),item['media']))):
-            media_to_download.append({"id":media["id"],"mediatype":media["type"],"url":media["source"]["source"],"count":count+1,"text":item["text"],"date":item["createdAt"],"responsetype":item["responseType"],"postid":item["id"],"value":"free" if item.get("IsFree") else "paid","postdate":item["createdAt"],"data":item})
-    return media_to_download
+
```

### Comparing `ofscraper-1.75/src/api/posts.py` & `ofscraper-1.80/src/api/timeline.py`

 * *Files 18% similar despite different names*

```diff
@@ -135,19 +135,10 @@
                 return posts
             posts += scrape_archived_posts(
                 headers, model_id, posts[-1]['postedAtPrecise'])
             return posts
         r.raise_for_status()
 
 
-def parse_posts(posts: list):
-    data = list(filter( lambda x:x.get('media')!=None,posts))
-    output=[]
-    for ele in data:
-        medialist=list(filter(lambda x:x["canView"],ele["media"]))
-        for count,media in enumerate(medialist):
-            output.append({"responsetype":ele["responseType"],"id":media["id"],"date":media["createdAt"]
-        ,"text":ele["text"],"count":count+1,"url":media["source"]["source"],"mediatype":media["type"],"value":"paid" if (ele["price"] or 0)>0 else "free" ,"postid":ele["id"],"postdate":ele["postedAt"],"data":ele})
-    return output
-
 
+
```

### Comparing `ofscraper-1.75/src/api/profile.py` & `ofscraper-1.80/src/api/profile.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 import httpx
 from rich.console import Console
 console=Console()
 from tenacity import retry,stop_after_attempt,wait_random
 from ..constants import profileEP
 from ..utils import auth, dates, encoding
+from xxhash import xxh32
 
 @retry(stop=stop_after_attempt(5),wait=wait_random(min=5, max=20),reraise=True)   
 def scrape_profile(headers, username) -> dict:
     with httpx.Client(http2=True, headers=headers) as c:
         url = profileEP.format(username)
 
         auth.add_cookies(c)
@@ -36,15 +37,15 @@
     media = []
     media.append(profile.get('avatar'))
     media.append(profile.get('profile'))
     media=list(filter(lambda x:x!=None,media))
 
     output=[]
     for ele in media:
-        output.append({"url":ele,"responsetype":"profile","mediatype":"images","value":"free","date":profile["joinDate"]})
+        output.append({"url":ele,"responsetype":"profile","mediatype":"photo","value":"free","createdAt":profile["joinDate"],"text":profile["about"],"id":xxh32(ele).hexdigest()})
 
 
     name = encoding.encode_utf_16(profile['name'])
     username = profile['username']
     id_ = profile['id']
     join_date = profile['joinDate']
     posts_count = profile['postsCount']
```

### Comparing `ofscraper-1.75/src/api/subscriptions.py` & `ofscraper-1.80/src/api/subscriptions.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.75/src/db/operations.py` & `ofscraper-1.80/src/db/operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,26 +29,25 @@
     createDir(datebase_path.parent)
     with contextlib.closing(sqlite3.connect(datebase_path,check_same_thread=False)) as conn:
         with contextlib.closing(conn.cursor()) as cur:
             cur.execute(queries.messagesCreate)
             conn.commit()
 
 
-
-def write_messages_table(data: dict, model_id,username):
-    datebase_path =databasePathHelper(model_id,username)
+def write_messages_table(message: dict):
+    datebase_path =databasePathHelper(message.model_id,message.username)
     createDir(datebase_path.parent)
     with contextlib.closing(sqlite3.connect(datebase_path,check_same_thread=False)) as conn:
         with contextlib.closing(conn.cursor()) as cur:
-            if len(cur.execute(queries.messageDupeCheck,(data['id'],)).fetchall())==0:
-                insertData=(data["id"],data["text"],data.get('price') or 0,len(list(filter(lambda x:x['canView']==False,data['media'])))==0,0,data["createdAt"],model_id)
+            if len(cur.execute(queries.messageDupeCheck,(message.id,)).fetchall())==0:
+                insertData=(message.id,message.text,message.price,message.paid,message.archived,message.date,message.model_id)
                 cur.execute(queries.messagesInsert,insertData)
                 conn.commit()
 
-def save_messages_response(model_id,username,messages):
+def save_messages_response(messages,model_id,username):
     messagepath =messageResponsePathHelper(model_id,username)
     createDir(messagepath.parent)
     with open(messagepath,"w") as p:
         p.write(json.dumps({"posts":messages}))
 
 def read_messages_response(model_id,username):
     messagepath =messageResponsePathHelper(model_id,username)
@@ -62,57 +61,57 @@
   
 
 def write_post_table(data: dict, model_id,username):
     datebase_path =databasePathHelper(model_id,username)
     createDir(datebase_path.parent)
     with contextlib.closing(sqlite3.connect(datebase_path,check_same_thread=False)) as conn:
         with contextlib.closing(conn.cursor()) as cur:
-            if len(cur.execute(queries.postDupeCheck,(data['id'],)).fetchall())==0:
-                insertData=(data["id"],data["text"],data.get('price') or 0,data.get("isOpen") or data.get("isOpened") or len(list(filter(lambda x:x['canView']==False,data['media'])))==0 ,data.get("isArchived") or 0,data.get("postedAt" or data.get("createdAt")))
+            if len(cur.execute(queries.postDupeCheck,(data.id,)).fetchall())==0:
+                insertData=(data.id,data.text,data.price,data.paid ,data.archived,data.date)
                 cur.execute(queries.postInsert,insertData)
                 conn.commit()
 
 def create_post_table(model_id,username):
     datebase_path =databasePathHelper(model_id,username)
     createDir(datebase_path.parent)
     with contextlib.closing(sqlite3.connect(datebase_path,check_same_thread=False)) as conn:
         with contextlib.closing(conn.cursor()) as cur:
             cur.execute(queries.postCreate)
             conn.commit()
 
-def save_timeline_response(model_id,username,posts):
+def save_timeline_response(posts,model_id,username,):
     messagepath =timelineResponsePathHelper(model_id,username)
     createDir(messagepath.parent)
     with open(messagepath,"w") as p:	
         p.write(json.dumps({"posts":posts}))
 
 def read_timeline_response(model_id,username):
     messagepath =timelineResponsePathHelper(model_id,username)
     if pathlib.Path(messagepath).exists():
         with open(messagepath,"r") as p:
             messages=json.loads(p.read() or '{"posts": []}')["posts"]
         if len(messages)>0:
             return messages
     return []
             
-def save_archive_response(model_id,username,posts):
+def save_archive_response(posts,model_id,username):
     messagepath =archiveResponsePathHelper(model_id,username)
     createDir(messagepath.parent)
     with open(messagepath,"w") as p:	
         p.write(json.dumps({"posts":posts}))
 
 def read_archive_response(model_id,username):
     messagepath =archiveResponsePathHelper(model_id,username)
     if pathlib.Path(messagepath).exists():
         with open(messagepath,"r") as p:
             messages=json.loads(p.read() or '{"posts": []}')["posts"]
         if len(messages)>0:
             return messages
     return []
-def save_pinned_response(model_id,username,posts):
+def save_pinned_response(posts,model_id,username):
     messagepath =pinnedResponsePathHelper(model_id,username)
     createDir(messagepath.parent)
     with open(messagepath,"w") as p:	
         p.write(json.dumps({"posts":posts}))           
 
 def read_pinned_response(model_id,username):
     messagepath =pinnedResponsePathHelper(model_id,username)
@@ -127,22 +126,21 @@
 def create_stories_table(model_id,username):
     datebase_path =databasePathHelper(model_id,username)
     createDir(datebase_path.parent)
     with contextlib.closing(sqlite3.connect(datebase_path,check_same_thread=False)) as conn:
         with contextlib.closing(conn.cursor()) as cur:
             cur.execute(queries.storiesCreate)
             conn.commit()
-
 def write_stories_table(data: dict, model_id,username):
     datebase_path =databasePathHelper(model_id,username)
     createDir(datebase_path.parent)
     with contextlib.closing(sqlite3.connect(datebase_path,check_same_thread=False)) as conn:
         with contextlib.closing(conn.cursor()) as cur:
-            if len(cur.execute(queries.storiesDupeCheck,(data['id'],)).fetchall())==0:
-                insertData=(data["id"],data.get("text") or data.get("title") or "",0,1 ,0,data["createdAt"])
+            if len(cur.execute(queries.storiesDupeCheck,(data.id,)).fetchall())==0:
+                insertData=(data.id,data.text or data.title or "",data.price,data.paid ,data.archived,data.date)
                 cur.execute(queries.storiesInsert,insertData)
                 conn.commit()
 
 def create_media_table(model_id,username):
     datebase_path =databasePathHelper(model_id,username)
     createDir(datebase_path.parent)
     with contextlib.closing(sqlite3.connect(datebase_path,check_same_thread=False)) as conn:
@@ -153,25 +151,25 @@
 def get_media_ids(model_id,username) -> list:
     datebase_path =databasePathHelper(model_id,username)
     with contextlib.closing(sqlite3.connect(datebase_path,check_same_thread=False)) as conn:
         with contextlib.closing(conn.cursor()) as cur:
             cur.execute(queries.allIDCheck)
             conn.commit()
             return list(map(lambda x:x[0],cur.fetchall()))
-def write_media(data,filename,model_id,username) -> list:
+def write_media_table(media,filename,model_id,username) -> list:
     datebase_path =databasePathHelper(model_id,username)
     with contextlib.closing(sqlite3.connect(datebase_path,check_same_thread=False)) as conn:
         with contextlib.closing(conn.cursor()) as cur:
-            insertData=[data["id"],data["data"]["id"],data['url'],str(pathlib.Path(filename).parent),pathlib.Path(filename).name,
-            math.ceil(pathlib.Path(filename).stat().st_size),data['responsetype'].capitalize(),data['mediatype'].capitalize() ,
-            1 if data["data"].get("preview")!=None else 0,None, 1,data["date"]]
-            if len(cur.execute(queries.mediaDupeCheck,(data['id'],)).fetchall())==0:
+            insertData=[media.id,media.postid,media.url,str(pathlib.Path(filename).parent),pathlib.Path(filename).name,
+            math.ceil(pathlib.Path(filename).stat().st_size),media.responsetype_.capitalize(),media.mediatype.capitalize() ,
+            media.preview,media.linked, 1,media.date]
+            if len(cur.execute(queries.mediaDupeCheck,(media.id,)).fetchall())==0:
                 cur.execute(queries.mediaInsert,insertData)
             else:
-                insertData.append(data["id"])
+                insertData.append(media.id)
                 cur.execute(queries.mediaUpdate,insertData)
             conn.commit()
    
 
 def create_products_table(model_id,username):
     datebase_path =databasePathHelper(model_id,username)
     createDir(datebase_path.parent)
@@ -190,46 +188,48 @@
 def create_profile_table(model_id,username):
     datebase_path =databasePathHelper(model_id,username)
     createDir(datebase_path.parent)
     with contextlib.closing(sqlite3.connect(datebase_path,check_same_thread=False)) as conn:
         with contextlib.closing(conn.cursor()) as cur:
             cur.execute(queries.profilesCreate)
             conn.commit()
-def read_foreign_profile_table(datebase_path):
-    with contextlib.closing(sqlite3.connect(datebase_path,check_same_thread=False)) as conn:
-        with contextlib.closing(conn.cursor()) as cur:
-            cur.execute(queries.profileData)
-            conn.commit()
-            return list(map(lambda x:x,cur.fetchall())) 
+
 
 def write_profile_table(model_id,username) -> list:
     datebase_path =databasePathHelper(model_id,username)
     with contextlib.closing(sqlite3.connect(datebase_path,check_same_thread=False)) as conn:
         with contextlib.closing(conn.cursor()) as cur:
             insertData=[model_id,username]
             if len(cur.execute(queries.profileDupeCheck,(model_id,)).fetchall())==0:
                 cur.execute(queries.profileInsert,insertData)
             else:
                 insertData.append(model_id)
                 cur.execute(queries.profileUpdate,insertData)
             conn.commit()
    
-def read_foreign_database(path) -> list:
-    database_files = glob.glob(path.strip('\'\"') + '/*.db')
-
-    database_results = []
-    for file in database_files:
-        with contextlib.closing(sqlite3.connect(file,check_same_thread=False)) as conn:
-            with contextlib.closing(conn.cursor()) as cur:
-                read_sql = """SELECT media_id, filename FROM medias"""
-                cur.execute(read_sql)
-                for result in cur.fetchall():
-                    database_results.append(result)
+# def read_foreign_profile_table(datebase_path):
+#     with contextlib.closing(sqlite3.connect(datebase_path,check_same_thread=False)) as conn:
+#         with contextlib.closing(conn.cursor()) as cur:
+#             cur.execute(queries.profileData)
+#             conn.commit()
+#             return list(map(lambda x:x,cur.fetchall())) 
+
+# def read_foreign_database(path) -> list:
+#     database_files = glob.glob(path.strip('\'\"') + '/*.db')
+
+#     database_results = []
+#     for file in database_files:
+#         with contextlib.closing(sqlite3.connect(file,check_same_thread=False)) as conn:
+#             with contextlib.closing(conn.cursor()) as cur:
+#                 read_sql = """SELECT media_id, filename FROM medias"""
+#                 cur.execute(read_sql)
+#                 for result in cur.fetchall():
+#                     database_results.append(result)
 
-    return database_results
+#     return database_results
 
 
 
 
 
 # def write_from_foreign_database(results: list, model_id):
 #     profile = profiles.get_current_profile()
```

### Comparing `ofscraper-1.75/src/db/queries.py` & `ofscraper-1.80/src/db/queries.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.75/src/interaction/like.py` & `ofscraper-1.80/src/interaction/like.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,41 +12,41 @@
 import time
 from typing import Union
 import asyncio
 import httpx
 from rich.console import Console
 console=Console()
 from halo import Halo
-from ..api import posts
+from ..api import timeline
 from ..constants import favoriteEP, postURL
 from ..utils import auth
 
 
 def get_posts(headers, model_id,username):
     with Halo(text='Getting posts...'):
-        pinned_posts = posts.scrape_pinned_posts(headers, model_id)
-        timeline_posts = asyncio.run(posts.get_timeline_post(headers, model_id,username))
-        archived_posts = posts.scrape_archived_posts(headers, model_id)
+        pinned_posts = timeline.scrape_pinned_posts(headers, model_id)
+        timeline_posts = asyncio.run(timeline.get_timeline_post(headers, model_id,username))
+        archived_posts = timeline.scrape_archived_posts(headers, model_id)
 
     return pinned_posts + timeline_posts + archived_posts
 
 
 def filter_for_unfavorited(posts: list) -> list:
-    unfavorited_posts = [post for post in posts if 'isFavorite' in post and not post['isFavorite']]
-    return unfavorited_posts
+    return list(filter(lambda x:x.get("isFavorite")==False,posts))
 
 
 def filter_for_favorited(posts: list) -> list:
-    favorited_posts = [post for post in posts if 'isFavorite' in post and post['isFavorite']]
-    return favorited_posts
+    return list(filter(lambda x:x.get("isFavorite")==True,posts))
+
 
 
 def get_post_ids(posts: list) -> list:
-    ids = [post['id'] for post in posts if 'isOpened' in post and post['isOpened']]
-    return ids
+    valid_post=list(filter(lambda x:x.get("isOpened")==True,posts))
+    return list(map(lambda x:x.get("id"),valid_post))
+   
 
 
 def like(headers, model_id, username, ids: list):
     _like(headers, model_id, username, ids, True)
 
 
 def unlike(headers, model_id, username, ids: list):
```

### Comparing `ofscraper-1.75/src/scraper.py` & `ofscraper-1.80/src/scraper.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,166 +4,198 @@
   _____/ ____\______ ________________    ____   ___________ 
  /  _ \   __\/  ___// ___\_  __ \__  \  /  _ \_/ __ \_  __ \
 (  <_> )  |  \___ \\  \___|  | \// __ \(  <_> )  ___/|  | \/
  \____/|__| /____  >\___  >__|  (____  /\____/ \___  >__|   
                  \/     \/           \/            \/         
 """
 
-import argparse
 import asyncio
 import os
 import sys
 import platform
-from random import randint, choice
-from time import sleep
 import time
 import schedule
 from contextlib import contextmanager
 import threading
 import queue
-import functools
 from itertools import chain
 import re
 from rich.console import Console
+
+from .prompts import prompts
 console=Console()
 from .constants import donateEP
-from .api import init, highlights, me, messages, posts, profile, subscriptions, paid
+from .api import init, highlights, me, messages, profile, subscriptions, paid, timeline
 from .db import operations
 from .interaction import like
-from .utils import auth, config, download, profiles, prompts
+from .utils import auth, config, download, profiles
 import webbrowser
 from halo import Halo
-from .utils.nap import nap_or_sleep
-from .__version__ import  __version__
 from .utils.config import read_config
+import src.api.posts as posts_
+import src.utils.args as args_
 
 
 
 
 @Halo(text='Getting messages...')
 def process_messages(headers, model_id,username):
     messages_ =asyncio.run(messages.get_messages(headers,  model_id,username)) 
-    operations.save_messages_response( model_id,username,messages_)
+    operations.save_messages_response(messages_,model_id,username)
+    messages_=list(map(lambda x:posts_.Post(x,model_id,username),messages_))
     for message in messages_:
-     operations.write_messages_table(message,model_id,username)
+     operations.write_messages_table(message)
     output=[]
-    if messages_:
-        [output.extend(messages.parse_messages([ele],model_id)) for ele in messages_] 
-        list(map(lambda x:mediaJsonHelper(x),output))      
-    return output
+    [ output.extend(message.media) for message in messages_]
+    return list(filter(lambda x:isinstance(x,posts_.Media),output))
+
+@Halo(text='Getting Paid Content...')
+def process_paid_post(headers, model_id,username):
+    paid_content=paid.scrape_paid(username)
+    paid_content=list(map(lambda x:posts_.Post(x,model_id,username,responsetype="paid"),paid_content))
+    for post in paid_content:
+        operations.write_post_table(post,model_id,username)
+    output=[]
+    [output.extend(post.media) for post in paid_content]
+    return list(filter(lambda x:isinstance(x,posts_.Media),output))
 
+         
 
 @Halo(text='Getting highlights and stories...')
 def process_highlights(headers, model_id,username):
     highlights_, stories = highlights.scrape_highlights(headers, model_id)
+    highlights_, stories=list(map(lambda x:posts_.Post(x,model_id,username,responsetype="highlights"),highlights_)),\
+    list(map(lambda x:posts_.Post(x,model_id,username,responsetype="stories"),stories))
     for post in highlights_:
         operations.write_stories_table(post,model_id,username)
     for post in stories:
-        operations.write_stories_table(post,model_id,username)    
+        operations.write_stories_table(post,model_id,username)   
+    output=[]
+    output2=[]
+    [ output.extend(highlight.media) for highlight in highlights_]
+    [ output2.extend(stories.media) for stories in stories]
+    return list(filter(lambda x:isinstance(x,posts_.Media),output)),list(filter(lambda x:isinstance(x,posts_.Media),output2))
 
-    highlight_list=list(map(lambda x:mediaJsonHelper(x),highlights.parse_highlights(highlights_)))
-    stories_list=list(map(lambda x:mediaJsonHelper(x),highlights.parse_stories(stories)))
-   
+     
 
-    return highlight_list,stories_list
 
 
 
 
-@Halo(text='Getting archived media...')
-def process_archived_posts(headers, model_id,username):
-    archived_posts = posts.get_archive_post(headers, model_id)
-    operations.save_archive_response(model_id,username,archived_posts)
-    for post in archived_posts:
-        responseJsonHelper(post)
-        operations.write_post_table(post,model_id,username)
-    return list(map(lambda x:mediaJsonHelper(x),posts.parse_posts(archived_posts)))
-
 
 @Halo(text='Getting timeline media...')
 def process_timeline_posts(headers, model_id,username):
-    timeline_posts = asyncio.run(posts.get_timeline_post(headers, model_id,username))
-    operations.save_timeline_response(model_id,username,timeline_posts)
+    timeline_posts = asyncio.run(timeline.get_timeline_post(headers, model_id,username))
+    operations.save_timeline_response(timeline_posts,model_id,username)
+    timeline_posts  =list(map(lambda x:posts_.Post(x,model_id,username,"timeline"), timeline_posts ))
     for post in timeline_posts:
-        responseJsonHelper(post)
         operations.write_post_table(post,model_id,username)
-    return list(map(lambda x:mediaJsonHelper(x),posts.parse_posts(timeline_posts)))
+    output=[]
+    [output.extend(post.media) for post in  timeline_posts ]
+    return list(filter(lambda x:isinstance(x,posts_.Media),output))
+
+@Halo(text='Getting archived media...')
+def process_archived_posts(headers, model_id,username):
+    archived_posts = timeline.get_archive_post(headers, model_id)
+    operations.save_archive_response(archived_posts,model_id,username)
+    archived_posts =list(map(lambda x:posts_.Post(x,model_id,username),archived_posts ))
+    for post in archived_posts:
+        operations.write_post_table(post,model_id,username)
+    output=[]
+    [ output.extend(post.media) for post in archived_posts ]
+    return list(filter(lambda x:isinstance(x,posts_.Media),output))
+
 
 
 
 @Halo(text='Getting pinned media...')
 def process_pinned_posts(headers, model_id,username):
-    pinned_posts = posts.get_pinned_post(headers, model_id,username)
-    operations.save_pinned_response(model_id,username, pinned_posts)
+    pinned_posts = timeline.get_pinned_post(headers, model_id,username)
+    operations.save_pinned_response(pinned_posts,model_id,username)
+    pinned_posts =list(map(lambda x:posts_.Post(x,model_id,username,"pinned"),pinned_posts ))
     for post in  pinned_posts:
-        responseJsonHelper(post)
         operations.write_post_table(post,model_id,username)
-    timeline_posts_urls = posts.parse_posts( pinned_posts)
-    return list(map(lambda x:mediaJsonHelper(x),posts.parse_posts(timeline_posts_urls)))
-
-
-
+    output=[]
+    [ output.extend(post.media) for post in pinned_posts ]
+    return list(filter(lambda x:isinstance(x,posts_.Media),output))
 
 def process_profile(headers, username) -> list:
     user_profile = profile.scrape_profile(headers, username)
     urls, info = profile.parse_profile(user_profile)
     profile.print_profile_info(info)
-    return urls
+    output=[]
+    for ele in enumerate(urls):
+        count=ele[0]
+        data=ele[1]
+        output.append(posts_.Media({"url":data["url"],"type":data["mediatype"]},count,posts_.Post(data,info[2],username,responsetype="profile")))
+    return output
 
 
 
 
 def process_areas(headers, ele, model_id) -> list:
     args.posts = list(map(lambda x:x.capitalize(),(args.posts or prompts.areas_prompt())
 ))
     timeline_posts_dicts  = []
     pinned_post_dict=[]
     archived_posts_dicts  = []
     highlights_dicts  = []
     messages_dicts  = []
     stories_dicts=[]
+    purchased_dict=[]
+    pinned_post_dict=[]
 
     username=ele['name']
     profile_dicts  = process_profile(headers,username)
 
+     
+    if ('Pinned' in args.posts or 'All' in args.posts) and ele["active"]:
+            pinned_post_dict = process_pinned_posts(headers, model_id,username)
     if ('Timeline' in args.posts or 'All' in args.posts) and ele["active"]:
             timeline_posts_dicts = process_timeline_posts(headers, model_id,username)
-            pinned_post_dict=process_pinned_posts(headers, model_id,username)
     if ('Archived' in args.posts or 'All' in args.posts) and ele["active"]:
             archived_posts_dicts = process_archived_posts(headers, model_id,username)
     if 'Messages' in args.posts or 'All' in args.posts:
             messages_dicts = process_messages(headers, model_id,username)
-
+    if "Purchased" in args.posts or "All" in args.posts:
+            purchased_dict=process_paid_post(headers, model_id,username)
     if ('Highlights'  in args.posts or 'Stories'  in args.posts or 'All' in args.posts)   and ele["active"]:
-            highlights_tuple = process_highlights(headers, model_id,username)
-            if 'All' in args.posts:
+            highlights_tuple = process_highlights(headers, model_id,username)  
+            if 'Highlights'  in args.posts:
                 highlights_dicts=highlights_tuple[0]
-                stories_dicts=highlights_tuple[1]    
-            elif 'Highlights'  in args.posts:
+            if 'Stories'  in args.posts:
+                stories_dicts=highlights_tuple[1]   
+            if 'All' in args.posts:
                 highlights_dicts=highlights_tuple[0]
-            elif 'Stories'  in args.posts:
-                stories_dicts=highlights_tuple[1]    
-    return posts_filter(list(chain(*[profile_dicts  , timeline_posts_dicts ,pinned_post_dict,
+                stories_dicts=highlights_tuple[1]               
+    return posts_filter(list(chain(*[profile_dicts  , timeline_posts_dicts ,pinned_post_dict,purchased_dict,
             archived_posts_dicts , highlights_dicts , messages_dicts,stories_dicts]))
 
 )
 
 def posts_filter(posts):
     filtersettings=config.read_config()["config"].get('filter')
+    output=[]
+    ids=set()
+    for post in posts:
+        if not post.id or post.id not in ids:
+            output.append(post)
+            ids.add(post.id)
     if isinstance(filtersettings,str):
         filtersettings=filtersettings.split(",")
     if isinstance(filtersettings,list):
         filtersettings=list(map(lambda x:x.lower().replace(" ",""),filtersettings))
         filtersettings=list(filter(lambda x:x!="",filtersettings))
         if len(filtersettings)==0:
             return posts
         console.print(f"filtering post to {filtersettings}")
-        return list(filter(lambda x:x["mediatype"] in filtersettings,posts))
-    console.print("The settings you picked for the filter are not valid\nNot Filtering")
-    return posts
+        return list(filter(lambda x:x.mediatype.lower() in filtersettings,output))
+    else:
+        console.print("The settings you picked for the filter are not valid\nNot Filtering")
+        return output
         
 
 
 def do_database_migration():
     operations.user_db_migration()
 
 
@@ -205,31 +237,28 @@
     me.print_user(name, username)
     return subscribe_count
 
 def setfilter():
     if prompts.decide_filters_prompts()=="Yes":
         global args
         args=prompts.modify_filters_prompt(args)
+        args_.changeargs(args)
 
 def process_prompts():
     changeusernames=True
     while  True:
         args.posts=None
         result_main_prompt = prompts.main_prompt()
         if changeusernames and result_main_prompt in [0,1,2]:
             setfilter()
             getselected_usernames()
         #download
         if result_main_prompt == 0:
             check_auth()
-            if prompts.download_paid_prompt()=="Yes":
-                process_post()
-                process_paid()
-            else:
-                process_post()     
+            process_post()     
 
         # like a user's posts
         elif result_main_prompt == 1:
             check_auth()
             process_like()
         # Unlike a user's posts
         elif result_main_prompt == 2:
@@ -290,59 +319,16 @@
         if selectedusers:
             changeusernames=False
             console.print(f"Currently Selected Users\n{list(map(lambda x:x['name'],selectedusers))}")
             if prompts.reset_username_prompt()=="Yes":
                 selectedusers=None
                 changeusernames=True
         
-def process_paid():
 
 
-    profiles.print_current_profile()
-    headers = auth.make_headers(auth.read_auth())
-
-    init.print_sign_status(headers)
-    userdata=getselected_usernames()
-    for ele in userdata:
-        print(f"Getting paid content for {ele['name']}")
-        try:
-            model_id = profile.get_id(headers, ele["name"])
-            create_tables(model_id,ele['name'])
-            operations.write_profile_table(model_id,ele['name'])
-            paid_url=process_paid_post(model_id,ele['name'])
-            profile.print_paid_info(paid_url,ele["name"])
-            asyncio.run(download.process_dicts_paid(
-            ele["name"],
-            model_id,
-            paid_url,
-            forced=args.dupe,
-            ))
-        except Exception as e:
-            console.print("run failed with exception: ", e)
-
-def process_paid_post(model_id,username):
-    paid_content=paid.scrape_paid(username)
-    for post in paid_content:
-        responseJsonHelper(post)
-        operations.write_post_table(post,model_id,username)
-    return list(map(lambda x:mediaJsonHelper(x),paid.parse_paid(paid_content)))
-def responseJsonHelper(data):
-    if data.get("responseType")=="post":
-        data["responseType"]="posts"
-    elif data.get("responseType")=="message":
-        data["responseType"]="messages"
-    return data
-def mediaJsonHelper(data):
-    if data.get("mediatype")=="photo" or data.get("mediatype")=="gif" :
-        data["mediatype"]="images"
-    elif data.get("mediatype")=="audio":
-        data["mediatype"]="audios"
-    elif data.get("mediatype")=="video":
-        data["mediatype"]="videos"
-    return data         
 def process_post():
     profiles.print_current_profile()
     headers = auth.make_headers(auth.read_auth())
     init.print_sign_status(headers)
     userdata=getselected_usernames()
     for ele in userdata:
         print(f"Getting Selected post type(s) for {ele['name']}\nSubscription Active: {ele['active']}")
@@ -430,15 +416,15 @@
             job_func()
             jobqueue.task_done()
                 
 def check_auth():
     status=None
     while status!="UP":
         headers = auth.make_headers(auth.read_auth())
-        status=init.print_sign_status(headers)
+        status=init.getstatus(headers)
         if status=="DOWN":
             auth.make_auth(auth=auth.read_auth())
             continue
         break
         
 
     
@@ -491,92 +477,56 @@
     operations.create_message_table(model_id,username)
     operations.create_media_table(model_id,username)
     operations.create_products_table(model_id,username)
     operations.create_others_table(model_id,username)
     operations.create_profile_table(model_id,username)
     operations.create_stories_table(model_id,username)
 
+@contextmanager
+def suppress_stdout():
+    with open(os.devnull, "w") as devnull:
+        old_stdout = sys.stdout
+        old_stderr=sys.stderr
+        sys.stdout = devnull
+        sys.stderr = devnull
+        try:  
+            yield
+        finally:
+            sys.stdout = old_stdout
+            sys.stderr = old_stderr
 
-
+args=args_.getargs()
 def main():
-    global args
     if platform.system == 'Windows':
         os.system('color')
     # try:
     #     webbrowser.open(donateEP)
     # except:
     #     pass
-
-
-    parser = argparse.ArgumentParser()
-
-    parser = argparse.ArgumentParser(add_help=False)   
-    general=parser.add_argument_group("General",description="General Args")  
-    general.add_argument('-v', '--version', action='version', version='%(prog)s ' + __version__)
-    general.add_argument('-h', '--help', action='help')
-
-                                    
-    general.add_argument(
-        '-u', '--username', help="select which username to process (name,name2)\nSet to ALL for all users",type=lambda x: list(filter( lambda y:y!="",x.split(",")))
-    )
-    general.add_argument(
-        '-d', '--daemon', help='run script in the background\nSet value to minimum minutes between script runs\nOverdue runs will run as soon as previous run finishes', type=int,default=None
-    )
-    general.add_argument(
-        '-s', '--silent', help = 'mute output', action = 'store_true',default=False
-    )
-    post=parser.add_argument_group("Post",description="What type of post to scrape")                                      
-
-    post.add_argument("-e","--dupe",action="store_true",default=False,help="Bypass the dupe check and redownload all files")
-    post.add_argument(
-        '-o', '--posts', help = 'Download content from a models wall',default=None,required=False,type = str.lower,choices=["highlights","all","archived","messages","timeline","stories"],nargs="*"
-    )
-    post.add_argument("-p","--purchased",action="store_true",default=False,help="Download individually purchased content")
-    post.add_argument("-a","--action",default=None,help="perform like or unlike action on each post",choices=["like","unlike"])
-
-     #Filters for accounts
-    filters=parser.add_argument_group("filters",description="Filters out usernames based on selected parameters")
-    
-    filters.add_argument(
-        '-t', '--account-type', help = 'Filter Free or paid accounts',default=None,required=False,type = str.lower,choices=["paid","free"]
-    )
-    filters.add_argument(
-        '-r', '--renewal', help = 'Filter by whether renewal is on or off for account',default=None,required=False,type = str.lower,choices=["active","disabled"]
-    )
-    filters.add_argument(
-        '-ss', '--sub-status', help = 'Filter by whether or not your subscription has expired or not',default=None,required=False,type = str.lower,choices=["active","expired"]
-    )
-
-     #Paths
-    paths=parser.add_argument_group("paths",description="Change or forced paths in program")
-
-    args = parser.parse_args()
     global selectedusers
     selectedusers=None
-    read_config()
 
 
     
-    if len(list(filter(lambda x:x!=None and x!=False,[args.action,args.purchased,args.posts])))==0:
+    if len(list(filter(lambda x:x!=None and x!=False,[args.action,args.posts])))==0:
         if args.daemon:
             console.print("You need to pass at least one scraping method\n--action\n--posts\n--purchase\nAre all valid options. Skipping and going to menu")
         process_prompts()
         sys.exit(0)
     
 
 
 
     if args.posts: 
         check_auth()
         run(process_post)        
-    if args.purchased:
-        check_auth()
-        run(process_paid)
     if args.action=="like":
         check_auth()
         run(process_like)
     if args.action=="unlike":
         check_auth()    
         run(process_unlike)  
 
 if __name__ == '__main__':
     main()
+
+
```

### Comparing `ofscraper-1.75/src/utils/auth.py` & `ofscraper-1.80/src/utils/auth.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,17 +14,16 @@
 import time
 from urllib.parse import urlparse
 import requests
 from rich.console import Console
 console=Console()
 import httpx
 import browser_cookie3
-from src.utils.browser import getuseragent
 from .profiles import get_current_profile
-from .prompts import auth_prompt, ask_make_auth_prompt,browser_prompt,\
+from ..prompts.prompts import auth_prompt, ask_make_auth_prompt,browser_prompt,\
 user_agent_prompt,xbc_prompt,auth_full_paste,manual_auth_prompt
 from ..constants import configPath, authFile, DC_EP, requestAuth
 
 
 
 def read_auth():
     make_request_auth()
@@ -109,15 +108,15 @@
 
     auth= auth or defaultAuth
     if  browserSelect!="Enter Each Field Manually" and browserSelect!="Paste From Cookie Helper":
         temp=requests.utils.dict_from_cookiejar(getattr(browser_cookie3, browserSelect.lower())(domain_name="onlyfans"))
         auth=auth or  defaultAuth
         for key in ["sess","auth_id","auth_uid_"]:
             auth["auth"][key]=temp.get(key,"")
-        console.print("You'll need to go to onlyfans.com and retrive header information\nGo to https://github.com/excludedBittern8/ofscraper and find the section named 'Getting Your Auth Info'\nCookie information has been retived automatically\nSo You only need to retrive the x-bc header and the user-agent",style="yellow")
+        console.print("You'll need to go to onlyfans.com and retrive header information\nGo to https://github.com/datawhores/ofscraper and find the section named 'Getting Your Auth Info'\nCookie information has been retived automatically\nSo You only need to retrive the x-bc header and the user-agent",style="yellow")
         if not auth["auth"].get("x-bc"):
             auth["auth"]["x-bc"]=xbc_prompt()
         auth["auth"]["user_agent"]= user_agent_prompt(auth["auth"].get("user_agent") or "")
 
 
  
     elif browserSelect=="Paste From Cookie Helper":
@@ -137,15 +136,15 @@
                 auth["auth"]["sess"]=ele.replace("sess=","")
             elif ele.find("auth_uid")!=-1:
                 auth["auth"]["auth_uid_"]=ele.replace("auth_uid_","").replace("=","")
            
 
 
     else:
-        console.print("You'll need to go to onlyfans.com and retrive header information\nGo to https://github.com/excludedBittern8/ofscraper and find the section named 'Getting Your Auth Info'\nYou only need to retrive the x-bc header,the user-agent, and cookie information",style="yellow")
+        console.print("You'll need to go to onlyfans.com and retrive header information\nGo to https://github.com/datawhores/ofscraper and find the section named 'Getting Your Auth Info'\nYou only need to retrive the x-bc header,the user-agent, and cookie information",style="yellow")
         auth['auth'].update(auth_prompt(auth['auth']))
     
     console.print(f"{auth}\nWriting to {path / authFile}",style="yellow")
     with open(path / authFile, 'w') as f:
         f.write(json.dumps(auth, indent=4))
```

### Comparing `ofscraper-1.75/src/utils/dates.py` & `ofscraper-1.80/src/utils/dates.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.75/src/utils/encoding.py` & `ofscraper-1.80/src/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `ofscraper-1.75/src/utils/paths.py` & `ofscraper-1.80/src/utils/paths.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from contextlib import contextmanager
 from pathlib import Path
 import pathlib
 import os
 import sys
 from rich.console import Console
 console=Console()
+import arrow
 
-from ..constants import configPath
+from ..constants import configPath,DIR_FORMAT_DEFAULT,DATE_DEFAULT,SAVE_LOCATION_DEFAULT
 from ..utils import profiles
 from .config import read_config
 
 homeDir=pathlib.Path.home()
 config = read_config()['config']
 @contextmanager
 def set_directory(path: Path):
@@ -34,17 +35,20 @@
 def createDir(path):
     try:
         path.mkdir(exist_ok=True,parents=True)
     except:
         console.print("Error creating directory, check the directory and make sure correct permissions have been issued.")
         sys.exit()
 def databasePathHelper(model_id,username):
-    return pathlib.Path(config.get("metadata").format(configpath=homeDir / configPath,profile=profiles.get_current_profile(),username=username,model_id=model_id,sitename="Onlyfans",first_letter=username[0]),"user_data.db)")
+    return pathlib.Path(config.get("metadata").format(configpath=homeDir / configPath,profile=profiles.get_current_profile(),model_username=username,username=username,model_id=model_id,sitename="Onlyfans",site_name="Onlyfans",first_letter=username[0]),"user_data.db")
 
-    
+def getmediadir(ele,username,model_id):
+    root= pathlib.Path((config.get('save_location') or SAVE_LOCATION_DEFAULT))
+    downloadDir=(config.get('dir_format') or DIR_FORMAT_DEFAULT ).format(sitename="onlyfans",first_letter=username[0].capitalize(),model_id=model_id,model_username=username,responsetype=ele.responsetype.capitalize(),mediatype=ele.mediatype.capitalize(),value=ele.value.capitalize(),date=arrow.get(ele.postdate).format(config.get('date') or DATE_DEFAULT))
+    return root /downloadDir   
 
 
 def messageResponsePathHelper(model_id,username):
     profile = profiles.get_current_profile()
     return homeDir / configPath / profile / ".data"/f"{username}_{model_id}"/"messages.json"
```

### Comparing `ofscraper-1.75/src/utils/prompts.py` & `ofscraper-1.80/src/prompts/prompts.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,167 +13,113 @@
 import sys
 from rich.console import Console
 import pathlib
 console=Console()
 from InquirerPy.resolver import prompt
 from InquirerPy.separator import Separator
 from InquirerPy.base import Choice
+from InquirerPy.validator import EmptyInputValidator,PathValidator
 
-from ..constants import mainPromptChoices, usernameOrListChoices, profilesPromptChoices
-
-
+from ..constants import mainPromptChoices, profilesPromptChoices,FILTER_DEFAULT
+from .prompt_strings import CHECKLISTINSTRUCTIONS,FUZZY_INSTRUCTION
+from .prompt_functions import cleanTextInput,emptyListValidator,jsonValidator,jsonloader,namevalitator,dirformatvalidator \
+,dateplaceholdervalidator,fileformatvalidator,metadatavalidator
+import src.utils.config as config
 def main_prompt() -> int:
     main_prompt_choices = [*mainPromptChoices]
     main_prompt_choices.insert(3, Separator())
 
     name = 'action'
 
     questions = [
         {
             'type': 'list',
             'name': name,
             'message': 'What would you like to do?',
-            'choices': [*main_prompt_choices]
+            'choices': [*main_prompt_choices],
         }
     ]
 
     answer = prompt(questions)
     return mainPromptChoices[answer[name]]
 
 
-def username_or_list_prompt() -> int:
-    name = 'username_or_list'
-
-    questions = [
-        {
-            'type': 'list',
-            'name': name,
-            'message': 'Choose one of the following options:',
-            'choices': [*usernameOrListChoices]
-        }
-    ]
-
-    answer = prompt(questions)
-    return usernameOrListChoices[answer[name]]
-
 
-def verify_all_users_username_or_list_prompt() -> bool:
-    name = 'all_users'
-
-    questions = [
-        {
-            'type': 'confirm',
-            'name': name,
-            'message': 'Are you sure you want to scrape every model that you\'re subscribed to?',
-            'default': False
-        }
-    ]
 
-    answer = prompt(questions)
-    return answer[name]
 
 
-def username_prompt() -> str:
-    name = 'username'
 
-    questions = [
-        {
-            'type': 'input',
-            'name': name,
-            'message': 'Enter a comma seperated list of model\'s usernames:'
-        }
-    ]
 
-    answer = prompt(questions)
-    return answer[name]
 
 
 def areas_prompt() -> list:
     name = 'areas'
 
     questions = [
         {
             'type': 'checkbox',
             'qmark': '[?]',
             'name': name,
             'message': 'Which area(s) would you like to scrape? (Press ENTER to continue)',
-             "validate":(lambda result: len(result)> 0),
-      "invalid_message":"Input cannot be empty",
+             "validate":emptyListValidator(),
             'choices': [
                 Choice('Timeline'),
+                Choice('Pinned'),
                 Choice('Archived'),
                 Choice('Highlights'),
                 Choice('Stories'),
                 Choice('Messages'),
+                Choice("Purchased")
             ]
-            ,"instruction":"\nKeybindings\nToggle all: Ctrl+R\nToggle single: spacebar\nPress enter when done",
+            ,"instruction":CHECKLISTINSTRUCTIONS,
 
         }
     ]
-
-    while True:
-        answers = prompt(questions)
-        if not answers[name]:
-            console.print('Error: You must select at least one.')
-        break
+    answers = prompt(questions)
     return answers[name]
 
 
-def database_prompt() -> tuple:
-    name1 = 'path'
-    name2 = 'username'
-
-    questions = [
-        {
-            'type': 'input',
-            'name': name1,
-            'message': 'Enter the path to the directory that contains your database files:'
-        },
-        {
-            'type': 'input',
-            'name': name2,
-            'message': 'Enter that model\'s username:'
-        }
-    ]
-
-    answers = prompt(questions)
-    return (answers[name1], answers[name2])
 
 
 def auth_prompt(auth) -> dict:
     questions = [
         {
             'type': 'input',
             'name': 'sess',
-            'message': 'Enter your `sess` cookie:',
+            'message': 'Enter your sess cookie:',
             'default': auth['sess']
+            ,'validate':EmptyInputValidator()
+
         },
         {
             'type': 'input',
             'name': 'auth_id',
-            'message': 'Enter your `auth_id` cookie:',
+            'message': 'Enter your auth_id cookie:',
             'default': auth['auth_id']
+            ,'validate':EmptyInputValidator()
         },
         {
             'type': 'input',
             'name': 'auth_uid_',
-            'message': 'Enter your `auth_uid_` cookie (leave blank if you don\'t use 2FA):',
+            'message': 'Enter your auth_uid cookie (leave blank if you don\'t use 2FA):',
             'default': auth['auth_uid_']
         },
         {
             'type': 'input',
             'name': 'user_agent',
             'message': 'Enter your `user agent`:',
             'default': auth['user_agent']
+            ,'validate':EmptyInputValidator()
         },
         {
             'type': 'input',
             'name': 'x-bc',
             'message': 'Enter your `x-bc` token:',
             'default': auth['x-bc']
+            ,'validate':EmptyInputValidator()
         }
     ]
 
     answers = prompt(questions)
     return answers
 
 
@@ -198,15 +144,15 @@
     if pythonver<3.9 or pythonver>=3.11:
         console.print("\nNote: Browser Extractions only works with default Profile\n\n")
         questions = [
             {
                 'type': 'list',
                 'message':msg ,
                 'choices':["Enter Each Field Manually","Paste From Cookie Helper", Separator(line="-----------\nBrowser Extractions"),"Chrome","Chromium","Firefox","Opera","Opera GX","Edge","Chromium","Brave","Vivaldi","Safari"],
-                "default":"Enter Each Field Manually"
+                "default":"Enter Each Field Manually",
 
             }
         ]
 
     else:
         console.print("\nNote:To enable automatic extraction install ofscraper with python 3.9 or 3.10\n\n")
         msg="Select how to retrive auth information"
@@ -217,46 +163,53 @@
             'choices':["Enter Each Field Manually","Paste From Cookie Helper"],
             "default":"Enter Each Field Manually"
 
         }
     ]  
       
     return prompt(questions)[0]
-def user_agent_prompt(current,new=None):
-    new =new or "Unknown Please Ignore"
-
+def user_agent_prompt(pcurrent):
     questions = [
         {
             'type': 'input',
             'message':'Enter User_Agent from browser',
-            'default':current
+            'default':current,
+            'validate':EmptyInputValidator(),
+            'filter':lambda x:cleanTextInput(x)
         }
     ]
-    return  prompt(questions)[0].strip()
+    return  prompt(questions)[0]
 
 def xbc_prompt():
     questions = [
         {
             'type': 'input',
             'message':'Enter x-bc request header',
-            'instruction':f"\nGo to browser network tools to view\nFor more instructions visit https://github.com/excludedBittern8/ofscraper\n\n"
+            'instruction':f"\nGo to browser network tools to view\nFor more instructions visit https://github.com/datawhores/ofscraper\n\n"
+            ,'validate':EmptyInputValidator(),
+            'filter':lambda x:cleanTextInput(x)
         }
     ]
-    return  prompt(questions)[0].strip()
+    return  prompt(questions)[0]
 
 
 
 
 def auth_full_paste():
     questions = [
         {
             'type': 'input',
             'message':'Paste Text from Extension',
-            "filter": lambda result: json.loads(result),
-             "instruction":"\n\nCookie Helper Repo:https://github.com/M-rcus/OnlyFans-Cookie-Helper/\n\n"
+            "validate": jsonValidator(),
+            "filter":jsonloader,
+             "instruction":\
+"""
+Cookie Helper Repo:https://github.com/M-rcus/OnlyFans-Cookie-Helper
+"""
+             
 
         }
     ]
     return prompt(questions)[0]
     
 def profiles_prompt() -> int:
     name = 'profile'
@@ -295,120 +248,237 @@
 def new_name_edit_profiles_prompt(old_profile_name) -> str:
     name = 'new_name'
 
     questions = [
         {
             'type': 'input',
             'name': name,
-            'message': f'What would you like to rename {old_profile_name} to?'
+            'message': f'What would you like to rename {old_profile_name} to?',
+            'validator':EmptyInputValidator()
         }
     ]
 
     answer = prompt(questions)
     return answer[name]
 
 
 def create_profiles_prompt() -> str:
     name = 'create'
 
     questions = [
         {
             'type': 'input',
             'name': name,
-            'message': 'What would you like to name your new profile? [ONLY letters, numbers, and underscores!]'
+            'message': 
+"""
+What would you like to name your new profile?
+only letters, numbers, and underscores are allowed
+""",
+            'validator':namevalitator()
+
         }
     ]
 
-    while True:
-        pattern = re.compile(r'[^\w+^\d+^_+]')
-        answer = prompt(questions)
-
-        if not answer[name]:
-            console.print('You must type a name. Try again.')
-
-        if re.search(pattern, answer[name]):
-            console.print('Profile name contains invalid characters. Try again.')
-        break
-
+    answer = prompt(questions)
     return answer[name]
 
 
 def get_profile_prompt(profiles: list) -> str:
     name = 'get_profile'
 
     questions = [
         {
             'type': 'list',
             'name': name,
             'message': 'Select Profile',
             'choices':profiles
-            ,"validate":(lambda result: len(result)> 0)
+            ,"validate":emptyListValidator()
         }
     ]
     answer = prompt(questions)
     profile = answer[name]
-
     return profile
 
 
-def config_prompt(config) -> dict:
+def config_prompt(config_) -> dict:
+
     questions = [
         {
             'type': 'input',
             'name': 'main_profile',
             'message': 'What would you like your main profile to be?',
-            'default': config.get('main_profile','main_profile')
+            'default': config.get_main_profile(config_),
+            "validate":lambda x:emptyListValidator() and  isinstance(x[0],str)
         },
         {
-            'type': 'input',
+            'type': 'filepath',
             'name': 'save_location',
-            'message': 'Where would you like to set as the root save downloaded directory?',
-            'default': config.get('save_location',str(pathlib.Path.home() /'Data/ofscraper'), )
+            'message':"save_location: ",
+            'long_instruction': 'Where would you like to set as the root save downloaded directory?',
+            'default':config.get_save_location(config_),
+            "filter":lambda x:cleanTextInput(x)
+            
         },
         {
-            'type': 'input',
+            'type': 'number',
             'name': 'file_size_limit',
-            'message': 'File size limit (enter a value in bytes)\nLeave empty string for no limit:',
-            'default': config.get('file_size_limit', '')
+            'message':"file_size_limit: ",
+            'long_instruction':
+"""
+File size limit (enter a value in bytes)
+Enter 0 for no limit
+""",
+            'default': config.get_filesize(config_),
+            'filter':int,
+             'min_allowed':0,
+      
         },
            {
             'type': 'input',
             'name': 'dir_format',
-            'message': 'What format do you want for download directories',
-            'default': config.get('dir_format', '{model_username}/{responsetype}/{mediatype}/')
+            'message':"dir_format: ",
+            'long_instruction': 'What format do you want for download directories',
+            'default': config.get_dirformat(config_),
+             "validate":dirformatvalidator()
         },
               {
             'type': 'input',
             'name': 'file_format',
             'message': 'What format do you want for downloaded files',
-            'default': config.get('file_format', '{filename}.{ext}')
+            'default':config.get_fileformat(config_),
+             "validate":fileformatvalidator()
         },
                      {
-            'type': 'input',
+            'type': 'number',
             'name': 'textlength',
-            'message': 'Enter the max length to extract for post text, 0 means unlimited',
-            'default': config.get('textlength', '0')
+            'message':"textlength: ",
+            'long_instruction': 'Enter the max length to extract for post text, 0 means unlimited\n',
+            'default': config.get_textlength(config_),
+            'min_allowed':0,
+             "validate":EmptyInputValidator()
         },
-                          {
+         {
             'type': 'input',
             'name': 'date',
-            'message': 'Enter Date formatting',
-            'default': config.get('date', 'MM-DD-YYYY')
+            'message': 'date: ',
+            "long_instruction":"Enter Date format",
+            'default': config.get_date(config_),
+             "validate":dateplaceholdervalidator()
         },
-                               {
+        {
             'type': 'input',
             'name': 'metadata',
-            'message': 'Where should metadata files be saved',
-            'default': config.get('metadata', '{configpath}/{profile}/.data/{username}_{model_id}')
+            "message":"metadata: ",
+            'long_instruction': 'Where should metadata files be saved',
+            'default':config.get_metadata(config_),
+             "validate":metadatavalidator()
+        },
+        {
+            'type': 'checkbox',
+            'name': 'filter',
+            "message":"filter: ",
+            'choices':list(map(lambda x:Choice(name=x,value=x, enabled=x.capitalize() in set(config.get_filter(config_))),FILTER_DEFAULT)),
+             "validate":emptyListValidator()
+        },
+  
+    ]
+
+    questions2 = [
+        {
+            'type': 'input',
+            'name': 'timeline',
+            'long_instruction': 
+            """
+set responsetype for timeline posts
+Empty string is consider to be 'posts'
+            """,
+            'default': config.get_timeline_responsetype(config_),
+            'message':"input: "
+        },
+             {
+            'type': 'input',
+            'name': 'archived',
+            'long_instruction': 
+            """
+set responsetype for archived posts
+Empty string is consider to be 'archived'
+            """,
+            'default': config.get_archived_responsetype(config_),
+            'message':"input: "
+        },
+
+    {
+            'type': 'input',
+            'name': 'pinned',
+            'long_instruction': 
+            """
+set responsetype for pinned posts
+Empty string is consider to be 'archived'
+            """,
+            'default': config.get_archived_responsetype(config_),
+            'message':"input: "
+        },
+                     {
+            'type': 'input',
+            'name': 'message',
+            'long_instruction': 
+            """
+set responsetype for message posts
+Empty string is consider to be 'message'
+            """,
+            'default': config.get_messages_responsetype(config_),
+            'message':"input: "
+        },
+                        {
+            'type': 'input',
+            'name': 'paid',
+            'long_instruction': 
+            """
+set responsetype for paid posts
+Empty string is consider to be 'paid'
+            """,
+            'default': config.get_paid_responsetype(config_),
+            'message':"input: "
+        },
+                             {
+    'type': 'input',
+            'name': 'stories',
+            'long_instruction': 
+            """
+set responsetype for stories
+Empty string is consider to be 'stories'
+            """,
+            'default': config.get_stories_responsetype(config_),
+            'message':"input: "
+        },
+                                    {
+    'type': 'input',
+            'name': 'highlights',
+            'long_instruction': 
+            """
+set responsetype for highlights
+Empty string is consider to be 'highlights'
+            """,
+            'default': config.get_highlights_responsetype(config_),
+            'message':"input: "
+        },
+                                          {
+    'type': 'input',
+            'name': 'profile',
+            'long_instruction': 
+            """
+set responsetype for profile
+Empty string is consider to be 'profile'
+            """,
+            'default': config.get_profile_responsetype(config_),
+            'message':"input: "
         }
-    ]
-
+     ]
     answers = prompt(questions)
-    answers.update({'save_location': answers.get(
-        'save_location').strip('\"')})
+    answers["responsetype"]=prompt(questions2)
     return answers
 def reset_username_prompt() -> bool:
     name = 'reset username'
     questions = [
         {
             'type': 'list',
             'name': name,
@@ -438,39 +508,28 @@
       "keybindings":{
                              "toggle": [{"key": "s-right"},{"key": ["pagedown","right"]},{"key": ["home","right"]}],
 
                               
                          }
                          
      ,"multiselect":True
-      ,"validate":(lambda result: len(result)> 0),
-      "invalid_message":"Input cannot be empty",
-      "instruction":"\nKeyBindings\nToggle all: Ctrl+r\nToggle single: Shift +Right or Home +Right or pageDown +Right\nPress Enter When Done\n\nParantheses indicates number of selected users\n\nValues: Name Renewal_Date/Expired_Date Active_Subscription","choices":list(map(lambda x:Choice(x,name=f"{x['name']} {x['date'] } {x['active']}")   ,sorted(models,key=lambda x:x['name']))),"transformer":lambda result:",".join(map(lambda x:x.split(" ")[0],result))
+      ,"validate":emptyListValidator(),
+      "instruction":FUZZY_INSTRUCTION,
+      "choices":list(map(lambda x:Choice(x,name=f"{x['name']} {x['date'] } {x['active']}")   ,sorted(models,key=lambda x:x['name']))),"transformer":lambda result:",".join(map(lambda x:x.split(" ")[0],result))
        ,"prompt":'Filter: ',
        "marker":"\u25c9 ",
        "marker_pl":"\u25cb "
 
       },
     
 ]
 
     return prompt(questions)[0]
 
 
-def download_paid_prompt() -> bool:
-    questions = [
-        {
-            'type': 'list',
-            'message': "Would you like to also download paid content",
-            'choices':["Yes","No"]
-        }
-    ]
-
-    answer = prompt(questions)
-    return answer[0]
 
 def decide_filters_prompts():
     questions = [
         {
             'type': 'list',
             'message': "Modify filters for your accounts list?\nSome usage examples are scraping free accounts only or paid accounts without renewal",
             'choices':["Yes","No"]
```

### Comparing `ofscraper-1.75/PKG-INFO` & `ofscraper-1.80/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,51 +1,68 @@
 Metadata-Version: 2.1
 Name: ofscraper
-Version: 1.75
+Version: 1.80
 Summary: automatically scrape onlyfans
-Author: excludedBittern8
-Author-email: excludedBittern8@riseup.net
+Author: datawhores
+Author-email: datawhores@riseup.net
 Requires-Python: >=3.7.0,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: arrow (>=1.2.3,<2.0.0)
 Requires-Dist: browser-cookie3 (>=0.17.1,<0.18.0)
 Requires-Dist: bs4 (>=0.0.1,<0.0.2)
 Requires-Dist: halo (>=0.0.31,<0.0.32)
 Requires-Dist: httpx[http2] (>=0.23.3,<0.24.0)
 Requires-Dist: inquirerpy (>=0.3.4,<0.4.0)
+Requires-Dist: pathvalidate (>=2.5.2,<3.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: rich (>=13.3.2,<14.0.0)
 Requires-Dist: schedule (>=1.1.0,<2.0.0)
 Requires-Dist: setuptools (>=67.6.0,<68.0.0)
 Requires-Dist: tenacity (>=8.2.2,<9.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: win32-setctime (>=1.1.0,<2.0.0)
-Project-URL: Homepage, https://github.com/excludedBittern8/ofscraper
+Requires-Dist: xxhash (>=3.2.0,<4.0.0)
+Project-URL: Homepage, https://github.com/datawhores/ofscraper
 Description-Content-Type: text/markdown
 
 A fork of onlyfans-scraper. It has been optimized to make it more feature complete with dc's onlyfans script.
 A matter of fact with the right settings transitioning between the two scripts should be a easy enough process
 
 In addition there are numerous filtering features to control exactly which type of content you want to scrape.
-https://github.com/excludedBittern8/ofscraper/blob/main/CHANGES.md
+https://github.com/datawhores/ofscraper/blob/main/CHANGES.md
 
 <h3>DISCLAIMERS:</h3>
 <ol>
     <li>
         This tool is not affiliated, associated, or partnered with OnlyFans in any way. We are not authorized, endorsed, or sponsored by OnlyFans. All OnlyFans trademarks remain the property of Fenix International Limited.
     </li>
     <li>
         This is a theoritical program only and is for educational purposes. If you choose to use it then it may or may not work. You solely accept full responsability and indemnify the creator, hostors, contributors and all other involved persons from any any all responsability.
     </li>
 
+ ## 1.80 Changes:
+ - sync keys names across config(old keys will still work)
+  * change username to model_username in metadata
+  * change site_name to sitename in metadata
+ - remove --purchased args
+ - add purchase and pinned as post types
+ - add letter-count argument
+   * This is counting letters and not words for
+   textlength
+ - added testing 
+    * to install run poetry install --with test 
+    * run with poetry run pytest
+ - print path for each file
+ - responsetype mapping in config
+    * This is for example keeping all messages or paid post in same folder, but also allow long time users to keep their current structure
 
   ## Description:
   command-line program to download media, and to process other batch operations such as liking and unliking posts.
     
 
 ![CopyQ nsUBdI](https://user-images.githubusercontent.com/67020411/227816586-fb685959-cd3f-45af-adea-14773b7154f9.png)
 
@@ -59,31 +76,31 @@
 # Windows: 
 ```
 pip install ofscraper
 ```
 or 
 
 ```
-pip install git+https://github.com/excludedBittern8/ofscraper.git 
+pip install git+https://github.com/datawhores/ofscraper.git 
 ```
 
 #  macOS/Linux
 ```
 pip3 install ofscraper
 ```
 or
 ```
-pip3 install git+https://github.com/excludedBittern8/ofscraper.git 
+pip3 install git+https://github.com/datawhores/ofscraper.git 
 ```
 
 ## Authentication
 
 You'll need to retrive your auth information 
     
-https://github.com/excludedBittern8/ofscraper/wiki/Auth
+https://github.com/datawhores/ofscraper/wiki/Auth
 
 
 
 # Usage
 
 Whenever you want to run the program, all you need to do is type `ofscraper` in your terminal:
 
@@ -104,37 +121,38 @@
 
 ![image](https://user-images.githubusercontent.com/67020411/230735256-2d8aa788-53dc-49ee-ada8-5ddf5546851c.png)
 
 ## Selecting specific users
 
 The fuzzy search system can be a little confusing see
     
-https://github.com/excludedBittern8/ofscraper/wiki/Fuzzy-Search 
+https://github.com/datawhores/ofscraper/wiki/Fuzzy-Search 
     
 ## Other menu options    
   
- See: https://github.com/excludedBittern8/ofscraper/wiki/Menu-Options 
+ See: https://github.com/datawhores/ofscraper/wiki/Menu-Options 
  
  # commandline
  While the menu is easy to use, and convient. You may want more automation.
  
  The best way to do this is through the commandline system. This will allow you to skip the menu, and for example scrape a provided list of accounts
  
-  https://github.com/excludedBittern8/ofscraper/wiki/command-line-args
+  https://github.com/datawhores/ofscraper/wiki/command-line-args
  
  # Customazation
     
-https://github.com/excludedBittern8/ofscraper/wiki/Customizing-save-path
-https://github.com/excludedBittern8/ofscraper/wiki/Config-Options
+https://github.com/datawhores/ofscraper/wiki/Customizing-save-path
+https://github.com/datawhores/ofscraper/wiki/Config-Options
 
   
 # Issues
 Open a issue in this repo, or you can mention your issue in the discord
 
-https://discord.gg/zRXgb5Nv
+https://discord.gg/wN7uxEVHRK
+    
     
 ## Common
 ### Status Down
       
 This typically means that your auth information is not correct, or onlyfans signed you out.
 ### 404 Issue 
     
@@ -152,30 +170,35 @@
 
 You will need to change the settings so that the metadata option is compatible with your current folders
 Additionally you might want to set the save_path, dir_path, and filename so they output similar outputs
 
 The metadata path from dc's script is used for duplicate check so as long as your set the right path.
 Files won't download a second time
 
-https://github.com/excludedBittern8/ofscraper/wiki/Migrating-from-DC-script
-https://github.com/excludedBittern8/ofscraper/wiki/Config-Options
-https://github.com/excludedBittern8/ofscraper/wiki/Customizing-save-path
+https://github.com/datawhores/ofscraper/wiki/Migrating-from-DC-script
+https://github.com/datawhores/ofscraper/wiki/Config-Options
+https://github.com/datawhores/ofscraper/wiki/Customizing-save-path
 
 Ask in the discord or open an issue if you need help with what to change to accomplish this
 
 
 
 # Discord
 
-https://discord.gg/zRXgb5Nv
+https://discord.gg/wN7uxEVHRK
     
+# Support
+buymeacoffee.com/datawhores
     
-
-  
+BTC: bc1qcnnetrgmtr86rmqvukl2e24f5upghpcsqqsy87
     
+ETH: 0x1d427a6E336edF6D95e589C16cb740A1372F6609
+
+
+[![codecov](https://codecov.io/github/datawhores/ofscraper/branch/main/graph/badge.svg?token=U1F1PQ7LGM)](https://codecov.io/github/datawhores/ofscraper)
```

