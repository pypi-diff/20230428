# Comparing `tmp/selfcord.py-0.1.0.tar.gz` & `tmp/selfcord.py-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selfcord.py-0.1.0.tar", last modified: Sun Apr 23 01:45:09 2023, max compression
+gzip compressed data, was "selfcord.py-0.1.1.tar", last modified: Fri Apr 28 16:33:46 2023, max compression
```

## Comparing `selfcord.py-0.1.0.tar` & `selfcord.py-0.1.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-04-23 01:45:09.386142 selfcord.py-0.1.0/
--rw-r--r--   0 shell     (1000) shell     (1001)     2338 2023-04-23 01:45:09.382809 selfcord.py-0.1.0/PKG-INFO
--rw-r--r--   0 shell     (1000) shell     (1001)     2051 2023-04-23 01:42:38.000000 selfcord.py-0.1.0/README.md
-drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-04-23 01:45:09.369475 selfcord.py-0.1.0/selfcord/
--rw-r--r--   0 shell     (1000) shell     (1001)       82 2022-11-11 20:03:04.000000 selfcord.py-0.1.0/selfcord/__init__.py
-drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-04-23 01:45:09.376142 selfcord.py-0.1.0/selfcord/api/
--rw-r--r--   0 shell     (1000) shell     (1001)      127 2022-11-11 20:02:32.000000 selfcord.py-0.1.0/selfcord/api/__init__.py
--rw-r--r--   0 shell     (1000) shell     (1001)      527 2022-11-11 01:44:22.000000 selfcord.py-0.1.0/selfcord/api/errors.py
--rw-r--r--   0 shell     (1000) shell     (1001)     7821 2023-04-22 21:54:23.000000 selfcord.py-0.1.0/selfcord/api/events.py
--rw-r--r--   0 shell     (1000) shell     (1001)    14248 2023-04-22 21:54:23.000000 selfcord.py-0.1.0/selfcord/api/gateway.py
--rw-r--r--   0 shell     (1000) shell     (1001)     7729 2023-04-21 02:29:42.000000 selfcord.py-0.1.0/selfcord/api/http.py
--rw-r--r--   0 shell     (1000) shell     (1001)    12960 2023-04-23 01:18:18.000000 selfcord.py-0.1.0/selfcord/bot.py
-drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-04-23 01:45:09.382809 selfcord.py-0.1.0/selfcord/models/
--rw-r--r--   0 shell     (1000) shell     (1001)      412 2022-11-21 22:16:05.000000 selfcord.py-0.1.0/selfcord/models/__init__.py
--rw-r--r--   0 shell     (1000) shell     (1001)    13535 2023-04-21 02:29:42.000000 selfcord.py-0.1.0/selfcord/models/channel.py
--rw-r--r--   0 shell     (1000) shell     (1001)      902 2022-11-21 18:38:16.000000 selfcord.py-0.1.0/selfcord/models/client.py
--rw-r--r--   0 shell     (1000) shell     (1001)      697 2022-10-31 21:14:11.000000 selfcord.py-0.1.0/selfcord/models/emoji.py
--rw-r--r--   0 shell     (1000) shell     (1001)     5149 2022-11-21 17:56:07.000000 selfcord.py-0.1.0/selfcord/models/guild.py
--rw-r--r--   0 shell     (1000) shell     (1001)      783 2022-11-21 18:38:32.000000 selfcord.py-0.1.0/selfcord/models/member.py
--rw-r--r--   0 shell     (1000) shell     (1001)     1558 2022-11-17 17:14:15.000000 selfcord.py-0.1.0/selfcord/models/message.py
--rw-r--r--   0 shell     (1000) shell     (1001)     2125 2022-10-18 15:17:31.000000 selfcord.py-0.1.0/selfcord/models/permission.py
--rw-r--r--   0 shell     (1000) shell     (1001)     1360 2022-11-22 16:33:43.000000 selfcord.py-0.1.0/selfcord/models/role.py
--rw-r--r--   0 shell     (1000) shell     (1001)     3024 2023-04-21 02:29:42.000000 selfcord.py-0.1.0/selfcord/models/user.py
--rw-r--r--   0 shell     (1000) shell     (1001)      999 2022-10-25 00:32:59.000000 selfcord.py-0.1.0/selfcord/models/webhook.py
-drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-04-23 01:45:09.382809 selfcord.py-0.1.0/selfcord/utils/
--rw-r--r--   0 shell     (1000) shell     (1001)      150 2022-11-27 03:03:09.000000 selfcord.py-0.1.0/selfcord/utils/__init__.py
--rw-r--r--   0 shell     (1000) shell     (1001)    12830 2023-04-23 01:21:27.000000 selfcord.py-0.1.0/selfcord/utils/command.py
-drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-04-23 01:45:09.372808 selfcord.py-0.1.0/selfcord.py.egg-info/
--rw-r--r--   0 shell     (1000) shell     (1001)     2338 2023-04-23 01:45:09.000000 selfcord.py-0.1.0/selfcord.py.egg-info/PKG-INFO
--rw-r--r--   0 shell     (1000) shell     (1001)      710 2023-04-23 01:45:09.000000 selfcord.py-0.1.0/selfcord.py.egg-info/SOURCES.txt
--rw-r--r--   0 shell     (1000) shell     (1001)        1 2023-04-23 01:45:09.000000 selfcord.py-0.1.0/selfcord.py.egg-info/dependency_links.txt
--rw-r--r--   0 shell     (1000) shell     (1001)       75 2023-04-23 01:45:09.000000 selfcord.py-0.1.0/selfcord.py.egg-info/requires.txt
--rw-r--r--   0 shell     (1000) shell     (1001)        9 2023-04-23 01:45:09.000000 selfcord.py-0.1.0/selfcord.py.egg-info/top_level.txt
--rw-r--r--   0 shell     (1000) shell     (1001)       38 2023-04-23 01:45:09.386142 selfcord.py-0.1.0/setup.cfg
--rw-r--r--   0 shell     (1000) shell     (1001)     1016 2023-04-23 01:44:56.000000 selfcord.py-0.1.0/setup.py
-drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-04-23 01:45:09.382809 selfcord.py-0.1.0/tests/
--rw-r--r--   0 shell     (1000) shell     (1001)      475 2022-10-24 15:21:37.000000 selfcord.py-0.1.0/tests/test_commands.py
+drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-04-28 16:33:46.158062 selfcord.py-0.1.1/
+-rw-r--r--   0 shell     (1000) shell     (1001)     2546 2023-04-28 16:33:46.158062 selfcord.py-0.1.1/PKG-INFO
+-rw-r--r--   0 shell     (1000) shell     (1001)     2259 2023-04-24 19:11:53.000000 selfcord.py-0.1.1/README.md
+drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-04-28 16:33:46.134728 selfcord.py-0.1.1/selfcord/
+-rw-r--r--   0 shell     (1000) shell     (1001)       82 2022-11-11 20:03:04.000000 selfcord.py-0.1.1/selfcord/__init__.py
+drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-04-28 16:33:46.144728 selfcord.py-0.1.1/selfcord/api/
+-rw-r--r--   0 shell     (1000) shell     (1001)      127 2022-11-11 20:02:32.000000 selfcord.py-0.1.1/selfcord/api/__init__.py
+-rw-r--r--   0 shell     (1000) shell     (1001)      527 2022-11-11 01:44:22.000000 selfcord.py-0.1.1/selfcord/api/errors.py
+-rw-r--r--   0 shell     (1000) shell     (1001)     9183 2023-04-27 18:19:43.000000 selfcord.py-0.1.1/selfcord/api/events.py
+-rw-r--r--   0 shell     (1000) shell     (1001)    16788 2023-04-27 16:47:37.000000 selfcord.py-0.1.1/selfcord/api/gateway.py
+-rw-r--r--   0 shell     (1000) shell     (1001)     7975 2023-04-27 16:53:31.000000 selfcord.py-0.1.1/selfcord/api/http.py
+-rw-r--r--   0 shell     (1000) shell     (1001)    17139 2023-04-28 02:03:57.000000 selfcord.py-0.1.1/selfcord/bot.py
+drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-04-28 16:33:46.154729 selfcord.py-0.1.1/selfcord/models/
+-rw-r--r--   0 shell     (1000) shell     (1001)      412 2022-11-21 22:16:05.000000 selfcord.py-0.1.1/selfcord/models/__init__.py
+-rw-r--r--   0 shell     (1000) shell     (1001)    16434 2023-04-27 15:34:03.000000 selfcord.py-0.1.1/selfcord/models/channel.py
+-rw-r--r--   0 shell     (1000) shell     (1001)     1052 2023-04-27 15:34:24.000000 selfcord.py-0.1.1/selfcord/models/client.py
+-rw-r--r--   0 shell     (1000) shell     (1001)      901 2023-04-27 15:34:29.000000 selfcord.py-0.1.1/selfcord/models/emoji.py
+-rw-r--r--   0 shell     (1000) shell     (1001)     7323 2023-04-28 16:04:21.000000 selfcord.py-0.1.1/selfcord/models/guild.py
+-rw-r--r--   0 shell     (1000) shell     (1001)      933 2023-04-27 15:34:49.000000 selfcord.py-0.1.1/selfcord/models/member.py
+-rw-r--r--   0 shell     (1000) shell     (1001)     1868 2023-04-27 15:35:44.000000 selfcord.py-0.1.1/selfcord/models/message.py
+-rw-r--r--   0 shell     (1000) shell     (1001)     2130 2023-04-27 15:35:57.000000 selfcord.py-0.1.1/selfcord/models/permission.py
+-rw-r--r--   0 shell     (1000) shell     (1001)     1556 2023-04-27 15:36:19.000000 selfcord.py-0.1.1/selfcord/models/role.py
+-rw-r--r--   0 shell     (1000) shell     (1001)     3898 2023-04-27 19:15:13.000000 selfcord.py-0.1.1/selfcord/models/user.py
+-rw-r--r--   0 shell     (1000) shell     (1001)     1331 2023-04-27 15:44:13.000000 selfcord.py-0.1.1/selfcord/models/webhook.py
+drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-04-28 16:33:46.158062 selfcord.py-0.1.1/selfcord/utils/
+-rw-r--r--   0 shell     (1000) shell     (1001)      150 2022-11-27 03:03:09.000000 selfcord.py-0.1.1/selfcord/utils/__init__.py
+-rw-r--r--   0 shell     (1000) shell     (1001)    15277 2023-04-27 16:27:44.000000 selfcord.py-0.1.1/selfcord/utils/command.py
+drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-04-28 16:33:46.138062 selfcord.py-0.1.1/selfcord.py.egg-info/
+-rw-r--r--   0 shell     (1000) shell     (1001)     2546 2023-04-28 16:33:46.000000 selfcord.py-0.1.1/selfcord.py.egg-info/PKG-INFO
+-rw-r--r--   0 shell     (1000) shell     (1001)      710 2023-04-28 16:33:46.000000 selfcord.py-0.1.1/selfcord.py.egg-info/SOURCES.txt
+-rw-r--r--   0 shell     (1000) shell     (1001)        1 2023-04-28 16:33:46.000000 selfcord.py-0.1.1/selfcord.py.egg-info/dependency_links.txt
+-rw-r--r--   0 shell     (1000) shell     (1001)       65 2023-04-28 16:33:46.000000 selfcord.py-0.1.1/selfcord.py.egg-info/requires.txt
+-rw-r--r--   0 shell     (1000) shell     (1001)        9 2023-04-28 16:33:46.000000 selfcord.py-0.1.1/selfcord.py.egg-info/top_level.txt
+-rw-r--r--   0 shell     (1000) shell     (1001)       38 2023-04-28 16:33:46.158062 selfcord.py-0.1.1/setup.cfg
+-rw-r--r--   0 shell     (1000) shell     (1001)     1004 2023-04-28 16:33:05.000000 selfcord.py-0.1.1/setup.py
+drwxr-xr-x   0 shell     (1000) shell     (1001)        0 2023-04-28 16:33:46.158062 selfcord.py-0.1.1/tests/
+-rw-r--r--   0 shell     (1000) shell     (1001)      455 2023-04-27 00:48:03.000000 selfcord.py-0.1.1/tests/test_commands.py
```

### Comparing `selfcord.py-0.1.0/PKG-INFO` & `selfcord.py-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: selfcord.py
-Version: 0.1.0
-Summary: A Discord API wrapper designed for selfbots!
-Home-page: https://github.com/Shell1010/Selfcord
-Author: Shell of OMEGA
-License: MIT
-Keywords: selfbot,discord,discordapi,discordwrapper
-Description-Content-Type: text/markdown
-
 # Selfcord
 A discord selfbot API wrapper (WIP)
 
 ## Installation
 
 Run this in the command line.
 ```
@@ -20,14 +10,20 @@
 
 ## Wiki
 
 Read our [Wiki](https://github.com/Shell1010/Selfcord/wiki) in regards to documentation and getting started.
 
 ## Examples
 
+### Aeterna Selfbot
+
+A simple selfbot designed to showcase the library's features, intended to be seen as a template or base for other users.
+
+[Aeterna Selfbot](https://github.com/Shell1010/Aeterna-Selfbot)
+
 ### Message logger
 ```python
 import selfcord
 
 token = "insert token"
 bot = selfcord.Bot(prefixes=["!", "?"])
```

### Comparing `selfcord.py-0.1.0/README.md` & `selfcord.py-0.1.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: selfcord.py
+Version: 0.1.1
+Summary: A Discord API wrapper designed for selfbots!
+Home-page: https://github.com/Shell1010/Selfcord
+Author: Shell of OMEGA
+License: MIT
+Keywords: selfbot,discord,discordapi,discordwrapper
+Description-Content-Type: text/markdown
+
 # Selfcord
 A discord selfbot API wrapper (WIP)
 
 ## Installation
 
 Run this in the command line.
 ```
@@ -10,14 +20,20 @@
 
 ## Wiki
 
 Read our [Wiki](https://github.com/Shell1010/Selfcord/wiki) in regards to documentation and getting started.
 
 ## Examples
 
+### Aeterna Selfbot
+
+A simple selfbot designed to showcase the library's features, intended to be seen as a template or base for other users.
+
+[Aeterna Selfbot](https://github.com/Shell1010/Aeterna-Selfbot)
+
 ### Message logger
 ```python
 import selfcord
 
 token = "insert token"
 bot = selfcord.Bot(prefixes=["!", "?"])
```

### Comparing `selfcord.py-0.1.0/selfcord/api/errors.py` & `selfcord.py-0.1.1/selfcord/api/errors.py`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.0/selfcord/api/events.py` & `selfcord.py-0.1.1/selfcord/api/events.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,17 +9,22 @@
     Used to handle discord events
     '''
     def __init__(self, bot, http):
         self._events = {}
         self.http    = http
         self.bot     = bot
 
-    async def handle_ready(self, data, user: Client, http):
-        '''Handles the ready event, what is executed when it appears
-        '''
+    async def handle_ready(self, data: dict, user: Client, http):
+        """Handles what happens when the ready event is fired, when the bot first connects
+
+        Args:
+            data (dict): JSON data from gateway
+            user (Client): The client instance
+            http (http): HTTP instance
+        """
         self.user = user
         for relationship in data.get('relationships'):
             if relationship.get('type') == 1:
                 self.user.friends.append(User(relationship['user'], self.bot, http))
 
         for channel in data.get('private_channels'):
             if channel.get('type') == 1: self.user.private_channels.append(DMChannel(channel,self.bot, http))
@@ -27,42 +32,55 @@
 
         for guild in data.get('guilds'):
             await self.handle_guild_create(guild, self.user, http)
 
         # Sends data from ready to the event handler in main.py (if it exists)
         await self.bot.emit('ready', perf_counter() - self.bot.t1)
 
-    async def handle_guild_create(self, data, user: Client, http):
-        '''
-        Handles what happens when a guild is created
-        '''
+    async def handle_guild_create(self, data: dict, user: Client, http):
+        """Handles what happens when a guild is created
+
+        Args:
+            data (dict): JSON data from gateway
+            user (Client): The client instance
+            http (http): HTTP instance
+        """
         self.user = user
         guild = Guild(data, self.bot, http)
         self.user.guilds.append(guild)
 
         # Sends data from ready to the event handler in main.py (if it exists)
         await self.bot.emit('guild_create', guild)
 
-    async def handle_message_create(self, data, user: Client, http):
-        '''Handles what happens when a message is created
-        '''
+    async def handle_message_create(self, data: dict, user: Client, http):
+        """Handles what happens when a message is created, or sent
+        Args:
+            data (dict): JSON data from gateway
+            user (Client): The client instance
+            http (http): HTTP instance
+        """
         self.user = user
         message = Message(data, self.bot, http)
         self.user.messages.append(message)
 
         # Sends data from ready to the event handler in main.py (if it exists)
         await self.bot.emit('message', message)
         if message.author.id == self.bot.user.id:
             for prefix in self.bot.prefixes:
                 # Attempts to invoke the command if has prefix and from the user
                 if message.content.startswith(prefix): await self.bot.process_commands(message)
 
-    async def handle_message_delete(self, data, user: Client, http):
-        '''Handles what happens when a message is created. Disclaimer: Only guild id, message id and channel id will be present if the message is not in bots cache.
-        '''
+    async def handle_message_delete(self, data: dict, user: Client, http):
+        """Handles what happens when a message is deleted. Very little data will be logged if the message is not in the bots cache.
+
+        Args:
+            data (dict): JSON data from gateway
+            user (Client): The client instance
+            http (http): HTTP instance
+        """
         self.user = user
         id =data.get('id')
         for message in self.user.messages:
             if message.id == id:
                 await self.bot.emit('message_delete', message)
                 self.user.deleted_messages.append(message)
                 self.user.messages.remove(message)
@@ -83,17 +101,22 @@
                     self.guild_id           = data.get('guild_id')
                     self.channel            = None
                     self.guild              = None
 
             message = deleted_message(data)
             await self.bot.emit('message_delete', message)
 
-    async def handle_channel_create(self, channel, user: Client, http):
-        '''Handles what happens when a channel is created
-        '''
+    async def handle_channel_create(self, channel: dict, user: Client, http):
+        """Handles what happens when a channel is created
+
+        Args:
+            channel (dict): JSON data from gateway
+            user (Client): The client instance
+            http (http): HTTP instance
+        """
         self.user = user
         if channel.get('type') == 0:
             id = channel.get('guild_id')
             for guild in self.user.guilds:
                 if guild.id == id:
                     channel = TextChannel(channel, self.bot, self.http)
                     guild.channels.append(channel)
@@ -115,33 +138,43 @@
                 if guild.id == id:
                     channel = TextChannel(channel, self.bot, self.http)
                     guild.channels.append(channel)
 
         # Sends data from ready to the event handler in main.py (if it exists)
         await self.bot.emit('channel_create', channel)
 
-    async def handle_guild_member_list_update(self, data, user: Client, http):
-        '''Handles what happens when member chunk payload is sent via gateway
-        '''
+    async def handle_guild_member_list_update(self, data: dict, user: Client, http):
+        """Handles what happens when a member chunk payload is received
+
+        Args:
+            data (dict): JSON data from gateway
+            user (Client): The client instance
+            http (http): HTTP instance
+        """
         members   = []
         self.user = user
 
         try:
             for item in data['ops'][0]['items']:
                 try: members.append(User(item['member']['user'], self.bot, http))
                 except: continue
 
             await self.bot.emit('member_chunk', members)
         except: pass
 
 
 
     async def handle_channel_delete(self, data, user: Client, http):
-        '''Handles what happens when a channel is deleted
-        '''
+        """Handles what happens when a channel is deleted
+
+        Args:
+            data (dict): JSON data from gateway
+            user (Client): The client instance
+            http (http): HTTP instance
+        """
         self.user = user
         id = data.get('id')
         for channel in self.user.private_channels:
             if channel.id == id:
                 await self.bot.emit('channel_delete', channel)
                 self.user.private_channels.remove(channel)
                 return
@@ -161,28 +194,38 @@
                     if channel.id == id:
                         await self.bot.emit('channel_delete', channel)
                         guild.channels.remove(channel)
                         return
 
 
     async def handle_guild_role_create(self, role, user: Client, http):
-        '''Handles what happens when a role is created
-        '''
+        """Handles what happens when a role is created
+
+        Args:
+            data (dict): JSON data from gateway
+            user (Client): The client instance
+            http (http): HTTP instance
+        """
         self.user = user
 
         for guild in self.user.guilds:
             if role.get('guild_id') == guild.id:
                 role = Role(role, self.http, guild_id=guild.id)
                 guild.roles.append(role)
 
         await self.bot.emit('role_create', role)
 
     async def handle_guild_role_delete(self, role, user: Client, http):
-        '''Handles what happens when a role is deleted
-        '''
+        """Handles what happens when a role is deleted
+
+        Args:
+            data (dict): JSON data from gateway
+            user (Client): The client instance
+            http (http): HTTP instance
+        """
         self.user = user
 
         for guild in self.user.guilds:
             if role.get('guild_id') == guild.id:
                 for role in guild.roles:
                     if role.get('id') == role.id:
                         await self.bot.emit('role_delete', role)
```

### Comparing `selfcord.py-0.1.0/selfcord/api/http.py` & `selfcord.py-0.1.1/selfcord/api/http.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,14 +28,16 @@
         await self.get_cookie()
         self.token = token
         data = await self.request('get', '/users/@me')
         self.client = Client(data)
         return data
 
     async def get_cookie(self):
+        """Gather cookie for user upon client start
+        """
         async with aiohttp.ClientSession() as session:
             async with session.get('https://discord.com', headers={'user-agent': 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) discord/0.0.139 Chrome/91.0.4472.164 Electron/13.6.6 Safari/537.36'}) as resp:
                 dcf = resp.headers['set-cookie'].split('__dcfduid=')[0].split(';')[0]
                 sdc = resp.headers['set-cookie'].split('__sdcfduid=')[0].split(';')[0]
                 cfr = resp.headers['set-cookie'].split('__cfruid=')[0].split(';')[0]
 
                 self.cookies['dcf'] = self.cookies.get('dcf') if dcf != "" else ""
@@ -141,15 +143,23 @@
         except: pass
 
         try:
             return data
         except:
             return None
 
-    async def encode_image(self, url):
+    async def encode_image(self, url: str) -> str:
+        """Turn an image url into a b64 payload
+
+        Args:
+            url (str): The URL of the image
+
+        Returns:
+            str: The b64 payload
+        """
         async with ClientSession() as session:
             async with session.get(f'{url}') as resp:
                 image = b64encode(await resp.read())
                 newobj = str(image).split('"', 2)
 
         return f'data:image/png;base64,{newobj[1]}'
```

### Comparing `selfcord.py-0.1.0/selfcord/bot.py` & `selfcord.py-0.1.1/selfcord/bot.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from .utils import Command, CommandCollection, Context, ExtensionCollection, Extension, Event
 import random
 import contextlib
 from traceback import format_exception
 import io
 from functools import partial
 import importlib
+import aiohttp
 
 
 class Bot:
     def __init__(self, show_beat: bool = False, prefixes: list = ["s!"], inbuilt_help=True) -> None:
         self.inbuilt_help= inbuilt_help
         self.show_beat = show_beat
         self.token = None
@@ -57,56 +58,96 @@
     async def inbuilt_commands(self):
         """
         I call this on bot initialisation, it's the inbuilt help command
         """
         if self.inbuilt_help:
             @self.cmd("The help command!", aliases=["test"])
             async def help(ctx, cat=None):
+                """The help command, dedicated to viewing all commands, extensions and information regarding commands.
+                """
                 if cat is None:
-                    msg = f"```diff\n"
-                    msg += f"+ {self.user} selfbot\n+ Prefixes:   {self.prefixes}\n\n"
-                    msg += f"- Commands\n"
-                    for ext in self.extensions:
-                        msg += f"- Ext {ext.name}: {ext.description}\n"
+                    msg = f"```ini\n[ {self.user.name} Selfbot ]\n"
+                    msg += f"[ {self.user} ]\nType <prefix>help <ext_name> to view commands relating to a specific extension. Type <prefix>help <cmd_name> to view information regarding a command.\n[ .Prefixes ] : {self.prefixes}\n\n"
+                    msg += f"[ .Commands ]\n"
                     for command in self.commands:
-                        msg += f"- {command.name}:    {command.description}\n"
+                        msg += f". {command.name}: {command.description}\n"
+                    msg += "\n[ .Extensions ]\n"
+                    for ext in self.extensions:
+                        msg += f"[ {ext.name} ] : [ {ext.description} ]\n"
 
-                        if len(msg) > 1980:
-                            msg += f"```"
                     msg += f"```"
                     return await ctx.reply(f"{msg}")
 
                 else:
                     name = cat.lower()
                     for ext in self.extensions:
                         if name == ext.name.lower():
-                            msg = f"```diff\n"
-                            msg += f"+ {self.user} selfbot\n+ Prefixes:   {self.prefixes}\n\n"
-                            msg += f"- {ext.name} Commands\n"
-
+                            msg = f"```ini\n[ {self.user.name} Selfbot ]\n"
+                            msg += f"[ {self.user} ]\n\nType <prefix>help <ext_name> to view commands relating to a specific extension. Type <prefix>help <cmd_name> to view information regarding a command.\n\n[ .Prefixes ] : {self.prefixes}\n\n"
+                            msg += f"[ .Commands ]\n"
                             for command in ext.commands:
-
                                 if command.ext == ext.ext:
-                                    msg += f"- {command.name}:    {command.description}\n"
+                                    msg += f". {command.name}: {command.description}\n"
 
                             msg += f"```"
                             return await ctx.reply(f"{msg}")
+                    else:
+                        for cmd in self.commands:
+                            if name == cmd.name.lower():
+                                msg = f"```ini\n[ {self.user.name} Selfbot ]\n"
+                                msg += f"[ {self.user} ]\n\nType <prefix>help <ext_name> to view commands relating to a specific extension. Type <prefix>help <cmd_name> to view information regarding a command.\n\n[ .Prefixes ] : {self.prefixes}\n\n"
+                                msg += f"[ .{cmd.name} ]\n"
+                                msg += f"[ Description ] :  {cmd.description} \n"
+                                msg += f"[ Long Description ] :\n{cmd.func.__doc__}\n"
+                                msg += f"[ Aliases ] : {cmd.aliases} \n"
+                                args = inspect.signature(cmd.func)
+                                msg += f"\n[ Example Usage ] :\n[ {self.prefixes[0]}{cmd.aliases[0]}"
+                                for arg in args.parameters.keys():
+                                    if arg == "self" or arg == "ctx":
+                                        continue
+                                    msg += f" <{arg}>"
+                                msg += f" ]"
+
+                                msg += f"```"
+                                return await ctx.reply(f"{msg}")
+                        for ext in self.extensions:
+                            for cmd in ext.commands:
+                                if name == cmd.name.lower():
+                                    msg = f"```ini\n[ {self.user.name} Selfbot ]\n"
+                                    msg += f"[ {self.user} ]\n\nType <prefix>help <ext_name> to view commands relating to a specific extension. Type <prefix>help <cmd_name> to view information regarding a command.\n\n[ .Prefixes ] : {self.prefixes}\n\n"
+                                    msg += f"[ .{cmd.name} ]\n"
+                                    msg += f"[ Description ] :  {cmd.description} \n"
+                                    msg += f"[ Long Description ] :\n{cmd.func.__doc__}\n"
+                                    msg += f"[ Aliases ] :  {cmd.aliases} \n"
+                                    args = inspect.signature(cmd.func)
+                                    msg += f"\n[ Example Usage ] :\n[ {self.prefixes[0]}{cmd.aliases[0]}"
+                                    for arg in args.parameters.keys():
+                                        if arg == "self" or arg == "ctx":
+                                            continue
+                                        msg += f" <{arg}>"
+                                    msg += f" ]"
+
+
+                                    msg += f"```"
+                                    return await ctx.reply(f"{msg}")
 
 
 
 
 
         def clean_code(content):
             if content.startswith("```") and content.endswith("```"):
                 return "\n".join(content.split("\n")[1:])[:-3]
             else:
                 return content
 
-        @self.cmd(description="Evaluates and runs code", aliases=['exec'])
+        @self.cmd(description="Executes and runs code", aliases=['exec'])
         async def eval(ctx, *, code: str):
+            """Runs python code via exec, intended for experienced usage. This can be DANGEROUS if you do not know what you are doing, use with caution.
+            """
             code = clean_code(code)
 
             try:
                 with contextlib.redirect_stdout(io.StringIO()) as f:
                     await aexec(code)
                     result = f"```{f.getvalue()}\n```"
             except Exception as e:
@@ -151,15 +192,15 @@
             await getattr(self, on_event)(*args, **kwargs)
         if event in self._events.keys():
 
             for Event in self._events[event]:
 
                 if Event.coro.__code__.co_varnames[0] == "self":
 
-                    return asyncio.create_task(Event.coro(Event.ext, *args, **kwargs))
+                    asyncio.create_task(Event.coro(Event.ext, *args, **kwargs))
 
                 else:
 
                     asyncio.create_task(Event.coro(*args, **kwargs))
 
 
     def cmd(self, description="", aliases=[]):
@@ -241,20 +282,22 @@
             spec.loader.exec_module(lib)
         except Exception as e:
             raise ModuleNotFoundError(f"Spec could not be loaded {e}")
         try:
             ext = getattr(lib, 'Ext')
         except Exception as e:
             raise ModuleNotFoundError(f"Extension does not exist {e}")
+
+        # Creates an Extension - ext in this case refers to the Ext class used for initialisation
         ext = Extension(name=ext.name, description=ext.description, ext=ext(self), _events=ext._events)
         self.extensions.add(ext)
         try:
             for name, event in ext._events.items():
                 for ext_event in event:
-                    self._events[name].append(Event(name=name, coro=ext_event.coro, ext=ext_event.ext))
+                    self._events[name].append(Event(name=name, coro=ext_event.coro, ext=ext.ext))
 
 
 
         except Exception as e:
             error = "".join(format_exception(e, e, e.__traceback__))
             print(error)
 
@@ -375,15 +418,34 @@
         if recipient_id is not None:
             data = await self.http.request(method="post", endpoint="/users/@me/channels",
                                            json={"recipient_id": recipient_id})
             return DMChannel(data, bot=self, http=self.http)
         else:
             raise TypeError("Recipient ID not specified")
 
+    async def redeem_nitro(self, code: str):
+        """Helper function to redeem nitro
+
+        Args:
+            code (str): Nitro code
+        """
+        async with aiohttp.ClientSession() as session:
+            async with session.post(f"https://canary.discord.com/api/v9/entitlements/gift-codes/{code}/redeem", headers={"authorization": f"{self.token}", "user-agent": "Mozilla/5.0 (X11; Linux x86_64; rv:109.0) Gecko/20100101 Firefox/112.0", "content-type":"application/json"}, json={}) as resp:
+                j = await resp.json()
+                await aprint(j, resp.status)
+
+
+
+
     async def change_hypesquad(self, house: str):
+        """Helper function to change hypesquad
+
+        Args:
+            house (str): Hypesquad name
+        """
         if house.lower() == "bravery":
             await self.http.request(method="post", endpoint = "/hypesquad/online", json = {"house_id": 1})
         if house.lower() == "brilliance":
             await self.http.request(method="post", endpoint = "/hypesquad/online", json = {"house_id": 2})
         if house.lower() == "balance":
             await self.http.request(method="post", endpoint = "/hypesquad/online", json = {"house_id": 3})
```

### Comparing `selfcord.py-0.1.0/selfcord/models/channel.py` & `selfcord.py-0.1.1/selfcord/models/channel.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,20 +8,22 @@
 
 
 
 
 
 
 class Messageable:
+    """Parent class specific for those classes that include a textchat for sending messages.
+    """
     def __init__(self, http, bot) -> None:
         self.http = http
         self.bot = bot
 
 
-    async def history(self):
+    async def history(self) -> list[Message]:
         """
         Get channel message history.
 
         Args:
             No arguments required
 
         Returns:
@@ -38,15 +40,15 @@
                 for msg in data:
                     messages.append(Message(msg, self.bot, self.http))
             else:
                 break
 
         return messages
 
-    async def purge(self, amount: int = None):
+    async def purge(self, amount: int = None) -> None:
         """
         Delete a number of messages, starting from the most recent.
 
         Args:
             amount(int) : Number of messages to purge/delete.
 
         Returns:
@@ -68,50 +70,64 @@
 #            for i in range(0, len(msgs[:amount]), 2):
 #                await asyncio.gather(*(asyncio.create_task(message.delete()) for message in msgs[:amount][i:i + 2]))
 #                await asyncio.sleep(0.2)
 #        else:
 #            for i in range(0, len(msgs), 2):
 #                await asyncio.gather(*(asyncio.create_task(message.delete()) for message in msgs[i:i + 2]))
 #                await asyncio.sleep(0.2)
-             
 
 
-    async def spam(self, amount: int, content: str, tts=False):
+
+    async def spam(self, amount: int, content: str, tts=False) -> None:
         """
         Send multiple of the same message.
 
         Args:
             - amount(int) : Number of spam messages to send.
             - content(str) : The message to send.
             - tts(bool) = False : Specify whether it is a TTS message.
 
         Returns:
-             No return value.
+            No return value.
         """
         amount: list[int] = [i + 1 for i in range(amount)]
         for i in range(0, len(amount), 3):
             await asyncio.gather(
                 *(asyncio.create_task(self.send(tts=tts, content=content)) for amoun in amount[i:i + 3]))
+            await asyncio.sleep(0.3)
 
-    async def send(self, content=None, tts=False):
+    async def send(self, content=None, tts=False) -> None:
         """
         Send a message to the text channel.
 
         Args:
             - content(str) : Message content. Should be string type or similar. Discord `embed` type is not allowed.
-            - tts(bool) :
+            - tts(bool) : Specify whether message is text-to-speech or not
+
+        Returns:
+            No return value.
         """
         if hasattr(self, "guild_id"):
             await self.http.request(method="post", endpoint=f"/channels/{self.id}/messages", headers={"origin": "https://discord.com", "referer": f"https://discord.com/channels/{self.guild_id}/{self.id}"},
                                     json={"content": content, "tts": tts})
         else:
             await self.http.request(method="post", endpoint=f"/channels/{self.id}/messages", headers={"origin": "https://discord.com", "referer": f"https://discord.com/channels/{self.id}"},
                                     json={"content": content, "tts": tts})
 
-    async def reply(self, message, content=None, tts=False):
+    async def reply(self, message: str, content=None, tts=False) -> None:
+        """Reply to a specific message
+
+        Args:
+            message (str): Message to reply to
+            content (_type_, optional): Message content to reply with. Defaults to None.
+            tts (bool, optional): Specify whether message is text-to-speech or not. Defaults to False.
+
+        Returns:
+            No return value.
+        """
         if hasattr(self, "guild_id"):
             await self.http.request(method="post", endpoint=f"/channels/{self.id}/messages", headers={"origin": "https://discord.com", "referer": f"https://discord.com/channels/{self.guild_id}/{self.id}"},
                                     json={"content": content, "tts": tts,
                                         "message_reference": {"channel_id": f"{self.id}", "message_id": f"{message.id}"},
                                         "allowed_mentions": {"parse": ["users", "roles", "everyone"],
                                                             "replied_user": False}})
         else:
@@ -168,15 +184,21 @@
         self.http = http
         self.bot = bot
         self._update(data)
 
     def __str__(self) -> str:
         return f"{self.name}"
 
-    def _update(self, data):
+    def _update(self, data: dict):
+        """Updater method intended to create the attributes for the object
+
+        Args:
+            data (dict): JSON data from gateway
+        """
+
         self.topic = data.get("topic")
         self.rate_limit_per_user = data.get("rate_limit_per_user")
         self.position = data.get("position")
         self.name = data.get("name")
         self.id = data.get("id")
         self.guild_id = data.get("guild_id")
         self.last_message_id = data.get("last_message_id")
@@ -226,25 +248,40 @@
         try:
             await self.http.request(method="patch", endpoint=f"/channels/{self.id}", json=payload)
         except Exception as e:
             from traceback import format_exception
             error = "".join(format_exception(e, e, e.__traceback__))
             return error
 
-    async def create_webhook(self, name: str = None, avatar_url: str = None):
+    async def create_webhook(self, name: str = None, avatar_url: str = None) -> Webhook:
+        """
+        Creates a webhook in the specified channel
+
+        Args:
+            name (str, optional): Name of the webhook. Defaults to None.
+            avatar_url (str, optional): Avatar of the webhook. Requires a URL. Defaults to None.
+
+        Returns:
+            webhook (Webhook): Returns the created webhook object.
+
+        Raises:
+            NameError: Name is required
+        """
         fields = {}
         if name != None:
             fields['name'] = name
         else:
             raise TypeError("Name is required...")
         if avatar_url != None:
             data = await self.http.encode_image(avatar_url)
             fields['avatar'] = data
         data = await self.http.request(method="post", endpoint=f"/channels/{self.id}/webhooks", json=fields)
-        self.webhooks.append(Webhook(data, self.bot, http=self.http))
+        webhook = Webhook(data, self.bot, http=self.http)
+        self.webhooks.append(webhook)
+        return webhook
 
 
 class VoiceChannel(Messageable):
     """Voice Channel Object
     """
 
     def __init__(self, data, bot, http) -> None:
@@ -254,48 +291,74 @@
         self.http = http
         self.bot = bot
         self._update(data)
 
     def __str__(self) -> str:
         return f"{self.name}"
 
-    def _update(self, data):
+    def _update(self, data: dict):
+        """Updater method intended to create the attributes for the object
+
+        Args:
+            data (dict): JSON data from gateway
+        """
         self.name = data.get("name")
         self.id = data.get("id")
         self.guild_id = data.get("guild_id")
         self.last_message_id = data.get("last_message_id")
         self.rtc_region = data.get("rtc_region")
         self.flags = data.get("flags")
         self.bitrate = data.get("bitrate")
         self.rate_limit_per_user = data.get("rate_limit_per_user")
         self.position = data.get("position")
         self.category_id = data.get("parent_id")
 
     async def delete(self):
+        """
+        Deletes the voice channel object.
+        """
         await self.http.request(method="delete", endpoint=f"/channels/{self.id}")
         del self
 
-    async def create_webhook(self, name: str = None, avatar_url: str = None):
+    async def create_webhook(self, name: str = None, avatar_url: str = None) -> Webhook :
+        """
+        Creates a webhook in the specified channel
+
+        Args:
+            name (str, optional): Name of the webhook. Defaults to None.
+            avatar_url (str, optional): Avatar of the webhook. Requires a URL. Defaults to None.
+
+        Returns:
+            webhook (Webhook): Returns the created webhook object.
+
+        Raises:
+            NameError: Name is required
+        """
+
         fields = {}
         if name != None:
             fields['name'] = name
         else:
             raise TypeError("Name is required...")
         if avatar_url != None:
             data = await self.http.encode_image(avatar_url)
             fields['avatar'] = data
         data = await self.http.request(method="post", endpoint=f"/channels/{self.id}/webhooks", json=fields)
         webhook = Webhook(data, self.bot, self.http)
         self.webhooks.append(webhook)
         return webhook
 
     async def call(self):
+        """Initiates a call on the specified channel
+        """
         await self.bot.gateway.ring(self.id, self.guild_id)
 
     async def leave(self):
+        """Leaves call on the specified channel
+        """
         await self.bot.gateway.leave_call()
 
 
 class Category:
     """Category Object
     """
 
@@ -304,22 +367,29 @@
         self.http = http
         self.permissions = []
         self._update(data)
 
     def __str__(self) -> str:
         return f"{self.name}"
 
-    def _update(self, data):
+    def _update(self, data: dict):
+        """Updater method intended to create the attributes for the object
+
+        Args:
+            data (dict): JSON data from gateway
+        """
         self.name = data.get("name")
         self.id = data.get("id")
         self.guild_id = data.get("guild_id")
         self.position = data.get("position")
         self.flags = data.get("flags")
 
     async def delete(self):
+        """Deletes the Category object.
+        """
         await self.http.request(method="delete", endpoint=f"/channels/{self.id}")
         del self
 
 
 class DMChannel(Messageable):
     """DM Channel Object
     """
@@ -329,28 +399,39 @@
         self.http = http
         self.bot = bot
         self._update(data)
 
     def __str__(self) -> str:
         return f"{self.recipient}"
 
-    def _update(self, data):
+    def _update(self, data: dict):
+        """Updater method intended to create the attributes for the object
+
+        Args:
+            data (dict): JSON data from gateway
+        """
         self.recipient = User(data.get("recipients")[0], self.bot, self.http)
         self.last_message_id = data.get("last_message_id")
         self.id = data.get("id")
         self.flags = data.get("id")
 
     async def delete(self):
+        """Deletes the DM Channel object.
+        """
         await self.http.request(method="delete", endpoint=f"/channels/{self.id}?silent=false")
         del self
 
     async def call(self):
+        """Initiates the call on the specified channel
+        """
         await self.bot.gateway.ring(self.id)
 
     async def leave(self):
+        """Leaves the call on the specified channel
+        """
         await self.bot.gateway.leave_call()
 
 
 class GroupChannel(Messageable):
     """Group Channel Object
     """
 
@@ -360,27 +441,38 @@
         self.http = http
         self.bot = bot
         self._update(data)
 
     def __str__(self) -> str:
         return f"{self.name}"
 
-    def _update(self, data):
+    def _update(self, data: dict):
+        """Updater method intended to create the attributes for the object
+
+        Args:
+            data (dict): JSON data from gateway
+        """
         for user in data.get("recipients"):
             self.recipients.append(User(user, self.bot, self.http))
         self.name = data.get("name")
         self.owner_id = data.get("owner_id")
         self.last_message_id = data.get("last_message_id")
         self.id = data.get("id")
         self.flags = data.get("flags")
         self.icon = data.get("icon")
 
     async def delete(self):
+        """Deletes the Group Channel Object
+        """
         await self.http.request(method="delete", endpoint=f"/channels/{self.id}?silent=true")
         del self
 
     async def call(self):
+        """Initiates the call on the specified channel
+        """
         await self.bot.gateway.ring(self.id)
 
     async def leave(self):
+        """Leaves the call on the specified channel
+        """
         await self.bot.gateway.leave_call()
```

### Comparing `selfcord.py-0.1.0/selfcord/models/client.py` & `selfcord.py-0.1.1/selfcord/models/member.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 
 
-class Client:
-    """Client Object
+class Member:
+    """Member Object
     """
     def __init__(self, UserPayload: dict) -> None:
+        self.roles = []
 
-        self.guilds = []
-        self.private_channels = []
-        self.friends = []
-        self.messages = []
-        self.deleted_messages = []
         self._update(UserPayload)
 
     def __str__(self):
         return f"""{self.name}#{self.discriminator}"""
 
 
     def _update(self, data):
-        self.name = data.get("username")
-        self.id = data.get("id")
-        self.discriminator = data.get("discriminator")
-        self.avatar = data.get("avatar")
-        self.banner = data.get("banner")
-        self.bio = data.get("bio")
-        self.email = data.get("email")
-        self.phone = data.get("phone")
-        self.accent_colour = data.get('accent_color')
-        self.public_flags = data.get('public_flags')
-        self.bot_acc = data.get('bot')
-        self.system = data.get('system')
-
+        """Updater method intended to create the attributes for the object
 
+        Args:
+            data (dict): JSON data from gateway
+        """
+        user = data.get("user")
+        self.name = user.get("username")
+        self.id = user.get("id")
+        self.discriminator = user.get("discriminator")
+        self._avatar = user.get("avatar")
+        self._banner = user.get("banner")
+        self._accent_colour = user.get('accent_color')
+        self._public_flags = user.get('public_flags')
+        self.bot_acc = user.get('bot')
+        self.joined_at = data.get('joined_at')
+        self.nick = data.get("nick")
+        self.system = data.get('system')
```

### Comparing `selfcord.py-0.1.0/selfcord/models/guild.py` & `selfcord.py-0.1.1/selfcord/models/guild.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from .channel import TextChannel, VoiceChannel, Category
 from .role import Role
 from .emoji import Emoji
 from itertools import zip_longest
 from aiohttp import ClientSession
 from base64 import b64encode
 import random
+from datetime import datetime, timedelta, timezone
 class Guild:
     """Guild Object
     """
     TEXTCHANNEL = 0
     VOICECHANNEL = 2
     CATEGORY = 4
     GUILD_ANNOUNCEMENT = 5
@@ -29,14 +30,19 @@
         self.bot = bot
         self._update(data)
 
     def __str__(self) -> str:
         return f"{self.name}"
 
     def _update(self, data):
+        """Updater method intended to create the attributes for the object
+
+        Args:
+            data (dict): JSON data from gateway
+        """
         self.id = data.get('id')
         self.name = data.get('name')
         self.icon = data.get('icon')
         self.region = data.get('region')
         self.splash = data.get('splash')
         self.mfa_level = data.get('mfa_level')
         self.features = data.get('features')
@@ -45,15 +51,15 @@
         self.verification_level = data.get('verification_level')
         self.explicit_content_filter = data.get('explicit_content_filter')
         self.owner_id = data.get('owner_id')
 
         for (member, channel, role, emoji) in zip_longest(data.get('members'), data.get("channels"), data.get("roles"), data.get("emojis")):
             if member != None:
                 user = User(member, self.bot, self.http)
-                
+
                 self.members.append(user)
 
             if channel != None:
                 type = channel.get("type")
                 if type == self.TEXTCHANNEL:
                     channel = TextChannel(channel, self.bot, self.http)
                     self.channels.append(channel)
@@ -72,46 +78,107 @@
                 self.roles.append(role)
 
             if emoji != None:
                 emoji = Emoji(emoji, self.bot, self.http)
                 self.emojis.append(emoji)
 
     async def ban(self, user_id: str):
+        """Bans a user from the guild
+
+        Args:
+            user_id (str): User ID specified to ban
+        """
         await self.http.request(method="put", endpoint=f"/guilds/{self.id}/bans/{user_id}", json={"delete_message_days":"7"})
 
     async def kick(self, user_id: str):
+        """Kicks a user from the guild
+
+        Args:
+            user_id (str): User ID specified to kick
+        """
         await self.http.request(method="delete", endpoint=f"/guilds/{self.id}/members/{user_id}")
 
+    def utc_now(self):
+        return datetime.now(timezone.utc)
+
+    async def timeout(self, user_id: str, hours=0, mins=0, seconds=0):
+        """Timeouts a user in the guild
 
-    async def txt_channel_create(self, name, parent_id=None):
+        Args:
+            user_id (str): User ID specified to timeout
+        """
+        duration = self.utc_now() + timedelta(hours, mins, seconds)
+        await self.http.request(method="patch", endpoint=f"/guilds/{self.id}/members/{user_id}", json={"communication_disabled_until": str(duration)})
+
+    async def txt_channel_create(self, name:str, parent_id: str=None):
+        """Creates a Text Channel in the guild
+
+        Args:
+            name (str): Name of the channel
+            parent_id (str, optional): ID of the category. Defaults to None.
+        """
         payload = {"name": name}
         payload.update({"permission_overwrites": []})
         payload.update({"type": 0})
         if parent_id:
             payload.update({"parent_id": parent_id})
 
         await self.http.request(method="post", endpoint=f"/guilds/{self.id}/channels", json=payload)
 
-    async def vc_channel_create(self, name):
+    async def vc_channel_create(self, name: str):
+        """Creates a voice channel in the guild
+
+        Args:
+            name (str): Name of the channel
+        """
         await self.http.request(method="post", endpoint=f"/guilds/{self.id}/channels", json={"name": f"{name}", "permission_overwrites": [], "type": 2})
 
-    async def role_create(self, name):
+    async def role_create(self, name: str):
+        """Creates a role in the guild
+
+        Args:
+            name (str): Name of the role
+        """
         await self.http.request(method = "post", endpoint = f"/guilds/{self.id}/roles", json = {"name": f"{name}"})
 
     async def category_channel_create(self, name):
+        """Creates a category in the guild
+
+        Args:
+            name (str): Name of the category
+        """
         await self.http.request(method = "post", endpoint = f"/guilds/{self.id}/channels", json={"name": f"{name}", "permission_overwrites": [], "type": 4})
 
     async def emoji_create(self, name: str, image_url: str):
+        """Creates an emoji in the guild
+
+        Args:
+            name (str): Name of the emoji
+            image_url (str): URL for an image
+        """
         image = await self.http.encode_image(image_url)
         await self.http.request(method = "post", endpoint = f"/guilds/{self.id}/emojis", json= {"name": f"{name}", "image": image})
 
     async def get_members(self, channel_id: str):
+        """Get guild members for a guild via chunking
+
+        Args:
+            channel_id (str): Channel ID to chunk from
+        """
         await self.bot.gateway.lazy_chunk(self.id, channel_id, self.member_count)
 
     async def edit(self, name: str=None, icon_url: str=None, banner_url: str=None, description: str=None):
+        """Edits attributes for a guild
+
+        Args:
+            name (str, optional): Name of the guild. Defaults to None.
+            icon_url (str, optional): Image URL for Icon. Defaults to None.
+            banner_url (str, optional): Image URL for Banner. Defaults to None.
+            description (str, optional): Description of the guild. Defaults to None.
+        """
         fields = {}
         if name != None:
             fields['name'] = name
 
         if description != None:
             fields['description'] = description
 
@@ -123,9 +190,11 @@
             data = await self.http.encode_image(banner_url)
             fields['banner'] = data
 
 
         await self.http.request(method = "patch", endpoint = f"/guilds/{self.id}", headers={"origin":"https://discord.com", "referer":f"https://discord.com/channels/{self.id}/{random.choice(self.channels)}"},json=fields)
 
     async def delete(self):
+        """Deletes the Guild Object
+        """
         await self.http.request(method = "delete", endpoint = f"/guilds/{self.id}")
```

### Comparing `selfcord.py-0.1.0/selfcord/models/permission.py` & `selfcord.py-0.1.1/selfcord/models/permission.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
             "SEND_MESSAGES_IN_THREADS" : 0x4000000000,
             "USE_EMBEDDED_ACTIVITIES" : 0x8000000000,
             "MODERATE_MEMBERS" : 0x10000000000
         }
         self.permissions = self.calculate_permissions(data)
 
 
-    def calculate_permissions(self, perm_value):
+    def calculate_permissions(self, perm_value: int):
         permissions = []
         for perm, value in self.perms.items():
             if (perm_value & value) == value:
                 permissions.append(perm)
 
         return permissions
```

### Comparing `selfcord.py-0.1.0/selfcord/models/role.py` & `selfcord.py-0.1.1/selfcord/models/role.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,14 +5,19 @@
     """
     def __init__(self, data: dict, http, **kwargs) -> None:
         self.guild_id = kwargs.get("guild_id")
         self.http = http
         self._update(data)
 
     def _update(self, data):
+        """Updater method intended to create the attributes for the object
+
+        Args:
+            data (dict): JSON data from gateway
+        """
         role = data.get("role")
 
         self.id = data.get("id") if role==None else role.get("id")
         self.permissions = Permission(int(data.get("permissions"))).permissions if role==None else Permission(int(role.get("permissions"))).permissions
         self.name = data.get("name") if role==None else role.get("name")
         self.mentionable = data.get("mentionable") if role==None else role.get("mentionable")
         self.managed = data.get("managed") if role==None else role.get("managed")
@@ -26,9 +31,11 @@
 
 
 
     def __str__(self) -> str:
         return f"{self.name}"
 
     async def delete(self):
+        """Delete the Role Object
+        """
         await self.http.request(method="delete", endpoint=f"/guilds/{self.guild_id}/roles/{self.id}")
         del self
```

### Comparing `selfcord.py-0.1.0/selfcord/models/webhook.py` & `selfcord.py-0.1.1/selfcord/models/webhook.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,36 @@
 class Webhook:
     def __init__(self, data: dict, bot, http) -> None:
         self.http = http
         self.bot = bot
         self._update(data)
 
     def _update(self, data):
+        """Updater method intended to create the attributes for the object
+
+        Args:
+            data (dict): JSON data from gateway
+        """
         self.id = data.get("id")
         self.type = data.get("type")
         self.guild_id = data.get("guild_id")
         self.channel_id = data.get("channel_id")
         self.name = data.get("name")
         self.avatar = data.get("avatar")
         self.token = data.get("token")
         self.application_id = data.get("application_id")
         self.webhook_url = f"https://discord.com/api/webhooks/{self.id}/{self.token}"
         self.source_guild = data.get("source_guild")
         self.source_channel = data.get("source_channel")
 
-    async def send(self, content):
+    async def send(self, content: str):
+        """Send a message via the webhook
+
+        Args:
+            content (str): Content of the message to send
+        """
         await self.http.request(method = "post", endpoint = f"/webhooks/{self.id}/{self.token}", json = {"content": content})
 
     async def delete(self):
+        """Deletes the webhook object
+        """
         await self.http.request(method = "delete", endpoint = f"/webhooks/{self.id}/{self.token}")
```

### Comparing `selfcord.py-0.1.0/selfcord/utils/command.py` & `selfcord.py-0.1.1/selfcord/utils/command.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 import inspect
 import re
 from collections import defaultdict
 
 
 class Extension:
-    """Extension object pretty much
+    """Extension object. Discord.py equivalent of cogs, a helper system to help manage and organise code into multiple files
     """
     def __init__(self, **kwargs):
         self.name: str | None = kwargs.get("name")
         self.description: str | None = kwargs.get('description')
         self.ext = kwargs.get("ext")
         self._events = defaultdict(list)
         _events = self.ext._events
@@ -23,43 +23,73 @@
         self._events.update(_events)
         _events.clear()
 
 
 
 
 class ExtensionCollection:
-    """Extension collection, where extensions are stored into
+    """Extension collection, where extensions are stored into. Utilised for Extender, Extensions as a whole. This is also used within help commands and command invocation.
     """
     def __init__(self):
         self.extensions = {}
 
     def __iter__(self):
         for cmd in self.extensions.values():
             yield cmd
 
-    def _is_already_registered(self, ext):
+    def _is_already_registered(self, ext: Extension) -> bool:
+        """Whether the specified Extension is already registered
+
+        Args:
+            ext (Extension): Extension to check
+
+        Returns:
+            bool: True or False
+        """
         for extension in self.extensions.values():
             if ext.name == extension:
                 return True
+            else:
+                return False
+        else:
+            return False
+
+    def add(self, ext: Extension):
+        """Adds an extension
+
+        Args:
+            ext (Extension): Extension to add
 
-    def add(self, ext):
+        Raises:
+            ValueError: Extension must be subclass of extension
+            ValueError: A name or alias is already registered
+        """
         if not isinstance(ext, Extension):
-            raise ValueError('cmd must be a subclass of Extension')
+            raise ValueError('ext must be a subclass of Extension')
         if self._is_already_registered(ext):
             raise ValueError('A name or alias is already registered')
+        # Add extension to the collection
         self.extensions[ext.name] = ext
 
-    def get(self, alias, prefix=''):
+    def get(self, alias: str) -> Extension:
+        """Get an extension
+
+        Args:
+            alias (str): Name of the extension
+
+        Returns:
+            Extension: Extension obtained
+        """
         try:
             return self.extensions[alias]
         except KeyError:
             pass
-        for command in self.extensions:
-            if command.name in command.aliases:
-                return command
+        for extension in self.extensions:
+            if extension.name in extension.aliases:
+                return extension
 
 
 
 class Command:
     """Command Object pretty much
     """
     def __init__(self, **kwargs):
@@ -67,91 +97,143 @@
         self.aliases = [self.name] + kwargs.get('aliases', [])
         self.description = kwargs.get('description')
         self.func = kwargs.get("func")
         self.check = inspect.signature(self.func).return_annotation
         self.signature = inspect.signature(self.func).parameters.items()
 
 class CommandCollection:
-    """Commands collection, where commands are stored into
+    """Commands collection, where commands are stored into. Utilised for help commands and general command invocation.
     """
     def __init__(self, **kwargs):
         self.commands = {}
         self.recent_commands = {}
 
     def __len__(self):
         return len(self.commands)
     def __iter__(self):
         for cmd in self.commands.values():
             yield cmd
 
-    def _is_already_registered(self, cmd):
+    def _is_already_registered(self, cmd: Command) -> bool:
+        """Whether the specified Command is already registered
+
+        Args:
+            cmd (Command): Command to check
+
+        Returns:
+            bool: True or False
+        """
         for command in self.commands.values():
             for alias in cmd.aliases:
                 if alias in command.aliases:
                     return True
+                else:
+                    return False
+            else:
+                return False
+        else:
+            return False
 
     def append(self, collection):
+        """Append to commands, and recent_commands
+
+        Args:
+            collection (CommandCollection): Collection instance
+
+        Raises:
+            ValueError: Collection must be subclass of CommandCollection
+        """
         if not isinstance(collection, CommandCollection):
-            raise ValueError('collection must be a subclass of ExtensionCollection')
+            raise ValueError('collection must be a subclass of CommandCollection')
         for item in collection:
             self.commands[item.name] = item
             self.recent_commands[item.name] = item
 
-    def add(self, cmd):
+    def add(self, cmd: Command):
+        """Add a Command to the collection
+
+        Args:
+            cmd (Command): Command to be added
+
+        Raises:
+            ValueError: cmd must be a subclass of Command
+            ValueError: Name or Alias is already registered
+        """
         if not isinstance(cmd, Command):
             raise ValueError('cmd must be a subclass of Command')
         if self._is_already_registered(cmd):
             raise ValueError('A name or alias is already registered')
         self.commands[cmd.name] = cmd
         self.recent_commands[cmd.name] = cmd
 
     def recents(self):
+        """View commands recently acquired
+
+        Yields:
+            Generator: [Command]
+        """
         for cmd in self.recent_commands.values():
             yield cmd
 
     def copy(self):
+        """Copy commands from recents to main collection
+        """
         self.commands.update(self.recent_commands)
         self.clear()
 
     def clear(self):
+        """Clear recents
+        """
         self.recent_commands.clear()
 
-    def get(self, alias, prefix=''):
+    def get(self, alias) -> Command:
+        """Get a specific command from the collection
+
+        Args:
+            alias (str): Name of the command
+
+        Returns:
+            Command: Command obtained
+        """
         try:
             return self.commands[alias]
         except KeyError:
             pass
         for command in self.commands:
             if alias in command.aliases:
                 return command
 class Event:
+    """Event object
+    """
     def __init__(self, name, coro, ext) -> None:
         self.name = name
         self.coro = coro
         self.ext = ext
 
 
 class Extender:
+    """Extender subclass for extensions, used for implementing the decorators.
+    """
     commands = CommandCollection()
     _events = defaultdict(list)
-    def __init_subclass__(cls, name=None, description="") -> None:
+    def __init_subclass__(cls, name: str =None, description: str="") -> None:
         super().__init_subclass__()
         cls.name = name
         cls.description = description
 
 
 
 
     @classmethod
-    def cmd(cls, description="", aliases=[]):
+    def cmd(cls, description: str="", aliases: list[str]=[]):
         """Decorator to add commands for the bot
 
         Args:
             description (str, optional): Description of command. Defaults to "".
-            aliases (list, optional): Alternative names for command. Defaults to [].
+            aliases (list[str], optional): Alternative names for command. Defaults to [].
 
         Raises:
             RuntimeWarning: If you suck and don't use a coroutine
         """
         if isinstance(aliases, str):
             aliases = [aliases]
 
@@ -175,18 +257,19 @@
             event (str): The event to check for
         """
 
         def decorator(coro):
             if not inspect.iscoroutinefunction(coro):
                 raise RuntimeWarning("Faulure")
             else:
-                cls._events[event].append(Event(name=event, coro=coro, ext=cls))
+                eve = Event(name=event, coro=coro, ext=cls)
+                cls._events[event].append(eve)
 
                 def wrapper(*args, **kwargs):
-                    result = cls._events[event].append(Event(name=event, coro=coro, ext=cls))
+                    result = cls._events[event].append(eve)
                     return result
 
                 return wrapper
         return decorator
 
 
     @classmethod
@@ -209,15 +292,15 @@
             raise RuntimeWarning("Not an async function!")
         else:
 
 
             cmd = Command(name=name, description=description, aliases=aliases, func=coro, ext=cls)
             cls.commands.add(cmd)
 class Context:
-    """Context related for commands, and invokation
+    """Context related for commands, and invocation
     """
     def __init__(self, bot, message, http) -> None:
         self.bot = bot
         self.message = message
         self.http = http
 
 
@@ -257,20 +340,20 @@
                         return command
         return None
 
     @property
     def alias(self):
         for command in self.bot.commands:
             for alias in command.aliases:
-                if self.content.startswith(self.prefix + alias):
+                if self.content.lower().startswith(self.prefix + alias.lower()):
                     return alias
         for extension in self.bot.extensions:
             for command in extension.commands:
                 for alias in command.aliases:
-                    if self.content.startswith(self.prefix + alias):
+                    if self.content.lower().startswith(self.prefix + alias.lower()):
                         self.extension = extension.ext
                         return alias
         return None
 
     @property
     def prefix(self):
         for prefix in self.bot.prefixes:
@@ -309,15 +392,15 @@
 
         Returns:
             Type[str]: The type of parameter
         """
         converter = self.get_converter(param)
         return converter(value)
 
-    async def get_arguments(self):
+    async def get_arguments(self) -> tuple[list, dict]:
         """Get arguments by checking function arguments and comparing to arguments in message.
 
         Returns:
             _type_: _description_
         """
         args = []
         kwargs = {}
```

### Comparing `selfcord.py-0.1.0/selfcord.py.egg-info/PKG-INFO` & `selfcord.py-0.1.1/selfcord.py.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selfcord.py
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Discord API wrapper designed for selfbots!
 Home-page: https://github.com/Shell1010/Selfcord
 Author: Shell of OMEGA
 License: MIT
 Keywords: selfbot,discord,discordapi,discordwrapper
 Description-Content-Type: text/markdown
 
@@ -20,14 +20,20 @@
 
 ## Wiki
 
 Read our [Wiki](https://github.com/Shell1010/Selfcord/wiki) in regards to documentation and getting started.
 
 ## Examples
 
+### Aeterna Selfbot
+
+A simple selfbot designed to showcase the library's features, intended to be seen as a template or base for other users.
+
+[Aeterna Selfbot](https://github.com/Shell1010/Aeterna-Selfbot)
+
 ### Message logger
 ```python
 import selfcord
 
 token = "insert token"
 bot = selfcord.Bot(prefixes=["!", "?"])
```

### Comparing `selfcord.py-0.1.0/selfcord.py.egg-info/SOURCES.txt` & `selfcord.py-0.1.1/selfcord.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `selfcord.py-0.1.0/setup.py` & `selfcord.py-0.1.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 this_directory = Path(__file__).parent
 if __name__ == "__main__":
     this_directory = Path(__file__).parent
     long_description = ( this_directory /"README.md").read_text()
     setup(
         name="selfcord.py",
         packages=find_packages(include=['selfcord', 'selfcord.api', 'selfcord.utils', 'selfcord.models']),
-        version="0.1.0",
+        version="0.1.1",
         description="A Discord API wrapper designed for selfbots!",
         readme="README.md",
         author="Shell of OMEGA",
         license="MIT",
-        install_requires=["aiohttp==3.7.4.post0","aioconsole==0.3.3", "websockets==10.1", "importlib", "requests"],
+        install_requires=["aiohttp==3.7.4.post0","aioconsole==0.3.3", "websockets==10.1", "requests"],
         setup_requires=['pytest-runner'],
         tests_require=['pytest'],
         test_suite='tests',
         keywords=["selfbot", "discord", "discordapi", "discordwrapper"],
         long_description=long_description,
         url="https://github.com/Shell1010/Selfcord",
         long_description_content_type="text/markdown",
-    )
+    )
```

