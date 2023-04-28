# Comparing `tmp/CharacterAPI-0.1.3.tar.gz` & `tmp/CharacterAPI-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\CharacterAPI-0.1.3.tar", last modified: Fri Apr 28 18:59:04 2023, max compression
+gzip compressed data, was "dist\CharacterAPI-0.1.4.tar", last modified: Fri Apr 28 20:02:59 2023, max compression
```

## Comparing `CharacterAPI-0.1.3.tar` & `CharacterAPI-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 18:59:04.076184 CharacterAPI-0.1.3/
-drwxrwxrwx   0        0        0        0 2023-04-28 18:59:03.990506 CharacterAPI-0.1.3/CharacterAPI/
--rw-rw-rw-   0        0        0     4468 2023-04-28 18:58:01.000000 CharacterAPI-0.1.3/CharacterAPI/CharacterAI.py
--rw-rw-rw-   0        0        0     4861 2023-04-28 18:58:06.000000 CharacterAPI-0.1.3/CharacterAPI/CharacterAI_async.py
--rw-rw-rw-   0        0        0       65 2023-04-28 18:57:56.000000 CharacterAPI-0.1.3/CharacterAPI/__init__.py
--rw-rw-rw-   0        0        0      126 2023-04-27 15:21:32.000000 CharacterAPI-0.1.3/CharacterAPI/errors.py
-drwxrwxrwx   0        0        0        0 2023-04-28 18:59:04.068194 CharacterAPI-0.1.3/CharacterAPI.egg-info/
--rw-rw-rw-   0        0        0      457 2023-04-28 18:59:03.000000 CharacterAPI-0.1.3/CharacterAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      315 2023-04-28 18:59:03.000000 CharacterAPI-0.1.3/CharacterAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 18:59:03.000000 CharacterAPI-0.1.3/CharacterAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-04-28 18:59:03.000000 CharacterAPI-0.1.3/CharacterAPI.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-28 18:59:03.000000 CharacterAPI-0.1.3/CharacterAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1082 2023-04-28 16:51:34.000000 CharacterAPI-0.1.3/LICENSE
--rw-rw-rw-   0        0        0      457 2023-04-28 18:59:04.076184 CharacterAPI-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0       63 2023-04-28 17:26:52.000000 CharacterAPI-0.1.3/README.md
--rw-rw-rw-   0        0        0       42 2023-04-28 18:59:04.076184 CharacterAPI-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      617 2023-04-28 18:59:00.000000 CharacterAPI-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 20:02:59.076851 CharacterAPI-0.1.4/
+drwxrwxrwx   0        0        0        0 2023-04-28 20:02:58.980828 CharacterAPI-0.1.4/CharacterAPI/
+-rw-rw-rw-   0        0        0     9211 2023-04-28 20:01:51.000000 CharacterAPI-0.1.4/CharacterAPI/CharacterAI.py
+-rw-rw-rw-   0        0        0       87 2023-04-28 20:00:52.000000 CharacterAPI-0.1.4/CharacterAPI/__init__.py
+-rw-rw-rw-   0        0        0      126 2023-04-27 15:21:32.000000 CharacterAPI-0.1.4/CharacterAPI/errors.py
+drwxrwxrwx   0        0        0        0 2023-04-28 20:02:59.068851 CharacterAPI-0.1.4/CharacterAPI.egg-info/
+-rw-rw-rw-   0        0        0      457 2023-04-28 20:02:58.000000 CharacterAPI-0.1.4/CharacterAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      281 2023-04-28 20:02:58.000000 CharacterAPI-0.1.4/CharacterAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 20:02:58.000000 CharacterAPI-0.1.4/CharacterAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-04-28 20:02:58.000000 CharacterAPI-0.1.4/CharacterAPI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-28 20:02:58.000000 CharacterAPI-0.1.4/CharacterAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1082 2023-04-28 16:51:34.000000 CharacterAPI-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0      457 2023-04-28 20:02:59.076851 CharacterAPI-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0       63 2023-04-28 17:26:52.000000 CharacterAPI-0.1.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-28 20:02:59.076851 CharacterAPI-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      617 2023-04-28 19:57:06.000000 CharacterAPI-0.1.4/setup.py
```

### Comparing `CharacterAPI-0.1.3/CharacterAPI/CharacterAI_async.py` & `CharacterAPI-0.1.4/CharacterAPI/CharacterAI.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from typing import Dict
 import asyncio
 import json
 import time
 
+from playwright.sync_api import sync_playwright
 from playwright.async_api import async_playwright
 
 from CharacterAPI import errors
 
-__all__ = ['pyCAI']
+__all__ = ['pyCAI', 'pyAioCAI']
 
 text = []
 page = None
 
-class pyCAI:
+class pyAioCAI:
     def __init__(self, token):
         self.token = token
         self.user = self.user()
         self.character = self.character()
         self.chat = self.chat()
 
     async def init(self):
@@ -124,8 +125,125 @@
 
             chat.new_chat('CHAR')
             """
             await pyCAI.goto(f'https://beta.character.ai/chat?char={char}')
             await page.wait_for_selector('div.col-auto.px-2.dropdown').click()
             await page.locator('"Save and Start New Chat"').click()
 
+            return True
+
+
+class pyCAI:
+    def __init__(self, token: str):
+        global page
+
+        self.token = token
+        self.browser = sync_playwright().start().firefox.launch(headless=True)
+        self.context = self.browser.new_context(extra_http_headers={"Authorization": f"Token {self.token}"})
+        page = self.context.new_page()
+
+        self.user = self.user()
+        self.character = self.character()
+        self.chat = self.chat()
+
+    # [FOR LIBRARY] Convert site to json
+    def GetResponce(link: str) -> Dict[str, str]:
+        pyCAI.goto(f'https://beta.character.ai/{link}/')
+        data = json.loads(page.locator('pre').inner_text())
+        
+        return data
+
+    # [FOR LIBRARY] Checking the page if it runs for the first time
+    def goto(link: str):
+        page.goto(link)
+
+        if page.title() != 'Waiting Room powered by Cloudflare':
+            if page.get_by_role("button", name="Accept").is_visible():
+                page.get_by_role("button", name="Accept").click()
+
+                return page
+        
+        else: raise errors.NoResponse('The Site is Overloaded')
+
+    class user:
+        """
+        Just a responces from site for user info
+
+        user.info()
+        """
+        def info(self) -> Dict[str, str]:
+            return pyCAI.GetResponce(link='chat/user')
+
+        def posts(self) -> Dict[str, str]:
+            return pyCAI.GetResponce(link='chat/posts/user/?scope=user&page=1&posts_to_load=5')
+
+        def followers(self) -> Dict[str, str]:
+            return pyCAI.GetResponce(link='chat/user/followers')
+
+        def following(self) -> Dict[str, str]:
+            return pyCAI.GetResponce(link='chat/user/following')
+
+    class character:
+        """
+        Just a responces from site for characters
+
+        character.trending()
+        character.get_info('CHAR')
+        """
+        def trending(self) -> Dict[str, str]:
+            return pyCAI.GetResponce(link='chat/characters/trending')
+        
+        def recommended(self) -> Dict[str, str]:
+            return pyCAI.GetResponce(link='chat/characters/recommended')
+
+        def categories(self) -> Dict[str, str]:
+            return pyCAI.GetResponce(link='chat/character/categories')
+
+        def get_info(self, char: str) -> Dict[str, str]:
+            try: return pyCAI.GetResponce(link=f'chat/character/info-cached/{char}')
+            except: raise errors.CharNotFound('Wrong Char')
+
+    class chat:
+        def get_history(self, char: str) -> Dict[str, str]:
+            """
+            Getting character chat history, return json responce
+
+            The post method doesn't work, so i get this from page.on('responce')
+
+            chat.get_history('CHAR')
+            """
+            page.on("response", lambda response: text.append(response.text()) if response.url.startswith('https://beta.character.ai/chat/history/msgs/user/') else None)
+            pyCAI.goto(f'https://beta.character.ai/chat?char={char}')
+            page.wait_for_selector('.msg.char-msg').is_visible()
+
+            return json.loads(text[0])
+
+        def send_message(self, char: str, message: str) -> Dict[str, str]:
+            """
+            Sending a message
+
+            chat.send_message('CHAR', 'MESSAGE')
+            """
+            pyCAI.goto(f'https://beta.character.ai/chat?char={char}')
+
+            time.sleep(1)
+            page.get_by_placeholder("Type a message").fill(message)
+            time.sleep(1)
+            page.get_by_role("button", name="Submit Message").click()
+            time.sleep(1)
+
+            page.wait_for_selector('.swiper-button-next', timeout=0).is_visible()
+            div = page.query_selector('div.markdown-wrapper.markdown-wrapper-last-msg.swiper-no-swiping')
+
+            return div.inner_text().replace('\n\n\n\n\n', '\n\n')
+
+        def new_chat(self, *, char: str) -> bool:
+            """
+            Starting new chat, return True when done
+
+            chat.new_chat('CHAR')
+            """
+            pyCAI.goto(f'https://beta.character.ai/chat?char={char}')
+            page.wait_for_selector('div.col-auto.px-2.dropdown').click()
+            page.locator('"Save and Start New Chat"').click()
+
             return True
```

### Comparing `CharacterAPI-0.1.3/LICENSE` & `CharacterAPI-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `CharacterAPI-0.1.3/setup.py` & `CharacterAPI-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as readme:
     long_description = readme.read()
 
 setup(
     name='CharacterAPI',
-    version='0.1.3',
+    version='0.1.4',
     author='kramcat',
     description='An unofficial API for character.ai for Python',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/kramcat/CharacterAPI',
     packages=find_packages(),
     install_requires=["playwright==1.32.1"],
```

