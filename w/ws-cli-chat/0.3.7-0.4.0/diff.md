# Comparing `tmp/ws_cli_chat-0.3.7.tar.gz` & `tmp/ws_cli_chat-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ws_cli_chat-0.3.7.tar", max compression
+gzip compressed data, was "ws_cli_chat-0.4.0.tar", max compression
```

## Comparing `ws_cli_chat-0.3.7.tar` & `ws_cli_chat-0.4.0.tar`

### file list

```diff
@@ -1,7 +1,10 @@
--rw-r--r--   0        0        0      597 2023-04-24 21:39:12.188084 ws_cli_chat-0.3.7/pyproject.toml
--rw-r--r--   0        0        0     1560 2023-04-22 08:02:07.727156 ws_cli_chat-0.3.7/README.md
--rw-r--r--   0        0        0       43 2023-04-23 22:38:40.233412 ws_cli_chat-0.3.7/ws_cli_chat/__init__.py
--rw-r--r--   0        0        0     3296 2023-04-24 21:25:40.373180 ws_cli_chat-0.3.7/ws_cli_chat/cli_chat.py
--rw-r--r--   0        0        0     2858 2023-04-24 21:21:06.167920 ws_cli_chat-0.3.7/ws_cli_chat/myconsole.py
--rw-r--r--   0        0        0      775 2023-04-23 22:38:40.265970 ws_cli_chat-0.3.7/ws_cli_chat/render.py
--rw-r--r--   0        0        0     2177 1970-01-01 00:00:00.000000 ws_cli_chat-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0      597 2023-04-28 07:08:39.037179 ws_cli_chat-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1560 2023-04-22 08:02:07.727156 ws_cli_chat-0.4.0/README.md
+-rw-r--r--   0        0        0       43 2023-04-23 22:38:40.233412 ws_cli_chat-0.4.0/ws_cli_chat/__init__.py
+-rw-r--r--   0        0        0     6568 2023-04-28 07:07:21.887992 ws_cli_chat-0.4.0/ws_cli_chat/ascii_arts.py
+-rw-r--r--   0        0        0     3348 2023-04-28 02:02:08.769276 ws_cli_chat-0.4.0/ws_cli_chat/cli_chat.py
+-rw-r--r--   0        0        0      669 2023-04-28 02:13:50.537740 ws_cli_chat-0.4.0/ws_cli_chat/code_window.py
+-rw-r--r--   0        0        0     1201 2023-04-28 06:58:32.293569 ws_cli_chat-0.4.0/ws_cli_chat/comands.py
+-rw-r--r--   0        0        0     2858 2023-04-24 21:21:06.167920 ws_cli_chat-0.4.0/ws_cli_chat/myconsole.py
+-rw-r--r--   0        0        0      775 2023-04-23 22:38:40.265970 ws_cli_chat-0.4.0/ws_cli_chat/render.py
+-rw-r--r--   0        0        0     2177 1970-01-01 00:00:00.000000 ws_cli_chat-0.4.0/PKG-INFO
```

### Comparing `ws_cli_chat-0.3.7/pyproject.toml` & `ws_cli_chat-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ws_cli_chat"
-version = "0.3.7"
+version = "0.4.0"
 description = "simple cli-websocket-ws-cli-chat"
 authors = ["__coelho__ <109885900+MikalROn@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{include = "ws_cli_chat"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `ws_cli_chat-0.3.7/README.md` & `ws_cli_chat-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `ws_cli_chat-0.3.7/ws_cli_chat/cli_chat.py` & `ws_cli_chat-0.4.0/ws_cli_chat/cli_chat.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import websockets
 import asyncio
 import typer
 import PySimpleGUI as sg
 from pysimpleevent import EventSimpleGUI
 from typing import Optional
 from ws_cli_chat.myconsole import MyConsole
+from comands import string_comand
 
 
 app = typer.Typer()
 MESSAGES: list[str] = []
 
 
 def rederizar_menssagens(lista_menssagens: list) -> None:
@@ -29,15 +30,15 @@
     except KeyboardInterrupt:
         return None
 
 
 def send_message(socket) -> None:
     while True:
         try:
-            msg: str = input()
+            msg: str = string_comand(input())
             if msg and msg != '':
                 asyncio.run(socket.send(msg))
         except KeyboardInterrupt:
             return None
 
 
 def winded_send_message(socket) -> None:
@@ -60,14 +61,15 @@
 
     @loop.event("enviar")
     def send_message(event: str, values: dict, win: sg.Window):
         if values.get('message', '') != '':
             input = win.FindElement('message')
             asyncio.run(socket.send(values['message']))
             input.update('')
+
     try:
         loop.run_window(win, close_event='fechar')
     except KeyboardInterrupt:
         return None
 
 
 async def main(
```

### Comparing `ws_cli_chat-0.3.7/ws_cli_chat/myconsole.py` & `ws_cli_chat-0.4.0/ws_cli_chat/myconsole.py`

 * *Files identical despite different names*

### Comparing `ws_cli_chat-0.3.7/ws_cli_chat/render.py` & `ws_cli_chat-0.4.0/ws_cli_chat/render.py`

 * *Files identical despite different names*

### Comparing `ws_cli_chat-0.3.7/PKG-INFO` & `ws_cli_chat-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ws-cli-chat
-Version: 0.3.7
+Version: 0.4.0
 Summary: simple cli-websocket-ws-cli-chat
 Author: __coelho__
 Author-email: 109885900+MikalROn@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

