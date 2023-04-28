# Comparing `tmp/schoolware_api-1.0.2.tar.gz` & `tmp/schoolware_api-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schoolware_api-1.0.2.tar", last modified: Wed Apr 26 09:09:16 2023, max compression
+gzip compressed data, was "schoolware_api-1.0.3.tar", last modified: Fri Apr 28 09:36:58 2023, max compression
```

## Comparing `schoolware_api-1.0.2.tar` & `schoolware_api-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:09:16.127255 schoolware_api-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-26 09:09:16.127255 schoolware_api-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-26 09:09:00.000000 schoolware_api-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-26 09:09:00.000000 schoolware_api-1.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:09:16.127255 schoolware_api-1.0.2/schoolware_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 09:09:00.000000 schoolware_api-1.0.2/schoolware_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11063 2023-04-26 09:09:00.000000 schoolware_api-1.0.2/schoolware_api/schoolware_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 09:09:16.127255 schoolware_api-1.0.2/schoolware_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-26 09:09:16.000000 schoolware_api-1.0.2/schoolware_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-26 09:09:16.000000 schoolware_api-1.0.2/schoolware_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 09:09:16.000000 schoolware_api-1.0.2/schoolware_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-26 09:09:16.000000 schoolware_api-1.0.2/schoolware_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-26 09:09:16.000000 schoolware_api-1.0.2/schoolware_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 09:09:16.127255 schoolware_api-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-26 09:09:00.000000 schoolware_api-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:36:58.460325 schoolware_api-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-28 09:36:58.460325 schoolware_api-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-28 09:36:46.000000 schoolware_api-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-28 09:36:46.000000 schoolware_api-1.0.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:36:58.460325 schoolware_api-1.0.3/schoolware_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-28 09:36:46.000000 schoolware_api-1.0.3/schoolware_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12404 2023-04-28 09:36:46.000000 schoolware_api-1.0.3/schoolware_api/schoolware_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 09:36:58.460325 schoolware_api-1.0.3/schoolware_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-28 09:36:58.000000 schoolware_api-1.0.3/schoolware_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-28 09:36:58.000000 schoolware_api-1.0.3/schoolware_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 09:36:58.000000 schoolware_api-1.0.3/schoolware_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-28 09:36:58.000000 schoolware_api-1.0.3/schoolware_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-28 09:36:58.000000 schoolware_api-1.0.3/schoolware_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 09:36:58.460325 schoolware_api-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-28 09:36:46.000000 schoolware_api-1.0.3/setup.py
```

### Comparing `schoolware_api-1.0.2/PKG-INFO` & `schoolware_api-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schoolware_api
-Version: 1.0.2
+Version: 1.0.3
 Summary: A api for schoolware written in python
 Author: Maarten Buelens
 Author-email: MB <schoolware_api@mb-server.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Maarten-buelens/schoolware_api
 Project-URL: Bug Tracker, https://github.com/Maarten-buelens/schoolware_api/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `schoolware_api-1.0.2/README.md` & `schoolware_api-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `schoolware_api-1.0.2/pyproject.toml` & `schoolware_api-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "schoolware_api"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name="MB", email="schoolware_api@mb-server.com" },
 ]
 description = "A api for schoolware written in python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `schoolware_api-1.0.2/schoolware_api/schoolware_api.py` & `schoolware_api-1.0.3/schoolware_api/schoolware_api.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+
+
 import requests
 from datetime import date, datetime, timedelta
 from playwright.sync_api import sync_playwright
 import time
 from termcolor import colored
 import threading
 
@@ -94,14 +96,19 @@
             ##########VERBOSE##########
             verbose_end(self,"check_token")
             ##########VERBOSE##########
             return True
 
 #todo
     def todo(self):
+        """gets all todo items from schoolware
+
+        Returns:
+            list: returns all todo items in a list
+        """
         ##########VERBOSE##########
         verbose_print(self,"todo")
         ##########VERBOSE##########
 
         self.check_if_valid()
         task_data = requests.get(f"https://{self.domain}/webleerling/bin/server.fcgi/REST/AgendaPunt/?_dc=1665240724814&MinVan={date.today()}T00:00:00&IsTaakOfToets=true", cookies=self.cookie).json()["data"]
         self.todo_list = []
@@ -132,14 +139,19 @@
         ##########VERBOSE##########
         verbose_end(self,"todo")
         ##########VERBOSE##########
         return self.todo_list
 
 #punten
     def punten(self):
+        """Gets points from the whole year
+
+        Returns:
+            list: A list containing the points orderd by date
+        """
         ##########VERBOSE##########
         verbose_print(self,"punten")
         ##########VERBOSE##########
         self.check_if_valid()
         punten_data = requests.get(f"https://{self.domain}/webleerling/bin/server.fcgi/REST/PuntenbladGridLeerling?&Leerling=15201&?BeoordelingMomentVan=1990-09-01+00:00:00", cookies=self.cookie).json()["data"]
         self.scores = []
         for vak in punten_data:
@@ -179,14 +191,22 @@
         ##########VERBOSE##########
         verbose_end(self,"punten")
         ##########VERBOSE##########
         return self.scores
 
 #agenda
     def agenda(self, datum=""):
+        """Gets all agenda points of a given date from schoolware
+
+        Args:
+            datum (str, optional): Date to get agenda for. Defaults to "".
+
+        Returns:
+            list: returns output from filter_agenda
+        """
         ##########VERBOSE##########
         verbose_print(self,"_agenda")
         ##########VERBOSE##########
         self.check_if_valid()
         #begin en einde week
         day = str(date.today())
         dt = datetime.strptime(day, '%Y-%m-%d')
@@ -204,14 +224,23 @@
                 self.rooster.append(agenda)
         ##########VERBOSE##########
         verbose_end(self,"agenda")
         ##########VERBOSE##########
         return self.filter_rooster(self.rooster, datum)
 
     def filter_rooster(self, rooster, datum=""):
+        """Internal function to filter a agenda rooster of a given date
+
+        Args:
+            rooster (list): The agenda points to filter
+            datum (str, optional): The date to filter agenda points for. Defaults to "".
+
+        Returns:
+            list: Filters agenda points for a given date and points
+        """
         ##########VERBOSE##########
         verbose_print(self,"filter_agenda")
         ##########VERBOSE##########
         today = []
         if(datum == ""):
             datum = datetime.today()
         datum = str(datum).split(' ')[0]
@@ -253,24 +282,28 @@
 
         return today_filterd
 
 ##########OTHER##########
 
 #bg procces
 def bg(self):
+    """Function to keep token valid
+    """
     from time import sleep
     if(self.verbose):
         print(colored("background procces started","blue"))
     while True:
         sleep(5*60)
         if(self.verbose):
             print(colored("background task: checking token","blue"))
         self.check_if_valid()
 #telegram bot
 def telegram_def(self):
+    """The setup function for Telegram
+    """
     import telegram
     from time import sleep
     import asyncio
     if(self.verbose):
         self.bot = telegram.Bot(self.config["bot_token"])
     print(colored("telegram started","blue"))
     while True:
@@ -281,24 +314,39 @@
         if(self.num_points < num_now):
             diff = num_now - self.num_points
             self.num_points = num_now
             
             asyncio.run(telegram_send_msg(self, diff))
 
 async def telegram_send_msg(self, diff):
+    """Function to send a telegram message to a set message-id
+
+    Args:
+        diff (int): the number to display in the message
+    """
     async with self.bot:
         await self.bot.send_message(text=f'{diff} New point(s)', chat_id=self.config["chat_id"])
 
 ##########VERBOSE##########
 def verbose_print(self,message):
+    """To print a message when verbose is set also times function
+
+    Args:
+        message (string): name of function to display
+    """
     if(self.verbose):
         print(colored("#"*50, "grey"))
         self.start_time = time.time()
         print(colored(f"• starting {message}", "green"))
         print(colored("#"*50, "grey"))
 def verbose_end(self,message):
+    """Ends verbose_print with done and the time for the function
+
+    Args:
+        message (string): name of function to display
+    """
     if(self.verbose):
         print(colored("#"*50, "grey"))
         end_time = time.time()
         print(colored(f"• Done {message} time:{end_time - self.start_time}", "green"))
         print(colored("#"*50, "grey"))
 ##########VERBOSE##########
```

### Comparing `schoolware_api-1.0.2/schoolware_api.egg-info/PKG-INFO` & `schoolware_api-1.0.3/schoolware_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schoolware-api
-Version: 1.0.2
+Version: 1.0.3
 Summary: A api for schoolware written in python
 Author: Maarten Buelens
 Author-email: MB <schoolware_api@mb-server.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Maarten-buelens/schoolware_api
 Project-URL: Bug Tracker, https://github.com/Maarten-buelens/schoolware_api/issues
 Classifier: Programming Language :: Python :: 3
```

