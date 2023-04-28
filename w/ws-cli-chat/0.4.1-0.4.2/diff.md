# Comparing `tmp/ws_cli_chat-0.4.1.tar.gz` & `tmp/ws_cli_chat-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ws_cli_chat-0.4.1.tar", max compression
+gzip compressed data, was "ws_cli_chat-0.4.2.tar", max compression
```

## Comparing `ws_cli_chat-0.4.1.tar` & `ws_cli_chat-0.4.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      597 2023-04-28 07:25:17.452873 ws_cli_chat-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     1560 2023-04-22 08:02:07.727156 ws_cli_chat-0.4.1/README.md
--rw-r--r--   0        0        0       43 2023-04-23 22:38:40.233412 ws_cli_chat-0.4.1/ws_cli_chat/__init__.py
--rw-r--r--   0        0        0     6568 2023-04-28 07:07:21.887992 ws_cli_chat-0.4.1/ws_cli_chat/ascii_arts.py
--rw-r--r--   0        0        0     3362 2023-04-28 07:23:29.148763 ws_cli_chat-0.4.1/ws_cli_chat/cli_chat.py
--rw-r--r--   0        0        0      669 2023-04-28 02:13:50.537740 ws_cli_chat-0.4.1/ws_cli_chat/code_window.py
--rw-r--r--   0        0        0     1213 2023-04-28 07:24:25.424801 ws_cli_chat-0.4.1/ws_cli_chat/comands.py
--rw-r--r--   0        0        0     2858 2023-04-24 21:21:06.167920 ws_cli_chat-0.4.1/ws_cli_chat/myconsole.py
--rw-r--r--   0        0        0      775 2023-04-23 22:38:40.265970 ws_cli_chat-0.4.1/ws_cli_chat/render.py
--rw-r--r--   0        0        0     2177 1970-01-01 00:00:00.000000 ws_cli_chat-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0      590 2023-04-28 07:38:30.354352 ws_cli_chat-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     1536 2023-04-28 07:32:18.000817 ws_cli_chat-0.4.2/README.md
+-rw-r--r--   0        0        0       43 2023-04-23 22:38:40.233412 ws_cli_chat-0.4.2/ws_cli_chat/__init__.py
+-rw-r--r--   0        0        0     6568 2023-04-28 07:07:21.887992 ws_cli_chat-0.4.2/ws_cli_chat/ascii_arts.py
+-rw-r--r--   0        0        0     3362 2023-04-28 07:23:29.148763 ws_cli_chat-0.4.2/ws_cli_chat/cli_chat.py
+-rw-r--r--   0        0        0      669 2023-04-28 02:13:50.537740 ws_cli_chat-0.4.2/ws_cli_chat/code_window.py
+-rw-r--r--   0        0        0     1213 2023-04-28 07:24:25.424801 ws_cli_chat-0.4.2/ws_cli_chat/comands.py
+-rw-r--r--   0        0        0     2858 2023-04-24 21:21:06.167920 ws_cli_chat-0.4.2/ws_cli_chat/myconsole.py
+-rw-r--r--   0        0        0      775 2023-04-23 22:38:40.265970 ws_cli_chat-0.4.2/ws_cli_chat/render.py
+-rw-r--r--   0        0        0     2146 1970-01-01 00:00:00.000000 ws_cli_chat-0.4.2/PKG-INFO
```

### Comparing `ws_cli_chat-0.4.1/pyproject.toml` & `ws_cli_chat-0.4.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "ws_cli_chat"
-version = "0.4.1"
-description = "simple cli-websocket-ws-cli-chat"
+version = "0.4.2"
+description = "simple cli-websocket chat"
 authors = ["__coelho__ <109885900+MikalROn@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{include = "ws_cli_chat"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 typer = {extras = ["all"], version = "^0.7.0"}
```

### Comparing `ws_cli_chat-0.4.1/README.md` & `ws_cli_chat-0.4.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # Chat Application
 This is a command-line chat application built with Python that allows users to connect to a websocket server and chat with other users in real-time.
 
 # Requirements
 - Python 3.7+
 - websockets library
 - asyncio library
+- PySimpleGUI
 
 # Installation
-To install the required libraries, run the following command in your terminal:
+To install run the following command in your terminal:
 ````shell
-pip install websockets
+pip install ws-cli-chat
 ````
 Usage
 To start the application, run the following command in your terminal:
 
 ````shell
-python ws_cli_chat
+chat
 ````
-
 You will be prompted to choose a username. After entering your username, the application will connect to the websocket server and you will be able to chat with other users in real-time.
 
 To send a message, simply type your message and hit enter. Your message will be sent to all other users currently connected to the chat room.
 
 # Features
 - Real-time messaging: Messages are sent and received in real-time, allowing for seamless communication between users.
 - Multiple users: The chat room can accommodate multiple users at the same time, allowing for group conversations.
```

### Comparing `ws_cli_chat-0.4.1/ws_cli_chat/ascii_arts.py` & `ws_cli_chat-0.4.2/ws_cli_chat/ascii_arts.py`

 * *Files identical despite different names*

### Comparing `ws_cli_chat-0.4.1/ws_cli_chat/cli_chat.py` & `ws_cli_chat-0.4.2/ws_cli_chat/cli_chat.py`

 * *Files identical despite different names*

### Comparing `ws_cli_chat-0.4.1/ws_cli_chat/code_window.py` & `ws_cli_chat-0.4.2/ws_cli_chat/code_window.py`

 * *Files identical despite different names*

### Comparing `ws_cli_chat-0.4.1/ws_cli_chat/comands.py` & `ws_cli_chat-0.4.2/ws_cli_chat/comands.py`

 * *Files identical despite different names*

### Comparing `ws_cli_chat-0.4.1/ws_cli_chat/myconsole.py` & `ws_cli_chat-0.4.2/ws_cli_chat/myconsole.py`

 * *Files identical despite different names*

### Comparing `ws_cli_chat-0.4.1/ws_cli_chat/render.py` & `ws_cli_chat-0.4.2/ws_cli_chat/render.py`

 * *Files identical despite different names*

### Comparing `ws_cli_chat-0.4.1/PKG-INFO` & `ws_cli_chat-0.4.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ws-cli-chat
-Version: 0.4.1
-Summary: simple cli-websocket-ws-cli-chat
+Version: 0.4.2
+Summary: simple cli-websocket chat
 Author: __coelho__
 Author-email: 109885900+MikalROn@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
@@ -19,27 +19,27 @@
 # Chat Application
 This is a command-line chat application built with Python that allows users to connect to a websocket server and chat with other users in real-time.
 
 # Requirements
 - Python 3.7+
 - websockets library
 - asyncio library
+- PySimpleGUI
 
 # Installation
-To install the required libraries, run the following command in your terminal:
+To install run the following command in your terminal:
 ````shell
-pip install websockets
+pip install ws-cli-chat
 ````
 Usage
 To start the application, run the following command in your terminal:
 
 ````shell
-python ws_cli_chat
+chat
 ````
-
 You will be prompted to choose a username. After entering your username, the application will connect to the websocket server and you will be able to chat with other users in real-time.
 
 To send a message, simply type your message and hit enter. Your message will be sent to all other users currently connected to the chat room.
 
 # Features
 - Real-time messaging: Messages are sent and received in real-time, allowing for seamless communication between users.
 - Multiple users: The chat room can accommodate multiple users at the same time, allowing for group conversations.
```

