# Comparing `tmp/scratchconnect-4.5.2.tar.gz` & `tmp/scratchconnect-5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scratchconnect-4.5.2.tar", last modified: Mon Feb 13 10:50:04 2023, max compression
+gzip compressed data, was "scratchconnect-5.0.tar", last modified: Fri Apr 28 15:08:48 2023, max compression
```

## Comparing `scratchconnect-4.5.2.tar` & `scratchconnect-5.0.tar`

### file list

```diff
@@ -1,32 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 10:50:04.186662 scratchconnect-4.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-02-13 10:49:51.000000 scratchconnect-4.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    37953 2023-02-13 10:50:04.182662 scratchconnect-4.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    37046 2023-02-13 10:49:51.000000 scratchconnect-4.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 10:50:04.182662 scratchconnect-4.5.2/scratchconnect/
--rw-r--r--   0 runner    (1001) docker     (123)     7077 2023-02-13 10:49:51.000000 scratchconnect-4.5.2/scratchconnect/CloudConnection.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-02-13 10:49:51.000000 scratchconnect-4.5.2/scratchconnect/Exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-02-13 10:49:51.000000 scratchconnect-4.5.2/scratchconnect/Forum.py
--rw-r--r--   0 runner    (1001) docker     (123)    22862 2023-02-13 10:49:51.000000 scratchconnect-4.5.2/scratchconnect/Project.py
--rw-r--r--   0 runner    (1001) docker     (123)    21357 2023-02-13 10:49:51.000000 scratchconnect-4.5.2/scratchconnect/ScratchConnect.py
--rw-r--r--   0 runner    (1001) docker     (123)    21039 2023-02-13 10:49:51.000000 scratchconnect-4.5.2/scratchconnect/Studio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-02-13 10:49:51.000000 scratchconnect-4.5.2/scratchconnect/TurbowarpCloudConnection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-02-13 10:49:51.000000 scratchconnect-4.5.2/scratchconnect/User.py
--rw-r--r--   0 runner    (1001) docker     (123)    13189 2023-02-13 10:49:51.000000 scratchconnect-4.5.2/scratchconnect/UserCommon.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-02-13 10:49:51.000000 scratchconnect-4.5.2/scratchconnect/Warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-02-13 10:49:51.000000 scratchconnect-4.5.2/scratchconnect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-02-13 10:49:51.000000 scratchconnect-4.5.2/scratchconnect/scChart.py
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-02-13 10:49:51.000000 scratchconnect-4.5.2/scratchconnect/scCloudEvents.py
--rw-r--r--   0 runner    (1001) docker     (123)    15525 2023-02-13 10:49:51.000000 scratchconnect-4.5.2/scratchconnect/scCloudRequests.py
--rw-r--r--   0 runner    (1001) docker     (123)    11780 2023-02-13 10:49:51.000000 scratchconnect-4.5.2/scratchconnect/scCloudStorage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-02-13 10:49:51.000000 scratchconnect-4.5.2/scratchconnect/scEncoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-02-13 10:49:51.000000 scratchconnect-4.5.2/scratchconnect/scImage.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-02-13 10:49:51.000000 scratchconnect-4.5.2/scratchconnect/scOnlineIDE.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-02-13 10:49:51.000000 scratchconnect-4.5.2/scratchconnect/scScratchTerminal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 10:50:04.182662 scratchconnect-4.5.2/scratchconnect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    37953 2023-02-13 10:50:04.000000 scratchconnect-4.5.2/scratchconnect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-02-13 10:50:04.000000 scratchconnect-4.5.2/scratchconnect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-13 10:50:04.000000 scratchconnect-4.5.2/scratchconnect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-02-13 10:50:04.000000 scratchconnect-4.5.2/scratchconnect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-13 10:50:04.000000 scratchconnect-4.5.2/scratchconnect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-13 10:50:04.186662 scratchconnect-4.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-02-13 10:49:51.000000 scratchconnect-4.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:08:48.622625 scratchconnect-5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-28 15:08:32.000000 scratchconnect-5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    37929 2023-04-28 15:08:48.622625 scratchconnect-5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    37046 2023-04-28 15:08:32.000000 scratchconnect-5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:08:48.618625 scratchconnect-5.0/scratchconnect/
+-rw-r--r--   0 runner    (1001) docker     (123)     7994 2023-04-28 15:08:32.000000 scratchconnect-5.0/scratchconnect/CloudConnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-28 15:08:32.000000 scratchconnect-5.0/scratchconnect/Exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-04-28 15:08:32.000000 scratchconnect-5.0/scratchconnect/Forum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24619 2023-04-28 15:08:32.000000 scratchconnect-5.0/scratchconnect/Project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19929 2023-04-28 15:08:32.000000 scratchconnect-5.0/scratchconnect/ScratchConnect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22427 2023-04-28 15:08:32.000000 scratchconnect-5.0/scratchconnect/Studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-04-28 15:08:32.000000 scratchconnect-5.0/scratchconnect/TurbowarpCloudConnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-04-28 15:08:32.000000 scratchconnect-5.0/scratchconnect/User.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13230 2023-04-28 15:08:32.000000 scratchconnect-5.0/scratchconnect/UserCommon.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-28 15:08:32.000000 scratchconnect-5.0/scratchconnect/Warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-04-28 15:08:32.000000 scratchconnect-5.0/scratchconnect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-04-28 15:08:32.000000 scratchconnect-5.0/scratchconnect/scCloudEvents.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15588 2023-04-28 15:08:32.000000 scratchconnect-5.0/scratchconnect/scCloudRequests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11908 2023-04-28 15:08:32.000000 scratchconnect-5.0/scratchconnect/scCloudStorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-04-28 15:08:32.000000 scratchconnect-5.0/scratchconnect/scEncoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-04-28 15:08:32.000000 scratchconnect-5.0/scratchconnect/scImage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-04-28 15:08:32.000000 scratchconnect-5.0/scratchconnect/scOnlineIDE.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-28 15:08:32.000000 scratchconnect-5.0/scratchconnect/scScratchTerminal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:08:48.618625 scratchconnect-5.0/scratchconnect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    37929 2023-04-28 15:08:48.000000 scratchconnect-5.0/scratchconnect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-28 15:08:48.000000 scratchconnect-5.0/scratchconnect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 15:08:48.000000 scratchconnect-5.0/scratchconnect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-28 15:08:48.000000 scratchconnect-5.0/scratchconnect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-28 15:08:48.000000 scratchconnect-5.0/scratchconnect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 15:08:48.622625 scratchconnect-5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-28 15:08:32.000000 scratchconnect-5.0/setup.py
```

### Comparing `scratchconnect-4.5.2/LICENSE` & `scratchconnect-5.0/LICENSE`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Siddhesh Chavan
+Copyright (c) 2023 Siddhesh Chavan
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `scratchconnect-4.5.2/PKG-INFO` & `scratchconnect-5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: scratchconnect
-Version: 4.5.2
+Version: 5.0
 Summary: Python Library to connect Scratch API and much more. This library can show the statistics of Users, Projects, Studios, Forums and also connect and set cloud variables of a project!
 Home-page: https://github.com/Sid72020123/scratchconnect/
 Author: Siddhesh Chavan
 Author-email: siddheshchavan2020@gmail.com
 License: MIT
 Keywords: connect scratch,scratch api,api,scratch,bot,scratch bot,scratch cloud,scratch cloud variables,scratch data,scratch stats,cloud requests,fast cloud requests
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 Provides-Extra: terminal
-Provides-Extra: chart
 License-File: LICENSE
 
 # ScratchConnect v4.5.2
 
 Python Library to connect Scratch API and much more.
 
 This library can show the statistics of Users, Projects, Studios, Forums and also connect and set cloud variables of a
```

### Comparing `scratchconnect-4.5.2/README.md` & `scratchconnect-5.0/README.md`

 * *Files identical despite different names*

### Comparing `scratchconnect-4.5.2/scratchconnect/CloudConnection.py` & `scratchconnect-5.0/scratchconnect/CloudConnection.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,88 +1,87 @@
 """
 The Cloud Variables File.
 Go to https://scratch.mit.edu/projects/578255313/ for the Scratch Encode/Decode Engine!
 """
 import json
-import requests
+import requests  # Needed to change the URL of the request while using the online IDE
 from ssl import SSLEOFError, SSLError
 import websocket
 import time
 from threading import Thread
 
+from scratchconnect.scOnlineIDE import _change_request_url
 from scratchconnect import Exceptions
 from scratchconnect.scEncoder import Encoder
 from scratchconnect.scCloudEvents import CloudEvents
 
 _website = "scratch.mit.edu"
 _login = f"https://{_website}/login/"
 _api = f"api.{_website}"
 
 
 class CloudConnection:
-    def __init__(self, project_id, client_username, csrf_token, session_id, token):
+    def __init__(self, project_id, client_username, csrf_token, session_id, token, session, online_ide):
         """
         Main class to connect cloud variables
         """
         self.project_id = str(project_id)
         self.client_username = client_username
         self.csrf_token = csrf_token
         self.session_id = session_id
         self.token = token
+        self.session = session
         self.headers = {
             "x-csrftoken": self.csrf_token,
             "X-Token": self.token,
             "x-requested-with": "XMLHttpRequest",
-            "Cookie": "scratchcsrftoken="
-                      + self.csrf_token
-                      + ";scratchlanguage=en;scratchsessionsid="
-                      + self.session_id
-                      + ";",
+            "Cookie": f"scratchcsrftoken={self.csrf_token};scratchlanguage=en;scratchsessionsid={self.session_id};",
             "referer": "https://scratch.mit.edu/projects/" + self.project_id + "/",
         }
 
         self.json_headers = {
             "x-csrftoken": self.csrf_token,
             "X-Token": self.token,
             "x-requested-with": "XMLHttpRequest",
-            "Cookie": "scratchcsrftoken="
-                      + self.csrf_token
-                      + ";scratchlanguage=en;scratchsessionsid="
-                      + self.session_id
-                      + ";",
+            "Cookie": f"scratchcsrftoken={self.csrf_token};scratchlanguage=en;scratchsessionsid={self.session_id};",
             "referer": "https://scratch.mit.edu/projects/" + str(self.project_id) + "/",
             "accept": "application/json",
             "Content-Type": "application/json",
+            "origin": f"https://{_website}"
         }
+        if online_ide:
+            _change_request_url()
         self._event = CloudEvents("Scratch", self)
         self.encoder = Encoder()
         self._make_connection()
         self._start_ping_thread()
 
-    def get_variable_data(self, limit=100, offset=0):
+    def get_variable_data(self, limit: int = 100, offset: int = 0) -> list[dict]:
         """
         Returns the cloud variable data
         :param limit: The limit
         :param offset: The offset or the number of values you want to skip from the beginning
         """
+        # Session is not required in the request below:
+        # If the session is used, the Scratch API sometimes returns cached results
         response = requests.get(
             f"https://clouddata.scratch.mit.edu/logs?projectid={self.project_id}&limit={limit}&offset={offset}").json()
         data = []
         for i in range(0, len(response)):
             data.append({'User': response[i]['user'],
                          'Action': response[i]['verb'],
                          'Name': response[i]['name'],
                          'Value': response[i]['value'],
                          'Timestamp': response[i]['timestamp']
                          })
         return data
 
-    def get_cloud_variable_value(self, variable_name, limit=100):
+    def get_cloud_variable_value(self, variable_name: str, limit: int = 100) -> list:
         """
-        Returns the cloud variable value
+        Returns the cloud variable value as a list. The first of the list is the latest value
         :param variable_name: The name of the variable
         :param limit: The limit
         """
         if str(variable_name.strip())[0] != "☁":
             n = f"☁ {variable_name.strip()}"
         else:
             n = f"{variable_name.strip()}"
@@ -135,15 +134,15 @@
                 "method": "handshake",
                 "user": self.client_username,
                 "project_id": str(self.project_id),
             }
         )
         self._event.emit('connect')
 
-    def set_cloud_variable(self, variable_name, value):
+    def set_cloud_variable(self, variable_name: str, value: int | str) -> bool:
         """
         Set a cloud variable
         :param variable_name: Variable name
         :param value: Variable value
         """
         if str(value).isdigit() and value == '':
             raise Exceptions.InvalidCloudValue(f"The Cloud Value should be a set of digits and not '{value}'!")
@@ -166,42 +165,50 @@
             self._send_packet(packet)
             return True
         except (ConnectionAbortedError, BrokenPipeError, SSLEOFError, SSLError):
             self._event.emit('disconnect')
             self._make_connection()
             return False
 
-    def encode(self, text, default=" "):
+    def encode(self, text: str, default: str = " ") -> str:
         """
         Encode a text. For example: A -> 1
         Go to https://scratch.mit.edu/projects/578255313/ for the Scratch Engine!
         :param text: The text to encode
+        :param default: The default value to encode when the character found is not accepted by the encoder
         """
         return self.encoder.encode(text, default=default)
 
-    def decode(self, encoded_text):
+    def decode(self, encoded_text: str | int | list) -> str:
         """
         Decode a text. For example: 1 -> A
         Go to https://scratch.mit.edu/projects/578255313/ for the Scratch Engine!
         :param encoded_text: The text to decode
         """
-        return self.encoder.decode(encoded_text)
+        if type(encoded_text) == list:
+            return self.encoder.decode(encoded_text[0])
+        else:
+            return self.encoder.decode(encoded_text)
 
-    def encode_list(self, data, default=" "):
+    def encode_list(self, data: list, default: str = " ") -> str:
         """
         Encode a Python List
-        :param data: The list
+        :param data: The list to encode
+        :param default: The default value to encode when the character found is not accepted by the encoder
         """
         return self.encoder.encode_list(data, default=default)
 
-    def decode_list(self, encoded_data):
+    def decode_list(self, encoded_data: str | int | list) -> list:
         """
         Decode a Python List
         :param encoded_data: The data to be decoded
         """
-        return self.encoder.decode_list(encoded_data)
+        if type(encoded_data) == list:
+            return self.encoder.decode_list(encoded_data[0])
+        else:
+            return self.encoder.decode_list(encoded_data)
 
-    def create_cloud_event(self):
+    def create_cloud_event(self) -> CloudEvents:
         """
         Create a Cloud Event
         """
         return self._event
```

### Comparing `scratchconnect-4.5.2/scratchconnect/Exceptions.py` & `scratchconnect-5.0/scratchconnect/Exceptions.py`

 * *Files identical despite different names*

### Comparing `scratchconnect-4.5.2/scratchconnect/Forum.py` & `scratchconnect-5.0/scratchconnect/Forum.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,127 +1,132 @@
 """
 The Forum File
 """
 import requests
+from requests.models import Response
 
 from scratchconnect.scOnlineIDE import _change_request_url
 from scratchconnect import Exceptions
 
 _website = "scratch.mit.edu"
 _login = f"https://{_website}/login/"
 _api = f"https://api.{_website}"
 
 
 class Forum:
-    def __init__(self, id, client_username, headers, logged_in, online_ide):
+    def __init__(self, id, client_username, headers, logged_in, online_ide, session):
         """
         The Main Forum Class
         :param id: The id of the forum
         """
         self.f_id = str(id)
         self.client_username = client_username
         self.headers = headers
         self._logged_in = logged_in
+        self.session = session
         if online_ide:
             _change_request_url()
         self.update_data()
 
-    def update_data(self):
+    def update_data(self) -> None:
         """
         Update the data
         """
         try:
             data = requests.get(f"https://scratchdb.lefty.one/v3/forum/topic/info/{self.f_id}").json()
         except KeyError:
             raise Exceptions.InvalidForumTopic(f"Forum with ID - '{self.f_id}' doesn't exist!")
         self.f_title = data['title']
         self.f_category = data['category']
         self.f_is_closed = data['closed'] == 1
         self.f_is_deleted = data['deleted'] == 1
         self.f_time = data['time']
         self.f_post_count = data["post_count"]
 
-    def id(self):
+    def id(self) -> str:
         """
         Returns the id of the forum
         """
         return self.f_id
 
-    def title(self):
+    def title(self) -> str:
         """
         Returns the title of the forum
         """
         return self.f_title
 
-    def category(self):
+    def category(self) -> str:
         """
         Returns the category of the forum
         """
         return self.f_category
 
-    def is_closed(self):
+    def is_closed(self) -> bool:
         """
         Returns whether the forum is closed or not
         """
         return self.f_is_closed
 
-    def is_deleted(self):
+    def is_deleted(self) -> bool:
         """
         Returns whether the forum is deleted or not
         """
         return self.f_is_deleted
 
-    def time(self):
+    def time(self) -> dict:
         """
         Returns the activity of the forum
         """
         return self.f_time
 
-    def post_count(self):
+    def post_count(self) -> int:
         """
         Returns the total post count of the forum
         """
         return self.f_post_count
 
-    def follow(self):
+    def follow(self) -> Response:
         """
         Follow a Forum
         """
         if self._logged_in is False:
             raise Exceptions.UnauthorizedAction("Cannot perform the action because the user is not logged in!")
         self.headers['referer'] = f"https://scratch.mit.edu/discuss/topic/{self.id}/"
-        return requests.post(f"https://scratch.mit.edu/discuss/subscription/topic/{self.id}/add/",
-                             headers=self.headers)
+        return self.session.post(f"https://scratch.mit.edu/discuss/subscription/topic/{self.id}/add/",
+                                 headers=self.headers)
 
-    def unfollow(self):
+    def unfollow(self) -> Response:
         """
         Unfollow a Forum
         """
         if self._logged_in is False:
             raise Exceptions.UnauthorizedAction("Cannot perform the action because the user is not logged in!")
         self.headers['referer'] = f"https://scratch.mit.edu/discuss/topic/{self.id}/"
-        return requests.post(f"https://scratch.mit.edu/discuss/subscription/topic/{self.id}/delete/",
-                             headers=self.headers)
+        return self.session.post(f"https://scratch.mit.edu/discuss/subscription/topic/{self.id}/delete/",
+                                 headers=self.headers)
 
-    def posts(self, page=1):
+    def posts(self, page: int = 0, order: str = "newest") -> list:
         """
         Get the post in Forum Topic of a specified page. Images and some other stuff will not appear!
-        :param page: The page
+        :param page: The page. Default (start) value is 0
+        :param order: Order to sort posts by, defaults to "newest", possible options include "oldest"
+        The data os fetched from Scratch DB. So, it may not be up-to-date!
         """
-        return requests.get(f"https://scratch-forum.sid72020123.repl.co/forum/?topic={self.f_id}&page={page}").json()
+        return requests.get(
+            f"https://scratchdb.lefty.one/v3/forum/topic/posts/{self.id()}/{page}?o={order}").json()
 
-    def ocular_reactions(self, post_id):
+    def ocular_reactions(self, post_id: int) -> dict:
         """
         Get the ocular reactions
         :param post_id: The id of the post
         """
         return requests.get(f"https://my-ocular.jeffalo.net/api/reactions/{post_id}").json()
 
-    def topic_post_history(self, usernames="total", segment="1", range="30"):
+    def topic_post_history(self, usernames: str = "total", segment: str = "1", range: str = "30") -> dict:
         """
         Get the post history of the topic
-        :param usernames: Values like "total" -> Gives all the data of the users who posted in that topic, "detail" -> Gives individual user's data or you can also put any username
+        :param usernames: Values like "total" -> Gives all the data of the users who posted in that topic, "detail" -> Gives individual user's data, or you can also put any username
         :param segment: The length of time between each segment, defaults to 1 day. Possible special cases include year(365) or month(30)
         :param range: Range of how far back to get history, defaults to 30 days. Possible special cases include year(365) or month(30)
         """
         return requests.get(
             f"https://scratchdb.lefty.one/v3/forum/topic/graph/{self.f_id}/{usernames}?segment={segment}&range={range}").json()
```

### Comparing `scratchconnect-4.5.2/scratchconnect/Project.py` & `scratchconnect-5.0/scratchconnect/Project.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,73 +1,73 @@
 """
 The Project File
 """
 import json
+
 import requests
+from requests.models import Response
 
 from scratchconnect.scOnlineIDE import _change_request_url
 from scratchconnect import CloudConnection
 from scratchconnect import TurbowarpCloudConnection
-from scratchconnect import scCloudStorage
 from scratchconnect import scCloudRequests
 from scratchconnect import Exceptions
+from scratchconnect import Warnings
 
 _website = "scratch.mit.edu"
 _login = f"https://{_website}/login/"
 _api = f"api.{_website}"
 _project = f"https://{_api}/projects/"
 
 
 class Project:
-    def __init__(self, id, client_username, headers, unshared, logged_in, session_id, online_ide):
+    def __init__(self, id, client_username, session, unshared, logged_in, session_id, online_ide):
         """
         The Project Class
         :param id: The project ID
         """
         self.access_unshared = unshared
         self.project_id = str(id)
         self.client_username = client_username
-        self.csrf_token = headers["x-csrftoken"]
+        self.session = session
+        self.csrf_token = self.session.headers["x-csrftoken"]
         self.session_id = session_id
-        self.token = headers["X-Token"]
-        self.headers = headers
+        self.token = self.session.headers["X-Token"]
         self._logged_in = logged_in
         self.json_headers = {
             "x-csrftoken": self.csrf_token,
             "X-Token": self.token,
             "x-requested-with": "XMLHttpRequest",
-            "Cookie": "scratchcsrftoken="
-                      + self.csrf_token
-                      + ";scratchlanguage=en;scratchsessionsid="
-                      + self.session_id
-                      + ";",
-            "referer": "https://scratch.mit.edu/projects/" + str(self.project_id) + "/",
+            "Cookie": f"scratchcsrftoken={self.csrf_token};scratchlanguage=en;scratchsessionsid={self.session_id};",
+            "referer": f"https://scratch.mit.edu/projects/{self.project_id}/",
             "accept": "application/json",
             "Content-Type": "application/json",
+            "origin": f"https://{_website}"
         }
         if online_ide:
             _change_request_url()
+        self.online_ide = online_ide
         self.update_data()
 
-    def update_data(self):
+    def update_data(self) -> None:
         self.project_author = None
         self.project_title = None
         self.project_notes = None
         self.project_instructions = None
         self.project_are_comments_allowed = None
         self.project_stats = None
         self.project_history = None
         self.project_remix_data = None
         self.project_visibility = None
         self.project_is_public = None
         self.project_is_published = None
         self.project_thubmnail_url = None
         self.project_token = None
 
-        data = requests.get(f"https://api.scratch.mit.edu/projects/{self.project_id}").json()
+        data = self.session.get(f"{_project}{self.project_id}").json()
         try:
             self.project_id = data["id"]
         except KeyError:
             if self.access_unshared:
                 pass
             else:
                 raise Exceptions.InvalidProject(
@@ -83,460 +83,464 @@
             self.project_remix_data = data["remix"]
             self.project_visibility = data["visibility"]
             self.project_is_public = data["public"] == True
             self.project_is_published = data["is_published"] == True
             self.project_thubmnail_url = data["images"]
             self.project_token = data["project_token"]
 
-    def id(self):
+    def id(self) -> int:
         """
         Returns the project ID
         """
         return self.project_id
 
-    def author(self):
+    def author(self) -> dict:
         """
         Returns the author of the project
         """
         if self.project_author is None:
             self.update_data()
         return self.project_author
 
-    def title(self):
+    def title(self) -> str:
         """
         Returns the title of the project
         """
         if self.title is None:
             self.update_data()
         return self.project_title
 
-    def notes(self):
+    def notes(self) -> str:
         """
         Returns the notes(Notes or Credits) of the project
         """
         if self.project_notes is None:
             self.update_data()
         return self.project_notes
 
-    def instructions(self):
+    def instructions(self) -> str:
         """
         Returns the instructions of the project
         """
         if self.project_instructions is None:
             self.update_data()
         return self.project_instructions
 
-    def are_comments_allowed(self):
+    def are_comments_allowed(self) -> bool:
         """
         Returns whether the comments are allowed in a project
         """
         if self.project_are_comments_allowed is None:
             self.update_data()
         return self.project_are_comments_allowed
 
-    def stats(self):
+    def stats(self) -> dict:
         """
         Returns the stats of a project
         """
         if self.project_stats is None:
             self.update_data()
         return self.project_stats
 
-    def history(self):
+    def history(self) -> dict:
         """
         Returns the history of a project
         """
         if self.project_history is None:
             self.update_data()
         return self.project_history
 
-    def remix_data(self):
+    def remix_data(self) -> dict:
         """
         Returns the remix data of a project
         """
         if self.project_remix_data is None:
             self.update_data()
         return self.project_remix_data
 
-    def visibility(self):
+    def visibility(self) -> str:
         """
         Returns whether the project is visible
         """
         if self.project_visibility is None:
             self.update_data()
         return self.project_visibility
 
-    def is_public(self):
+    def is_public(self) -> bool:
         """
         Returns whether the project is public
         """
         if self.project_is_public is None:
             self.update_data()
         return self.project_is_public
 
-    def is_published(self):
+    def is_published(self) -> bool:
         """
         Returns whether the project is published
         """
         if self.project_is_published is None:
             self.update_data()
         return self.project_is_public
 
-    def thumbnail_url(self):
+    def thumbnail_url(self) -> dict:
         """
         Returns the thumbnail url of a project
         """
         if self.project_thubmnail_url is None:
             self.update_data()
         return self.project_thubmnail_url
 
-    def assets_info(self):
+    def assets_info(self) -> dict:
         """
         Returns the Assets info of a project
         """
         return requests.get(f"https://scratchdb.lefty.one/v3/project/info/{self.project_id}").json()[
             "metadata"]
 
-    def scripts(self):
+    def scripts(self) -> dict:
         """
         Returns the scripts of a project
         """
-        return requests.get(f"https://projects.scratch.mit.edu/{self.project_id}?token={self.project_token}").json()
+        return self.session.get(f"https://projects.scratch.mit.edu/{self.project_id}?token={self.project_token}").json()
 
-    def love(self):
+    def love(self) -> dict:
         """
         Love a project
         """
         if self._logged_in is False:
             raise Exceptions.UnauthorizedAction("Cannot perform the action because the user is not logged in!")
-        return requests.post(
-            f"https://api.scratch.mit.edu/proxy/projects/{self.project_id}/loves/user/{self.client_username}",
-            headers=self.headers,
-        ).json()
+        return self.session.post(
+            f"https://api.scratch.mit.edu/proxy/projects/{self.project_id}/loves/user/{self.client_username}").json()
 
-    def unlove(self):
+    def unlove(self) -> dict:
         """
         UnLove a project
         """
         if self._logged_in is False:
             raise Exceptions.UnauthorizedAction("Cannot perform the action because the user is not logged in!")
-        return requests.delete(
-            f"https://api.scratch.mit.edu/proxy/projects/{self.project_id}/loves/user/{self.client_username}",
-            headers=self.headers,
-        ).json()
+        return self.session.delete(
+            f"https://api.scratch.mit.edu/proxy/projects/{self.project_id}/loves/user/{self.client_username}").json()
 
-    def favourite(self):
+    def favourite(self) -> dict:
         """
         Favourite a project
         """
         if self._logged_in is False:
             raise Exceptions.UnauthorizedAction("Cannot perform the action because the user is not logged in!")
-        return requests.post(
-            f"https://api.scratch.mit.edu/proxy/projects/{self.project_id}/favorites/user/{self.client_username}",
-            headers=self.headers,
-        ).json()
+        return self.session.post(
+            f"https://api.scratch.mit.edu/proxy/projects/{self.project_id}/favorites/user/{self.client_username}").json()
 
     def unfavourite(self):
         """
         UnFavourite a project
         """
         if self._logged_in is False:
             raise Exceptions.UnauthorizedAction("Cannot perform the action because the user is not logged in!")
-        return requests.delete(
-            f"https://api.scratch.mit.edu/proxy/projects/{self.project_id}/favorites/user/{self.client_username}",
-            headers=self.headers,
-        ).json()
+        return self.session.delete(
+            f"https://api.scratch.mit.edu/proxy/projects/{self.project_id}/favorites/user/{self.client_username}").json()
 
-    def comments(self, all=False, limit=20, offset=0, comment_id=None):
+    def comments(self, all: bool = False, limit: int = 20, offset: int = 0, comment_id: int = None) -> list:
         """
         Returns the list of comments of a project
         :param all: True if you want all
         :param limit: The limit
         :param offset: The offset or the data which you want after the beginning
         :param comment_id: If you want a comment from its ID then use this
         """
         if self.project_author is None:
             self.update_data()
         comments = []
         if all:
             offset = 40
             limit = 40
             while True:
-                response = requests.get(
-                    f"https://api.scratch.mit.edu/users/{self.project_author['username']}/projects/{str(self.project_id)}/comments/?limit={limit}&offset={offset}"
-                ).json()
+                response = self.session.get(
+                    f"https://api.scratch.mit.edu/users/{self.project_author['username']}/projects/{self.project_id}/comments/?limit={limit}&offset={offset}").json()
                 if len(response) != 40:
                     break
                 offset += 40
             comments.append(response)
         if not all:
-            comments.append(requests.get(
-                f"https://api.scratch.mit.edu/users/{self.project_author['username']}/projects/{str(self.project_id)}/comments/?limit={limit}&offset={offset}"
+            comments.append(self.session.get(
+                f"https://api.scratch.mit.edu/users/{self.project_author['username']}/projects/{self.project_id}/comments/?limit={limit}&offset={offset}"
             ).json())
         if comment_id is not None:
             comments = []
-            comments.append(requests.get(
-                f"https://api.scratch.mit.edu/users/{self.project_author['username']}/projects/{str(self.project_id)}/comments/{comment_id}"
+            comments.append(self.session.get(
+                f"https://api.scratch.mit.edu/users/{self.project_author['username']}/projects/{self.project_id}/comments/{comment_id}"
             ).json())
         return comments
 
-    def remixes(self, all=False, limit=20, offset=0):
+    def comment_replies(self, comment_id: int, limit: int = 20, offset: int = 0) -> list:
+        """
+        Get the replies of the comment
+        :param comment_id: ID of the comment
+        :param limit: The limit (max: 40)
+        :param offset: The number of replies to skip from the beginning
+        """
+        return self.session.get(
+            f"https://api.scratch.mit.edu/users/{self.project_author['username']}/projects/{self.project_id}/comments/{comment_id}/replies?limit={limit}&offset={offset}").json()
+
+    def remixes(self, all: bool = False, limit: int = 20, offset: int = 0) -> list:
         """
         Returns the list of remixes of a project
         :param all: True if you want all
         :param limit: The limit
         :param offset: The offset or the data which you want after the beginning
         """
         projects = []
         if all:
             offset = 0
             while True:
-                response = requests.get(
+                response = self.session.get(
                     f"https://api.scratch.mit.edu/projects/{self.project_id}/remixes/?limit=40&offset={offset}").json()
                 projects += response
                 if len(response) != 40:
                     break
                 offset += 40
         else:
-            projects.append(requests.get(
+            projects.append(self.session.get(
                 f"https://api.scratch.mit.edu/projects/{self.project_id}/remixes/?limit={limit}&offset={offset}").json())
         return projects
 
-    def post_comment(self, content, parent_id="", commentee_id=""):
+    def post_comment(self, content: str, parent_id: int = "", commentee_id: int = "") -> Response:
         """
         Post a comment
         :param content: The comment or the content
         """
         if self._logged_in is False:
             raise Exceptions.UnauthorizedAction("Cannot perform the action because the user is not logged in!")
         data = {
             "commentee_id": commentee_id,
             "content": content,
             "parent_id": parent_id,
         }
-        return requests.post(
-            "https://api.scratch.mit.edu/proxy/comments/project/" + str(self.project_id) + "/",
-            headers=self.json_headers,
-            data=json.dumps(data),
-        )
+        return self.session.post(f"https://api.scratch.mit.edu/proxy/comments/project/{self.project_id}/",
+                                 data=json.dumps(data), headers=self.json_headers)
 
-    def reply_comment(self, content, comment_id):
+    def reply_comment(self, content: str, comment_id: int) -> Response:
         """
         Reply a comment
         :param content: The content
         :param comment_id: The comment ID
         """
         if self._logged_in is False:
             raise Exceptions.UnauthorizedAction("Cannot perform the action because the user is not logged in!")
         return self.post_comment(content=content, parent_id=comment_id)
 
-    def toggle_commenting(self):
+    def toggle_commenting(self) -> dict:
         """
         Toggle the commenting of a project
         """
         if self._logged_in is False:
             raise Exceptions.UnauthorizedAction("Cannot perform the action because the user is not logged in!")
         if self.author()['username'] != self.client_username:
             raise Exceptions.UnauthorizedAction(
                 f"You are not allowed to do that because you are not the owner of the project with ID - '{self.project_id}'!")
-        data = {"comments_allowed": not self.comments_allowed()}
-        return requests.put(f"https://api.scratch.mit.edu/projects/{self.project_id}/",
-                            data=json.dumps(data),
-                            headers=self.json_headers,
-                            ).json()
+        data = {"comments_allowed": not self.are_comments_allowed()}
+        return self.session.put(f"https://api.scratch.mit.edu/projects/{self.project_id}/", data=json.dumps(data),
+                                headers=self.json_headers).json()
 
-    def turn_on_commenting(self):
+    def turn_on_commenting(self) -> dict:
         """
         Turn On the commenting of a project
         """
         if self._logged_in is False:
             raise Exceptions.UnauthorizedAction("Cannot perform the action because the user is not logged in!")
         if self.author()['username'] != self.client_username:
             raise Exceptions.UnauthorizedAction(
                 f"You are not allowed to do that because you are not the owner of the project with ID - '{self.project_id}'!")
         data = {"comments_allowed": True}
-        return requests.put(f"https://api.scratch.mit.edu/projects/{self.project_id}/",
-                            data=json.dumps(data),
-                            headers=self.json_headers,
-                            ).json()
+        return self.session.put(f"https://api.scratch.mit.edu/projects/{self.project_id}/", data=json.dumps(data),
+                                headers=self.json_headers).json()
 
-    def turn_off_commenting(self):
+    def turn_off_commenting(self) -> dict:
         """
         Turn Off the commenting of a project
         """
         if self._logged_in is False:
             raise Exceptions.UnauthorizedAction("Cannot perform the action because the user is not logged in!")
         if self.author()['username'] != self.client_username:
             raise Exceptions.UnauthorizedAction(
                 f"You are not allowed to do that because you are not the owner of the project with ID - '{self.project_id}'!")
         data = {"comments_allowed": False}
-        return requests.put(f"https://api.scratch.mit.edu/projects/{self.project_id}/",
-                            data=json.dumps(data),
-                            headers=self.json_headers,
-                            ).json()
+        return self.session.put(f"https://api.scratch.mit.edu/projects/{self.project_id}/", data=json.dumps(data),
+                                headers=self.json_headers, ).json()
 
-    def report(self, category, reason, image=None):
+    def report(self, category: str, reason: str, image: str = None) -> str:
         """
         Report a project
         :param category: The category
         :param reason: The reason
         """
         if self._logged_in is False:
             raise Exceptions.UnauthorizedAction("Cannot perform the action because the user is not logged in!")
         if self.author()['username'] == self.client_username:
             raise Exceptions.UnauthorizedAction("You can't report your own project!")
         if not image:
-            self.thumbnail_url()
+            image = self.thumbnail_url()
         data = {"notes": reason, "report_category": category, "thumbnail": image}
-        return requests.post(f"https://api.scratch.mit.edu/proxy/comments/project/{self.project_id}/",
-                             data=json.dumps(data),
-                             headers=self.json_headers,
-                             ).text
+        return self.session.post(f"https://api.scratch.mit.edu/proxy/comments/project/{self.project_id}/",
+                                 data=json.dumps(data), headers=self.json_headers).text
 
-    def unshare(self):
+    def unshare(self) -> Response:
         """
         Unshare a project
         """
         if self._logged_in is False:
             raise Exceptions.UnauthorizedAction("Cannot perform the action because the user is not logged in!")
         if self.author()['username'] != self.client_username:
             raise Exceptions.UnauthorizedAction(
                 f"You are not allowed to do that because you are not the owner of the project with ID - '{self.project_id}'!")
-        return requests.put(f"https://api.scratch.mit.edu/proxy/projects/{self.project_id}/unshare/",
-                            headers=self.json_headers,
-                            )
+        return self.session.put(f"https://api.scratch.mit.edu/proxy/projects/{self.project_id}/unshare/",
+                                headers=self.json_headers)
+
+    def share(self) -> Response:
+        """
+        Share a project
+        """
+        Warnings.warn(
+            "[1m[33mScratchConnect Warning: [31mThe 'share()' function doesn't work sometimes because the Scratch server blocks the request returning the status code 503.[0m")
+        if self._logged_in is False:
+            raise Exceptions.UnauthorizedAction("Cannot perform the action because the user is not logged in!")
+        return self.session.put(f"https://api.scratch.mit.edu/proxy/projects/{self.project_id}/share/",
+                                headers=self.json_headers)
 
-    def view(self):
+    def view(self) -> Response:
         """
         Just view a project
         """
         if self._logged_in is False:
             raise Exceptions.UnauthorizedAction("Cannot perform the action because the user is not logged in!")
-        return requests.post(
-            f"https://api.scratch.mit.edu/users/{self.client_username}/projects/{self.project_id}/views/",
-            headers=self.headers,
-        )
+        return self.session.post(
+            f"https://api.scratch.mit.edu/users/{self.client_username}/projects/{self.project_id}/views/")
 
-    def set_thumbnail(self, file):
+    def set_thumbnail(self, file: str) -> Response:
         """
         Set the thumbnail of a project
         :param file: The location of the file
         """
         if self._logged_in is False:
             raise Exceptions.UnauthorizedAction("Cannot perform the action because the user is not logged in!")
         if self.author()['username'] != self.client_username:
             raise Exceptions.UnauthorizedAction(
                 f"You are not allowed to do that because you are not the owner of the project with ID - '{self.project_id}'!")
         with open(file, "rb") as f:
             image = f.read()
-        return requests.post(f"https://scratch.mit.edu/internalapi/project/thumbnail/{self.project_id}/set/",
-                             data=image,
-                             headers=self.headers,
-                             )
+        return self.session.post(f"https://scratch.mit.edu/internalapi/project/thumbnail/{self.project_id}/set/",
+                                 data=image)
 
-    def delete_comment(self, comment_id):
+    def delete_comment(self, comment_id: int) -> Response:
         """
         Delete a comment
         :param comment_id: Comment ID
         """
         if self._logged_in is False:
             raise Exceptions.UnauthorizedAction("Cannot perform the action because the user is not logged in!")
-        return requests.delete(
-            f"https://api.scratch.mit.edu/proxy/comments/project/{self.project_id}/comment/{comment_id}",
-            headers=self.headers,
-        )
+        return self.session.delete(
+            f"https://api.scratch.mit.edu/proxy/comments/project/{self.project_id}/comment/{comment_id}")
 
-    def report_comment(self, comment_id):
+    def report_comment(self, comment_id: int) -> Response:
         """
         Report a comment
         :param comment_id: Comment ID
         """
         if self._logged_in is False:
             raise Exceptions.UnauthorizedAction("Cannot perform the action because the user is not logged in!")
-        return requests.delete(
-            f"https://api.scratch.mit.edu/proxy/comments/project/{self.project_id}/comment/{comment_id}/report",
-            headers=self.headers,
-        )
+        return self.session.delete(
+            f"https://api.scratch.mit.edu/proxy/comments/project/{self.project_id}/comment/{comment_id}/report")
 
-    def set_title(self, title):
+    def set_title(self, title: str) -> dict:
         """
         Set the title of the project
         :param title: The title
         """
         if self._logged_in is False:
             raise Exceptions.UnauthorizedAction("Cannot perform the action because the user is not logged in!")
         data = {'title': title}
-        return requests.put(f"{_project}{self.project_id}", data=json.dumps(data), headers=self.json_headers).json()
+        return self.session.put(f"{_project}{self.project_id}", data=json.dumps(data), headers=self.json_headers).json()
 
-    def set_description(self, description):
+    def set_description(self, description: str) -> dict:
         """
         Set the description of the project
         :param description: The description
         """
         if self._logged_in is False:
             raise Exceptions.UnauthorizedAction("Cannot perform the action because the user is not logged in!")
         data = {'description': description}
-        return requests.put(f"{_project}{self.project_id}", data=json.dumps(data), headers=self.json_headers).json()
+        return self.session.put(f"{_project}{self.project_id}", data=json.dumps(data), headers=self.json_headers).json()
 
-    def set_instruction(self, instruction):
+    def set_instruction(self, instruction: str) -> dict:
         """
         Set the instruction of the project
         :param instruction: The instruction
         """
         if self._logged_in is False:
             raise Exceptions.UnauthorizedAction("Cannot perform the action because the user is not logged in!")
         data = {'instructions': instruction}
-        return requests.put(f"{_project}{self.project_id}", data=json.dumps(data), headers=self.json_headers).json()
+        return self.session.put(f"{_project}{self.project_id}", data=json.dumps(data), headers=self.json_headers).json()
 
-    def connect_cloud_variables(self):
+    def remix_project(self, title: str) -> dict:
+        """
+        Remix the project
+        :param title: The title of the remixed project
+        """
+        Warnings.warn(
+            "[1m[33mScratchConnect Warning: [31mThe 'remix_project()' function doesn't work sometimes because the Scratch server blocks the request returning the status code 503.[0m")
+        if self._logged_in is False:
+            raise Exceptions.UnauthorizedAction("Cannot perform the action because the user is not logged in!")
+        if self.access_unshared:
+            raise Exceptions.UnauthorizedAction(
+                "Cannot perform the action because the project as is accessed as an unshared project.")
+        return self.session.post(
+            f"https://projects.scratch.mit.edu/?is_remix=1&original_id={self.id()}&title={title}",
+            data=json.dumps(self.scripts()), headers={"origin": f"https://{_website}"})
+
+    def connect_cloud_variables(self) -> CloudConnection.CloudConnection:
         """
         Connect the cloud variables of the project
         """
         if self._logged_in is False:
             raise Exceptions.UnauthorizedAction("Cannot perform the action because the user is not logged in!")
         return CloudConnection.CloudConnection(project_id=self.project_id, client_username=self.client_username,
                                                csrf_token=self.csrf_token,
-                                               session_id=self.session_id, token=self.token)
+                                               session_id=self.session_id, token=self.token, session=self.session,
+                                               online_ide=self.online_ide)
 
-    def connect_turbowarp_cloud(self, username=None):
+    def connect_turbowarp_cloud(self, username: str = None) -> TurbowarpCloudConnection.TurbowarpCloudConnection:
         """
         Connect the cloud variables of the project
         """
         if username is None:
             username = self.client_username
         return TurbowarpCloudConnection.TurbowarpCloudConnection(project_id=self.project_id,
                                                                  username=username)
 
-    def create_cloud_storage(self, file_name="data", rewrite_file=True, edit_access=None, all_access=False):
+    def create_cloud_storage(self):
         """
         Create a Cloud Database/Storage in a project
         """
-        if self._logged_in is False:
-            raise Exceptions.UnauthorizedAction("Cannot perform the action because the user is not logged in!")
-        if edit_access is None:
-            edit_access = []
-        return scCloudStorage.CloudStorage(file_name=file_name, rewrite_file=rewrite_file, project_id=self.project_id,
-                                           client_username=self.client_username,
-                                           csrf_token=self.csrf_token,
-                                           session_id=self.session_id, token=self.token, edit_access=edit_access,
-                                           all_access=all_access)
+        Warnings.warn(
+            "[1m[33mScratchConnect Warning: [31mThe Cloud Storage feature is deprecated since the v5.0 of the library. Please use the new alternative Cloud Requests feature instead![0m")
 
-    def create_cloud_requests(self, handle_all_errors=True, print_logs=True):
+    def create_cloud_requests(self, handle_all_errors: bool = True,
+                              print_logs: bool = True) -> scCloudRequests.CloudRequests:
         """
         Create a Cloud Database/Storage in a project
         """
         if self._logged_in is False:
             raise Exceptions.UnauthorizedAction("Cannot perform the action because the user is not logged in!")
         return scCloudRequests.CloudRequests(project_id=self.project_id,
                                              client_username=self.client_username,
                                              csrf_token=self.csrf_token,
                                              session_id=self.session_id, token=self.token,
-                                             handle_all_errors=handle_all_errors, print_logs=print_logs)
+                                             handle_all_errors=handle_all_errors, print_logs=print_logs,
+                                             session=self.session, online_ide=self.online_ide)
 
-    def all_data(self):
+    def all_data(self) -> dict:
         """
         Returns all the data of a Scratch Project
         """
         data = {
             'Project ID': self.id(),
             'Project Name': self.title(),
             'Author': self.author()['username'],
```

### Comparing `scratchconnect-4.5.2/scratchconnect/ScratchConnect.py` & `scratchconnect-5.0/scratchconnect/ScratchConnect.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 """
 Main File to Connect all the Scratch API and the Scratch DB
 """
 
 import requests
+from requests.models import Response
 import json
 import re
 
 from scratchconnect.UserCommon import UserCommon
 from scratchconnect import Exceptions
 from scratchconnect import Warnings
 from scratchconnect import Project
 from scratchconnect import Studio
 from scratchconnect import User
 from scratchconnect import Forum
 from scratchconnect.scOnlineIDE import _change_request_url
 from scratchconnect.scScratchTerminal import _terminal
-from scratchconnect.scChart import _chart
 from scratchconnect.scImage import Image
 
 _website = "scratch.mit.edu"
 _login = f"https://{_website}/login/"
 _api = f"api.{_website}"
 
 
 class ScratchConnect(UserCommon):
-    def __init__(self, username=None, password=None, cookie=None, auto_cookie_login=False, online_ide_cookie=None):
+    def __init__(self, username: str = None, password: str = None, cookie: dict = None, auto_cookie_login: bool = False,
+                 online_ide_cookie: dict = None):
         """
         Class to make a connection to Scratch
         :param username: The username of a Scratch Profile
         :param password: The password of a Scratch Profile
         """
+        self.session = requests.Session()  # The main Session object
         self.username = username
         self.password = password
         self.cookie = cookie
-        self.session = None
+        self.scratch_session = None
         self._online_ide = False
         self.auto_cookie_login = auto_cookie_login
         self.online_ide_cookie = online_ide_cookie
 
         if self.username is not None and self.password is not None:
             self._login(cookie=False, auto_cookie_login=self.auto_cookie_login)
             self._logged_in = True
@@ -46,38 +48,27 @@
             self._logged_in = True
         elif self.online_ide_cookie is not None:
             _change_request_url()
             self._online_ide = True
             self._login(online_ide=True)
             self._logged_in = True
         else:
-            self.headers = {
-                "x-csrftoken": "a",
-                "x-requested-with": "XMLHttpRequest",
-                "Cookie": "scratchcsrftoken=a;scratchlanguage=en;",
-                "referer": "https://scratch.mit.edu",
-                "user-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.101 Safari/537.36"
-            }
             self._logged_in = False
             self.session_id = ""
             self.headers = {
                 "x-csrftoken": "",
                 "X-Token": "",
                 "x-requested-with": "XMLHttpRequest",
-                "Cookie": "scratchcsrftoken="
-                          + ""
-                          + ";scratchlanguage=en;scratchsessionsid="
-                          + ""
-                          + ";",
+                "Cookie": "scratchcsrftoken=" + "" + ";scratchlanguage=en;scratchsessionsid=" + "" + ";",
                 "referer": "https://scratch.mit.edu",
             }
             Warnings.warn(
-                "[1m[33mScratchConnect: [31mLogin with Username/Password and Cookie Failed! Continuing without login...[0m")
-        super().__init__(self.username,
-                         self.headers,
+                "[1m[33mScratchConnect Warning: [31mLogin with Username/Password and Cookie Failed! Continuing without login...[0m")
+        self.session.headers.update(self.headers)  # Update the session headers
+        super().__init__(self.username, self.session,
                          self._online_ide)  # Get other properties and methods from the parent(UserCommon) class
         self.update_data()
 
     def _login(self, cookie=False, auto_cookie_login=False, online_ide=False):
         """
         Function to login(don't use this)
         """
@@ -116,19 +107,15 @@
         elif online_ide is not False:
             self._online_ide_login()
 
         self.headers = {
             "x-csrftoken": self.csrf_token,
             "X-Token": self.token,
             "x-requested-with": "XMLHttpRequest",
-            "Cookie": "scratchcsrftoken="
-                      + self.csrf_token
-                      + ";scratchlanguage=en;scratchsessionsid="
-                      + self.session_id
-                      + ";",
+            "Cookie": f"scratchcsrftoken={self.csrf_token};scratchlanguage=en;scratchsessionsid={self.session_id};",
             "referer": "https://scratch.mit.edu",
         }
 
     def _get_csrf_token(self):
         headers = {
             "x-requested-with": "XMLHttpRequest",
             "Cookie": "scratchlanguage=en;permissions=%7B%7D;",
@@ -141,16 +128,16 @@
         response = requests.post("https://scratch.mit.edu/session", headers={
             'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.101 Safari/537.36',
             "x-csrftoken": "a",
             "x-requested-with": "XMLHttpRequest",
             "referer": "https://scratch.mit.edu",
         }, cookies={"scratchsessionsid": self.session_id, "scratchcsrftoken": "a", "scratchlanguage": "en"}).json()
         self.token = response['user']['token']
-        self.session = response
-        if self.session["user"]["banned"]:
+        self.scratch_session = response
+        if self.scratch_session["user"]["banned"]:
             raise Exceptions.UnauthorizedAction(
                 "You are banned on Scratch! You cannot login from ScratchConnect unless you are unbanned! This error is raised because ScratchConnect won't allow the banned users to login and do something inappropriate!")
 
     def _cookie_login(self):
         if self.cookie is None:
             raise Exceptions.InvalidInfo("Cookie Not Provided!")
         try:
@@ -158,18 +145,18 @@
             self.session_id = self.cookie["SessionID"]
         except KeyError:
             raise Exceptions.InvalidInfo("Required Cookie Headers are missing!")
         try:
             self._get_token()
             self._get_csrf_token()
             Warnings.warn(
-                "[1m[33mScratchConnect: [31mYou are logging in with cookie. Some features might not work if the cookie values are wrong![0m")
+                "[1m[33mScratchConnect Warning: [31mYou are logging in with cookie. Some features might not work if the cookie values are wrong![0m")
         except KeyError:
             Warnings.warn(
-                "[1m[33mScratchConnect: [31mCookie Login Failed because the cookie values may be wrong![0m")
+                "[1m[33mScratchConnect Warning: [31mCookie Login Failed because the cookie values may be wrong![0m")
             self.csrf_token = ""
             self.token = ""
 
     def _online_ide_login(self):
         if self.online_ide_cookie is None:
             raise Exceptions.InvalidInfo("Cookie Info Not Provided!")
         try:
@@ -177,337 +164,274 @@
             self.session_id = self.online_ide_cookie["SessionID"]
         except KeyError:
             raise Exceptions.InvalidInfo("Required Cookie Headers are missing!")
         try:
             self._get_token()
             self._get_csrf_token()
             Warnings.warn(
-                "[1m[33mScratchConnect: [31mYou are logging in on Replit or some other online IDE. Some features might not work if the cookie values are wrong or it may be slow! Also, you can't do any social interactions![0m")
+                "[1m[33mScratchConnect Warning: [31mYou are logging in on Replit or some other online IDE. Some features might not work if the cookie values are wrong or it may be slow! Also, you can't do any social interactions![0m")
         except (KeyError, TypeError, ValueError):
             Warnings.warn(
-                "[1m[33mScratchConnect: [31mFetching token or csrf_token failed! You can still continue but social interactions won't work![0m")
+                "[1m[33mScratchConnect Warning: [31mFetching token or csrf_token failed! You can still continue but social interactions won't work![0m")
             self.csrf_token = ""
             self.token = ""
 
-    def check(self, username):
+    def check(self, username) -> None:
         try:
-            requests.get(f"https://{_api}/users/{username}").json()["id"]
+            self.session.get(f"https://{_api}/users/{username}").json()["id"]
         except KeyError:
             raise Exceptions.InvalidUser(f"Username '{username}' doesn't exist!")
 
-    def messages(self, all=False, limit=20, offset=0, filter="all"):
+    def messages(self, all: bool = False, limit: int = 20, offset: int = 0, filter: str = "all") -> dict:
         """
         Get the list of messages
         :param all: True if you want all the messages
         :param limit: The limit of the messages
         :param offset: The number of messages to be skipped from the beginning
         :param filter: Filter the messages
         :return: The list of the messages
         """
         if self._logged_in is False:
             raise Exceptions.UnauthorizedAction("Cannot perform the action because the user is not logged in!")
-        headers = {
-            "x-csrftoken": self.csrf_token,
-            "X-Token": self.token,
-            "x-requested-with": "XMLHttpRequest",
-            "Cookie": "scratchcsrftoken="
-                      + self.csrf_token
-                      + ";scratchlanguage=en;scratchsessionsid="
-                      + self.session_id
-                      + ";",
-            "referer": "https://scratch.mit.edu",
-        }
+
         if self.user_messages is None:
             messages = []
             if all:
                 offset = 0
                 while True:
-                    request = requests.get(
-                        f"https://api.scratch.mit.edu/users/{self.username}/messages/?limit=40&offset={offset}&filter={filter}",
-                        headers=headers).json()
-                    messages.append(request)
-                    if len(request) != 40:
+                    response = self.session.get(
+                        f"https://api.scratch.mit.edu/users/{self.username}/messages/?limit=40&offset={offset}&filter={filter}").json()
+                    messages.append(response)
+                    if len(response) != 40:
                         break
                     offset += 40
             if not all:
                 for i in range(1, limit + 1):
-                    request = requests.get(
-                        f"https://api.scratch.mit.edu/users/{self.username}/messages/?limit={limit}&offset={offset}&filter={filter}",
-                        headers=headers).json()
-                    messages.append(request)
+                    response = self.session.get(
+                        f"https://api.scratch.mit.edu/users/{self.username}/messages/?limit={limit}&offset={offset}&filter={filter}").json()
+                    messages.append(response)
             self.user_messages = messages
         return self.user_messages
 
-    def clear_messages(self):
+    def clear_messages(self) -> str:
         """
         Clear the messages
         """
         if self._logged_in is False:
             raise Exceptions.UnauthorizedAction("Cannot perform the action because the user is not logged in!")
-        return requests.post(f"https://scratch.mit.edu/site-api/messages/messages-clear/", headers=self.headers).text
+        return self.session.post(f"https://scratch.mit.edu/site-api/messages/messages-clear/").text
 
-    def my_stuff_projects(self, order="all", page=1, sort_by=""):
+    def my_stuff_projects(self, order: str = "all", page: int = 1, sort_by: str = "") -> dict:
         """
         Get the projects in the MyStuff section of the logged in user
         :param order: the order
         :param page: the page
         :param sort_by: sort
         """
         if self._logged_in is False:
             raise Exceptions.UnauthorizedAction("Cannot perform the action because the user is not logged in!")
-        return requests.get(
-            f"https://scratch.mit.edu/site-api/projects/{order}/?page={page}&ascsort=&descsort={sort_by}",
-            headers=self.headers).json()
+        return self.session.get(
+            f"https://scratch.mit.edu/site-api/projects/{order}/?page={page}&ascsort=&descsort={sort_by}").json()
 
-    def toggle_commenting(self):
+    def toggle_commenting(self) -> Response:
         """
         Toggle the commenting of the profile
         """
-        return requests.post(
-            "https://scratch.mit.edu/site-api/comments/user/"
-            + self.username
-            + "/toggle-comments/",
-            headers=self.headers,
-        )
+        return self.session.post(f"https://scratch.mit.edu/site-api/comments/user/{self.username}/toggle-comments/")
 
-    def follow_user(self, username):
+    def follow_user(self, username: str) -> Response:
         """
         Follow a user
         :param username: The username
         """
         self.check(username)
         if username == self.username:
             raise Exceptions.UnauthorizedAction(f"You can't follow yourself!")
-        return requests.put(
-            "https://scratch.mit.edu/site-api/users/followers/"
-            + username
-            + "/add/?usernames="
-            + self.username,
-            headers=self.headers,
-        )
+        return self.session.put(
+            f"https://scratch.mit.edu/site-api/users/followers/{username}/add/?usernames={self.username}")
 
-    def unfollow_user(self, username):
+    def unfollow_user(self, username: str) -> Response:
         """
         UnFollow a user
         :param username: The username
         """
         self.check(username)
         if username == self.username:
             raise Exceptions.UnauthorizedAction(f"You can't unfollow yourself!")
-        return requests.put(
-            "https://scratch.mit.edu/site-api/users/followers/"
-            + username
-            + "/remove/?usernames="
-            + self.username,
-            headers=self.headers,
-        )
+        return self.session.put(
+            f"https://scratch.mit.edu/site-api/users/followers/{username}/remove/?usernames={self.username}")
 
-    def set_bio(self, content):
+    def set_bio(self, content: str) -> Response:
         """
         Set the bio or 'About Me' of the profile
         :param content: The bio or the content.
         Thanks to QuantumCodes for helping me in the error!
         """
         data = json.dumps({"bio": content})
-        return requests.put(f"https://scratch.mit.edu/site-api/users/all/{self.username}/",
-                            data=data,
-                            headers=self.headers,
-                            )
+        return self.session.put(f"https://scratch.mit.edu/site-api/users/all/{self.username}/", data=data)
 
-    def set_work(self, content):
+    def set_work(self, content: str) -> Response:
         """
         Set the status or 'What I am Working On' of the profile
         :param content: The work or the content.
         Thanks to QuantumCodes for helping me in the error!
         """
         data = json.dumps({"status": content})
-        return requests.put(f"https://scratch.mit.edu/site-api/users/all/{self.username}/",
-                            data=data,
-                            headers=self.headers,
-                            )
+        return self.session.put(f"https://scratch.mit.edu/site-api/users/all/{self.username}/", data=data)
 
-    def _check_project(self, project_id):
+    def _check_project(self, project_id: int) -> None:
         """
         Don't use this function
         """
         try:
-            json.loads(requests.get(f"https://api.scratch.mit.edu/projects/{project_id}/").text)["id"]
+            self.session.get(f"https://api.scratch.mit.edu/projects/{project_id}/").json()["id"]
         except KeyError:
             raise Exceptions.InvalidProject(f"The project with ID - '{project_id}' doesn't exist!")
 
-    def feed(self, limit=40, offset=0):
+    def feed(self, limit: int = 40, offset: int = 0) -> dict:
         """
         Returns the "What's Happening" section of the front page
         :param limit: the limit; max: 40
         :param offset: the offset
         """
         if self._logged_in is False:
             raise Exceptions.UnauthorizedAction("Cannot perform the action because the user is not logged in!")
-        return requests.get(
-            f"https://api.scratch.mit.edu/users/{self.username}/following/users/activity?limit={limit}&offset={offset}",
-            headers=self.headers).json()
+        return self.session.get(
+            f"https://api.scratch.mit.edu/users/{self.username}/following/users/activity?limit={limit}&offset={offset}").json()
 
-    def site_health(self):
+    def site_health(self) -> dict:
         """
         Returns the health of the Scratch Website.
         """
-        return requests.get("https://api.scratch.mit.edu/health").json()
+        return self.session.get("https://api.scratch.mit.edu/health").json()
 
-    def site_news(self):
+    def site_news(self) -> dict:
         """
         Returns the news of the Scratch Website.
         """
-        return requests.get("https://api.scratch.mit.edu/news").json()
+        return self.session.get("https://api.scratch.mit.edu/news").json()
 
-    def site_front_page_projects(self):
+    def site_front_page_projects(self) -> dict:
         """
         Returns the front page projects of the Scratch Website.
         """
-        return requests.get("https://api.scratch.mit.edu/proxy/featured").json()
+        return self.session.get("https://api.scratch.mit.edu/proxy/featured").json()
 
-    def explore_projects(self, mode="trending", query="*"):
+    def explore_projects(self, mode: str = "trending", query: str = "*") -> dict:
         """
         Explore the projects
         :param mode: The mode such as 'popular' or 'trending'
         :param query: The query
         """
-        return requests.get(
-            "https://api.scratch.mit.edu/explore/projects/?mode="
-            + mode
-            + "&q="
-            + query
-        ).json()
+        return self.session.get(f"https://api.scratch.mit.edu/explore/projects/?mode={mode}&q={query}").json()
 
-    def explore_studios(self, mode="trending", query="*"):
+    def explore_studios(self, mode: str = "trending", query: str = "*") -> dict:
         """
         Explore the studios
         :param mode: The mode such as 'popular' or 'trending'
         :param query: The query
         """
-        return json.loads(requests.get(
-            "https://api.scratch.mit.edu/explore/studios/?mode="
-            + mode
-            + "&q="
-            + query
-        ).text)
+        return self.session.get(f"https://api.scratch.mit.edu/explore/studios/?mode={mode}&q={query}").json()
 
-    def search_projects(self, mode="trending", search="*"):
+    def search_projects(self, mode: str = "trending", search: str = "*") -> dict:
         """
         Search the projects
         :param mode: The mode such as 'popular' or 'trending'
         :param query: The query
         """
-        return json.loads(requests.get(
-            "https://api.scratch.mit.edu/search/projects/?mode="
-            + mode
-            + "&q="
-            + search
-        ).text)
+        return self.session.get(f"https://api.scratch.mit.edu/search/projects/?mode={mode}&q={search}").json()
 
-    def search_studios(self, mode="trending", search="*"):
+    def search_studios(self, mode: str = "trending", search: str = "*") -> dict:
         """
         Search the studios
         :param mode: The mode such as 'popular' or 'trending'
         :param query: The query
         """
-        return json.loads(requests.get(
-            "https://api.scratch.mit.edu/search/studios/?mode="
-            + mode
-            + "&q="
-            + search
-        ).text)
+        return self.session.get(f"https://api.scratch.mit.edu/search/studios/?mode={mode}&q={search}").json()
 
-    def set_featured_project(self, project_id, label='featured_project'):
+    def set_featured_project(self, project_id: int, label: str = "featured_project") -> dict:
         """
         Set the 'Featured Project' of a Scratch Profile
         :param project_id: The project id
         :param label: The Label, options:
                 "featured_project": "",
                 "featured_tutorial": 0,
                 "work_in_progress": 1,
                 "remix_this": 2,
                 "my_favorite_things": 3,
                 "why_i_scratch": 4,
         """
         if self._logged_in is False:
             raise Exceptions.UnauthorizedAction("Cannot perform the action because the user is not logged in!")
         self._check_project(project_id)
-        if not requests.get(f"https://api.scratch.mit.edu/projects/{project_id}/").json()["author"][
+        if not self.session.get(f"https://api.scratch.mit.edu/projects/{project_id}/").json()["author"][
                    "username"] == self.username:
             raise Exceptions.UnauthorizedAction(
                 f"The project with ID - '{project_id}' cannot be set because the owner of that project is not '{self.username}'!")
         _label = (
             {
                 "featured_project": "",
                 "featured_tutorial": 0,
                 "work_in_progress": 1,
                 "remix_this": 2,
                 "my_favorite_things": 3,
                 "why_i_scratch": 4,
             }
         )[label]
         data = {"featured_project": project_id, "featured_project_label": _label}
-        return requests.put(f"https://scratch.mit.edu/site-api/users/all/{self.username}/",
-                            data=json.dumps(data),
-                            headers=self.headers,
-                            ).json()
+        return self.session.put(f"https://scratch.mit.edu/site-api/users/all/{self.username}/",
+                                data=json.dumps(data)).json()
 
-    def search_forum(self, q, order="relevance", page=0):
+    def search_forum(self, q: str, order: str = "relevance", page: int = 0) -> dict:
         """
         Search the forum
         :param q: query
         :param order: The order. Use values like "relevance", "newest", "oldest"
         :param page: page
         """
         return requests.get(f"https://scratchdb.lefty.one/v3/forum/search?q={q}&o={order}&page={page}").json()
 
-    def connect_user(self, username):
+    def connect_user(self, username: str) -> User.User:
         """
         Connect a Scratch User
         :param username: A valid Username
         """
-        return User.User(username=username, client_username=self.username, headers=self.headers,
+        return User.User(username=username, client_username=self.username, session=self.session,
                          logged_in=self._logged_in, online_ide=self._online_ide)
 
-    def connect_studio(self, studio_id):
+    def connect_studio(self, studio_id: int) -> Studio.Studio:
         """
         Connect a Scratch Studio
         :param studio_id: A valid studio ID
         """
-        return Studio.Studio(id=studio_id, client_username=self.username, headers=self.headers,
+        return Studio.Studio(id=studio_id, client_username=self.username, session=self.session,
                              logged_in=self._logged_in, online_ide=self._online_ide)
 
-    def connect_project(self, project_id, access_unshared=False):
+    def connect_project(self, project_id: int, access_unshared: bool = False) -> Project.Project:
         """
         Connect a Scratch Project
         :param project_id: A valid project ID
         :param access_unshared: Set to True if you want to connect an unshared project
         """
-        return Project.Project(id=project_id, client_username=self.username, headers=self.headers,
+        return Project.Project(id=project_id, client_username=self.username, session=self.session,
                                logged_in=self._logged_in, unshared=access_unshared, session_id=self.session_id,
                                online_ide=self._online_ide)
 
-    def connect_forum_topic(self, forum_id):
+    def connect_forum_topic(self, forum_id: int) -> Forum.Forum:
         """
         Connect a Scratch Forum Topic
         :param forum_id: A valid forum topic ID
         """
         return Forum.Forum(id=forum_id, client_username=self.username, headers=self.headers, logged_in=self._logged_in,
-                           online_ide=self._online_ide)
+                           online_ide=self._online_ide, session=self.session)
 
-    def create_new_terminal(self):
+    def create_new_terminal(self) -> _terminal:
         """
         Create a new Terminal object
         """
         return _terminal(sc=self)
 
-    def create_new_chart(self):
-        """
-        Create a new Chart object
-        """
-        return _chart(sc=self)
-
-    def create_new_image(self):
+    def create_new_image(self) -> Image:
         """
         Create a new scImage object
         """
         return Image(online_ide=self._online_ide)
```

### Comparing `scratchconnect-4.5.2/scratchconnect/Studio.py` & `scratchconnect-5.0/scratchconnect/Studio.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 """
 The Studio File
 """
 import requests
+from requests.models import Response
 import json
 
 import scratchconnect.ScratchConnect
 from scratchconnect.scOnlineIDE import _change_request_url
 from scratchconnect import Exceptions
 
 _website = "scratch.mit.edu"
 _login = f"https://{_website}/login/"
 _api = f"https://api.{_website}"
 
 
 class Studio:
-    def __init__(self, id, client_username, headers, logged_in, online_ide):
+    def __init__(self, id, client_username, session, logged_in, online_ide):
         """
         The Studio Class
         :param id: The ID of the studio
         """
         self.client_username = client_username
         self._logged_in = logged_in
         self.studio_id = str(id)
-        self.headers = headers
+        self.session = session
+        self.session.headers["referer"] = f"https://scratch.mit.edu/studios/{self.studio_id}"
         if online_ide:
             _change_request_url()
         self.update_data()
 
-    def update_data(self):
+    def update_data(self) -> None:
         """
         Update the studio data
         """
         self.studio_title = None
         self.studio_owner = None
         self.studio_description = None
         self.studio_visibility = None
@@ -41,15 +43,15 @@
         self.studio_thumbnail_url = None
         self.studio_projects = None
         self.studio_comments = None
         self.studio_curators = None
         self.studio_managers = None
         self.studio_activity = None
 
-        data = requests.get(f"{_api}/studios/{self.studio_id}").json()
+        data = self.session.get(f"{_api}/studios/{self.studio_id}").json()
         try:
             self.studio_id = data["id"]
         except KeyError:
             raise Exceptions.InvalidStudio(f"Studio with ID - '{self.studio_id}' doesn't exist!")
         self.studio_title = data["title"]
         self.studio_owner = data["host"]
         self.studio_description = data["description"]
@@ -57,475 +59,470 @@
         self.studio_is_public = data["public"] == True
         self.studio_is_open_to_all = data["open_to_all"] == True
         self.studio_are_comments_allowed = data["comments_allowed"] == True
         self.studio_history = data["history"]
         self.studio_stats = data["stats"]
         self.studio_thumbnail_url = data["image"]
 
-    def _check_project(self, project_id):
+    def _check_project(self, project_id: int) -> None:
         """
         Don't use this function
         """
         try:
             requests.get(f"https://api.scratch.mit.edu/projects/{project_id}/").json()["id"]
         except KeyError:
             raise Exceptions.InvalidProject(f"The project with ID - '{project_id}' doesn't exist!")
 
-    def _check_username(self, username):
+    def _check_username(self, username) -> None:
         """
         Don't use this function
         """
         try:
             requests.get(f"{_api}/users/{username}").json()["id"]
         except KeyError:
             raise scratchconnect.Exceptions.InvalidUser(f"Username '{username}' doesn't exist!")
 
-    def user_id(self, username):
+    def user_id(self, username) -> int:
         """
         Returns the user ID
         :param username: Username
         """
-        return requests.get(f"{_api}/users/{username}").json()["id"]
+        return self.session.get(f"{_api}/users/{username}").json()["id"]
 
-    def id(self):
+    def id(self) -> int:
         """
         Returns the studio ID
         """
         if self.studio_id is None:
             self.update_data()
         return self.studio_id
 
-    def title(self):
+    def title(self) -> str:
         """
         Returns the studio title
         """
         if self.studio_title is None:
             self.update_data()
         return self.studio_title
 
-    def host_id(self):
+    def host_id(self) -> int:
         """
         Returns the studio owner/host ID
         """
         if self.studio_owner is None:
             self.update_data()
         return self.studio_owner
 
-    def description(self):
+    def description(self) -> str:
         """
         Returns the studio description
         """
         if self.studio_description is None:
             self.update_data()
         return self.studio_description
 
-    def visibility(self):
+    def visibility(self) -> str:
         """
         Returns the studio visibility
         """
         if self.studio_visibility is None:
             self.update_data()
         return self.studio_visibility
 
-    def is_public(self):
+    def is_public(self) -> bool:
         """
         Returns whether a studio is public
         """
         if self.studio_is_public is None:
             self.update_data()
         return self.studio_is_public
 
-    def is_open_to_all(self):
+    def is_open_to_all(self) -> bool:
         """
         Returns whether a studio is open to all
         """
         if self.studio_is_open_to_all is None:
             self.update_data()
         return self.studio_is_open_to_all
 
-    def are_comments_allowed(self):
+    def are_comments_allowed(self) -> bool:
         """
         Returns whether a studio has comments allowed
         """
         if self.studio_are_comments_allowed is None:
             self.update_data()
         return self.studio_are_comments_allowed
 
-    def history(self):
+    def history(self) -> dict:
         """
         Returns the history of the studio
         """
         if self.studio_history is None:
             self.update_data()
         return self.studio_history
 
-    def stats(self):
+    def stats(self) -> dict:
         """
         Returns the stats of the studio
         """
         if self.studio_stats is None:
             self.update_data()
         return self.studio_stats
 
-    def thumbnail_url(self):
+    def thumbnail_url(self) -> str:
         """
         Returns the thumbnail URL of the studio
         """
         if self.studio_thumbnail_url is None:
             self.update_data()
         return self.studio_thumbnail_url
 
-    def add_project(self, project_id):
+    def add_project(self, project_id) -> dict:
         """
         Add a project to a studio
         :param project_id: The project ID
         """
         if self._logged_in is False:
             raise Exceptions.UnauthorizedAction("Cannot perform the action because the user is not logged in!")
         self._check_project(project_id)
-        headers = self.headers
-        headers["referer"] = f"https://scratch.mit.edu/projects/{project_id}/"
-        return requests.post(f"https://api.scratch.mit.edu/studios/{self.studio_id}/project/{project_id}/",
-                             headers=headers,
-                             ).json()
+        headers = {"referer": f"https://scratch.mit.edu/projects/{project_id}/"}
+        return self.session.post(f"https://api.scratch.mit.edu/studios/{self.studio_id}/project/{project_id}/",
+                                 headers=headers).json()
 
-    def remove_project(self, project_id):
+    def remove_project(self, project_id) -> dict:
         """
         Remove a project from a studio
         :param project_id: The project ID
         """
         if self._logged_in is False:
             raise Exceptions.UnauthorizedAction("Cannot perform the action because the user is not logged in!")
         self._check_project(project_id)
-        headers = self.headers
-        headers["referer"] = f"https://scratch.mit.edu/projects/{project_id}/"
-        return requests.post(
-            "https://api.scratch.mit.edu/studios/"
-            + str(self.studio_id)
-            + "/project/"
-            + str(project_id)
-            + "/",
-            headers=headers,
-        ).json()
+        headers = {"referer": f"https://scratch.mit.edu/projects/{project_id}/"}
+        return self.session.post(f"https://api.scratch.mit.edu/studios/{self.studio_id}/project/{project_id}/",
+                                 headers=headers).json()
 
-    def open_to_public(self):
+    def open_to_public(self) -> dict:
         """
         Open the studio to public
         """
         if self._logged_in is False:
             raise Exceptions.UnauthorizedAction("Cannot perform the action because the user is not logged in!")
-        return requests.put(
-            f"https://scratch.mit.edu/site-api/galleries/{self.studio_id}/mark/open/",
-            headers=self.headers,
-        ).json()
+        return self.session.put(
+            f"https://scratch.mit.edu/site-api/galleries/{self.studio_id}/mark/open/").json()
 
-    def close_to_public(self):
+    def close_to_public(self) -> dict:
         """
         Close the studio to public
         """
         if self._logged_in is False:
             raise Exceptions.UnauthorizedAction("Cannot perform the action because the user is not logged in!")
         return requests.put(
-            f"https://scratch.mit.edu/site-api/galleries/{self.studio_id}/mark/closed/",
-            headers=self.headers,
-        ).json()
+            f"https://scratch.mit.edu/site-api/galleries/{self.studio_id}/mark/closed/").json()
 
-    def follow_studio(self):
+    def follow_studio(self) -> dict:
         """
         Follow the studio
         """
         if self._logged_in is False:
             raise Exceptions.UnauthorizedAction("Cannot perform the action because the user is not logged in!")
-        return requests.put(
-            f"https://scratch.mit.edu/site-api/users/bookmarkers/{self.studio_id}/add/?usernames={self.client_username}",
-            headers=self.headers,
-        ).json()
+        return self.session.put(
+            f"https://scratch.mit.edu/site-api/users/bookmarkers/{self.studio_id}/add/?usernames={self.client_username}").json()
 
-    def unfollow_studio(self):
+    def unfollow_studio(self) -> dict:
         """
         UnFollow the studio
         """
         if self._logged_in is False:
             raise Exceptions.UnauthorizedAction("Cannot perform the action because the user is not logged in!")
-        return requests.put(
-            f"https://scratch.mit.edu/site-api/users/bookmarkers/{self.studio_id}/remove/?usernames={self.client_username}",
-            headers=self.headers,
-        ).json()
+        return self.session.put(
+            f"https://scratch.mit.edu/site-api/users/bookmarkers/{self.studio_id}/remove/?usernames={self.client_username}").json()
 
-    def toggle_commenting(self):
+    def toggle_commenting(self) -> str:
         """
         Toggle the commenting of the studio
         """
         if self._logged_in is False:
             raise Exceptions.UnauthorizedAction("Cannot perform the action because the user is not logged in!")
-        headers = self.headers
-        headers["referer"] = (
-            f"https://scratch.mit.edu/studios/{self.studio_id}/comments/"
-        )
-        return requests.post(f"https://scratch.mit.edu/site-api/comments/gallery/{self.studio_id}/toggle-comments/",
-                             headers=headers,
-                             ).text
+        headers = {"referer": f"https://scratch.mit.edu/studios/{self.studio_id}/comments/"}
+        return self.session.post(f"https://scratch.mit.edu/site-api/comments/gallery/{self.studio_id}/toggle-comments/",
+                                 headers=headers).text
 
-    def post_comment(self, content, parent_id="", commentee_id=""):
+    def post_comment(self, content: str, parent_id: int = "", commentee_id: int = "") -> Response:
         """
         Post comment in the studio
         :param content: The comment
         """
         if self._logged_in is False:
             raise Exceptions.UnauthorizedAction("Cannot perform the action because the user is not logged in!")
-        headers = self.headers
-        headers["referer"] = (f"https://scratch.mit.edu/studios/{self.studio_id}/comments/"
-                              )
+        headers = {"referer": f"https://scratch.mit.edu/studios/{self.studio_id}/comments/"}
         data = {
             "commentee_id": commentee_id,
             "content": content,
             "parent_id": parent_id,
         }
-        return requests.post(f"https://scratch.mit.edu/site-api/comments/gallery/{self.studio_id}/add/",
-                             headers=headers,
-                             data=json.dumps(data),
-                             )
+        return self.session.post(f"https://scratch.mit.edu/site-api/comments/gallery/{self.studio_id}/add/",
+                                 headers=headers,
+                                 data=json.dumps(data)
+                                 )
 
-    def reply_comment(self, content, comment_id):
+    def reply_comment(self, content: str, comment_id: int) -> Response:
         """
         Reply a comment
         :param content: The content
         :param comment_id: The comment ID
         """
         if self._logged_in is False:
             raise Exceptions.UnauthorizedAction("Cannot perform the action because the user is not logged in!")
         return self.post_comment(content=content, parent_id=comment_id)
 
-    def delete_comment(self, comment_id):
+    def delete_comment(self, comment_id: int) -> Response:
         """
         Delete comment in the studio
         :param comment_id: The comment ID
         """
         if self._logged_in is False:
             raise Exceptions.UnauthorizedAction("Cannot perform the action because the user is not logged in!")
-        headers = self.headers
-        headers["referer"] = (f"https://scratch.mit.edu/studios/{self.studio_id}/comments/")
+        headers = {"referer": f"https://scratch.mit.edu/studios/{self.studio_id}/comments/"}
         data = {"id": comment_id}
-        return requests.post(f"https://scratch.mit.edu/site-api/comments/user/{self.client_username}/del/",
-                             headers=headers,
-                             data=json.dumps(data),
-                             )
+        return self.session.post(f"https://scratch.mit.edu/site-api/comments/user/{self.client_username}/del/",
+                                 headers=headers, data=json.dumps(data))
 
-    def report_comment(self, comment_id):
+    def report_comment(self, comment_id: int) -> Response:
         """
         Report comment in the studio
         :param comment_id: The comment ID
         """
         if self._logged_in is False:
             raise Exceptions.UnauthorizedAction("Cannot perform the action because the user is not logged in!")
-        headers = self.headers
-        headers["referer"] = (f"https://scratch.mit.edu/studios/{self.studio_id}/comments/")
+        headers = {"referer": f"https://scratch.mit.edu/studios/{self.studio_id}/comments/"}
         data = {"id": comment_id}
-        return requests.post(f"https://scratch.mit.edu/site-api/comments/user/{self.client_username}/rep/",
-                             headers=headers,
-                             data=json.dumps(data),
-                             )
+        return self.session.post(f"https://scratch.mit.edu/site-api/comments/user/{self.client_username}/rep/",
+                                 headers=headers, data=json.dumps(data))
 
-    def invite_curator(self, username):
+    def invite_curator(self, username: str) -> Response:
         """
         Invite a user to the studio
         :param username: The Username
         """
         if self._logged_in is False:
             raise Exceptions.UnauthorizedAction("Cannot perform the action because the user is not logged in!")
         self._check_username(username)
-        headers = self.headers
-        headers["referer"] = (f"https://scratch.mit.edu/studios/{self.studio_id}/curators/")
-        return requests.put(
+        headers = {"referer": f"https://scratch.mit.edu/studios/{self.studio_id}/curators/"}
+        return self.session.put(
             f"https://scratch.mit.edu/site-api/users/curators-in/{self.studio_id}/invite_curator/?usernames={username}",
-            headers=headers,
-        )
+            headers=headers)
+
+    def remove_curator(self, username: str) -> Response:
+        """
+        Remove a user from the studio
+        :param username: The Username
+        """
+        if self._logged_in is False:
+            raise Exceptions.UnauthorizedAction("Cannot perform the action because the user is not logged in!")
+        self._check_username(username)
+        headers = {"referer": f"https://scratch.mit.edu/studios/{self.studio_id}/curators/"}
+        return self.session.put(
+            f"https://scratch.mit.edu/site-api/users/curators-in/{self.studio_id}/remove/?usernames={username}",
+            headers=headers)
 
-    def accept_curator(self):
+    def accept_curator(self) -> Response:
         """
         Accept the curator invitation in a studio
         """
         if self._logged_in is False:
             raise Exceptions.UnauthorizedAction("Cannot perform the action because the user is not logged in!")
-        headers = self.headers
-        headers["referer"] = (f"https://scratch.mit.edu/studios/{self.studio_id}/curators/")
-        return requests.put(
+        headers = {"referer": f"https://scratch.mit.edu/studios/{self.studio_id}/curators/"}
+        return self.session.put(
             f"https://scratch.mit.edu/site-api/users/curators-in/{self.studio_id}/add/?usernames={self.client_username}",
-            headers=headers,
-        )
+            headers=headers)
 
-    def promote_curator(self, username):
+    def promote_curator(self, username: str) -> Response:
         """
         Promote a user in the studio
         :param username: The Username
         """
         if self._logged_in is False:
             raise Exceptions.UnauthorizedAction("Cannot perform the action because the user is not logged in!")
         self._check_username(username)
-        headers = self.headers
-        headers["referer"] = (
-                "https://scratch.mit.edu/studios/" + str(self.studio_id) + "/curators/"
-        )
-        return requests.put(
+        headers = {"referer": f"https://scratch.mit.edu/studios/{self.studio_id}/curators/"}
+        return self.session.put(
             f"https://scratch.mit.edu/site-api/users/curators-in/{self.studio_id}/promote/?usernames={username}",
-            headers=headers,
-        )
+            headers=headers)
 
-    def set_description(self, content):
+    def set_description(self, content: str) -> dict:
         """
         Set the description of a Studio
         :param content: The description or content
         """
         if self._logged_in is False:
             raise Exceptions.UnauthorizedAction("Cannot perform the action because the user is not logged in!")
-        data = {"description": content}
-        return requests.put(f"https://scratch.mit.edu/site-api/galleries/all/{self.studio_id}/",
-                            headers=self.headers,
-                            data=json.dumps(data),
-                            ).json()
+        data = json.dumps({"description": content})
+        return self.session.put(f"https://scratch.mit.edu/site-api/galleries/all/{self.studio_id}/",
+                                data=data).json()
 
-    def set_title(self, content):
+    def set_title(self, content: str) -> dict:
         """
         Set the title of a Studio
         :param content: The title or content
         """
         if self._logged_in is False:
             raise Exceptions.UnauthorizedAction("Cannot perform the action because the user is not logged in!")
-        data = {"title": content}
-        return requests.put(f"https://scratch.mit.edu/site-api/galleries/all/{self.studio_id}/",
-                            headers=self.headers,
-                            data=json.dumps(data),
-                            ).json()
+        data = json.dumps({"title": content})
+        return self.session.put(f"https://scratch.mit.edu/site-api/galleries/all/{self.studio_id}/",
+                                data=data).json()
 
-    def projects(self, all=False, limit=20, offset=0):
+    def projects(self, all: bool = False, limit: int = 20, offset: int = 0) -> list:
         """
         Get the projects of the studio
         :param all: If you want all the projects then set it to True
         :param limit: The limit
         :param offset: The offset or the number of data you want from the beginning
         """
         if self.studio_projects is None:
             projects = []
             if all:
                 limit = 40
                 offset = 0
                 while True:
-                    response = json.loads(requests.get(
-                        f"https://api.scratch.mit.edu/studios/{self.studio_id}/projects/?limit={limit}&offset={offset}").text)
+                    response = self.session.get(
+                        f"https://api.scratch.mit.edu/studios/{self.studio_id}/projects/?limit={limit}&offset={offset}").json()
                     projects.append(response)
                     offset += 40
                     if len(response) != 40:
                         break
             if not all:
-                projects.append(json.loads(requests.get(
-                    f"https://api.scratch.mit.edu/studios/{self.studio_id}/projects/?limit={limit}&offset={offset}").text))
+                projects.append(self.session.get(
+                    f"https://api.scratch.mit.edu/studios/{self.studio_id}/projects/?limit={limit}&offset={offset}").json())
             self.studio_projects = projects
         return self.studio_projects
 
-    def comments(self, all=False, limit=20, offset=0):
+    def comments(self, all: bool = False, limit: int = 20, offset: int = 0) -> list:
         """
         Get the comments of the studio
         :param all: If you want all the comments then set it to True
         :param limit: The limit
         :param offset: The offset or the number of data you want from the beginning
         """
         if self.studio_comments is None:
             comments = []
             if all:
                 limit = 40
                 offset = 0
                 while True:
-                    response = json.loads(requests.get(
-                        f"https://api.scratch.mit.edu/studios/{self.studio_id}/comments/?limit={limit}&offset={offset}").text)
+                    response = self.session.get(
+                        f"https://api.scratch.mit.edu/studios/{self.studio_id}/comments/?limit={limit}&offset={offset}").json()
                     comments.append(response)
                     offset += 40
                     if len(response) != 40:
                         break
             if not all:
-                comments.append(json.loads(requests.get(
-                    f"https://api.scratch.mit.edu/studios/{self.studio_id}/comments/?limit={limit}&offset={offset}").text))
+                comments.append(self.session.get(
+                    f"https://api.scratch.mit.edu/studios/{self.studio_id}/comments/?limit={limit}&offset={offset}").json())
             self.studio_comments = comments
         return self.studio_comments
 
-    def curators(self, all=False, limit=20, offset=0):
+    def comment_replies(self, comment_id: int, limit: int = 20, offset: int = 0) -> list:
+        """
+        Get the comment replies from the comment ID
+        :param comment_id: The comment ID
+        :param limit: The limit (max: 40)
+        :param offset: The offset or the number of replies to skip from the beginning
+        """
+        return self.session.get(
+            f"https://api.scratch.mit.edu/studios/{self.studio_id}/comments/{comment_id}/replies?limit={limit}&offset={offset}").json()
+
+    # Doesn't work :/
+    # def set_thumbnail(self, image_path: str) -> Response:
+    #     """
+    #     Set the thumbnail of the Studio
+    #     :param image_path: The path of the image
+    #     """
+    #     if self._logged_in is False:
+    #         raise Exceptions.UnauthorizedAction("Cannot perform the action because the user is not logged in!")
+    #     with open(image_path, "rb") as f:
+    #         image = f.read()
+    #     return self.session.post(f"https://scratch.mit.edu/site-api/galleries/all/{self.studio_id}",
+    #                              data=image)
+
+    def curators(self, all: bool = False, limit: int = 20, offset: int = 0) -> list:
         """
         Get the curators of the studio
         :param all: If you want all the curators then set it to True
         :param limit: The limit
         :param offset: The offset or the number of data you want from the beginning
         """
         if self.studio_curators is None:
             curators = []
             if all:
                 limit = 40
                 offset = 0
                 while True:
-                    response = json.loads(requests.get(
-                        f"https://api.scratch.mit.edu/studios/{self.studio_id}/curators/?limit={limit}&offset={offset}").text)
+                    response = self.session.get(
+                        f"https://api.scratch.mit.edu/studios/{self.studio_id}/curators/?limit={limit}&offset={offset}").json()
                     curators.append(response)
                     offset += 40
                     if len(response) != 40:
                         break
             if not all:
-                curators.append(json.loads(requests.get(
-                    f"https://api.scratch.mit.edu/studios/{self.studio_id}/curators/?limit={limit}&offset={offset}").text))
+                curators.append(self.session.get(
+                    f"https://api.scratch.mit.edu/studios/{self.studio_id}/curators/?limit={limit}&offset={offset}").json())
             self.studio_curators = curators
         return self.studio_curators
 
-    def managers(self, all=False, limit=20, offset=0):
+    def managers(self, all: bool = False, limit: int = 20, offset: int = 0) -> list:
         """
         Get the managers of the studio
         :param all: If you want all the managers then set it to True
         :param limit: The limit
         :param offset: The offset or the number of data you want from the beginning
         """
         if self.studio_managers is None:
             managers = []
             if all:
                 limit = 40
                 offset = 0
                 while True:
-                    response = json.loads(requests.get(
-                        f"https://api.scratch.mit.edu/studios/{self.studio_id}/managers/?limit={limit}&offset={offset}").text)
+                    response = self.session.get(
+                        f"https://api.scratch.mit.edu/studios/{self.studio_id}/managers/?limit={limit}&offset={offset}").json()
                     managers.append(response)
                     offset += 40
                     if len(response) != 40:
                         break
             if not all:
-                managers.append(json.loads(requests.get(
-                    f"https://api.scratch.mit.edu/studios/{self.studio_id}/managers/?limit={limit}&offset={offset}").text))
+                managers.append(self.session.get(
+                    f"https://api.scratch.mit.edu/studios/{self.studio_id}/managers/?limit={limit}&offset={offset}").json())
             self.studio_managers = managers
         return self.studio_managers
 
-    def activity(self, all=False, limit=20, offset=0):
+    def activity(self, all: bool = False, limit: int = 20, offset: int = 0) -> list:
         """
         Get the activity of the studio
         :param all: If you want all the activity then set it to True
         :param limit: The limit
         :param offset: The offset or the number of data you want from the beginning
         """
         if self.studio_activity is None:
             activity = []
             if all:
                 limit = 40
                 offset = 0
                 while True:
-                    response = json.loads(requests.get(
-                        f"https://api.scratch.mit.edu/studios/{self.studio_id}/activity/?limit={limit}&offset={offset}").text)
+                    response = self.session.get(
+                        f"https://api.scratch.mit.edu/studios/{self.studio_id}/activity/?limit={limit}&offset={offset}").json()
                     activity.append(response)
                     offset += 40
                     if len(response) != 40:
                         break
             if not all:
-                activity.append(json.loads(requests.get(
-                    f"https://api.scratch.mit.edu/studios/{self.studio_id}/activity/?limit={limit}&offset={offset}").text))
+                activity.append(self.session.get(
+                    f"https://api.scratch.mit.edu/studios/{self.studio_id}/activity/?limit={limit}&offset={offset}").json())
             self.studio_activity = activity
-        return activity
+        return self.studio_activity
 
-    def all_data(self):
+    def all_data(self) -> dict:
         """
         Returns all the data of a Scratch Studio
         """
         data = {
             'Studio ID': self.id(),
             'Title': self.title(),
             'Host ID': self.host_id(),
```

### Comparing `scratchconnect-4.5.2/scratchconnect/TurbowarpCloudConnection.py` & `scratchconnect-5.0/scratchconnect/TurbowarpCloudConnection.py`

 * *Files 23% similar despite different names*

```diff
@@ -47,37 +47,37 @@
                 "method": "handshake",
                 "user": self.username,
                 "project_id": str(self.project_id),
             }
         )
         self._event.emit('connect')
 
-    def get_variable_data(self):
+    def get_variable_data(self) -> list:
         """
         Returns the cloud variable data
         """
         self.set_cloud_variable("@sc_temp", "123")
         data = []
         for d in self._cloud_d.split("\n"):
             one = json.loads(d)
             if one["name"] != "☁ @sc_temp":
                 data.append(one)
         if len(data) == 0:
             return None
         return data
 
-    def get_cloud_variable_value(self, variable_name, limit):
+    def get_cloud_variable_value(self, variable_name: str, limit: int) -> list:
         value = []
         data = self.get_variable_data()
         for d in data:
             if d["name"] == f"☁ {variable_name}":
                 value.append(d["value"])
         return value[0:limit]
 
-    def set_cloud_variable(self, variable_name, value):
+    def set_cloud_variable(self, variable_name: str, value: int | str) -> bool:
         """
         Set a cloud variable
         :param variable_name: Variable name
         :param value: Variable value
         """
         if str(value).isdigit() and value == '':
             raise Exceptions.InvalidCloudValue(f"The Cloud Value should be a set of digits and not '{value}'!")
@@ -101,42 +101,44 @@
             self._cloud_d = self._ws.recv()
             return True
         except (ConnectionAbortedError, BrokenPipeError, SSLEOFError, SSLError):
             self._event.emit('disconnect')
             self._make_connection()
             return False
 
-    def encode(self, text):
+    def encode(self, text: str, default: str = " ") -> str:
         """
         Encode a text. For example: A -> 1
         Go to https://scratch.mit.edu/projects/578255313/ for the Scratch Engine!
         :param text: The text to encode
+        :param default: The default value to encode when the character found is not accepted by the encoder
         """
-        return self.encoder.encode(text)
+        return self.encoder.encode(text, default=default)
 
-    def decode(self, encoded_text):
+    def decode(self, encoded_text: str | int) -> str:
         """
         Decode a text. For example: 1 -> A
         Go to https://scratch.mit.edu/projects/578255313/ for the Scratch Engine!
         :param encoded_text: The text to decode
         """
         return self.encoder.decode(encoded_text)
 
-    def encode_list(self, data):
+    def encode_list(self, data: list, default: str = " ") -> str:
         """
         Encode a Python List
-        :param data: The list
+        :param data: The list to encode
+        :param default: The default value to encode when the character found is not accepted by the encoder
         """
-        return self.encoder.encode_list(data)
+        return self.encoder.encode_list(data, default=default)
 
-    def decode_list(self, encoded_data):
+    def decode_list(self, encoded_data: str | int) -> list:
         """
         Decode a Python List
         :param encoded_data: The data to be decoded
         """
         return self.encoder.decode_list(encoded_data)
 
-    def create_cloud_event(self):
+    def create_cloud_event(self) -> CloudEvents:
         """
         Create a Cloud Event
         """
         return self._event
```

### Comparing `scratchconnect-4.5.2/scratchconnect/User.py` & `scratchconnect-5.0/scratchconnect/User.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,73 +1,69 @@
 """
 The Users File
 """
-import requests
+
+from requests.models import Response
 import json
 
 from scratchconnect.UserCommon import UserCommon
 from scratchconnect.scOnlineIDE import _change_request_url
 from scratchconnect import Exceptions
 
 _website = "scratch.mit.edu"
-_login = f"https://{_website}/login/"
 _api = f"https://api.{_website}"
 
 
 class User(UserCommon):
-    def __init__(self, username, client_username, headers, logged_in, online_ide):
+    def __init__(self, username, client_username, session, logged_in, online_ide):
         """
         The User Class to connect a Scratch user.
         :param username: The username
         """
-        super().__init__(username, headers, online_ide)  # Get other properties and methods from the parent(UserCommon) class
+        super().__init__(username, session,
+                         online_ide)  # Get other properties and methods from the parent(UserCommon) class
         self.username = username
         self.client_username = client_username
         self._logged_in = logged_in
         self._user_link = f"{_api}/users/{self.username}"
-        self.headers = headers
+        self.session = session
         if online_ide:
             _change_request_url()
         self.update_data()
 
-    def post_comment(self, content, commentee_id="", parent_id=""):
+    def post_comment(self, content: str, commentee_id: int = "", parent_id: int = "") -> Response:
         """
         Post a comment on the user's profile
         :param content: The comment
         """
         if self._logged_in is False:
             raise Exceptions.UnauthorizedAction("Cannot perform the action because the user is not logged in!")
         data = {
             "commentee_id": commentee_id,
             "content": content,
             "parent_id": parent_id,
         }
-        return requests.post(
-            f"https://scratch.mit.edu/site-api/comments/user/{self.username}/add/",
-            headers=self.headers,
-            data=json.dumps(data),
-        )
+        return self.session.post(f"https://scratch.mit.edu/site-api/comments/user/{self.username}/add/",
+                                 data=json.dumps(data))
 
-    def reply_comment(self, content, comment_id):
+    def reply_comment(self, content: str, comment_id: int) -> Response:
         """
         Reply a comment
         :param content: The message
         :param comment_id: The ID of the comment you want to reply
         """
         if self._logged_in is False:
             raise Exceptions.UnauthorizedAction("Cannot perform the action because the user is not logged in!")
         return self.post_comment(content=content, parent_id=comment_id)
 
-    def report(self, field):
+    def report(self, field: str) -> Response:
         """
         Report an user
         :param field: The field or the reason of report.
         """
         if self._logged_in is False:
             raise Exceptions.UnauthorizedAction("Cannot perform the action because the user is not logged in!")
         if self.username == self.client_username:
             raise Exceptions.UnauthorizedAction("You are not allowed to do that!")
         data = {"selected_field": field}
-        requests.post(f"https://scratch.mit.edu/site-api/users/all/{self.username}/report/",
-                      headers=self.headers,
-                      data=json.dumps(data),
-                      )
+        return self.session.post(f"https://scratch.mit.edu/site-api/users/all/{self.username}/report/",
+                                 data=json.dumps(data))
```

### Comparing `scratchconnect-4.5.2/scratchconnect/UserCommon.py` & `scratchconnect-5.0/scratchconnect/UserCommon.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,32 +5,31 @@
 import json
 import requests
 
 from scratchconnect.scOnlineIDE import _change_request_url
 from scratchconnect import Exceptions
 
 _website = "scratch.mit.edu"
-_login = f"https://{_website}/login/"
 _api = f"https://api.{_website}"
 
 
 class UserCommon:
-    def __init__(self, username, headers, online_ide):
+    def __init__(self, username, session, online_ide):
         """
         The User Class to connect a Scratch user.
         :param username: The username
         """
         self.username = username
+        self.session = session
         self._user_link = f"{_api}/users/{self.username}"
-        self.headers = headers
         if online_ide:
             _change_request_url()
         self.update_data()
 
-    def update_data(self):
+    def update_data(self) -> None:
         """
         Update the stored data
         """
         self.user_id = None
         self.user_messages_count = None
         self.user_messages = None
         self.user_work = None
@@ -46,15 +45,15 @@
         self.user_total_faves = None
         self.user_following = None
         self.user_followers = None
         self.user_favourites = None
         self.user_projects_count = None
         self.user_projects_count = None
 
-        data = requests.get(f"{self._user_link}").json()
+        data = self.session.get(f"{self._user_link}").json()
         try:
             self.user_id = data["id"]
         except KeyError:
             raise Exceptions.InvalidUser(f"Username '{self.username}' doesn't exist!")
         self.user_work = data["profile"]["status"]
         self.user_bio = data["profile"]["bio"]
         self.user_joined_date = data["history"]["joined"]
@@ -72,249 +71,250 @@
             self.user_following_count = data["statistics"]["following"]
             self.user_total_views = data["statistics"]["views"]
             self.user_total_loves = data["statistics"]["loves"]
             self.user_total_faves = data["statistics"]["favorites"]
         except json.decoder.JSONDecodeError:
             pass
 
-    def id(self):
+    def id(self) -> int:
         """
         Get the ID of a user's profile
         """
         if self.id is None:
             self.update_data()
         return self.user_id
 
-    def thumbnail_url(self):
+    def thumbnail_url(self) -> dict:
         """Return the thumbnail URL of a user"""
         if self.user_thumbnail_url is None:
             self.update_data()
         return self.user_thumbnail_url
 
-    def messages_count(self):
+    def messages_count(self) -> int:
         """
         Get the messages count of the logged in user
         """
         headers = {
             "user-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.101 Safari/537.36"}
         if self.user_messages_count is None:
             self.user_messages_count = \
-                requests.get(f"https://api.scratch.mit.edu/users/{self.username}/messages/count",
-                             headers=headers).json()[
+                self.session.get(f"https://api.scratch.mit.edu/users/{self.username}/messages/count",
+                                 headers=headers).json()[
                     "count"]
         return self.user_messages_count
 
-    def work(self):
+    def work(self) -> str:
         """
         Returns the 'What I am working on' of a Scratch profile
         """
         if self.user_work is None:
             self.update_data()
         return self.user_work
 
-    def bio(self):
+    def bio(self) -> str:
         """
         Returns the 'About me' of a Scratch profile
         """
         if self.user_bio is None:
             self.update_data()
         return self.user_bio
 
-    def status(self):
+    def status(self) -> str:
         """
         Returns the status(Scratcher or New Scratcher) of a Scratch profile
         """
         if self.user_status is None:
             self._update_db_data()
         return self.user_status
 
-    def joined_date(self):
+    def joined_date(self) -> str:
         """
         Returns the joined date of a Scratch profile
         """
         if self.user_joined_date is None:
             self.update_data()
         return self.user_joined_date
 
-    def country(self):
+    def country(self) -> str:
         """
         Returns the country of a Scratch profile
         """
         if self.user_country is None:
             self.update_data()
         return self.user_country
 
-    def followers_count(self):
+    def followers_count(self) -> int:
         """
         Returns the follower count of a user
         """
         if self.user_followers_count is None:
             self._update_db_data()
         return self.user_followers_count
 
-    def following_count(self):
+    def following_count(self) -> int:
         """
         Returns the following count of a user
         """
         if self.user_following_count is None:
             self._update_db_data()
         return self.user_following_count
 
-    def total_views(self):
+    def total_views(self) -> int:
         """
         Returns the total views count of all the shared projects of a user
         """
         if self.user_total_views is None:
             self._update_db_data()
         return self.user_total_views
 
-    def total_loves_count(self):
+    def total_loves_count(self) -> int:
         """
         Returns the total loves count of all the shared projects of a user
         """
         if self.user_total_loves is None:
             self._update_db_data()
         return self.user_total_loves
 
-    def total_favourites_count(self):
+    def total_favourites_count(self) -> int:
         """
         Returns the total favourites count of all the shared projects of a user
         """
         if self.user_total_faves is None:
             self._update_db_data()
         return self.user_total_faves
 
-    def featured_data(self):
+    def featured_data(self) -> dict:
         """
         Returns the featured project data of the Scratch profile
         """
         if self.user_featured_data is None:
-            self.user_featured_data = requests.get(f"https://scratch.mit.edu/site-api/users/all/{self.username}").json()
+            self.user_featured_data = self.session.get(
+                f"https://scratch.mit.edu/site-api/users/all/{self.username}").json()
         return self.user_featured_data
 
-    def projects(self, all=False, limit=20, offset=0):
+    def projects(self, all=False, limit=20, offset=0) -> list:
         """
         Returns the list of shared projects of a user
         :param all: If you want all then set it to True
         :param limit: The limit of the projects
         :param offset: The number of projects to be skipped from the beginning
         """
         if self.user_projects is None:
             projects = []
             if all:
                 offset = 0
                 while True:
-                    request = requests.get(
-                        f"https://api.scratch.mit.edu/users/{self.username}/projects/?limit=40&offset={offset}").json()
+                    request = self.session.get(
+                        f"{_api}/users/{self.username}/projects/?limit=40&offset={offset}").json()
                     projects.append(request)
                     if len(request) != 40:
                         break
                     offset += 40
             if not all:
                 for i in range(1, limit + 1):
-                    request = requests.get(
-                        f"https://api.scratch.mit.edu/users/{self.username}/projects/?limit={limit}&offset={offset}").json()
+                    request = self.session.get(
+                        f"{_api}/users/{self.username}/projects/?limit={limit}&offset={offset}").json()
                     projects.append(request)
             self.user_projects = projects
         return self.user_projects
 
-    def projects_count(self):
+    def projects_count(self) -> int:
         if self.user_projects_count is None:
             all_projects = self.projects(all=True)
             count = 0
             for i in all_projects:
                 count += len(i)
             self.user_projects_count = count
         return self.user_projects_count
 
-    def following(self, all=False, limit=20, offset=0):
+    def following(self, all=False, limit=20, offset=0) -> list:
         """
         Returns the list of the user following
         :param all: If you want all then set it to True
         :param limit: The limit of the users
         :param offset: The number of users to be skipped from the beginning
         """
         if self.user_following is None:
             following = []
             if all:
                 offset = 0
                 while True:
-                    response = requests.get(
-                        f"https://api.scratch.mit.edu/users/{self.username}/following/?limit=40&offset={offset}").json()
+                    response = self.session.get(
+                        f"{_api}/users/{self.username}/following/?limit=40&offset={offset}").json()
                     offset += 40
                     following.append(response)
                     if len(response) != 40:
                         break
             if not all:
-                response = requests.get(
-                    f"https://api.scratch.mit.edu/users/{self.username}/following/?limit={limit}&offset={offset}").json()
+                response = self.session.get(
+                    f"{_api}/users/{self.username}/following/?limit={limit}&offset={offset}").json()
                 following.append(response)
             self.user_following = following
         return self.user_following
 
-    def followers(self, all=False, limit=20, offset=0):
+    def followers(self, all=False, limit=20, offset=0) -> list:
         """
         Returns the list of the user followers
         :param all: If you want all then set it to True
         :param limit: The limit of the users
         :param offset: The number of users to be skipped from the beginning
         """
         if self.user_followers is None:
             followers = []
             if all:
                 offset = 0
                 while True:
-                    response = requests.get(
-                        f"https://api.scratch.mit.edu/users/{self.username}/followers/?limit=40&offset={offset}").json()
+                    response = self.session.get(
+                        f"{_api}/users/{self.username}/followers/?limit=40&offset={offset}").json()
                     offset += 40
                     followers.append(response)
                     if len(response) != 40:
                         break
             if not all:
-                response = requests.get(
-                    f"https://api.scratch.mit.edu/users/{self.username}/followers/?limit={limit}&offset={offset}").json()
+                response = self.session.get(
+                    f"{_api}/users/{self.username}/followers/?limit={limit}&offset={offset}").json()
                 followers.append(response)
             self.user_followers = followers
         return self.user_followers
 
-    def favourites(self, all=False, limit=20, offset=0):
+    def favourites(self, all=False, limit=20, offset=0) -> list:
         """
         Returns the list of the user favourites
         :param all: If you want all then set it to True
         :param limit: The limit of the projects
         :param offset: The number of projects to be skipped from the beginning
         """
         if self.user_favourites is None:
             favourites = []
             if all:
                 offset = 0
                 while True:
-                    response = requests.get(
-                        f"https://api.scratch.mit.edu/users/{self.username}/favorites/?limit=40&offset={offset}").json()
+                    response = self.session.get(
+                        f"{_api}/users/{self.username}/favorites/?limit=40&offset={offset}").json()
                     offset += 40
                     favourites.append(response)
                     if len(response) != 40:
                         break
             if not all:
-                response = requests.get(
-                    f"https://api.scratch.mit.edu/users/{self.username}/favorites/?limit={limit}&offset={offset}").json()
+                response = self.session.get(
+                    f"{_api}/users/{self.username}/favorites/?limit={limit}&offset={offset}").json()
                 favourites.append(response)
             self.user_favourites = favourites
         return self.user_favourites
 
-    def user_follower_history(self, segment="", range=30):
+    def user_follower_history(self, segment="", range=30) -> list:
         """
         Return the follower history of the user
         :param segment: The length of time between each segment, defaults to 1 day.
         :param range: Of how far back to get history, defaults to 30 days
         """
         return requests.get(
             f"https://scratchdb.lefty.one/v3/user/graph/{self.username}/followers?segment={segment}&range={range}").json()
 
-    def all_data(self):
+    def all_data(self) -> dict:
         """
         Returns all the data of the user
         """
         data = {
             'UserName': self.username,
             'UserId': self.id(),
             'Messages Count': self.messages_count(),
@@ -328,28 +328,28 @@
             'Total Views': self.total_views(),
             'Total Loves': self.total_loves_count(),
             'Total Favourites': self.total_favourites_count(),
             'Total Projects Count': self.projects_count()
         }
         return data
 
-    def ocular_data(self):
+    def ocular_data(self) -> dict:
         """
         Get ocular data of the user
         """
         return requests.get(f"https://my-ocular.jeffalo.net/api/user/{self.username}").json()
 
-    def aviate_data(self, code=False):
+    def aviate_data(self, code=False) -> dict:
         """
         Get Aviate Status of the user
         :param code: True to get the status code
         """
         return requests.get(f"https://aviateapp.eu.org/api/{self.username}?code={str(code).lower()}").json()['status']
 
-    def comments(self, limit=5, page=1):
+    def comments(self, limit=5, page=1) -> dict:
         """
         Get comments of the profile of the user
         :param limit: The limit
         :param page: The page
         """
         return requests.get(
-            f"https://scratch-comments-api.sid72020123.repl.co/user/?username={self.username}&limit={limit}&page={page}").json()
+            f"https://apis.scratchconnect.eu.org/comments/user/?username={self.username}&limit={limit}&page={page}").json()
```

### Comparing `scratchconnect-4.5.2/scratchconnect/__init__.py` & `scratchconnect-5.0/scratchconnect/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 __name__ = "scratchconnect"
-__version__ = "4.5.2"
+__version__ = "5.0"
 __author__ = "Siddhesh Chavan"
 __documentation__ = "https://sid72020123.github.io/scratchconnect/"
 __doc__ = f"""
 ScratchConnect is a Python Library to connect Scratch API and much more.
-This library can show the statistics of Users, Projects, Studios, Forums and also connect and set cloud variables of a project!
+This library can show/fetch the statistics of Users, Projects, Studios, Forums and also connect and set cloud variables of a project!
 Import Statement:
     import scratchconnect
 Documentation(Tutorial):
     For documentation, go to {__documentation__}
 Required Libraries:
     requests*, re*, json*, time*, traceback*, threading*, urllib*, PIL*, websocket-client
     * -> In-built
 Optional Libraries:
-    pyhtmlchart - For Chart feature
     rich - For Terminal feature
 Change Log:
     View all the change log at: https://github.com/Sid72020123/scratchconnect#change-log
 Credits:
     View all the contributors: https://github.com/Sid72020123/scratchconnect#contributors
 """
```

### Comparing `scratchconnect-4.5.2/scratchconnect/scCloudEvents.py` & `scratchconnect-5.0/scratchconnect/scCloudEvents.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
             "create": None,
             "delete": None,
             "set": None,
             "disconnect": None
         }
         self.run = False
 
-    def on(self, e_type):
+    def on(self, e_type: str):
         """
         Decorator
         """
 
         def wrapper(func):
             if e_type not in list(self._event_functions.keys()):
                 raise TypeError(
@@ -74,22 +74,22 @@
                               variable_name=data['Name'], value=data['Value'],
                               timestamp=data['Timestamp'])
                 elif self.cloud_object_type == "Turbowarp":
                     self.emit(emit_action, action=data['method'],
                               variable_name=data['name'], value=data['value'])
             time.sleep(up)
 
-    def start(self, update_time=1):
+    def start(self, update_time: int = 1) -> None:
         """
         Start the events loop
         :param update_time: The update time
         """
         self.cloud_object._make_connection()
         self.run = True
         self.t = Thread(target=self._event, args=(update_time,))
         self.t.start()
 
-    def stop(self):
+    def stop(self) -> None:
         """
         Stop the events loop
         """
         self.run = False
```

### Comparing `scratchconnect-4.5.2/scratchconnect/scCloudRequests.py` & `scratchconnect-5.0/scratchconnect/scCloudRequests.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,52 +7,51 @@
 import traceback
 from threading import Thread
 
 from scratchconnect import Warnings
 from scratchconnect.CloudConnection import CloudConnection
 from scratchconnect.scImage import Image
 
-VERSION = "2.1 (stable)"
+VERSION = "2.5 (stable)"
 RESPONSE_VARIABLES = [f"Response_{i}" for i in range(1, 9)]
 cloud_variable_length_limit = 256
 FAIL = 0
 SUCCESS = 1
 
 
 class CloudRequests:
     def __init__(self, project_id, client_username, csrf_token, session_id, token, handle_all_errors,
-                 print_logs, default=" "):
+                 print_logs, online_ide, session, default=" "):
         print(f"[33m[1mScratchConnect [36mCloudRequests [37m- [35mv{VERSION}[3m[0m")
         self.t = None
         self.run_thread = False
         self.handle_all_errors = handle_all_errors
         self._request_functions = {}
         self._event_functions = {}
         self._request_value = ""
         self.print_logs = print_logs
         self.default = default
         self.max_tries = 3
-        self.cloud = CloudConnection(project_id=project_id,
-                                     client_username=client_username,
-                                     csrf_token=csrf_token,
-                                     session_id=session_id, token=token)
+        self.session = session
+        self.cloud = CloudConnection(project_id=project_id, client_username=client_username, csrf_token=csrf_token,
+                                     session_id=session_id, token=token, online_ide=online_ide, session=self.session)
         self._REQUESTS = []
         self._request = {}
 
-    def request(self, req_name):
+    def request(self, req_name: str):
         """
         Decorator
         """
 
         def wrapper(func):
             self._request_functions[req_name] = func
 
         return wrapper
 
-    def event(self, n):
+    def event(self, n: str):
         """
         Decorator
         """
 
         def wrapper(func):
             self._event_functions[n] = func
 
@@ -332,28 +331,28 @@
             i += 1
         if len(temp_str) > 0:
             result.append(temp_str)
         while (len(result) % len(RESPONSE_VARIABLES)) != 0:
             result.append("")
         return result
 
-    def get_request_info(self):
+    def get_request_info(self) -> dict:
         """
         Get the request info
         """
         return self._request
 
-    def start(self, update_time=1):
+    def start(self, update_time: int = 1) -> None:
         """
         Start the events loop
         :param update_time: The update time
         """
         self.run_thread = True
         self.t = Thread(target=self._event, args=(update_time,))
         self.t.start()
         self.emit("connect", t="event")
 
-    def stop(self):
+    def stop(self) -> None:
         """
         Stop the events loop
         """
         self.run = False
```

### Comparing `scratchconnect-4.5.2/scratchconnect/scCloudStorage.py` & `scratchconnect-5.0/scratchconnect/scCloudStorage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+# This feature is deprecated since the v5.0 of the library. Please use the new alternative Cloud Requests feature instead.
+
 """
 The Cloud Storage File.
-"""
+
 import time
 import json
 import string
 from threading import Thread
 
 from scratchconnect.CloudConnection import CloudConnection
 from scratchconnect.scEncoder import Encoder
@@ -246,7 +248,8 @@
             if len(text) >= letters_length:
                 divide.append(text)
                 text = ""
             i += 1
         if len(text) > 0:
             divide.append(text)
         return divide
+"""
```

### Comparing `scratchconnect-4.5.2/scratchconnect/scEncoder.py` & `scratchconnect-5.0/scratchconnect/scEncoder.py`

 * *Files identical despite different names*

### Comparing `scratchconnect-4.5.2/scratchconnect/scImage.py` & `scratchconnect-5.0/scratchconnect/scImage.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,39 +11,40 @@
 
 class Image:
     def __init__(self, online_ide):
         self.length = []
         self._image_size = None
         self.image_success = None
         self.name = None
+        self.hex_values = ""
         if online_ide:
             _change_request_url()
 
     def _shorten_code(self, r, g, b):
         """
         Don't use this
         """
         decimal = str((r * 256 * 256) + (g * 256) + b)
         code = ("0" * (8 - len(decimal))) + str(decimal)
         return code
 
-    def download_image(self, url, name):
+    def download_image(self, url: str, name: str) -> None:
         """
         Download the image
         """
         self.name = name
         try:
             response = requests.get(url).content
             with open(f"{self.name}.png", 'wb') as file:
                 file.write(response)
             self.image_success = True
         except:
             self.image_success = False
 
-    def resize_image(self, size, name, maintain_aspect_ratio=True):
+    def resize_image(self, size: tuple, name: str, maintain_aspect_ratio: bool = True) -> None:
         """
         Resize the given image
         :param size: The size (in tuple format)
         :param name: The new name of the image you want to save
         :param maintain_aspect_ratio: Set it to "True" if you want to maintain the aspect ratio of the image while resizing
         """
         image = pyImage.open(f"{self.name}.png")
@@ -51,37 +52,37 @@
             image.thumbnail(size)
             image.save(f"{name}.png")
         else:
             new_image = image.resize(size)
             new_image.save(f"{name}.png")
         self.name = name
 
-    def get_user_image(self, query, size=32, name="scImage"):
+    def get_user_image(self, query: str, size: int = 32, name: str = "scImage") -> None:
         """
         Get the image of a user on Scratch
         """
         user_id = requests.get(f"{_scratch_api}users/{query}").json()["id"]
         url = f"https://cdn2.scratch.mit.edu/get_image/user/{user_id}_{size}x{size}.png?v="
         self.download_image(url, name)
 
-    def get_studio_image(self, studio_id, name="scImage"):
+    def get_studio_image(self, studio_id: int, name: str = "scImage") -> None:
         """
         Get the image of a studio on Scratch
         """
         url = f"https://uploads.scratch.mit.edu/get_image/gallery/{studio_id}_170x100.png"
         self.download_image(url, name)
 
-    def get_project_image(self, project_id, size=32, name="scImage"):
+    def get_project_image(self, project_id: str, size: int = 32, name: str = "scImage") -> None:
         """
         Get the image of a project on Scratch
         """
         url = f"https://uploads.scratch.mit.edu/get_image/project/{project_id}_{size}x{size}.png"
         self.download_image(url, name)
 
-    def encode_image(self):
+    def encode_image(self) -> bool | None:
         """
         Encode the image data to numbers. Use the function get_data() to get the encoded data
         """
         try:
             if self.image_success in [False, None]:
                 return False
             image = pyImage.open(f"{self.name}.png").convert('RGBA')
@@ -109,18 +110,18 @@
                 hex_values += self._shorten_code(pixel_color[0], pixel_color[1], pixel_color[2])
             self.hex_values = hex_values
             return True
         except Exception as E:
             print(E)
             return None
 
-    def get_image_data(self):
+    def get_image_data(self) -> str:
         """
         Get the encoded image data
         """
         return self.hex_values
 
-    def get_size(self):
+    def get_size(self) -> tuple:
         """
         Get the size of the image
         """
         return self._image_size
```

### Comparing `scratchconnect-4.5.2/scratchconnect.egg-info/PKG-INFO` & `scratchconnect-5.0/scratchconnect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: scratchconnect
-Version: 4.5.2
+Version: 5.0
 Summary: Python Library to connect Scratch API and much more. This library can show the statistics of Users, Projects, Studios, Forums and also connect and set cloud variables of a project!
 Home-page: https://github.com/Sid72020123/scratchconnect/
 Author: Siddhesh Chavan
 Author-email: siddheshchavan2020@gmail.com
 License: MIT
 Keywords: connect scratch,scratch api,api,scratch,bot,scratch bot,scratch cloud,scratch cloud variables,scratch data,scratch stats,cloud requests,fast cloud requests
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 Provides-Extra: terminal
-Provides-Extra: chart
 License-File: LICENSE
 
 # ScratchConnect v4.5.2
 
 Python Library to connect Scratch API and much more.
 
 This library can show the statistics of Users, Projects, Studios, Forums and also connect and set cloud variables of a
```

### Comparing `scratchconnect-4.5.2/scratchconnect.egg-info/SOURCES.txt` & `scratchconnect-5.0/scratchconnect.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 scratchconnect/ScratchConnect.py
 scratchconnect/Studio.py
 scratchconnect/TurbowarpCloudConnection.py
 scratchconnect/User.py
 scratchconnect/UserCommon.py
 scratchconnect/Warnings.py
 scratchconnect/__init__.py
-scratchconnect/scChart.py
 scratchconnect/scCloudEvents.py
 scratchconnect/scCloudRequests.py
 scratchconnect/scCloudStorage.py
 scratchconnect/scEncoder.py
 scratchconnect/scImage.py
 scratchconnect/scOnlineIDE.py
 scratchconnect/scScratchTerminal.py
```

### Comparing `scratchconnect-4.5.2/setup.py` & `scratchconnect-5.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,26 +6,25 @@
     'Operating System :: OS Independent',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3'
 ]
 
 setup(
     name="scratchconnect",
-    version="4.5.2",
+    version="5.0",
     description="Python Library to connect Scratch API and much more. This library can show the statistics of Users, Projects, Studios, Forums and also connect and set cloud variables of a project!",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/Sid72020123/scratchconnect/",
     author="Siddhesh Chavan",
     author_email="siddheshchavan2020@gmail.com",
     license="MIT",
     classifiers=classifiers,
     keywords=['connect scratch', 'scratch api', 'api', 'scratch', 'bot', 'scratch bot',
               'scratch cloud', 'scratch cloud variables', 'scratch data', 'scratch stats', 'cloud requests',
               'fast cloud requests'],
     packages=["scratchconnect"],
     install_requires=['requests', 'websocket-client', 'Pillow'],
     extras_require={
-        'terminal': ['scScratchTerminal'],
-        'chart': ['scChart']
+        'terminal': ['scScratchTerminal']
     }
 )
```

