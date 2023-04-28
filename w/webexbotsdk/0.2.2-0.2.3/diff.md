# Comparing `tmp/webexbotsdk-0.2.2.tar.gz` & `tmp/webexbotsdk-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webexbotsdk-0.2.2.tar", last modified: Fri Apr 28 20:56:38 2023, max compression
+gzip compressed data, was "webexbotsdk-0.2.3.tar", last modified: Fri Apr 28 21:31:40 2023, max compression
```

## Comparing `webexbotsdk-0.2.2.tar` & `webexbotsdk-0.2.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:56:38.819895 webexbotsdk-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-28 20:56:25.000000 webexbotsdk-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-28 20:56:25.000000 webexbotsdk-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-04-28 20:56:38.819895 webexbotsdk-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-04-28 20:56:25.000000 webexbotsdk-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-28 20:56:25.000000 webexbotsdk-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 20:56:38.819895 webexbotsdk-0.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:56:38.819895 webexbotsdk-0.2.2/webexbotsdk/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 20:56:25.000000 webexbotsdk-0.2.2/webexbotsdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:56:38.819895 webexbotsdk-0.2.2/webexbotsdk/teams/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-28 20:56:25.000000 webexbotsdk-0.2.2/webexbotsdk/teams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-04-28 20:56:25.000000 webexbotsdk-0.2.2/webexbotsdk/teams/bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-04-28 20:56:25.000000 webexbotsdk-0.2.2/webexbotsdk/teams/hook.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-28 20:56:25.000000 webexbotsdk-0.2.2/webexbotsdk/teams/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-28 20:56:25.000000 webexbotsdk-0.2.2/webexbotsdk/tinydb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:56:38.819895 webexbotsdk-0.2.2/webexbotsdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-04-28 20:56:38.000000 webexbotsdk-0.2.2/webexbotsdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-28 20:56:38.000000 webexbotsdk-0.2.2/webexbotsdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 20:56:38.000000 webexbotsdk-0.2.2/webexbotsdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-28 20:56:38.000000 webexbotsdk-0.2.2/webexbotsdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-28 20:56:38.000000 webexbotsdk-0.2.2/webexbotsdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:31:40.415064 webexbotsdk-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-28 21:31:21.000000 webexbotsdk-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-28 21:31:21.000000 webexbotsdk-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-04-28 21:31:40.415064 webexbotsdk-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-04-28 21:31:21.000000 webexbotsdk-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-28 21:31:21.000000 webexbotsdk-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 21:31:40.415064 webexbotsdk-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:31:40.411064 webexbotsdk-0.2.3/webexbotsdk/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 21:31:21.000000 webexbotsdk-0.2.3/webexbotsdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:31:40.415064 webexbotsdk-0.2.3/webexbotsdk/teams/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-28 21:31:21.000000 webexbotsdk-0.2.3/webexbotsdk/teams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-04-28 21:31:21.000000 webexbotsdk-0.2.3/webexbotsdk/teams/bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-04-28 21:31:21.000000 webexbotsdk-0.2.3/webexbotsdk/teams/hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-28 21:31:21.000000 webexbotsdk-0.2.3/webexbotsdk/teams/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-28 21:31:21.000000 webexbotsdk-0.2.3/webexbotsdk/tinydb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 21:31:40.411064 webexbotsdk-0.2.3/webexbotsdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-04-28 21:31:40.000000 webexbotsdk-0.2.3/webexbotsdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-28 21:31:40.000000 webexbotsdk-0.2.3/webexbotsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 21:31:40.000000 webexbotsdk-0.2.3/webexbotsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-28 21:31:40.000000 webexbotsdk-0.2.3/webexbotsdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-28 21:31:40.000000 webexbotsdk-0.2.3/webexbotsdk.egg-info/top_level.txt
```

### Comparing `webexbotsdk-0.2.2/LICENSE` & `webexbotsdk-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `webexbotsdk-0.2.2/PKG-INFO` & `webexbotsdk-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webexbotsdk
-Version: 0.2.2
+Version: 0.2.3
 Summary: Webex bot creation framework and tools
 License: The MIT License (MIT)
         
         Copyright (c) 2016-2020 Cisco and/or its affiliates.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `webexbotsdk-0.2.2/README.md` & `webexbotsdk-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `webexbotsdk-0.2.2/pyproject.toml` & `webexbotsdk-0.2.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "webexbotsdk"
 description = "Webex bot creation framework and tools"
-version = "0.2.2"
+version = "0.2.3"
 readme = "README.md"
 license = { file = "LICENSE" }
 classifiers = [
   "License :: OSI Approved :: MIT License",
   "Development Status :: 3 - Alpha",
   "Topic :: Communications :: Chat"
 ]
```

### Comparing `webexbotsdk-0.2.2/webexbotsdk/teams/bot.py` & `webexbotsdk-0.2.3/webexbotsdk/teams/bot.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from bottle import Bottle, request
 from webexteamssdk import WebexTeamsAPI, Webhook, Message, Person, Membership
 from webexteamssdk.models.cards import AdaptiveCard
-from pyngrok import ngrok
+from pyngrok import ngrok, conf, exception
 from typing import Literal, overload
-from re import Pattern
+from re import Pattern, sub
 from tinydb import TinyDB
 from tinydb.storages import JSONStorage
 import tinydb_encrypted_jsonstorage as tae
 from os.path import dirname, join
 from logging import Logger, basicConfig, getLogger, INFO
 import json
 
@@ -52,15 +52,15 @@
   "botName": "mywebexbot",
   "encryptDb": false
 }
 ```
 - `ngrokAuthToken` not recommended
     '''
     if isinstance(config, str):
-      with open(join(dirname(__file__), 'config.json')) as f:
+      with open(config) as f:
         config = json.loads(f.read())
         return self.setup(config)
       
     if config:
       self.config.update(config)
     botAccessToken:str|None = get_config_value(self.config, 'botAccessToken')
     ngrokAuthToken:str|Literal[False] = get_config_value(self.config, 'ngrokAuthToken', False)
@@ -88,17 +88,20 @@
 
   def run(self):
     port = get_config_value(self.config, 'port', 8080)
     botName = get_config_value(self.config, 'botName', 'mywebexbot')
     # Set up ngrok tunnel
     for tunnel in ngrok.get_tunnels():
       if botName in tunnel.public_url:
-        ngrok.disconnect(tunnel.public_url)
-    tunnel:ngrok.NgrokTunnel = ngrok.connect(port, 'http')
-    public_url = tunnel.public_url.replace('http', 'https')
+        try:
+          ngrok.disconnect(tunnel.public_url)
+        except exception.PyngrokNgrokHTTPError as e:
+          self.log.error(f"Could not close tunnel: {e.message}")
+    tunnel:ngrok.NgrokTunnel = ngrok.connect(port)
+    public_url = sub(r'https?', 'https', tunnel.public_url)
     # Init webex api
     for webhook in self.api.webhooks.list():
       self.api.webhooks.delete(webhookId=webhook.id)
     self.webhook = self.api.webhooks.create("bot_webhook_events", f"{public_url}/{botName}/events", WebhookResource.ALL.value, WebhookEvent.ALL.value)
     self.webhook = self.api.webhooks.create("bot_webhook_aa", f"{public_url}/{botName}/attachmentActions", WebhookResource.ATTACHMENT_ACTIONS.value, WebhookEvent.ALL.value)
     # Start server
     def callback(*args, **kwargs):
```

### Comparing `webexbotsdk-0.2.2/webexbotsdk/teams/hook.py` & `webexbotsdk-0.2.3/webexbotsdk/teams/hook.py`

 * *Files identical despite different names*

### Comparing `webexbotsdk-0.2.2/webexbotsdk.egg-info/PKG-INFO` & `webexbotsdk-0.2.3/webexbotsdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webexbotsdk
-Version: 0.2.2
+Version: 0.2.3
 Summary: Webex bot creation framework and tools
 License: The MIT License (MIT)
         
         Copyright (c) 2016-2020 Cisco and/or its affiliates.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

