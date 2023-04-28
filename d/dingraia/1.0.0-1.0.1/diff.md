# Comparing `tmp/dingraia-1.0.0.tar.gz` & `tmp/dingraia-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dingraia-1.0.0.tar", last modified: Sun Apr 16 08:38:31 2023, max compression
+gzip compressed data, was "dingraia-1.0.1.tar", last modified: Fri Apr 28 16:15:20 2023, max compression
```

## Comparing `dingraia-1.0.0.tar` & `dingraia-1.0.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 08:38:31.824880 dingraia-1.0.0/
--rw-rw-rw-   0        0        0    35824 2023-04-16 04:58:06.000000 dingraia-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      312 2023-04-16 08:38:31.809867 dingraia-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2229 2023-04-16 05:03:24.000000 dingraia-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-16 08:38:31.047863 dingraia-1.0.0/dingraia/
--rw-rw-rw-   0        0        0    11019 2023-03-11 05:41:32.000000 dingraia-1.0.0/dingraia/DingTalk.py
--rw-rw-rw-   0        0        0        0 2023-03-01 04:51:52.000000 dingraia-1.0.0/dingraia/__init__.py
--rw-rw-rw-   0        0        0       69 2023-04-16 07:01:45.000000 dingraia-1.0.0/dingraia/__main__.py
--rw-rw-rw-   0        0        0     1917 2023-04-16 08:21:55.000000 dingraia-1.0.0/dingraia/bcc.py
-drwxrwxrwx   0        0        0        0 2023-04-16 08:38:31.256879 dingraia-1.0.0/dingraia/event/
--rw-rw-rw-   0        0        0      387 2023-03-01 05:00:26.000000 dingraia-1.0.0/dingraia/event/__init__.py
--rw-rw-rw-   0        0        0      198 2023-02-28 04:59:29.000000 dingraia-1.0.0/dingraia/event/message.py
--rw-rw-rw-   0        0        0     1230 2023-02-18 02:55:54.000000 dingraia-1.0.0/dingraia/login.py
-drwxrwxrwx   0        0        0        0 2023-04-16 08:38:31.320878 dingraia-1.0.0/dingraia/message/
--rw-rw-rw-   0        0        0        0 2023-02-28 04:29:37.000000 dingraia-1.0.0/dingraia/message/__init__.py
--rw-rw-rw-   0        0        0     1723 2023-03-04 07:54:03.000000 dingraia-1.0.0/dingraia/message/chain.py
--rw-rw-rw-   0        0        0     3653 2023-03-04 08:06:00.000000 dingraia-1.0.0/dingraia/message/element.py
-drwxrwxrwx   0        0        0        0 2023-04-16 08:38:31.327884 dingraia-1.0.0/dingraia/model/
--rw-rw-rw-   0        0        0     2068 2023-02-28 04:59:29.000000 dingraia-1.0.0/dingraia/model/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-16 08:38:31.423872 dingraia-1.0.0/dingraia/saya/
--rw-rw-rw-   0        0        0     1899 2023-03-02 04:31:35.000000 dingraia-1.0.0/dingraia/saya/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-16 08:38:31.446876 dingraia-1.0.0/dingraia/saya/builtins/
--rw-rw-rw-   0        0        0        0 2023-02-18 13:40:40.000000 dingraia-1.0.0/dingraia/saya/builtins/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-16 08:38:31.597890 dingraia-1.0.0/dingraia/saya/builtins/broadcast/
--rw-rw-rw-   0        0        0       66 2023-02-18 13:57:35.000000 dingraia-1.0.0/dingraia/saya/builtins/broadcast/__init__.py
--rw-rw-rw-   0        0        0      761 2023-02-18 13:57:35.000000 dingraia-1.0.0/dingraia/saya/builtins/broadcast/schema.py
--rw-rw-rw-   0        0        0     2406 2023-04-16 04:18:39.000000 dingraia-1.0.0/dingraia/saya/channel.py
--rw-rw-rw-   0        0        0      125 2023-02-17 14:10:02.000000 dingraia-1.0.0/dingraia/saya/context.py
--rw-rw-rw-   0        0        0     4995 2023-03-04 03:37:47.000000 dingraia-1.0.0/dingraia/signer.py
-drwxrwxrwx   0        0        0        0 2023-04-16 08:38:31.645862 dingraia-1.0.0/dingraia/tools/
--rw-rw-rw-   0        0        0      518 2023-03-11 09:51:12.000000 dingraia-1.0.0/dingraia/tools/__init__.py
--rw-rw-rw-   0        0        0     7208 2023-03-20 10:09:31.000000 dingraia-1.0.0/dingraia/tools/debug.py
--rw-rw-rw-   0        0        0      416 2023-04-16 03:58:21.000000 dingraia-1.0.0/dingraia/tools/timer.py
-drwxrwxrwx   0        0        0        0 2023-04-16 08:38:31.226872 dingraia-1.0.0/dingraia.egg-info/
--rw-rw-rw-   0        0        0      312 2023-04-16 08:38:30.000000 dingraia-1.0.0/dingraia.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      813 2023-04-16 08:38:30.000000 dingraia-1.0.0/dingraia.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 08:38:30.000000 dingraia-1.0.0/dingraia.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-04-16 08:38:30.000000 dingraia-1.0.0/dingraia.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-16 08:38:30.000000 dingraia-1.0.0/dingraia.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-04-16 08:38:30.000000 dingraia-1.0.0/dingraia.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2023-04-16 08:38:31.825883 dingraia-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      514 2023-04-16 08:38:11.000000 dingraia-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-16 08:38:31.804865 dingraia-1.0.0/slog/
--rw-rw-rw-   0        0        0     5548 2023-04-15 03:57:06.000000 dingraia-1.0.0/slog/__init__.py
--rw-rw-rw-   0        0        0    13453 2023-03-25 16:07:34.000000 dingraia-1.0.0/slog/element.py
--rw-rw-rw-   0        0        0        3 2023-03-26 06:50:17.000000 dingraia-1.0.0/slog/filter.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:15:20.620679 dingraia-1.0.1/
+-rw-rw-rw-   0        0        0    35824 2023-04-16 04:58:06.000000 dingraia-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      312 2023-04-28 16:15:20.618670 dingraia-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2247 2023-04-28 16:06:18.000000 dingraia-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-28 16:15:20.137660 dingraia-1.0.1/dingraia/
+-rw-rw-rw-   0        0        0    11008 2023-04-28 16:06:18.000000 dingraia-1.0.1/dingraia/DingTalk.py
+-rw-rw-rw-   0        0        0        0 2023-03-01 04:51:52.000000 dingraia-1.0.1/dingraia/__init__.py
+-rw-rw-rw-   0        0        0       69 2023-04-28 16:06:18.000000 dingraia-1.0.1/dingraia/__main__.py
+-rw-rw-rw-   0        0        0     1968 2023-04-28 16:06:18.000000 dingraia-1.0.1/dingraia/bcc.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:15:20.418681 dingraia-1.0.1/dingraia/event/
+-rw-rw-rw-   0        0        0      387 2023-03-01 05:00:26.000000 dingraia-1.0.1/dingraia/event/__init__.py
+-rw-rw-rw-   0        0        0      198 2023-02-28 04:59:29.000000 dingraia-1.0.1/dingraia/event/message.py
+-rw-rw-rw-   0        0        0     1230 2023-02-18 02:55:54.000000 dingraia-1.0.1/dingraia/login.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:15:20.445684 dingraia-1.0.1/dingraia/message/
+-rw-rw-rw-   0        0        0        0 2023-02-28 04:29:37.000000 dingraia-1.0.1/dingraia/message/__init__.py
+-rw-rw-rw-   0        0        0     1723 2023-03-04 07:54:03.000000 dingraia-1.0.1/dingraia/message/chain.py
+-rw-rw-rw-   0        0        0     3827 2023-04-28 16:06:18.000000 dingraia-1.0.1/dingraia/message/element.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:15:20.450672 dingraia-1.0.1/dingraia/model/
+-rw-rw-rw-   0        0        0     2262 2023-04-28 16:06:18.000000 dingraia-1.0.1/dingraia/model/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:15:20.481661 dingraia-1.0.1/dingraia/saya/
+-rw-rw-rw-   0        0        0     1899 2023-03-02 04:31:35.000000 dingraia-1.0.1/dingraia/saya/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:15:20.496684 dingraia-1.0.1/dingraia/saya/builtins/
+-rw-rw-rw-   0        0        0        0 2023-02-18 13:40:40.000000 dingraia-1.0.1/dingraia/saya/builtins/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:15:20.535678 dingraia-1.0.1/dingraia/saya/builtins/broadcast/
+-rw-rw-rw-   0        0        0       66 2023-02-18 13:57:35.000000 dingraia-1.0.1/dingraia/saya/builtins/broadcast/__init__.py
+-rw-rw-rw-   0        0        0      761 2023-02-18 13:57:35.000000 dingraia-1.0.1/dingraia/saya/builtins/broadcast/schema.py
+-rw-rw-rw-   0        0        0     2406 2023-04-16 04:18:39.000000 dingraia-1.0.1/dingraia/saya/channel.py
+-rw-rw-rw-   0        0        0      125 2023-02-17 14:10:02.000000 dingraia-1.0.1/dingraia/saya/context.py
+-rw-rw-rw-   0        0        0     4995 2023-03-04 03:37:47.000000 dingraia-1.0.1/dingraia/signer.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:15:20.571665 dingraia-1.0.1/dingraia/tools/
+-rw-rw-rw-   0        0        0      518 2023-03-11 09:51:12.000000 dingraia-1.0.1/dingraia/tools/__init__.py
+-rw-rw-rw-   0        0        0     7208 2023-03-20 10:09:31.000000 dingraia-1.0.1/dingraia/tools/debug.py
+-rw-rw-rw-   0        0        0      416 2023-04-16 03:58:21.000000 dingraia-1.0.1/dingraia/tools/timer.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:15:20.405667 dingraia-1.0.1/dingraia.egg-info/
+-rw-rw-rw-   0        0        0      312 2023-04-28 16:15:19.000000 dingraia-1.0.1/dingraia.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      813 2023-04-28 16:15:19.000000 dingraia-1.0.1/dingraia.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 16:15:19.000000 dingraia-1.0.1/dingraia.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-04-28 16:15:19.000000 dingraia-1.0.1/dingraia.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-28 16:15:19.000000 dingraia-1.0.1/dingraia.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-04-16 08:38:30.000000 dingraia-1.0.1/dingraia.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2023-04-28 16:15:20.625670 dingraia-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      514 2023-04-28 16:15:10.000000 dingraia-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 16:15:20.605686 dingraia-1.0.1/slog/
+-rw-rw-rw-   0        0        0     5548 2023-04-15 03:57:06.000000 dingraia-1.0.1/slog/__init__.py
+-rw-rw-rw-   0        0        0    13453 2023-03-25 16:07:34.000000 dingraia-1.0.1/slog/element.py
+-rw-rw-rw-   0        0        0        3 2023-03-26 06:50:17.000000 dingraia-1.0.1/slog/filter.py
```

### Comparing `dingraia-1.0.0/LICENSE` & `dingraia-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dingraia-1.0.0/README.md` & `dingraia-1.0.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,59 +1,59 @@
 ﻿# 这是什么？
 这个是一个关于能套用Graia-Ariadne项目的小部分模块
 并运行的异步钉钉机器人代码，用来运行 基础 的Webhook类型
 的微型机器人，只实现了10%的功能，将来可能会完善。
 作者是Python废物，请不要催，你行你上。
 
 # 特点
-支持协程，支持阻塞函数的并发，函数捕捉报错等
+支持协程，支持阻塞函数的并发，函数捕捉报错等，支持At含有userid的人员
 
 # 注意
-本项目适用于一般聊天机器人开发，99%不适应生产环境
+本项目适用于一般聊天机器人开发，不建议用于生产环境
 作者自身已经挂着该框架，保证框架确实可用
 
 # 需求
 首先得有一个公网IP，还得拥有企业内部开发权限
 
 # 实现方法
 通过使用简单的Flask服务端和非常简单的装饰器进行非常简单
-的广播方法，非常容易在运作过程中报错。
+的广播方法。
 
 # 如何使用？
-把导入的模块相应地替换成Ding中的模块即可。
+把导入的模块相应地替换成Dingraia中的模块即可。
 具体请观看[Dingraia使用方法](https://wps.lxyddice.top/meihuaguangshuo/dingraia%E4%BD%BF%E7%94%A8%E6%96%B9%E6%B3%95/)
-由于cloudflare的原因，博客无法使用，如需帮助请联系我
-## 接受函数
+
+由于Cloudflare和lj服务器的原因，博客可能无法使用，如需帮助请联系我
+## 接收函数
 ```python
-@channel.use(ListenerSchema(listening_events[GroupMessage]))
+@channel.use(ListenerSchema(listening_events[GroupMessage]))  # 目前只支持GroupMessage
 async def example(group: Group):  # 此处暂不支持传入机器人实例
     ...
 ```
 当然，也可以这样
 ```python
 @channel.use(ListenerSchema(listening_events[GroupMessage]))
 def example(group: Group):  # 此处暂不支持传入机器人实例
     ...
 ```
 它们都会并发执行
+~~(你不会异步的话建议直接使用def，这样理论上效率会快一点)~~
 ## 发送消息
 ```python
 app = Dingtalk()
-app.send_message(MessageChain()) # 当然也可以传入任意对象，前提是支持str方法
-# 从 element 导入元素即可发送 MarkDown, ActionCard等支持的消息卡片
+app.send_message(MessageChain("Message")) # 当然也可以传入任意对象，前提是支持str方法
+# 从 element 导入元素即可发送 MarkDown, ActionCard等支持的消息卡片，如
+app.send_message(MarkDown(...))
 ```
 注意：机器人的发送提示实际是在准备发送时提示的，不一定代表确实发送成功
 
 # 兼容度？
-10%...
+30%...
 
 # TODO
 Flask服务端分离，Websocket链接，消息等待
 
 # 最后要说
 求梨膏，去看看[Graia](https://github.com/GraiaProject/Ariadne)项目吧，这个机器人框架真的很好用，
 至少目前用起来真的很不错。
 
-# 开源协议？
-由于Graia项目使用 GNU AGPL-3.0 协议，故本开源协议相同
 
-如果你觉得我的$hit代码侵犯了您的著作权，请联系我删除
```

### Comparing `dingraia-1.0.0/dingraia/DingTalk.py` & `dingraia-1.0.1/dingraia/DingTalk.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,27 +7,26 @@
 from .message.chain import MessageChain
 from .login import url_res
 from .model import Group
 from .message.element import *
 from .saya import Channel, Saya
 from .tools.debug import delog
 
-delog.start()
 
 send_url = "https://oapi.dingtalk.com/robot/send?access_token={}&timestamp={}&sign={}"
 
 
 @logger.catch
 def get_sign(secure_key: str):
     timestamp = str(round(time.time() * 1000))
     sign_str = timestamp + '\n' + secure_key
     sign = hmac.new(secure_key.encode("utf-8"), sign_str.encode("utf-8"), hashlib.sha256).digest()
     sign = base64.b64encode(sign)
     sign = urllib.parse.quote_plus(sign)
-    # logger.success(f"成功加签")
+    delog.success(f"成功加签", no=40)
     return sign, timestamp
 
 
 class Dingtalk:
     """
     send_message: msg\n
     send_link: title, text, message_url,  picture_url\n
@@ -77,15 +76,15 @@
                 "text"   : {
                     "content": str(msg)
                 }
             }
         if type(msg) == MessageChain:
             if ats := msg.include(At):
                 at = reduce(lambda x, y: x + y, ats)
-                send_data.update(at.data)
+                send_data["at"] = at.data
         sign = self.get_sign(Dingtalk.sec_key)
         if target is None:
             url = send_url.format(Dingtalk.access_token, sign[1], sign[0])
             self.log.info(f"[SEND] <- {repr(str(msg))[1:-1]}")
         elif type(target) == Group:
             url = target.send_url
             self.log.info(f"[SEND][{target.name}({int(target)})] <- {repr(str(msg))[1:-1]}")
@@ -283,15 +282,15 @@
         try:
             resp = await url_res(url, method='POST', data=send_data, header=header, res='json')
             delog.success("发送完成")
         except Exception as err:
             logger.exception(f"端口发送失败！", err)
             return [False]
         else:
-            delog.info(resp, no=50)
+            delog.info(resp, no=40)
             if not resp['errcode']:
                 delog.success(f"成功!", no=40)
                 return [True]
             else:
                 logger.error(f"发送失败！错误代码：{resp['errcode']}，错误信息：{resp['errmsg']}")
                 return [False, resp['errcode'], resp['errmsg']]
```

### Comparing `dingraia-1.0.0/dingraia/bcc.py` & `dingraia-1.0.1/dingraia/bcc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,26 @@
-﻿from flask import request
+﻿import json
+
+from flask import request
 from .DingTalk import Dingtalk
 from .model import Group, Member, Bot
 from .event import MessageEvent
 from .message.chain import MessageChain
 from .saya import Channel
 from .event.message import GroupMessage
 from loguru import logger
+from .tools.debug import delog
 channel = Channel.current()
 callbacks = []
 
 
 @logger.catch
 async def bcc():
     res = request.get_json()
-    # logger.info(json.dumps(res, indent=2))
+    delog.info(json.dumps(res, indent=2), no=50)
     _e = dispackage(res)
     if not _e:
         logger.warning("无法解包！")
         return
     log(_e)
     await channel.radio(GroupMessage, *_e)
```

### Comparing `dingraia-1.0.0/dingraia/login.py` & `dingraia-1.0.1/dingraia/login.py`

 * *Files identical despite different names*

### Comparing `dingraia-1.0.0/dingraia/message/chain.py` & `dingraia-1.0.1/dingraia/message/chain.py`

 * *Files identical despite different names*

### Comparing `dingraia-1.0.0/dingraia/message/element.py` & `dingraia-1.0.1/dingraia/message/element.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,39 +6,39 @@
 
 class Link:
     
     def __init__(self, url: str, title: str = "[Link]", text: str = "", pic_url: str = ""):
         self.url = url
         self.title = title
         self.text = text
-        self.pic_url = pic_url
+        self.pic_url = pic_url if pic_url else url
         self.data = {
             "msgtype": "link",
             "link"   : {
-                "title"     : str(title),
-                "text"      : str(text),
-                "picUrl"    : _link_detect(str(pic_url)),
-                "messageUrl": _link_detect(str(url))
+                "title"     : str(self.title),
+                "text"      : str(self.text),
+                "picUrl"    : _link_detect(str(self.pic_url)),
+                "messageUrl": _link_detect(str(self.url))
             }
         }
         
     def __str__(self):
-        return "[Link]"
+        return f"[Link]({self.url})"
         
         
 class Markdown:
     
     def __init__(self, text: str, title: str = "[Markdown]"):
         self.text = text
         self.title = title
         self.data = {
             "msgtype" : "markdown",
             "markdown": {
-                "title": str(title),
-                "text" : str(text),
+                "title": str(self.title),
+                "text" : str(self.text),
             }
         }
         
     def __str__(self):
         return "[Markdown]"
         
         
@@ -48,25 +48,25 @@
         self.orientation = orientation
         self.button = button
         self.text = text
         self.title = title
         self.data = {
             "msgtype"   : "actionCard",
             "actionCard": {
-                "title"         : str(title),
-                "text"          : str(text),
-                "btnOrientation": str(orientation)
+                "title"         : str(self.title),
+                "text"          : str(self.text),
+                "btnOrientation": str(self.orientation)
             }
         }
-        if len(button) == 1:
-            self.data['actionCard']['singleTitle'] = str(button[0][0])
-            self.data['actionCard']['singleURL'] = _link_detect(str(button[0][1]))
+        if len(self.button) == 1:
+            self.data['actionCard']['singleTitle'] = str(self.button[0][0])
+            self.data['actionCard']['singleURL'] = _link_detect(str(self.button[0][1]))
         else:
             self.data['actionCard']['btns'] = []
-            for b in button:
+            for b in self.button:
                 if b[0] and b[1]:
                     self.data['actionCard']['btns'].append(
                         {"title": str(b[0]), "actionURL": _link_detect(str(b[1]))})
                 
     def __str__(self):
         return "[ActionCard]"
         
@@ -77,45 +77,47 @@
         self.links = links
         self.data = {
             "msgtype" : "feedCard",
             "feedCard": {
                 "links": []
             }
         }
-        for link in links:
+        for link in self.links:
             if link[0] and link[1]:
                 self.data['feedCard']['links'].append({
                     "title" : str(link[0]), "messageURL": _link_detect(str(link[1])),
                     "picURL": _link_detect(str(link[2]))
                 })
                 
     def __str__(self):
         return "[FeedCard]"
     
 
 class At:
     
-    def __init__(self, target: Union[str, Member], display: str = ""):
+    def __init__(self, target: Union[int, Member], display: str = ""):
         if type(target) == Member:
-            self.target = "$:LWCP_v1:" + str(target.origin_id)
+            self.id = (int(hashlib.sha1(str(target.id)[str(target.id).rfind("$"):].encode('utf-8')).hexdigest(), 16)) % \
+                      (10 ** 10) + 1000
+            self.target = str(target.staffid)
         else:
-            self.target = target
-        self.id = (int(hashlib.sha1(self.target[self.target.rfind("$"):].encode('utf-8')).hexdigest(), 16)) % (10 ** 10) + 1000
-        self.display = display
+            self.target = self.id = target
+        self.display = display if display else self.target
         self.data = {
-            "atDingtalkIds": [self.target]
+            "atUserIds": [str(self.target)]
         }
         
     def __str__(self):
         return "@" + str(self.display)
     
     def __add__(self, other):
         to = copy.deepcopy(self)
-        for i in other.data["atDingtalkIds"]:
-            to.data["atDingtalkIds"].append(i)
+        for i in other.data["atUserIds"]:
+            to.data["atUserIds"].append(i)
         return to
         
 
 def _link_detect(link: str) -> str:
-    if not str(link).startswith("http"):
-        link = "https://" + str(link)
+    if link:
+        if not str(link).startswith("http"):
+            link = "https://" + str(link)
     return link
```

### Comparing `dingraia-1.0.0/dingraia/model/__init__.py` & `dingraia-1.0.1/dingraia/model/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,22 +21,29 @@
     
     def __str__(self) -> str:
         return self.name
 
 
 class Member:
     
-    def __init__(self, id: str = None, name: str = None, group: Group = None, admin: bool = None, origin: dict = None):
+    def __init__(self, id: str = None,
+                 staffid: int = None,
+                 name: str = None,
+                 group: Group = None,
+                 admin: bool = None,
+                 origin: dict = None):
         if origin is not None:
             id = origin.get('senderId')
             name = origin.get("senderNick")
+            staffid = origin.get("senderStaffId")
             admin = origin.get("isAdmin")
         self.origin_id = id[id.rfind("$"):]
         self.id = (int(hashlib.sha1(self.origin_id.encode('utf-8')).hexdigest(), 16)) % (10 ** 10) + 1000
         self.name = name
+        self.staffid = staffid
         self.group = group
         self.admin = admin
     
     def __int__(self) -> int:
         return self.id
     
     def __str__(self) -> str:
```

### Comparing `dingraia-1.0.0/dingraia/saya/__init__.py` & `dingraia-1.0.1/dingraia/saya/__init__.py`

 * *Files identical despite different names*

### Comparing `dingraia-1.0.0/dingraia/saya/builtins/broadcast/schema.py` & `dingraia-1.0.1/dingraia/saya/builtins/broadcast/schema.py`

 * *Files identical despite different names*

### Comparing `dingraia-1.0.0/dingraia/saya/channel.py` & `dingraia-1.0.1/dingraia/saya/channel.py`

 * *Files identical despite different names*

### Comparing `dingraia-1.0.0/dingraia/signer.py` & `dingraia-1.0.1/dingraia/signer.py`

 * *Files identical despite different names*

### Comparing `dingraia-1.0.0/dingraia/tools/__init__.py` & `dingraia-1.0.1/dingraia/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `dingraia-1.0.0/dingraia/tools/debug.py` & `dingraia-1.0.1/dingraia/tools/debug.py`

 * *Files identical despite different names*

### Comparing `dingraia-1.0.0/dingraia.egg-info/SOURCES.txt` & `dingraia-1.0.1/dingraia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dingraia-1.0.0/setup.py` & `dingraia-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ﻿from setuptools import setup, find_packages
 setup(
     name='dingraia',
-    version='1.0.0',
+    version='1.0.1',
     packages=find_packages(),
     url='https://github.com/MeiHuaGuangShuo/Dingraia',
     author='MeiHuaGuangShuo',
     author_email='meihuaguangshuo@gmail.com',
     description='A Dingtalk robot framework based on Python',
     install_requires=[
         "loguru",
```

### Comparing `dingraia-1.0.0/slog/__init__.py` & `dingraia-1.0.1/slog/__init__.py`

 * *Files identical despite different names*

### Comparing `dingraia-1.0.0/slog/element.py` & `dingraia-1.0.1/slog/element.py`

 * *Files identical despite different names*

