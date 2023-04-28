# Comparing `tmp/nonebot-plugin-chatgpt-on-qq-1.2.0.tar.gz` & `tmp/nonebot-plugin-chatgpt-on-qq-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-chatgpt-on-qq-1.2.0.tar", last modified: Mon Apr 10 17:07:23 2023, max compression
+gzip compressed data, was "nonebot-plugin-chatgpt-on-qq-1.3.0.tar", last modified: Fri Apr 28 17:00:39 2023, max compression
```

## Comparing `nonebot-plugin-chatgpt-on-qq-1.2.0.tar` & `nonebot-plugin-chatgpt-on-qq-1.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 17:07:23.007055 nonebot-plugin-chatgpt-on-qq-1.2.0/
--rw-rw-rw-   0        0        0      770 2023-04-10 17:07:23.007055 nonebot-plugin-chatgpt-on-qq-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-03-07 17:39:40.000000 nonebot-plugin-chatgpt-on-qq-1.2.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-10 17:07:22.983122 nonebot-plugin-chatgpt-on-qq-1.2.0/nonebot_plugin_chatgpt_on_qq/
--rw-rw-rw-   0        0        0    12808 2023-04-10 03:38:53.000000 nonebot-plugin-chatgpt-on-qq-1.2.0/nonebot_plugin_chatgpt_on_qq/__init__.py
--rw-rw-rw-   0        0        0     3660 2023-04-09 15:33:24.000000 nonebot-plugin-chatgpt-on-qq-1.2.0/nonebot_plugin_chatgpt_on_qq/chatGPT.py
--rw-rw-rw-   0        0        0      416 2023-04-08 19:05:12.000000 nonebot-plugin-chatgpt-on-qq-1.2.0/nonebot_plugin_chatgpt_on_qq/config.py
--rw-rw-rw-   0        0        0     4351 2023-04-08 19:05:35.000000 nonebot-plugin-chatgpt-on-qq-1.2.0/nonebot_plugin_chatgpt_on_qq/conversation.py
--rw-rw-rw-   0        0        0      502 2023-03-07 16:08:33.000000 nonebot-plugin-chatgpt-on-qq-1.2.0/nonebot_plugin_chatgpt_on_qq/custom_errors.py
--rw-rw-rw-   0        0        0     6773 2023-04-10 17:03:53.000000 nonebot-plugin-chatgpt-on-qq-1.2.0/nonebot_plugin_chatgpt_on_qq/loadpresets.py
-drwxrwxrwx   0        0        0        0 2023-04-10 17:07:22.999040 nonebot-plugin-chatgpt-on-qq-1.2.0/nonebot_plugin_chatgpt_on_qq.egg-info/
--rw-rw-rw-   0        0        0      770 2023-04-10 17:07:22.000000 nonebot-plugin-chatgpt-on-qq-1.2.0/nonebot_plugin_chatgpt_on_qq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      533 2023-04-10 17:07:22.000000 nonebot-plugin-chatgpt-on-qq-1.2.0/nonebot_plugin_chatgpt_on_qq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 17:07:22.000000 nonebot-plugin-chatgpt-on-qq-1.2.0/nonebot_plugin_chatgpt_on_qq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      114 2023-04-10 17:07:22.000000 nonebot-plugin-chatgpt-on-qq-1.2.0/nonebot_plugin_chatgpt_on_qq.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2023-04-10 17:07:22.000000 nonebot-plugin-chatgpt-on-qq-1.2.0/nonebot_plugin_chatgpt_on_qq.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 17:07:23.007055 nonebot-plugin-chatgpt-on-qq-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1220 2023-04-10 17:07:09.000000 nonebot-plugin-chatgpt-on-qq-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 17:00:39.676866 nonebot-plugin-chatgpt-on-qq-1.3.0/
+-rw-rw-rw-   0        0        0      770 2023-04-28 17:00:39.674336 nonebot-plugin-chatgpt-on-qq-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-03-07 17:39:40.000000 nonebot-plugin-chatgpt-on-qq-1.3.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-28 17:00:39.645585 nonebot-plugin-chatgpt-on-qq-1.3.0/nonebot_plugin_chatgpt_on_qq/
+-rw-rw-rw-   0        0        0    14817 2023-04-28 16:59:15.000000 nonebot-plugin-chatgpt-on-qq-1.3.0/nonebot_plugin_chatgpt_on_qq/__init__.py
+-rw-rw-rw-   0        0        0     3855 2023-04-28 16:59:15.000000 nonebot-plugin-chatgpt-on-qq-1.3.0/nonebot_plugin_chatgpt_on_qq/chatGPT.py
+-rw-rw-rw-   0        0        0      490 2023-04-28 16:59:15.000000 nonebot-plugin-chatgpt-on-qq-1.3.0/nonebot_plugin_chatgpt_on_qq/config.py
+-rw-rw-rw-   0        0        0     4412 2023-04-28 16:59:15.000000 nonebot-plugin-chatgpt-on-qq-1.3.0/nonebot_plugin_chatgpt_on_qq/conversation.py
+-rw-rw-rw-   0        0        0      527 2023-04-28 16:59:15.000000 nonebot-plugin-chatgpt-on-qq-1.3.0/nonebot_plugin_chatgpt_on_qq/custom_errors.py
+-rw-rw-rw-   0        0        0     5258 2023-04-28 16:59:15.000000 nonebot-plugin-chatgpt-on-qq-1.3.0/nonebot_plugin_chatgpt_on_qq/loadpresets.py
+drwxrwxrwx   0        0        0        0 2023-04-28 17:00:39.671220 nonebot-plugin-chatgpt-on-qq-1.3.0/nonebot_plugin_chatgpt_on_qq.egg-info/
+-rw-rw-rw-   0        0        0      770 2023-04-28 17:00:39.000000 nonebot-plugin-chatgpt-on-qq-1.3.0/nonebot_plugin_chatgpt_on_qq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      533 2023-04-28 17:00:39.000000 nonebot-plugin-chatgpt-on-qq-1.3.0/nonebot_plugin_chatgpt_on_qq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 17:00:39.000000 nonebot-plugin-chatgpt-on-qq-1.3.0/nonebot_plugin_chatgpt_on_qq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      114 2023-04-28 17:00:39.000000 nonebot-plugin-chatgpt-on-qq-1.3.0/nonebot_plugin_chatgpt_on_qq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2023-04-28 17:00:39.000000 nonebot-plugin-chatgpt-on-qq-1.3.0/nonebot_plugin_chatgpt_on_qq.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-28 17:00:39.677844 nonebot-plugin-chatgpt-on-qq-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1220 2023-04-28 17:00:11.000000 nonebot-plugin-chatgpt-on-qq-1.3.0/setup.py
```

### Comparing `nonebot-plugin-chatgpt-on-qq-1.2.0/PKG-INFO` & `nonebot-plugin-chatgpt-on-qq-1.3.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-chatgpt-on-qq
-Version: 1.2.0
+Version: 1.3.0
 Summary: 具有多对话功能的chatGPT聊天插件
 Home-page: https://github.com/Suxmx/nonebot_plugin_chatgpt_turbo_on_qq
 Author: 颜曦
 Author-email: 424504326@qq.com
 Maintainer: 颜曦
 Maintainer-email: 424504326@qq.com
 License: BSD License
```

### Comparing `nonebot-plugin-chatgpt-on-qq-1.2.0/nonebot_plugin_chatgpt_on_qq/__init__.py` & `nonebot-plugin-chatgpt-on-qq-1.3.0/nonebot_plugin_chatgpt_on_qq/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,285 +1,323 @@
 import json
 import re
-import openai
+from json import JSONDecodeError
+from typing import Optional, Dict, List
 
+import openai
 from nonebot import get_driver
 from nonebot.adapters.onebot.v11 import (Bot,
-                                         Event,
-                                         GroupMessageEvent, PrivateMessageEvent)
+                                         Event, MessageEvent,
+                                         GroupMessageEvent, PrivateMessageEvent,
+                                         GROUP_ADMIN, GROUP_OWNER)
 from nonebot.log import logger
-from nonebot.plugin import on_regex, on_fullmatch
+from nonebot.plugin import on_regex
 from nonebot.params import ArgPlainText
+from nonebot.permission import SUPERUSER, Permission
+from nonebot.plugin import PluginMetadata
 
-from .conversation import Conversation, GroupPanel,listpresets
+from .config import Config
+from .conversation import Conversation, GroupPanel, presets_str
 from .custom_errors import NoApiKeyError
 
-Chat = on_regex(r"^/talk\s+.+")  # 聊天
-CallMenu = on_fullmatch("/chat")  # 呼出菜单
-ShowList = on_regex(r"^/chat\s+list\s*$")  # 展示群聊天列表
-Join = on_regex(r"^/chat\s+join\s+\d+")  # 加入对话
-Delete = on_regex(r"^/chat\s+delete\s+\d+")  # 删除对话
-Dump = on_regex(r"^/chat\s+dump$")  # 导出json
-CreateConversationWithPrompt = on_regex(r"^/chat\s+create\s+.+$")# 利用自定义prompt创建对话
-CreateConversationWithTemplate = on_regex(r"^/chat\s+create$")# 利用模板创建对话
-CreateConversationWithJson = on_regex(r"^/chat\s+json$")# 利用json创建对话
+__usage__: str = (
+        "太长不看版:\n"
+        + "先用/chat create命令,选择模板来创建对话,随后/talk 内容 来对话\n\n"
+        + "/chat :获取菜单\n"
+        + "/chat create :利用模板创建一个对话并加入\n"
+        + "/talk <内容> :在当前的对话进行聊天\n"
+        + "/chat list :获得当前已创建的对话列表\n"
+        + "/chat join 序号(指/chat list中的序号) :参与list中的某个对话\n"
+        + "/chat create (prompt) :自定义prompt来创建一个新的对话\n"
+        + "/chat delete 序号(指/chat list中的序号) :删除list中的某个对话\n"
+        + "/chat dump :导出当前对话的历史记录json\n"
+)
+__plugin_meta__ = PluginMetadata(
+    name="多功能ChatGPT插件",
+    description="基于chatGPT-3.5-turbo API的nonebot插件",
+    usage=__usage__,
+    config=Config,
+    extra={
+        "License": "BSD License",
+        "Author": "颜曦",
+        "version": "1.3.0",
+    },
+)
+
+plugin_config: Config = Config.parse_obj(get_driver().config.dict())
+temperature: float = plugin_config.temperature
+allow_private: bool = plugin_config.allow_private
+# 因为电脑端的qq在输入/chat xxx时候经常被转换成表情，所以支持自定义指令前缀替换"chat"
+change_chat_to: str = plugin_config.change_chat_to
+pattern_str = f'(chat|{change_chat_to})' if change_chat_to else 'chat'
+
+
+async def _allow_private_checker(event: MessageEvent) -> bool:
+    return isinstance(event, GroupMessageEvent) or allow_private
+
+
+ALLOW_PRIVATE = Permission(_allow_private_checker)
+
+Chat = on_regex(r"^/talk\s+.+", permission=ALLOW_PRIVATE)  # 聊天
+CallMenu = on_regex(rf"^/{pattern_str}$", permission=ALLOW_PRIVATE)  # 呼出菜单
+ShowList = on_regex(rf"^/{pattern_str}\s+list\s*$", permission=ALLOW_PRIVATE)  # 展示群聊天列表
+Join = on_regex(rf"^/{pattern_str}\s+join\s+\d+", permission=ALLOW_PRIVATE)  # 加入对话
+Delete = on_regex(rf"^/{pattern_str}\s+delete\s+\d+", permission=ALLOW_PRIVATE)  # 删除对话
+Dump = on_regex(rf"^/{pattern_str}\s+dump$", permission=ALLOW_PRIVATE)  # 导出json
+CreateConversationWithPrompt = on_regex(rf"^/{pattern_str}\s+create\s+.+$", permission=ALLOW_PRIVATE)  # 利用自定义prompt创建对话
+CreateConversationWithTemplate = on_regex(rf"^/{pattern_str}\s+create$", permission=ALLOW_PRIVATE)  # 利用模板创建对话
+CreateConversationWithJson = on_regex(rf"^/{pattern_str}\s+json$", permission=ALLOW_PRIVATE)  # 利用json创建对话
 
-groupPanels: dict[int:GroupPanel] = {}
-privateConversations: dict[int, Conversation] = {}
+groupPanels: Dict[int, GroupPanel] = {}
+privateConversations: Dict[int, Conversation] = {}
 
 
 @Dump.handle()
 async def _(event: Event):
-    userId = event.get_user_id()
+    userId: int = int(event.get_user_id())
+    userConver: Optional["Conversation"] = None
     if isinstance(event, GroupMessageEvent):
-        groupId = event.group_id
+        groupId: int = event.group_id
         groupPanel = groupPanels.get(groupId)
         if groupPanel:
             userConver: Conversation = groupPanel.userInConversation.get(
                 userId)
     else:
         userConver: Conversation = privateConversations.get(userId)
     if userConver:
         await Dump.finish(userConver.dumpJson())
 
 
 @Chat.handle()
-async def _(bot: Bot, event: Event):
+async def _(event: Event):
     msg = event.get_plaintext()
     userInput: str = re.sub(r"^/talk\s+", '', msg)
     if not userInput:
         await Chat.finish("输入不能为空!", at_sender=True)
     if isinstance(event, GroupMessageEvent):
-        groupId = event.group_id
-        userId = event.get_user_id()
-        if not groupPanels.get(groupId) or not groupPanels.get(groupId).userInConversation.get(userId):# 若没有对话则先自动创建一个
+        groupId: int = event.group_id
+        userId: int = int(event.get_user_id())
+        groupPanel: GroupPanel = groupPanels.setdefault(groupId, GroupPanel())
+        if not groupPanels.get(groupId).userInConversation.get(userId):  # 若没有对话则先自动创建一个
             try:
-                newConversation = Conversation.CreateWithTemplate("1", userId)
-            except:
+                newConversation: Conversation = Conversation.CreateWithTemplate("1", userId)
+            except KeyError:
                 await Chat.finish("自动创建失败!请检查模板是否存在", at_sender=True)
-            await Chat.send(f"自动创建{newConversation.name}成功",at_sender=True)
-            groupPanels[event.group_id] = GroupPanel()
-            groupPanels[event.group_id].userInConversation[userId] = newConversation
-            groupPanels[event.group_id].conversations.append(newConversation)
-            try:
-                answer = await newConversation.ask(userInput)
-                await newConversation.GroupAutoSave(groupId)
-            except openai.InvalidRequestError as e:
-                await Chat.finish(str(e))
-            
+            await Chat.send(f"自动创建{newConversation.name}成功", at_sender=True)
+            groupPanel.userInConversation[userId] = newConversation
+            groupPanel.conversations.append(newConversation)
+            fin_conversation: Conversation = newConversation
+
         else:  # 获取GroupPanel以及用户所在的对话
-            groupPanel = groupPanels.get(groupId)
             userConversation: Conversation = groupPanel.userInConversation.get(
                 userId)
-            try:
-                answer = await userConversation.ask(userInput)
-                await userConversation.GroupAutoSave(groupId)
-            except openai.InvalidRequestError as e:
-                await Chat.finish(str(e))
-
+            fin_conversation: Conversation = userConversation
+        try:
+            answer: str = await fin_conversation.ask(userInput, temperature)
+            await fin_conversation.GroupAutoSave(groupId)
+        except ConnectionError:
+            logger.error('连接错误...')
+            await Chat.finish('连接错误...')
+        except openai.InvalidRequestError as e:
+            await Chat.finish(str(e))
         await Chat.finish(answer, at_sender=True)
+
     if isinstance(event, PrivateMessageEvent):
-        userId = event.get_user_id()
-        if not privateConversations.get(userId):# 自动创建
-            newConversation=None
+        userId: int = int(event.get_user_id())
+        if not privateConversations.get(userId):  # 自动创建
+            newConversation: Optional["Conversation"] = None
             try:
                 newConversation = Conversation.CreateWithTemplate("1", userId)
-            except:
+            except KeyError:
                 await Chat.finish("自动创建失败!请检查模板是否存在")
-            if newConversation is not None:
-                await Chat.send(f"自动创建{newConversation.name}成功",at_sender=True)
-                privateConversations[userId] = newConversation
-                try:
-                    answer = await newConversation.ask(userInput)
-                    await Chat.send(answer)
-                    await newConversation.PrivateAutoSave()
-                except openai.InvalidRequestError as e:
-                    await Chat.finish(str(e))
+            await Chat.send(f"自动创建{newConversation.name}成功", at_sender=True)
+            privateConversations[userId] = newConversation
+            fin_conversation: Conversation = newConversation
+
         else:
             userConversation: Conversation = privateConversations.get(userId)
-            try:
-                answer = await userConversation.ask(userInput)
-                await Chat.send(answer)
-                await userConversation.PrivateAutoSave()
-            except openai.InvalidRequestError as e:
-                    await Chat.finish(str(e))
-
+            fin_conversation: Conversation = userConversation
+        try:
+            answer = await fin_conversation.ask(userInput, temperature)
+            await Chat.send(answer)
+            await fin_conversation.PrivateAutoSave()
+        except ConnectionError:
+            logger.error('连接错误...')
+            await Chat.finish('连接错误...')
+        except openai.InvalidRequestError as e:
+            await Chat.finish(str(e))
 
 
 @Join.handle()
 async def _(event: Event):
     msg = event.get_plaintext()
-    msg = re.sub(r"^/chat\s+join\s+", '', msg)
-    id = int(msg)
+    msg = re.sub(rf"^/{pattern_str}\s+join\s+", '', msg)
+    conversation_id = int(msg)
     if isinstance(event, GroupMessageEvent):
         groupPanel = groupPanels.get(event.group_id)
         if not groupPanel:
             await Join.finish("本群尚未创建过对话!请用/chat create命令来创建对话!", at_sender=True)
-        if id < 1 or id > len(groupPanel.conversations):
+        if conversation_id < 1 or conversation_id > len(groupPanel.conversations):
             await Join.finish("序号超出!", at_sender=True)
-        userId = event.get_user_id()
-        conversation = groupPanel.conversations[id-1]
-        groupPanel.userInConversation[userId] = conversation
-        await Join.finish(f"加入对话{id}成功!", at_sender=True)
+        userId: int = int(event.get_user_id())
+        fin_conversation = groupPanel.conversations[conversation_id - 1]
+        groupPanel.userInConversation[userId] = fin_conversation
+        await Join.finish(f"加入对话{conversation_id}成功!", at_sender=True)
     else:
         await Join.finish("私聊中无法加入对话!")
 
 
 @CallMenu.handle()
-async def _(bot: Bot, event: Event):
-    menu: str = (
-        "太长不看版:\n"
-        + "先用/chat create命令,选择模板来创建对话,随后/talk 内容 来对话\n\n"
-        + "/chat :获取菜单\n"
-        + "/chat create :利用模板创建一个对话并加入\n"
-        + "/talk <内容> :在当前的对话进行聊天\n"
-        + "/chat list :获得当前已创建的对话列表\n"
-        + "/chat join 序号(指/chat list中的序号) :参与list中的某个对话\n"
-        + "/chat create (prompt) :自定义prompt来创建一个新的对话\n"
-        + "/chat delete 序号(指/chat list中的序号) :删除list中的某个对话\n"
-        + "/chat dump :导出当前对话的历史记录json\n"
-    )
+async def _():
+    menu: str = __usage__
     await CallMenu.finish(menu, at_sender=True)
 
 
 @Delete.handle()
-async def _(event: Event):
+async def _(bot: Bot, event: Event):
     msg = event.get_plaintext()
-    msg = re.sub(r"^/chat\s+delete\s+", '', msg)
-    id = int(msg)
+    msg = re.sub(rf"^/{pattern_str}\s+delete\s+", '', msg)
+    conversation_id = int(msg)
     if isinstance(event, GroupMessageEvent):
         groupPanel = groupPanels.get(event.group_id)
         if not groupPanel:
             await Join.finish("本群尚未创建过对话!", at_sender=True)
-        if id < 1 or id > len(groupPanel.conversations):
+        if conversation_id < 1 or conversation_id > len(groupPanel.conversations):
             await Join.finish("序号超出!", at_sender=True)
-        userId = event.get_user_id()
-        if groupPanel.conversations[id-1].owner.id == userId:
-            conver = groupPanel.conversations[id-1]
-            jointUser: list[int] = []
-            for user, conversation in groupPanel.userInConversation.items():
-                if conver == conversation:
+        userId: int = int(event.get_user_id())
+        perm_check = (await SUPERUSER(bot, event)) or (await GROUP_ADMIN(bot, event)) or (await GROUP_OWNER(bot, event))
+        if groupPanel.conversations[conversation_id - 1].owner.id == userId or perm_check:
+            conver = groupPanel.conversations[conversation_id - 1]
+            jointUser: List[int] = []
+            for user, _conversation in groupPanel.userInConversation.items():
+                if conver == _conversation:
                     jointUser.append(user)
             for user in jointUser:
                 groupPanel.userInConversation.pop(user)
 
-            groupPanel.conversations.pop(id-1)
+            groupPanel.conversations.pop(conversation_id - 1)
             await Delete.finish("删除成功!")
         else:
             await Delete.finish("您不是该对话的创建者或管理员!")
     else:
-        privateConversations.pop(event.get_user_id())
+        privateConversations.pop(int(event.get_user_id()))
         await Delete.finish("已删除当前对话")
+
+
 # 暂时已完成
 
 
 @ShowList.handle()
-async def _(bot: Bot, event: Event):
+async def _(event: Event):
     if isinstance(event, GroupMessageEvent):
         curPanel: GroupPanel = groupPanels.get(event.group_id)
         if not curPanel:
             await ShowList.finish("本群尚未创建过对话", at_sender=True)
         elif len(curPanel.conversations) == 0:
             await ShowList.finish("本群对话已全部被清除", at_sender=True)
         else:
             msg: str = "\n"
-            for conversation in curPanel.conversations:
-                msg += f"{curPanel.conversations.index(conversation)+1} 创建者:{conversation.owner.id}\n"
+            for _conversation in curPanel.conversations:
+                msg += f"{curPanel.conversations.index(_conversation) + 1}. {_conversation.name} " \
+                       f"创建者:{_conversation.owner.id}\n"
             await ShowList.finish(msg, at_sender=True)
     elif isinstance(event, PrivateMessageEvent):
         await ShowList.finish("私聊中无法展示列表(最多只有一个对话)")
 
+
 # 暂时完成
 
 
 @CreateConversationWithPrompt.handle()
-async def _(bot: Bot, event: Event):
+async def _(event: Event):
     msg = event.get_plaintext()
-    customPrompt: str = re.sub(r"^/chat\s+create\s*", '', msg)  # 获取用户自定义prompt
+    customPrompt: str = re.sub(rf"^/{pattern_str}\s+create\s*", '', msg)  # 获取用户自定义prompt
     if customPrompt:
-        userID = event.get_user_id()
+        userID: int = int(event.get_user_id())
         try:
-            newConversation = Conversation.CreateWithStr(
-                customPrompt, userID)
+            newConversation: Conversation = Conversation.CreateWithStr(
+                customPrompt, userID, customPrompt[:5])
         except NoApiKeyError:
             await CreateConversationWithPrompt.finish("请机器人管理员在设置中添加APIKEY！")
         if isinstance(event, GroupMessageEvent):  # 当在群聊中时
-            if not groupPanels.get(event.group_id):  # 没有时创建新的groupPanel
-                groupPanels[event.group_id] = GroupPanel()
-            groupPanels[event.group_id].conversations.append(newConversation)
-            groupPanels[event.group_id].userInConversation[userID] = newConversation
+            groupId: int = event.group_id
+            group_panel: GroupPanel = groupPanels.setdefault(groupId, GroupPanel())
+            group_panel.conversations.append(newConversation)
+            group_panel.userInConversation[userID] = newConversation
             await CreateConversationWithPrompt.finish(f"创建成功!", at_sender=True)
 
         elif isinstance(event, PrivateMessageEvent):  # 当在私聊中时
             if privateConversations[userID]:
                 await CreateConversationWithPrompt.finish("已存在一个对话,请先删除")
             else:
                 privateConversations[userID] = Conversation.CreateWithStr(
-                    customPrompt, userID)
+                    customPrompt, userID, customPrompt[:6])
                 await CreateConversationWithPrompt.finish(f"用户{str(userID)}创建成功")
     else:  # 若prompt全为空
         await CreateConversationWithPrompt.finish("输入prompt不能为空格!")
 
 
 @CreateConversationWithTemplate.handle()
-async def CreateConversation(event: Event):
-    ans=listpresets()
-    await CreateConversationWithTemplate.send(ans, at_sender=True)
+async def CreateConversation():
+    await CreateConversationWithTemplate.send(presets_str, at_sender=True)
+
 
 # 暂时完成
 
 
 @CreateConversationWithTemplate.got(key="template")
-async def Create(event: Event, id: str = ArgPlainText("template")):
-    ifGroup = True
-    userId = event.get_user_id()
+async def Create(event: Event, template_id: str = ArgPlainText("template")):
+    userId: int = int(event.get_user_id())
     if isinstance(event, PrivateMessageEvent):
-        ifGroup = False
         if privateConversations.get(userId):
             await CreateConversationWithTemplate.finish("已存在一个对话，请先删除该对话!")
-    if not id.isdigit():
+    if not template_id.isdigit():
         await CreateConversationWithTemplate.reject("输入ID无效!")
-    newConversation = None
+
+    newConversation: Optional["Conversation"] = None
     try:
-        newConversation = Conversation.CreateWithTemplate(id, userId)
+        newConversation = Conversation.CreateWithTemplate(template_id, userId)
     except NoApiKeyError:
         await CreateConversationWithTemplate.finish("请机器人管理员在设置中添加APIKEY！")
-    if newConversation is not None:
-        await CreateConversationWithTemplate.send(f"创建{newConversation.name}模板成功!",at_sender=True)
-    else :
+    if newConversation is None:
         await CreateConversationWithTemplate.finish("输入ID无效!")
-    if ifGroup:
-        if not groupPanels.get(event.group_id):
-            groupPanels[event.group_id] = GroupPanel()
-        groupPanels[event.group_id].userInConversation[userId] = newConversation
-        groupPanels[event.group_id].conversations.append(newConversation)
+    await CreateConversationWithTemplate.send(f"使用模板{template_id}创建{newConversation.name}对话成功!",
+                                              at_sender=True)
+    if isinstance(event, GroupMessageEvent):
+        groupId: int = event.group_id
+        group_panel: GroupPanel = groupPanels.setdefault(groupId, GroupPanel())
+
+        group_panel.userInConversation[userId] = newConversation
+        group_panel.conversations.append(newConversation)
     else:
         privateConversations[userId] = newConversation
 
 
 @CreateConversationWithJson.handle()
 async def CreateConversation():
     pass
 
 
 @CreateConversationWithJson.got("jsonStr", "请直接输入json")
 async def GetJson(event: Event, jsonStr: str = ArgPlainText("jsonStr")):
     try:
         history = json.loads(jsonStr)
-    except:
-        logger.error("json文件错误!")
+    except JSONDecodeError:
+        logger.error("json字符串错误!")
         await CreateConversationWithJson.reject("Json错误!")
     if not history[0].get("role"):
         await CreateConversationWithJson.reject("Json错误!")
+    userId: int = int(event.get_user_id())
     try:
-        newConversation = Conversation(history, event.get_user_id())
+        newConversation: Conversation = Conversation(history, userId, history[0].get('content', '')[:6])
     except NoApiKeyError:
         await CreateConversationWithJson.finish("请机器人管理员在设置中添加APIKEY！")
 
     if isinstance(event, GroupMessageEvent):
-        groupPanels[event.group_id].conversations.append(newConversation)
-        groupPanels[event.group_id].userInConversation[event.get_user_id()
-                                                       ] = newConversation
+        groupId: int = event.group_id
+        group_panel: GroupPanel = groupPanels.setdefault(groupId, GroupPanel())
+        group_panel.conversations.append(newConversation)
+        group_panel.userInConversation[userId] = newConversation
         await CreateConversationWithJson.send("创建对话成功!", at_sender=True)
     elif isinstance(event, PrivateMessageEvent):
-        privateConversations[event.get_user_id()] = newConversation
+        privateConversations[userId] = newConversation
         await CreateConversationWithJson.send("创建对话成功!")
```

### Comparing `nonebot-plugin-chatgpt-on-qq-1.2.0/nonebot_plugin_chatgpt_on_qq/chatGPT.py` & `nonebot-plugin-chatgpt-on-qq-1.3.0/nonebot_plugin_chatgpt_on_qq/chatGPT.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,107 +1,109 @@
+import json
+from typing import Dict, List
+
 import openai
 # import tiktoken
-import json
 from nonebot.log import logger
 from nonebot import get_driver
 
 from .config import Config
-from .custom_errors import OverMaxTokenLengthError, NoResponseError,NoApiKeyError
+from .custom_errors import OverMaxTokenLengthError, NoResponseError, NoApiKeyError
 
 plugin_config = Config.parse_obj(get_driver().config.dict())
 
 # ENCODER = tiktoken.get_encoding("gpt2")
 MAX_TOKEN = 4000
-MODEL = "gpt-3.5-turbo"
+MODEL = plugin_config.model_name
 
 
 class PromptManager:
-    def __init__(self,  basic_prompt, history_max: int) -> None:
-        self.history: list[dict[str:str]] = basic_prompt
+    def __init__(self, basic_prompt, history_max: int) -> None:
+        self.history: List[Dict[str, str]] = basic_prompt
         self.history_max = history_max
-        self.basic_len=len(basic_prompt)
-        self.count=0
+        self.basic_len = len(basic_prompt)
+        self.count = 0
 
     # def check_token_length(self, dicts) -> int:
     #     msgs: str = ""
     #     for dict in dicts:
     #         msgs += (dict["content"])+(dict["role"])+":::\n\n\n" #人工补正
     #     # print("预估长度："+str(len(ENCODER.encode(msgs))))
     #     return len(ENCODER.encode(msgs))
 
     def construct_prompt(
             self,
             new_prompt: str,
-    ) -> list[dict[str:str]]:
+    ) -> List[Dict[str, str]]:
         self.history.append({"role": "user", "content": new_prompt})
-        #if (len(self.history)-self.basic_len > self.history_max+1):
-        while len(self.history)-self.basic_len > self.history_max+1:
+        # if (len(self.history)-self.basic_len > self.history_max+1):
+        while len(self.history) - self.basic_len > self.history_max + 1:
             self.history.pop(self.basic_len)
-            logger.info(f"{len(self.history)-self.basic_len}  {self.history_max}")
+            logger.info(f"{len(self.history) - self.basic_len}  {self.history_max}")
         return self.history
 
-    def add_to_history(self, completion):
+    def add_to_history(self, completion) -> None:
         role = completion["choices"][0]["message"]["role"]
         content = completion["choices"][0]["message"]["content"]
         self.history.append({"role": role, "content": content})
-    def dumpJsonStr(self):
-        self.count=self.count+1
+
+    def dumpJsonStr(self) -> str:
+        self.count = self.count + 1
         try:
-            jsonStr=json.dumps(self.history,ensure_ascii=False)
+            jsonStr = json.dumps(self.history, ensure_ascii=False)
         except UnicodeEncodeError:
-            jsonStr=json.dumps(self.history,ensure_ascii=True)
+            jsonStr = json.dumps(self.history, ensure_ascii=True)
         return jsonStr
-        
-
 
 
 class ChatGPTBot:
-    def __init__(self, api_key: str, basic_prompt,history_max:int) -> None:
+    def __init__(self, api_key: str, basic_prompt, history_max: int) -> None:
         if api_key != "NoKey":
             openai.api_key = api_key
         else:
             raise NoApiKeyError("未设置ApiKey")
-        self.prompt_manager = PromptManager(basic_prompt=basic_prompt,history_max=history_max)
-        self.talk_count=0
+        self.prompt_manager = PromptManager(basic_prompt=basic_prompt, history_max=history_max)
+        self.talk_count = 0
 
     async def ask(
-        self,
-        user_input: str,
-        temperature: float = 0.5,
-    ) -> dict:
+            self,
+            user_input: str,
+            temperature: float = 0.5,
+    ) -> str:
 
         try:
-            completion = await self._get_completion(user_input, temperature)
+            completion: dict = await self._get_completion(user_input, temperature)
             await self._process_completion(completion=completion)
             return completion["choices"][0]["message"]["content"]
-        except:
+        except Exception as e:
+            logger.error(f'get completion error.\n{type(e)}:{e}')
             self.prompt_manager.history.pop()
             raise ConnectionError
-        
 
     async def _get_completion(
             self,
             user_input: str,
             temperature: float = 0.5
-    ):
+    ) -> dict:
 
         return await openai.ChatCompletion.acreate(
             model=MODEL,
             messages=self.prompt_manager.construct_prompt(user_input),
             temperature=temperature,
             max_tokens=1000
         )
 
     async def _process_completion(
-        self,
-        completion: dict
-    ):
+            self,
+            completion: dict
+    ) -> None:
         if completion.get("choices") is None:
             raise NoResponseError("未返回任何choices")
-        if (len(completion["choices"]) == 0):
+        if len(completion["choices"]) == 0:
             raise NoResponseError("返回的choices长度为0")
         if completion["choices"][0].get("message") is None:
             raise NoResponseError("未返回任何文本!")
 
         self.prompt_manager.add_to_history(completion)
-    def dumpJsonStr(self):
+
+    def dumpJsonStr(self) -> str:
         return self.prompt_manager.dumpJsonStr()
```

### Comparing `nonebot-plugin-chatgpt-on-qq-1.2.0/nonebot_plugin_chatgpt_on_qq/conversation.py` & `nonebot-plugin-chatgpt-on-qq-1.3.0/nonebot_plugin_chatgpt_on_qq/conversation.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,133 +1,120 @@
+import os
 import json
 import copy
 import time
-import os
-import openai
-
-from datetime import date
 from pathlib import Path
+from typing import List, Dict, Optional
 
-from .chatGPT import ChatGPTBot
-from .loadpresets import presetcls,loadall,listPresets,createdict
-from typing import List
+import openai
 from nonebot import get_driver
 from nonebot.log import logger
 
 from .config import Config
+from .chatGPT import ChatGPTBot
+from .loadpresets import Preset, load_all_preset
 
-plugin_config = Config.parse_obj(get_driver().config.dict())
+plugin_config: Config = Config.parse_obj(get_driver().config.dict())
 # 设置代理
-proxy = plugin_config.openai_proxy
-api_base = plugin_config.openai_api_base
+proxy: Optional[str] = plugin_config.openai_proxy
+api_base: Optional[str] = plugin_config.openai_api_base
 
-if proxy == None:
+if not proxy:
     logger.error("请设置代理!")
 else:
     openai.proxy = {'http': f"http://{proxy}", 'https': f'http://{proxy}'}
-if api_base != None:
+if api_base:
     openai.api_base = api_base
 
 # 设置保存路径
-START_TIME = time.strftime("%Y-%m-%d-%H-%M-%S", time.localtime())
+START_TIME: str = time.strftime("%Y-%m-%d-%H-%M-%S", time.localtime())
 SAVE_PATH: Path = plugin_config.history_save_path.joinpath(START_TIME)
 # 设置API
-API_KEY = plugin_config.api_key
+API_KEY: str = plugin_config.api_key
 # 设置基础模板
-preset_path=plugin_config.preset_path
-loadedPresets=loadall(preset_path)
-templateDict=createdict(presets=loadedPresets)
-    
+preset_path: Path = plugin_config.preset_path
+presets_list: List[Preset] = load_all_preset(preset_path)
+presets_str: str = Preset.presets2str(presets_list)
+templateDict: Dict[str, Preset] = {str(preset.preset_id): preset for preset in presets_list}
+
 # 设置历史记录上限
 HISTORY_MAX: int = plugin_config.history_max if plugin_config.history_max > 2 else 2
 
 conversationUID: int = 0
 
 
 class GroupPanel:
     def __init__(self) -> None:
         self.conversations: List[Conversation] = []
-        self.userInConversation: dict[int:Conversation] = {}
-
-    def CreateConversation(self):
-        self.conversations.append(Conversation())
+        self.userInConversation: Dict[int, Conversation] = {}
 
 
 class Conversation:
+    isAsking: bool = False
+    name: str = ""
 
-    isAsking = False
-    name=""
-    def __init__(self, prompt: list[dict[str:str]], ownerId: int,name:str="") -> None:
+    def __init__(self, prompt: List[Dict[str, str]], ownerId: int, name: str = "") -> None:
         logger.debug(f"初始化prompt:{prompt}")
-        self.bot = ChatGPTBot(API_KEY, prompt, HISTORY_MAX)
-        self.owner = User(ownerId)
+        self.bot: ChatGPTBot = ChatGPTBot(API_KEY, prompt, HISTORY_MAX)
+        self.owner: User = User(ownerId)
         self.participants: List[User] = []
         global conversationUID
-        self.uid = conversationUID
+        self.uid: int = conversationUID
         conversationUID += 1
-        self.name=name
+        self.name: str = name
 
     @classmethod
-    def CreateWithStr(cls, customPrompt: str, ownerId: int):
+    def CreateWithStr(cls, customPrompt: str, ownerId: int, name: str = '') -> "Conversation":
         customPrompt = [{"role": "user", "content": customPrompt}, {
             "role": "assistant", "content": "好"}]
-        return cls(customPrompt, ownerId)
+        return cls(customPrompt, ownerId, name)
 
     @classmethod
-    def CreateWithJson(cls, jsonStr: str, ownerId: int):
-        messages = json.loads(jsonStr)
-        return cls(messages, ownerId)
+    def CreateWithJson(cls, jsonStr: str, ownerId: int, name: str = '') -> "Conversation":
+        messages: List[Dict[str, str]] = json.loads(jsonStr)
+        return cls(messages, ownerId, name)
 
     @classmethod
-    def CreateWithTemplate(cls, id, ownerId: int):
-        if templateDict.get(id):
-            deepCopy = copy.deepcopy(templateDict[id].preset)
-            return cls(prompt=deepCopy, ownerId=ownerId,name=templateDict[id].name)
-        else:
-            return None
-
-    def ask(self, userInput: str) -> str:
-        answer = self.bot.ask(userInput)
-        return answer
+    def CreateWithTemplate(cls, template_id: str, ownerId: int) -> "Conversation":
+        deepCopy: List[Dict[str, str]] = copy.deepcopy(templateDict[template_id].preset)
+        return cls(prompt=deepCopy, ownerId=ownerId, name=templateDict[template_id].name)
 
-    def dumpJson(self):
+    async def ask(self, userInput: str, temperature: float) -> str:
+        return await self.bot.ask(userInput, temperature)
+
+    def dumpJson(self) -> str:
         return self.bot.dumpJsonStr()
 
-    async def GroupAutoSave(self, groupID: int):
+    async def GroupAutoSave(self, groupID: int) -> None:
         groupID = str(groupID)
         fileName: str = time.strftime(
-            "%Y-%m-%d-%H-%M-%S", time.localtime())+".json"
+            "%Y-%m-%d-%H-%M-%S", time.localtime()) + ".json"
         savePath: Path = SAVE_PATH.joinpath("GroupConversations").joinpath(
             str(groupID)).joinpath(str(self.owner.id)).joinpath(str(self.uid))
-        if (not savePath.exists()):
+        if not savePath.exists():
             os.makedirs(savePath)
         savePath = savePath.joinpath(fileName)
         await self.AutoSave(savePath)
 
-    async def PrivateAutoSave(self):
+    async def PrivateAutoSave(self) -> None:
         fileName: str = time.strftime(
-            "%Y-%m-%d-%H-%M-%S", time.localtime())+".json"
+            "%Y-%m-%d-%H-%M-%S", time.localtime()) + ".json"
         savePath: Path = SAVE_PATH.joinpath(
             "PrivateConversations").joinpath(str(self.owner.id))
         if not savePath.exists():
             os.makedirs(savePath)
         savePath = savePath.joinpath(fileName)
         await self.AutoSave(savePath)
 
-    async def AutoSave(self, path: Path):
-        with open(path, "w", encoding="GB2312") as f:
+    async def AutoSave(self, path: Path) -> None:
+        with open(path, "w", encoding="utf8") as f:
             try:
                 json.dump(self.bot.prompt_manager.history,
                           f, ensure_ascii=False)
-                logger.debug("save")
-            except UnicodeEncodeError:
-                json.dump(self.bot.prompt_manager.history,
-                          f, ensure_ascii=True)
-            except:
-                logger.error("保存Historyjson失败!")
+                logger.debug(f"auto save History json {path}")
+            except Exception:
+                logger.error("保存History json失败!")
 
 
 class User:
-    def __init__(self, userId: str) -> None:
+    def __init__(self, userId: int) -> None:
         self.id = userId
-def listpresets()->str:
-    return listPresets(loadedPresets)
```

### Comparing `nonebot-plugin-chatgpt-on-qq-1.2.0/nonebot_plugin_chatgpt_on_qq.egg-info/PKG-INFO` & `nonebot-plugin-chatgpt-on-qq-1.3.0/nonebot_plugin_chatgpt_on_qq.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-chatgpt-on-qq
-Version: 1.2.0
+Version: 1.3.0
 Summary: 具有多对话功能的chatGPT聊天插件
 Home-page: https://github.com/Suxmx/nonebot_plugin_chatgpt_turbo_on_qq
 Author: 颜曦
 Author-email: 424504326@qq.com
 Maintainer: 颜曦
 Maintainer-email: 424504326@qq.com
 License: BSD License
```

### Comparing `nonebot-plugin-chatgpt-on-qq-1.2.0/nonebot_plugin_chatgpt_on_qq.egg-info/SOURCES.txt` & `nonebot-plugin-chatgpt-on-qq-1.3.0/nonebot_plugin_chatgpt_on_qq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-chatgpt-on-qq-1.2.0/setup.py` & `nonebot-plugin-chatgpt-on-qq-1.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # coding:utf-8
 
 from setuptools import find_packages, setup
 
 setup(
     name='nonebot-plugin-chatgpt-on-qq',
-    version='1.2.0',
+    version='1.3.0',
     description='具有多对话功能的chatGPT聊天插件',
     long_description=open('README.rst').read(),
     author='颜曦',
     author_email='424504326@qq.com',
     maintainer='颜曦',
     maintainer_email='424504326@qq.com',
     packages=find_packages(),
```

