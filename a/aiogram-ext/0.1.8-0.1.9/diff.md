# Comparing `tmp/aiogram-ext-0.1.8.tar.gz` & `tmp/aiogram-ext-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiogram-ext-0.1.8.tar", last modified: Mon Apr 24 03:32:35 2023, max compression
+gzip compressed data, was "aiogram-ext-0.1.9.tar", last modified: Mon Apr 24 03:51:49 2023, max compression
```

## Comparing `aiogram-ext-0.1.8.tar` & `aiogram-ext-0.1.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1059 2023-04-24 03:32:27.312633 aiogram-ext-0.1.8/botty/__init__.py
--rw-r--r--   0        0        0      251 2023-04-14 12:15:49.770806 aiogram-ext-0.1.8/botty/bot.py
--rw-r--r--   0        0        0     1175 2023-04-12 11:18:11.688903 aiogram-ext-0.1.8/botty/buttons.py
--rw-r--r--   0        0        0      294 2023-04-24 02:27:10.096409 aiogram-ext-0.1.8/botty/config.py
--rw-r--r--   0        0        0     1651 2023-04-12 11:05:16.344725 aiogram-ext-0.1.8/botty/context.py
--rw-r--r--   0        0        0     1665 2023-04-16 22:10:48.295151 aiogram-ext-0.1.8/botty/deps.py
--rw-r--r--   0        0        0     5999 2023-04-20 17:26:03.233411 aiogram-ext-0.1.8/botty/dispatcher.py
--rw-r--r--   0        0        0      892 2023-04-10 18:37:24.358984 aiogram-ext-0.1.8/botty/env.py
--rw-r--r--   0        0        0     3800 2023-04-11 11:53:07.707408 aiogram-ext-0.1.8/botty/filters.py
--rw-r--r--   0        0        0      992 2023-04-24 03:32:31.850775 aiogram-ext-0.1.8/botty/helpers.py
--rw-r--r--   0        0        0      722 2023-04-12 14:37:01.113297 aiogram-ext-0.1.8/botty/keyboards.py
--rw-r--r--   0        0        0      669 2023-04-24 03:10:12.100277 aiogram-ext-0.1.8/botty/loader.py
--rw-r--r--   0        0        0      142 2023-04-15 18:38:40.809162 aiogram-ext-0.1.8/botty/middlewares/__init__.py
--rw-r--r--   0        0        0     6971 2023-04-15 18:38:40.842420 aiogram-ext-0.1.8/botty/middlewares/_conversation.py
--rw-r--r--   0        0        0     1534 2023-04-11 11:53:07.675758 aiogram-ext-0.1.8/botty/middlewares/_membership.py
--rw-r--r--   0        0        0     1503 2023-04-11 11:53:07.675758 aiogram-ext-0.1.8/botty/middlewares/misc.py
--rw-r--r--   0        0        0     2178 2023-04-11 11:53:07.691383 aiogram-ext-0.1.8/botty/middlewares/throttling.py
--rw-r--r--   0        0        0      455 2023-04-24 03:32:31.857280 aiogram-ext-0.1.8/pyproject.toml
--rw-r--r--   0        0        0       21 2023-04-11 11:28:20.640417 aiogram-ext-0.1.8/README.md
--rw-r--r--   0        0        0      239 2023-04-16 23:01:01.500707 aiogram-ext-0.1.8/tests/__main__.py
--rw-r--r--   0        0        0      152 1970-01-01 00:00:00.000000 aiogram-ext-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1059 2023-04-24 03:32:27.312633 aiogram-ext-0.1.9/botty/__init__.py
+-rw-r--r--   0        0        0      251 2023-04-14 12:15:49.770806 aiogram-ext-0.1.9/botty/bot.py
+-rw-r--r--   0        0        0     1175 2023-04-12 11:18:11.688903 aiogram-ext-0.1.9/botty/buttons.py
+-rw-r--r--   0        0        0      294 2023-04-24 02:27:10.096409 aiogram-ext-0.1.9/botty/config.py
+-rw-r--r--   0        0        0     1651 2023-04-12 11:05:16.344725 aiogram-ext-0.1.9/botty/context.py
+-rw-r--r--   0        0        0     1665 2023-04-16 22:10:48.295151 aiogram-ext-0.1.9/botty/deps.py
+-rw-r--r--   0        0        0     5999 2023-04-20 17:26:03.233411 aiogram-ext-0.1.9/botty/dispatcher.py
+-rw-r--r--   0        0        0      892 2023-04-10 18:37:24.358984 aiogram-ext-0.1.9/botty/env.py
+-rw-r--r--   0        0        0     3800 2023-04-11 11:53:07.707408 aiogram-ext-0.1.9/botty/filters.py
+-rw-r--r--   0        0        0      993 2023-04-24 03:51:46.752347 aiogram-ext-0.1.9/botty/helpers.py
+-rw-r--r--   0        0        0      722 2023-04-12 14:37:01.113297 aiogram-ext-0.1.9/botty/keyboards.py
+-rw-r--r--   0        0        0      669 2023-04-24 03:10:12.100277 aiogram-ext-0.1.9/botty/loader.py
+-rw-r--r--   0        0        0      142 2023-04-15 18:38:40.809162 aiogram-ext-0.1.9/botty/middlewares/__init__.py
+-rw-r--r--   0        0        0     6971 2023-04-15 18:38:40.842420 aiogram-ext-0.1.9/botty/middlewares/_conversation.py
+-rw-r--r--   0        0        0     1534 2023-04-11 11:53:07.675758 aiogram-ext-0.1.9/botty/middlewares/_membership.py
+-rw-r--r--   0        0        0     1503 2023-04-11 11:53:07.675758 aiogram-ext-0.1.9/botty/middlewares/misc.py
+-rw-r--r--   0        0        0     2178 2023-04-11 11:53:07.691383 aiogram-ext-0.1.9/botty/middlewares/throttling.py
+-rw-r--r--   0        0        0      455 2023-04-24 03:51:46.760862 aiogram-ext-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-04-11 11:28:20.640417 aiogram-ext-0.1.9/README.md
+-rw-r--r--   0        0        0      239 2023-04-16 23:01:01.500707 aiogram-ext-0.1.9/tests/__main__.py
+-rw-r--r--   0        0        0      152 1970-01-01 00:00:00.000000 aiogram-ext-0.1.9/PKG-INFO
```

### Comparing `aiogram-ext-0.1.8/botty/__init__.py` & `aiogram-ext-0.1.9/botty/__init__.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.1.8/botty/buttons.py` & `aiogram-ext-0.1.9/botty/buttons.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.1.8/botty/context.py` & `aiogram-ext-0.1.9/botty/context.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.1.8/botty/deps.py` & `aiogram-ext-0.1.9/botty/deps.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.1.8/botty/dispatcher.py` & `aiogram-ext-0.1.9/botty/dispatcher.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.1.8/botty/env.py` & `aiogram-ext-0.1.9/botty/env.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.1.8/botty/filters.py` & `aiogram-ext-0.1.9/botty/filters.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.1.8/botty/helpers.py` & `aiogram-ext-0.1.9/botty/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     return msg.answer(text, reply_markup=markup)
 
 
 async def ask(
     state: State,
     msg: Message,
     text: str,
-    markup: ReplyMarkup | bool = None,
+    markup: ReplyMarkup | bool = False,
 ):
     await state.set()
     await reply(msg, text, markup)
 
 
 def is_channel(chat: Chat) -> bool:
     return chat.type in [ChatType.CHANNEL]
```

### Comparing `aiogram-ext-0.1.8/botty/keyboards.py` & `aiogram-ext-0.1.9/botty/keyboards.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.1.8/botty/loader.py` & `aiogram-ext-0.1.9/botty/loader.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.1.8/botty/middlewares/_conversation.py` & `aiogram-ext-0.1.9/botty/middlewares/_conversation.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.1.8/botty/middlewares/_membership.py` & `aiogram-ext-0.1.9/botty/middlewares/_membership.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.1.8/botty/middlewares/misc.py` & `aiogram-ext-0.1.9/botty/middlewares/misc.py`

 * *Files identical despite different names*

### Comparing `aiogram-ext-0.1.8/botty/middlewares/throttling.py` & `aiogram-ext-0.1.9/botty/middlewares/throttling.py`

 * *Files identical despite different names*

