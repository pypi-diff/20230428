# Comparing `tmp/onebot_qqguild_extension-0.1.0.tar.gz` & `tmp/onebot_qqguild_extension-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onebot_qqguild_extension-0.1.0.tar", max compression
+gzip compressed data, was "onebot_qqguild_extension-0.1.1.tar", max compression
```

## Comparing `onebot_qqguild_extension-0.1.0.tar` & `onebot_qqguild_extension-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1073 2023-03-19 10:00:58.198371 onebot_qqguild_extension-0.1.0/LICENSE
--rw-r--r--   0        0        0     2358 2023-03-22 02:50:51.401743 onebot_qqguild_extension-0.1.0/onebot_qqguild_extension/__init__.py
--rw-r--r--   0        0        0     1460 2023-03-22 02:52:34.921210 onebot_qqguild_extension-0.1.0/onebot_qqguild_extension/bot.py
--rw-r--r--   0        0        0     1225 2023-03-22 02:50:56.152577 onebot_qqguild_extension-0.1.0/onebot_qqguild_extension/event.py
--rw-r--r--   0        0        0      905 2023-03-22 02:38:20.835988 onebot_qqguild_extension-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      786 2023-03-19 11:21:09.601013 onebot_qqguild_extension-0.1.0/README.md
--rw-r--r--   0        0        0     1400 1970-01-01 00:00:00.000000 onebot_qqguild_extension-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-28 15:55:22.035600 onebot_qqguild_extension-0.1.1/LICENSE
+-rw-r--r--   0        0        0      786 2023-04-28 15:55:22.035600 onebot_qqguild_extension-0.1.1/README.md
+-rw-r--r--   0        0        0     2120 2023-04-28 15:55:22.035600 onebot_qqguild_extension-0.1.1/onebot_qqguild_extension/__init__.py
+-rw-r--r--   0        0        0     1413 2023-04-28 15:55:22.035600 onebot_qqguild_extension-0.1.1/onebot_qqguild_extension/bot.py
+-rw-r--r--   0        0        0     1165 2023-04-28 15:55:22.035600 onebot_qqguild_extension-0.1.1/onebot_qqguild_extension/event.py
+-rw-r--r--   0        0        0      859 2023-04-28 15:55:22.035600 onebot_qqguild_extension-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1400 1970-01-01 00:00:00.000000 onebot_qqguild_extension-0.1.1/PKG-INFO
```

### Comparing `onebot_qqguild_extension-0.1.0/LICENSE` & `onebot_qqguild_extension-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `onebot_qqguild_extension-0.1.0/onebot_qqguild_extension/__init__.py` & `onebot_qqguild_extension-0.1.1/onebot_qqguild_extension/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,61 +1,59 @@
-import inspect
-from typing import Any, Union
-
-from nonebot.adapters.onebot.v12 import Adapter, Bot, Event, Message, MessageSegment
-
-from . import event
-
-for model_name in event.__all__:
-    model = getattr(event, model_name)
-    if not inspect.isclass(model) or not issubclass(model, Event):
-        continue
-    Adapter.add_custom_model(model, platform="qqguild", impl="nonebot-plugin-all4one")
-
-
-async def send(
-    bot: Bot,
-    event: Event,
-    message: Union[str, Message, MessageSegment],
-    at_sender: bool = False,
-    reply_message: bool = False,
-    **params: Any,
-):
-    """支持 QQ 频道"""
-    event_dict = event.dict()
-
-    params.setdefault("detail_type", event_dict["detail_type"])
-
-    if "user_id" in event_dict:  # copy the user_id to the API params if exists
-        params.setdefault("user_id", event_dict["user_id"])
-    else:
-        at_sender = False  # if no user_id, force disable at_sender
-
-    if "group_id" in event_dict:  # copy the group_id to the API params if exists
-        params.setdefault("group_id", event_dict["group_id"])
-
-    if (
-        "guild_id" in event_dict and "channel_id" in event_dict
-    ):  # copy the guild_id to the API params if exists
-        params.setdefault("guild_id", event_dict["guild_id"])
-        params.setdefault("channel_id", event_dict["channel_id"])
-
-    full_message = Message()  # create a new message with at sender segment
-    if reply_message and "message_id" in event_dict:
-        full_message += MessageSegment.reply(event_dict["message_id"])
-    if at_sender and params["detail_type"] != "private":
-        full_message += MessageSegment.mention(params["user_id"]) + " "
-    full_message += message
-    params.setdefault("message", full_message)
-
-    # 传递 event_id，用来支持频道的被动消息
-    params.setdefault("event_id", event_dict["id"])
-    # 传递 guild_id，以支持私信
-    if params["detail_type"] == "private":
-        params.setdefault("guild_id", event_dict["qqguild"]["guild_id"])
-
-    return await bot.send_message(**params)
-
-
-# FIXME: 暂时反着写，因为适配器写反了，等发布新版之后改回来
-# https://github.com/nonebot/adapter-onebot/commit/0e8dddc662c271b235d7d0ae4bc6f2312c675f75
-Adapter.custom_send(send, impl="qqguild", platform="nonebot-plugin-all4one")
+import inspect
+from typing import Any, Union
+
+from nonebot.adapters.onebot.v12 import Adapter, Bot, Event, Message, MessageSegment
+
+from . import event
+
+for model_name in event.__all__:
+    model = getattr(event, model_name)
+    if not inspect.isclass(model) or not issubclass(model, Event):
+        continue
+    Adapter.add_custom_model(model, platform="qqguild", impl="nonebot-plugin-all4one")
+
+
+async def send(
+    bot: Bot,
+    event: Event,
+    message: Union[str, Message, MessageSegment],
+    at_sender: bool = False,
+    reply_message: bool = False,
+    **params: Any,
+):
+    """支持 QQ 频道"""
+    event_dict = event.dict()
+
+    params.setdefault("detail_type", event_dict["detail_type"])
+
+    if "user_id" in event_dict:  # copy the user_id to the API params if exists
+        params.setdefault("user_id", event_dict["user_id"])
+    else:
+        at_sender = False  # if no user_id, force disable at_sender
+
+    if "group_id" in event_dict:  # copy the group_id to the API params if exists
+        params.setdefault("group_id", event_dict["group_id"])
+
+    if (
+        "guild_id" in event_dict and "channel_id" in event_dict
+    ):  # copy the guild_id to the API params if exists
+        params.setdefault("guild_id", event_dict["guild_id"])
+        params.setdefault("channel_id", event_dict["channel_id"])
+
+    full_message = Message()  # create a new message with at sender segment
+    if reply_message and "message_id" in event_dict:
+        full_message += MessageSegment.reply(event_dict["message_id"])
+    if at_sender and params["detail_type"] != "private":
+        full_message += MessageSegment.mention(params["user_id"]) + " "
+    full_message += message
+    params.setdefault("message", full_message)
+
+    # 传递 event_id，用来支持频道的被动消息
+    params.setdefault("event_id", event_dict["id"])
+    # 传递 guild_id，以支持私信
+    if params["detail_type"] == "private":
+        params.setdefault("guild_id", event_dict["qqguild"]["guild_id"])
+
+    return await bot.send_message(**params)
+
+
+Adapter.custom_send(send, platform="qqguild", impl="nonebot-plugin-all4one")
```

### Comparing `onebot_qqguild_extension-0.1.0/onebot_qqguild_extension/event.py` & `onebot_qqguild_extension-0.1.1/onebot_qqguild_extension/event.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-from datetime import datetime
-from typing import List, Optional
-
-from nonebot.adapters.onebot.v12 import ChannelMessageEvent as BaseChannelMessageEvent
-from nonebot.adapters.onebot.v12 import PrivateMessageEvent as BasePrivateMessageEvent
-from pydantic import BaseModel
-
-
-class User(BaseModel):
-    """消息创建者"""
-
-    id: str
-    username: str
-    avatar: str
-    bot: bool
-    union_openid: Optional[str]
-    union_user_account: Optional[str]
-
-
-class Member(BaseModel):
-    """消息创建者的成员信息"""
-
-    user: Optional[User]
-    nick: str
-    roles: List[int]
-    joined_at: datetime
-
-
-class PrivateMessageExtension(BaseModel):
-    """私聊消息扩展"""
-
-    guild_id: str
-    src_guild_id: str
-    author: User
-    member: Member
-
-
-class PrivateMessageEvent(BasePrivateMessageEvent):
-    """私聊消息"""
-
-    qqguild: PrivateMessageExtension
-
-
-class ChannelMessageExtension(BaseModel):
-    """频道消息扩展"""
-
-    author: User
-    member: Member
-
-
-class ChannelMessageEvent(BaseChannelMessageEvent):
-    """频道消息"""
-
-    qqguild: ChannelMessageExtension
-
-
-__all__ = [
-    "PrivateMessageEvent",
-    "ChannelMessageEvent",
-]
+from datetime import datetime
+from typing import List, Optional
+
+from nonebot.adapters.onebot.v12 import ChannelMessageEvent as BaseChannelMessageEvent
+from nonebot.adapters.onebot.v12 import PrivateMessageEvent as BasePrivateMessageEvent
+from pydantic import BaseModel
+
+
+class User(BaseModel):
+    """消息创建者"""
+
+    id: str
+    username: str
+    avatar: str
+    bot: bool
+    union_openid: Optional[str]
+    union_user_account: Optional[str]
+
+
+class Member(BaseModel):
+    """消息创建者的成员信息"""
+
+    user: Optional[User]
+    nick: str
+    roles: List[int]
+    joined_at: datetime
+
+
+class PrivateMessageExtension(BaseModel):
+    """私聊消息扩展"""
+
+    guild_id: str
+    src_guild_id: str
+    author: User
+    member: Member
+
+
+class PrivateMessageEvent(BasePrivateMessageEvent):
+    """私聊消息"""
+
+    qqguild: PrivateMessageExtension
+
+
+class ChannelMessageExtension(BaseModel):
+    """频道消息扩展"""
+
+    author: User
+    member: Member
+
+
+class ChannelMessageEvent(BaseChannelMessageEvent):
+    """频道消息"""
+
+    qqguild: ChannelMessageExtension
+
+
+__all__ = [
+    "PrivateMessageEvent",
+    "ChannelMessageEvent",
+]
```

### Comparing `onebot_qqguild_extension-0.1.0/pyproject.toml` & `onebot_qqguild_extension-0.1.1/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-[tool.poetry]
-name = "onebot-qqguild-extension"
-version = "0.1.0"
-description = ""
-authors = ["hemengyang <hmy0119@gmail.com>"]
-license = "MIT"
-readme = "README.md"
-
-[tool.poetry.dependencies]
-python = "^3.8"
-nonebot2 = "^2.0.0-rc.1"
-nonebot-adapter-onebot = "^2.2.2"
-
-[tool.poetry.group.dev.dependencies]
-black = "*"
-isort = "*"
-pre-commit = "*"
-nonebug = "^0.3.1"
-pytest-cov = "^4.0.0"
-pytest-xdist = "^3.1.0"
-pytest-mock = "^3.7.0"
-pytest-asyncio = "^0.20.3"
-mkdocs = "^1.4.2"
-mkdocs-material = "^9.1.3"
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
-
-[tool.nonebot]
-plugins = ["onebot_qqguild_extension"]
-
-[tool.black]
-line-length = 88
-
-[tool.isort]
-profile = "black"
-line_length = 88
-skip_gitignore = true
-
-[tool.pytest.ini_options]
-asyncio_mode = "auto"
-
-[tool.pyright]
-pythonVersion = "3.8"
-pythonPlatform = "All"
+[tool.poetry]
+name = "onebot-qqguild-extension"
+version = "0.1.1"
+description = ""
+authors = ["hemengyang <hmy0119@gmail.com>"]
+license = "MIT"
+readme = "README.md"
+
+[tool.poetry.dependencies]
+python = "^3.8"
+nonebot2 = "^2.0.0-rc.1"
+nonebot-adapter-onebot = "^2.2.3"
+
+[tool.poetry.group.dev.dependencies]
+black = "*"
+isort = "*"
+pre-commit = "*"
+nonebug = "^0.3.1"
+pytest-cov = "^4.0.0"
+pytest-xdist = "^3.1.0"
+pytest-mock = "^3.7.0"
+pytest-asyncio = "^0.20.3"
+mkdocs = "^1.4.2"
+mkdocs-material = "^9.1.3"
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
+
+[tool.nonebot]
+plugins = ["onebot_qqguild_extension"]
+
+[tool.black]
+line-length = 88
+
+[tool.isort]
+profile = "black"
+line_length = 88
+skip_gitignore = true
+
+[tool.pytest.ini_options]
+asyncio_mode = "auto"
+
+[tool.pyright]
+pythonVersion = "3.8"
+pythonPlatform = "All"
```

### Comparing `onebot_qqguild_extension-0.1.0/README.md` & `onebot_qqguild_extension-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `onebot_qqguild_extension-0.1.0/PKG-INFO` & `onebot_qqguild_extension-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: onebot-qqguild-extension
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 License: MIT
 Author: hemengyang
 Author-email: hmy0119@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: nonebot-adapter-onebot (>=2.2.2,<3.0.0)
+Requires-Dist: nonebot-adapter-onebot (>=2.2.3,<3.0.0)
 Requires-Dist: nonebot2 (>=2.0.0-rc.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # OneBot QQ频道 扩展标准
 
 **QQ频道 扩展标准** 旨在统一不同实现的扩展方法，避免混乱局面的出现。
```

