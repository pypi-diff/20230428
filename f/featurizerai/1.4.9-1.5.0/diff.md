# Comparing `tmp/featurizerai-1.4.9.tar.gz` & `tmp/featurizerai-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featurizerai-1.4.9.tar", last modified: Fri Apr 28 06:01:06 2023, max compression
+gzip compressed data, was "featurizerai-1.5.0.tar", last modified: Fri Apr 28 06:22:19 2023, max compression
```

## Comparing `featurizerai-1.4.9.tar` & `featurizerai-1.5.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 06:01:06.050402 featurizerai-1.4.9/
--rw-r--r--   0 burakkebapci   (501) staff       (20)     1079 2023-03-26 20:50:31.000000 featurizerai-1.4.9/LICENSE
--rw-r--r--   0 burakkebapci   (501) staff       (20)       85 2023-03-26 20:50:31.000000 featurizerai-1.4.9/MANIFEST.in
--rw-r--r--   0 burakkebapci   (501) staff       (20)      857 2023-04-28 06:01:06.050473 featurizerai-1.4.9/PKG-INFO
--rw-r--r--   0 burakkebapci   (501) staff       (20)       98 2023-03-26 20:50:31.000000 featurizerai-1.4.9/pyproject.toml
--rw-r--r--   0 burakkebapci   (501) staff       (20)      115 2023-04-28 06:01:06.050688 featurizerai-1.4.9/setup.cfg
--rw-r--r--   0 burakkebapci   (501) staff       (20)     1378 2023-04-28 06:00:21.000000 featurizerai-1.4.9/setup.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 06:01:06.046934 featurizerai-1.4.9/src/
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 06:01:06.048745 featurizerai-1.4.9/src/features/
--rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-04-22 17:23:59.000000 featurizerai-1.4.9/src/features/__init__.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)      686 2023-04-22 23:39:43.000000 featurizerai-1.4.9/src/features/authenticate.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)     3287 2023-04-28 05:58:45.000000 featurizerai-1.4.9/src/features/create_stream.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)      845 2023-04-23 11:45:28.000000 featurizerai-1.4.9/src/features/custom_schema.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)     4695 2023-04-25 17:12:53.000000 featurizerai-1.4.9/src/features/materialize.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 06:01:06.049431 featurizerai-1.4.9/src/features/tests/
--rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-04-25 16:35:40.000000 featurizerai-1.4.9/src/features/tests/__init__.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)     2764 2023-04-26 01:15:16.000000 featurizerai-1.4.9/src/features/tests/test_materialize.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)     1515 2023-04-28 02:38:55.000000 featurizerai-1.4.9/src/features/tests/test_pipeline.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 06:01:06.050285 featurizerai-1.4.9/src/featurizerai.egg-info/
--rw-r--r--   0 burakkebapci   (501) staff       (20)      857 2023-04-28 06:01:06.000000 featurizerai-1.4.9/src/featurizerai.egg-info/PKG-INFO
--rw-r--r--   0 burakkebapci   (501) staff       (20)      500 2023-04-28 06:01:06.000000 featurizerai-1.4.9/src/featurizerai.egg-info/SOURCES.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)        1 2023-04-28 06:01:06.000000 featurizerai-1.4.9/src/featurizerai.egg-info/dependency_links.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)       22 2023-04-28 06:01:06.000000 featurizerai-1.4.9/src/featurizerai.egg-info/requires.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)        9 2023-04-28 06:01:06.000000 featurizerai-1.4.9/src/featurizerai.egg-info/top_level.txt
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 06:22:19.514257 featurizerai-1.5.0/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     1079 2023-03-26 20:50:31.000000 featurizerai-1.5.0/LICENSE
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       85 2023-03-26 20:50:31.000000 featurizerai-1.5.0/MANIFEST.in
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      857 2023-04-28 06:22:19.514333 featurizerai-1.5.0/PKG-INFO
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       98 2023-03-26 20:50:31.000000 featurizerai-1.5.0/pyproject.toml
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      115 2023-04-28 06:22:19.514623 featurizerai-1.5.0/setup.cfg
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     1378 2023-04-28 06:22:10.000000 featurizerai-1.5.0/setup.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 06:22:19.509530 featurizerai-1.5.0/src/
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 06:22:19.511641 featurizerai-1.5.0/src/features/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-04-22 17:23:59.000000 featurizerai-1.5.0/src/features/__init__.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      686 2023-04-22 23:39:43.000000 featurizerai-1.5.0/src/features/authenticate.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     4229 2023-04-28 06:11:42.000000 featurizerai-1.5.0/src/features/create_stream.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      845 2023-04-23 11:45:28.000000 featurizerai-1.5.0/src/features/custom_schema.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     4695 2023-04-25 17:12:53.000000 featurizerai-1.5.0/src/features/materialize.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 06:22:19.512548 featurizerai-1.5.0/src/features/tests/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-04-25 16:35:40.000000 featurizerai-1.5.0/src/features/tests/__init__.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     2764 2023-04-26 01:15:16.000000 featurizerai-1.5.0/src/features/tests/test_materialize.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     1515 2023-04-28 02:38:55.000000 featurizerai-1.5.0/src/features/tests/test_pipeline.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 06:22:19.514106 featurizerai-1.5.0/src/featurizerai.egg-info/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      857 2023-04-28 06:22:19.000000 featurizerai-1.5.0/src/featurizerai.egg-info/PKG-INFO
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      500 2023-04-28 06:22:19.000000 featurizerai-1.5.0/src/featurizerai.egg-info/SOURCES.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        1 2023-04-28 06:22:19.000000 featurizerai-1.5.0/src/featurizerai.egg-info/dependency_links.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       22 2023-04-28 06:22:19.000000 featurizerai-1.5.0/src/featurizerai.egg-info/requires.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        9 2023-04-28 06:22:19.000000 featurizerai-1.5.0/src/featurizerai.egg-info/top_level.txt
```

### Comparing `featurizerai-1.4.9/LICENSE` & `featurizerai-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `featurizerai-1.4.9/PKG-INFO` & `featurizerai-1.5.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurizerai
-Version: 1.4.9
+Version: 1.5.0
 Summary: Python library for Featurizer AI
 Home-page: https://github.com/burakglobal/featurizerai
 Author: Burak
 Author-email: burakgblobal@gmail.com
 Keywords: featurizer,package
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `featurizerai-1.4.9/setup.py` & `featurizerai-1.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 setuptools.setup(
     name='featurizerai',
     author='Burak',
-    version='1.4.9',
+    version='1.5.0',
     author_email='burakgblobal@gmail.com',
     description='Python library for Featurizer AI',
     keywords='featurizer, package',
     url='https://github.com/burakglobal/featurizerai',
     package_dir={'': 'src'},
     packages=setuptools.find_packages(where='src'),
     classifiers=[
```

### Comparing `featurizerai-1.4.9/src/features/authenticate.py` & `featurizerai-1.5.0/src/features/authenticate.py`

 * *Files identical despite different names*

### Comparing `featurizerai-1.4.9/src/features/create_stream.py` & `featurizerai-1.5.0/src/features/create_stream.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,83 +1,106 @@
 import json
 import ast
 import logging
 from datetime import datetime
 from http.client import HTTPException
 
-from motor.motor_asyncio import AsyncIOMotorClient
+from pymongo import MongoClient
 from pymongo.server_api import ServerApi
-from aiokafka import AIOKafkaConsumer
+from confluent_kafka import Consumer, KafkaError
 import certifi
 import os
-import asyncio
+import threading
 import jwt
 
-
 class create_stream:
     def __init__(self, kafka_connection, mongo_connection=None, topicname="", timestamp_attr="timestamp"):
         self.topicname = topicname
         self.kafka_connection = kafka_connection
         self.mongo_connection = mongo_connection
         self.timestamp_attr = timestamp_attr
-        self.stop_event = asyncio.Event()
+        self._stop_event = threading.Event()
 
     def is_epoch(self, timestamp):
         try:
             datetime.fromtimestamp(int(timestamp))
             return True
         except ValueError:
             return False
 
-    async def _run(self, token):
-        mongo_client = AsyncIOMotorClient(self.mongo_connection['uri'], server_api=ServerApi('1'),
-                                          tlsCAFile=certifi.where())
+    def _run(self, token):
+        mongo_client = MongoClient(self.mongo_connection['uri'], server_api=ServerApi('1'), tlsCAFile=certifi.where())
         mongo_db = mongo_client[self.mongo_connection['database']]
         raw_data_collection = mongo_db[self.mongo_connection['rawcollection']]
 
-        consumer = AIOKafkaConsumer(
-            self.topicname,
-            bootstrap_servers=self.kafka_connection["bootstrap.servers"],
-            group_id=self.kafka_connection["group.id"],
-            auto_offset_reset=self.kafka_connection["auto.offset.reset"],
-            enable_auto_commit=self.kafka_connection['enable.auto.commit'],
-            value_deserializer=lambda m: json.loads(m.decode('utf-8'))
-        )
-
-        await consumer.start()
-        try:
-            while not self.stop_event.is_set():
-                msg = await consumer.getone()
-                message_value = msg.value
+        consumer = Consumer(self.kafka_connection)
+        print(self.topicname)
+        consumer.subscribe([self.topicname])
+
+        while not self._stop_event.is_set():
+            msg = consumer.poll(10.0)
+            print("Poll executed")
+            print(msg)
+            if msg is None:
+                continue
+            if msg.error():
+                print("Consumer error: {}".format(msg.error()))
+            else:
+                message_value = ast.literal_eval(msg.value().decode("utf-8"))
                 print(message_value)
 
+                # New lines added for validation
                 if self.timestamp_attr not in message_value:
                     print(
                         f"Error: Message does not contain the required timestamp attribute '{self.timestamp_attr}'. Skipping message.")
                     continue
 
                 if self.is_epoch(message_value.get(self.timestamp_attr)):
                     if self.is_epoch(message_value.get(self.timestamp_attr)):
                         message_value[self.timestamp_attr] = int(message_value[self.timestamp_attr])
                     else:
                         message_value[self.timestamp_attr] = datetime.now().timestamp()
 
-                await raw_data_collection.insert_one(message_value)
+                raw_data_collection.insert_one(message_value)
                 print("Message received: {}".format(message_value))
-        finally:
-            await consumer.stop()
+        consumer.close()
 
-    async def start(self, token):
-        if not hasattr(self, '_consumer_task') or self._consumer_task.done():
-            self.stop_event.clear()
-            self._consumer_task = asyncio.create_task(self._run(token))
-            print('featurizerai: Started consumer task.')
+    def start(self, token):
+        # authenicate token
+        mongo_client = MongoClient(self.mongo_connection['uri'], server_api=ServerApi('1'), tlsCAFile=certifi.where())
+        mongo_db = mongo_client[self.mongo_connection['database']]
+        mongo_db_featurizer = mongo_client['featurizer']
+        users_collection = mongo_db_featurizer["users"]
+        SECRET_KEY = "features"  # Change this to your desired secret key
+        TOKEN_EXPIRATION = 3600  # Token expiration in seconds (1 hour)
+
+        try:
+            payload = jwt.decode(token, SECRET_KEY, algorithms=["HS256"])
+            user_id: str = payload.get("user_id")
+            if user_id is None:
+                print("User not found")
+                return ("Invalid token")
+            print(user_id)
+            user = users_collection.find_one({"userid": user_id})
+            if user is None:
+                print("User not found")
+                return ("Invalid token")
+        except Exception as e:
+            print(e)
+            return ("Invalid token")
+
+
+        if not hasattr(self, '_consumer_thread') or not self._consumer_thread.is_alive():
+            self._stop_event.clear()
+            self._consumer_thread = threading.Thread(target=self._run(self))
+            self._consumer_thread.start()
+            print('featurizerai: Started consumer thread.')
         else:
-            print("Task is already running. Cannot start it again.")
+            print("Thread is already running. Cannot start it again.")
 
-    async def stop(self):
-        if hasattr(self, '_consumer_task') and not self._consumer_task.done():
-            self.stop_event.set()
-            await self._consumer_task
-            print('featurizerai: Stopped consumer task.')
+    def stop(self):
+        if hasattr(self, '_consumer_thread') and self._consumer_thread.is_alive():
+            self._stop_event.set()
+            self._consumer_thread.join()
+            print('featurizerai: Stopped consumer thread.')
         else:
-            print("Task is not running. Cannot stop it.")
+            print("Thread is not running. Cannot stop it.")
```

### Comparing `featurizerai-1.4.9/src/features/custom_schema.py` & `featurizerai-1.5.0/src/features/custom_schema.py`

 * *Files identical despite different names*

### Comparing `featurizerai-1.4.9/src/features/materialize.py` & `featurizerai-1.5.0/src/features/materialize.py`

 * *Files identical despite different names*

### Comparing `featurizerai-1.4.9/src/features/tests/test_materialize.py` & `featurizerai-1.5.0/src/features/tests/test_materialize.py`

 * *Files identical despite different names*

### Comparing `featurizerai-1.4.9/src/features/tests/test_pipeline.py` & `featurizerai-1.5.0/src/features/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `featurizerai-1.4.9/src/featurizerai.egg-info/PKG-INFO` & `featurizerai-1.5.0/src/featurizerai.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurizerai
-Version: 1.4.9
+Version: 1.5.0
 Summary: Python library for Featurizer AI
 Home-page: https://github.com/burakglobal/featurizerai
 Author: Burak
 Author-email: burakgblobal@gmail.com
 Keywords: featurizer,package
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

