# Comparing `tmp/ws_cli_chat-0.4.2.tar.gz` & `tmp/ws_cli_chat-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ws_cli_chat-0.4.2.tar", max compression
+gzip compressed data, was "ws_cli_chat-0.4.3.tar", max compression
```

## Comparing `ws_cli_chat-0.4.2.tar` & `ws_cli_chat-0.4.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      590 2023-04-28 07:38:30.354352 ws_cli_chat-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     1536 2023-04-28 07:32:18.000817 ws_cli_chat-0.4.2/README.md
--rw-r--r--   0        0        0       43 2023-04-23 22:38:40.233412 ws_cli_chat-0.4.2/ws_cli_chat/__init__.py
--rw-r--r--   0        0        0     6568 2023-04-28 07:07:21.887992 ws_cli_chat-0.4.2/ws_cli_chat/ascii_arts.py
--rw-r--r--   0        0        0     3362 2023-04-28 07:23:29.148763 ws_cli_chat-0.4.2/ws_cli_chat/cli_chat.py
--rw-r--r--   0        0        0      669 2023-04-28 02:13:50.537740 ws_cli_chat-0.4.2/ws_cli_chat/code_window.py
--rw-r--r--   0        0        0     1213 2023-04-28 07:24:25.424801 ws_cli_chat-0.4.2/ws_cli_chat/comands.py
--rw-r--r--   0        0        0     2858 2023-04-24 21:21:06.167920 ws_cli_chat-0.4.2/ws_cli_chat/myconsole.py
--rw-r--r--   0        0        0      775 2023-04-23 22:38:40.265970 ws_cli_chat-0.4.2/ws_cli_chat/render.py
--rw-r--r--   0        0        0     2146 1970-01-01 00:00:00.000000 ws_cli_chat-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0      590 2023-04-29 00:30:56.175558 ws_cli_chat-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     1536 2023-04-28 07:32:18.000817 ws_cli_chat-0.4.3/README.md
+-rw-r--r--   0        0        0       43 2023-04-23 22:38:40.233412 ws_cli_chat-0.4.3/ws_cli_chat/__init__.py
+-rw-r--r--   0        0        0     6568 2023-04-28 07:07:21.887992 ws_cli_chat-0.4.3/ws_cli_chat/ascii_arts.py
+-rw-r--r--   0        0        0     3362 2023-04-28 07:23:29.148763 ws_cli_chat-0.4.3/ws_cli_chat/cli_chat.py
+-rw-r--r--   0        0        0      668 2023-04-29 00:30:38.341471 ws_cli_chat-0.4.3/ws_cli_chat/code_window.py
+-rw-r--r--   0        0        0     1213 2023-04-28 07:24:25.424801 ws_cli_chat-0.4.3/ws_cli_chat/comands.py
+-rw-r--r--   0        0        0     2858 2023-04-24 21:21:06.167920 ws_cli_chat-0.4.3/ws_cli_chat/myconsole.py
+-rw-r--r--   0        0        0      775 2023-04-23 22:38:40.265970 ws_cli_chat-0.4.3/ws_cli_chat/render.py
+-rw-r--r--   0        0        0     2146 1970-01-01 00:00:00.000000 ws_cli_chat-0.4.3/PKG-INFO
```

### Comparing `ws_cli_chat-0.4.2/pyproject.toml` & `ws_cli_chat-0.4.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ws_cli_chat"
-version = "0.4.2"
+version = "0.4.3"
 description = "simple cli-websocket chat"
 authors = ["__coelho__ <109885900+MikalROn@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{include = "ws_cli_chat"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `ws_cli_chat-0.4.2/README.md` & `ws_cli_chat-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `ws_cli_chat-0.4.2/ws_cli_chat/ascii_arts.py` & `ws_cli_chat-0.4.3/ws_cli_chat/ascii_arts.py`

 * *Files identical despite different names*

### Comparing `ws_cli_chat-0.4.2/ws_cli_chat/cli_chat.py` & `ws_cli_chat-0.4.3/ws_cli_chat/cli_chat.py`

 * *Files identical despite different names*

### Comparing `ws_cli_chat-0.4.2/ws_cli_chat/code_window.py` & `ws_cli_chat-0.4.3/ws_cli_chat/code_window.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 def run_code_window() -> None | str:
     loop = EventSimpleGUI()
     code_win = sg.Window(
         "Escreva o codigo",
         [
-            [sg.Text("puts your code here!" )],
+            [sg.Text("puts your code here!")],
             [sg.Multiline( k='code', expand_x=True, expand_y=True )],
             [sg.Button("send", expand_x=True, key='send'), sg.Button('close', key='send')]
         ], resizable=True
     )
     try:
         obj = loop.run_window(code_win, return_values=True, close_event='send')
         if obj:
```

### Comparing `ws_cli_chat-0.4.2/ws_cli_chat/comands.py` & `ws_cli_chat-0.4.3/ws_cli_chat/comands.py`

 * *Files identical despite different names*

### Comparing `ws_cli_chat-0.4.2/ws_cli_chat/myconsole.py` & `ws_cli_chat-0.4.3/ws_cli_chat/myconsole.py`

 * *Files identical despite different names*

### Comparing `ws_cli_chat-0.4.2/ws_cli_chat/render.py` & `ws_cli_chat-0.4.3/ws_cli_chat/render.py`

 * *Files identical despite different names*

### Comparing `ws_cli_chat-0.4.2/PKG-INFO` & `ws_cli_chat-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ws-cli-chat
-Version: 0.4.2
+Version: 0.4.3
 Summary: simple cli-websocket chat
 Author: __coelho__
 Author-email: 109885900+MikalROn@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

