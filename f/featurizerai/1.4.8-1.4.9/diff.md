# Comparing `tmp/featurizerai-1.4.8.tar.gz` & `tmp/featurizerai-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featurizerai-1.4.8.tar", last modified: Tue Apr 25 17:13:05 2023, max compression
+gzip compressed data, was "featurizerai-1.4.9.tar", last modified: Fri Apr 28 06:01:06 2023, max compression
```

## Comparing `featurizerai-1.4.8.tar` & `featurizerai-1.4.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-25 17:13:05.988199 featurizerai-1.4.8/
--rw-r--r--   0 burakkebapci   (501) staff       (20)     1079 2023-03-26 20:50:31.000000 featurizerai-1.4.8/LICENSE
--rw-r--r--   0 burakkebapci   (501) staff       (20)       85 2023-03-26 20:50:31.000000 featurizerai-1.4.8/MANIFEST.in
--rw-r--r--   0 burakkebapci   (501) staff       (20)      857 2023-04-25 17:13:05.988263 featurizerai-1.4.8/PKG-INFO
--rw-r--r--   0 burakkebapci   (501) staff       (20)       98 2023-03-26 20:50:31.000000 featurizerai-1.4.8/pyproject.toml
--rw-r--r--   0 burakkebapci   (501) staff       (20)      115 2023-04-25 17:13:05.988492 featurizerai-1.4.8/setup.cfg
--rw-r--r--   0 burakkebapci   (501) staff       (20)     1378 2023-04-25 17:13:02.000000 featurizerai-1.4.8/setup.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-25 17:13:05.985083 featurizerai-1.4.8/src/
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-25 17:13:05.987025 featurizerai-1.4.8/src/features/
--rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-04-22 17:23:59.000000 featurizerai-1.4.8/src/features/__init__.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)      686 2023-04-22 23:39:43.000000 featurizerai-1.4.8/src/features/authenticate.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)     4229 2023-04-23 11:29:31.000000 featurizerai-1.4.8/src/features/create_stream.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)      845 2023-04-23 11:45:28.000000 featurizerai-1.4.8/src/features/custom_schema.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)     4695 2023-04-25 17:12:53.000000 featurizerai-1.4.8/src/features/materialize.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-25 17:13:05.987410 featurizerai-1.4.8/src/features/tests/
--rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-04-25 16:35:40.000000 featurizerai-1.4.8/src/features/tests/__init__.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)     2309 2023-04-25 16:43:12.000000 featurizerai-1.4.8/src/features/tests/test_materialize.py
--rw-r--r--   0 burakkebapci   (501) staff       (20)     1490 2023-04-25 16:15:10.000000 featurizerai-1.4.8/src/features/tests/test_pipeline.py
-drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-25 17:13:05.988076 featurizerai-1.4.8/src/featurizerai.egg-info/
--rw-r--r--   0 burakkebapci   (501) staff       (20)      857 2023-04-25 17:13:05.000000 featurizerai-1.4.8/src/featurizerai.egg-info/PKG-INFO
--rw-r--r--   0 burakkebapci   (501) staff       (20)      500 2023-04-25 17:13:05.000000 featurizerai-1.4.8/src/featurizerai.egg-info/SOURCES.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)        1 2023-04-25 17:13:05.000000 featurizerai-1.4.8/src/featurizerai.egg-info/dependency_links.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)       22 2023-04-25 17:13:05.000000 featurizerai-1.4.8/src/featurizerai.egg-info/requires.txt
--rw-r--r--   0 burakkebapci   (501) staff       (20)        9 2023-04-25 17:13:05.000000 featurizerai-1.4.8/src/featurizerai.egg-info/top_level.txt
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 06:01:06.050402 featurizerai-1.4.9/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     1079 2023-03-26 20:50:31.000000 featurizerai-1.4.9/LICENSE
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       85 2023-03-26 20:50:31.000000 featurizerai-1.4.9/MANIFEST.in
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      857 2023-04-28 06:01:06.050473 featurizerai-1.4.9/PKG-INFO
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       98 2023-03-26 20:50:31.000000 featurizerai-1.4.9/pyproject.toml
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      115 2023-04-28 06:01:06.050688 featurizerai-1.4.9/setup.cfg
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     1378 2023-04-28 06:00:21.000000 featurizerai-1.4.9/setup.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 06:01:06.046934 featurizerai-1.4.9/src/
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 06:01:06.048745 featurizerai-1.4.9/src/features/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-04-22 17:23:59.000000 featurizerai-1.4.9/src/features/__init__.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      686 2023-04-22 23:39:43.000000 featurizerai-1.4.9/src/features/authenticate.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     3287 2023-04-28 05:58:45.000000 featurizerai-1.4.9/src/features/create_stream.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      845 2023-04-23 11:45:28.000000 featurizerai-1.4.9/src/features/custom_schema.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     4695 2023-04-25 17:12:53.000000 featurizerai-1.4.9/src/features/materialize.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 06:01:06.049431 featurizerai-1.4.9/src/features/tests/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        0 2023-04-25 16:35:40.000000 featurizerai-1.4.9/src/features/tests/__init__.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     2764 2023-04-26 01:15:16.000000 featurizerai-1.4.9/src/features/tests/test_materialize.py
+-rw-r--r--   0 burakkebapci   (501) staff       (20)     1515 2023-04-28 02:38:55.000000 featurizerai-1.4.9/src/features/tests/test_pipeline.py
+drwxr-xr-x   0 burakkebapci   (501) staff       (20)        0 2023-04-28 06:01:06.050285 featurizerai-1.4.9/src/featurizerai.egg-info/
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      857 2023-04-28 06:01:06.000000 featurizerai-1.4.9/src/featurizerai.egg-info/PKG-INFO
+-rw-r--r--   0 burakkebapci   (501) staff       (20)      500 2023-04-28 06:01:06.000000 featurizerai-1.4.9/src/featurizerai.egg-info/SOURCES.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        1 2023-04-28 06:01:06.000000 featurizerai-1.4.9/src/featurizerai.egg-info/dependency_links.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)       22 2023-04-28 06:01:06.000000 featurizerai-1.4.9/src/featurizerai.egg-info/requires.txt
+-rw-r--r--   0 burakkebapci   (501) staff       (20)        9 2023-04-28 06:01:06.000000 featurizerai-1.4.9/src/featurizerai.egg-info/top_level.txt
```

### Comparing `featurizerai-1.4.8/LICENSE` & `featurizerai-1.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `featurizerai-1.4.8/PKG-INFO` & `featurizerai-1.4.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurizerai
-Version: 1.4.8
+Version: 1.4.9
 Summary: Python library for Featurizer AI
 Home-page: https://github.com/burakglobal/featurizerai
 Author: Burak
 Author-email: burakgblobal@gmail.com
 Keywords: featurizer,package
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `featurizerai-1.4.8/setup.py` & `featurizerai-1.4.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 setuptools.setup(
     name='featurizerai',
     author='Burak',
-    version='1.4.8',
+    version='1.4.9',
     author_email='burakgblobal@gmail.com',
     description='Python library for Featurizer AI',
     keywords='featurizer, package',
     url='https://github.com/burakglobal/featurizerai',
     package_dir={'': 'src'},
     packages=setuptools.find_packages(where='src'),
     classifiers=[
```

### Comparing `featurizerai-1.4.8/src/features/authenticate.py` & `featurizerai-1.4.9/src/features/authenticate.py`

 * *Files identical despite different names*

### Comparing `featurizerai-1.4.8/src/features/create_stream.py` & `featurizerai-1.4.9/src/features/create_stream.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,106 +1,83 @@
 import json
 import ast
 import logging
 from datetime import datetime
 from http.client import HTTPException
 
-from pymongo import MongoClient
+from motor.motor_asyncio import AsyncIOMotorClient
 from pymongo.server_api import ServerApi
-from confluent_kafka import Consumer, KafkaError
+from aiokafka import AIOKafkaConsumer
 import certifi
 import os
-import threading
+import asyncio
 import jwt
 
+
 class create_stream:
     def __init__(self, kafka_connection, mongo_connection=None, topicname="", timestamp_attr="timestamp"):
         self.topicname = topicname
         self.kafka_connection = kafka_connection
         self.mongo_connection = mongo_connection
         self.timestamp_attr = timestamp_attr
-        self._stop_event = threading.Event()
+        self.stop_event = asyncio.Event()
 
     def is_epoch(self, timestamp):
         try:
             datetime.fromtimestamp(int(timestamp))
             return True
         except ValueError:
             return False
 
-    def _run(self, token):
-        mongo_client = MongoClient(self.mongo_connection['uri'], server_api=ServerApi('1'), tlsCAFile=certifi.where())
+    async def _run(self, token):
+        mongo_client = AsyncIOMotorClient(self.mongo_connection['uri'], server_api=ServerApi('1'),
+                                          tlsCAFile=certifi.where())
         mongo_db = mongo_client[self.mongo_connection['database']]
         raw_data_collection = mongo_db[self.mongo_connection['rawcollection']]
 
-        consumer = Consumer(self.kafka_connection)
-        print(self.topicname)
-        consumer.subscribe([self.topicname])
-
-        while not self._stop_event.is_set():
-            msg = consumer.poll(10.0)
-            print("Poll executed")
-            print(msg)
-            if msg is None:
-                continue
-            if msg.error():
-                print("Consumer error: {}".format(msg.error()))
-            else:
-                message_value = ast.literal_eval(msg.value().decode("utf-8"))
+        consumer = AIOKafkaConsumer(
+            self.topicname,
+            bootstrap_servers=self.kafka_connection["bootstrap.servers"],
+            group_id=self.kafka_connection["group.id"],
+            auto_offset_reset=self.kafka_connection["auto.offset.reset"],
+            enable_auto_commit=self.kafka_connection['enable.auto.commit'],
+            value_deserializer=lambda m: json.loads(m.decode('utf-8'))
+        )
+
+        await consumer.start()
+        try:
+            while not self.stop_event.is_set():
+                msg = await consumer.getone()
+                message_value = msg.value
                 print(message_value)
 
-                # New lines added for validation
                 if self.timestamp_attr not in message_value:
                     print(
                         f"Error: Message does not contain the required timestamp attribute '{self.timestamp_attr}'. Skipping message.")
                     continue
 
                 if self.is_epoch(message_value.get(self.timestamp_attr)):
                     if self.is_epoch(message_value.get(self.timestamp_attr)):
                         message_value[self.timestamp_attr] = int(message_value[self.timestamp_attr])
                     else:
                         message_value[self.timestamp_attr] = datetime.now().timestamp()
 
-                raw_data_collection.insert_one(message_value)
+                await raw_data_collection.insert_one(message_value)
                 print("Message received: {}".format(message_value))
-        consumer.close()
+        finally:
+            await consumer.stop()
 
-    def start(self, token):
-        # authenicate token
-        mongo_client = MongoClient(self.mongo_connection['uri'], server_api=ServerApi('1'), tlsCAFile=certifi.where())
-        mongo_db = mongo_client[self.mongo_connection['database']]
-        mongo_db_featurizer = mongo_client['featurizer']
-        users_collection = mongo_db_featurizer["users"]
-        SECRET_KEY = "features"  # Change this to your desired secret key
-        TOKEN_EXPIRATION = 3600  # Token expiration in seconds (1 hour)
-
-        try:
-            payload = jwt.decode(token, SECRET_KEY, algorithms=["HS256"])
-            user_id: str = payload.get("user_id")
-            if user_id is None:
-                print("User not found")
-                return ("Invalid token")
-            print(user_id)
-            user = users_collection.find_one({"userid": user_id})
-            if user is None:
-                print("User not found")
-                return ("Invalid token")
-        except Exception as e:
-            print(e)
-            return ("Invalid token")
-
-
-        if not hasattr(self, '_consumer_thread') or not self._consumer_thread.is_alive():
-            self._stop_event.clear()
-            self._consumer_thread = threading.Thread(target=self._run(self))
-            self._consumer_thread.start()
-            print('featurizerai: Started consumer thread.')
+    async def start(self, token):
+        if not hasattr(self, '_consumer_task') or self._consumer_task.done():
+            self.stop_event.clear()
+            self._consumer_task = asyncio.create_task(self._run(token))
+            print('featurizerai: Started consumer task.')
         else:
-            print("Thread is already running. Cannot start it again.")
+            print("Task is already running. Cannot start it again.")
 
-    def stop(self):
-        if hasattr(self, '_consumer_thread') and self._consumer_thread.is_alive():
-            self._stop_event.set()
-            self._consumer_thread.join()
-            print('featurizerai: Stopped consumer thread.')
+    async def stop(self):
+        if hasattr(self, '_consumer_task') and not self._consumer_task.done():
+            self.stop_event.set()
+            await self._consumer_task
+            print('featurizerai: Stopped consumer task.')
         else:
-            print("Thread is not running. Cannot stop it.")
+            print("Task is not running. Cannot stop it.")
```

### Comparing `featurizerai-1.4.8/src/features/custom_schema.py` & `featurizerai-1.4.9/src/features/custom_schema.py`

 * *Files identical despite different names*

### Comparing `featurizerai-1.4.8/src/features/materialize.py` & `featurizerai-1.4.9/src/features/materialize.py`

 * *Files identical despite different names*

### Comparing `featurizerai-1.4.8/src/features/tests/test_materialize.py` & `featurizerai-1.4.9/src/features/tests/test_materialize.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,51 @@
+import features
 from flask import Flask, request, jsonify, json
 from features.materialize import materialize
 from features.custom_schema import custom_schema
 
-app = Flask(__name__)
-
-mongo_connection = {
-    'uri': "mongodb+srv://admin:6lHqq9LqgwDlninK@cluster0.aqtcyq2.mongodb.net/?retryWrites=true&w=majority",
-    'database': 'kafkastream',
-    'rawdata': 'rawdata',
-    'collection': 'sparkaggregate'
-}
-
 schema_fields = [
     {"name": "timestamp", "type": "integer"},
     {"name": "name", "type": "string"},
     {"name": "email", "type": "string"},
     {"name": "deviceid", "type": "integer"}
 ]
 
 custom_schema = custom_schema(schema_fields)
 
+app = Flask(__name__)
+
 @app.route('/aggregate', methods=['POST'])
 def aggregate():
-    # Define the dynamic Spark SQL queries to be executed
-    sparksql = [
-        "SELECT COUNT(email) AS email_count_last_24_hours, COUNT(name) AS name_count_last_24_hours, deviceid FROM temp_table WHERE deviceid={deviceid} AND timestamp_unix > {timestamp} - 86400 and timestamp_unix < {timestamp_base} GROUP BY deviceid",
-        "SELECT COUNT(email) AS email_count_last_7_days, COUNT(name) AS name_count_last_7_days, deviceid FROM temp_table WHERE deviceid={deviceid} AND timestamp_unix > {timestamp} - 604800 and timestamp_unix < {timestamp_base} GROUP BY deviceid",
-        "SELECT COUNT(email) AS email_count_last_15_days, COUNT(name) AS name_count_last_15_days, deviceid FROM temp_table WHERE deviceid={deviceid} AND timestamp_unix > {timestamp} - 1296000 and timestamp_unix < {timestamp_base} GROUP BY deviceid",
-        "SELECT COUNT(email) AS email_count_last_30_days, COUNT(name) AS name_count_last_30_days, deviceid FROM temp_table WHERE deviceid={deviceid} AND timestamp_unix > {timestamp} - 2.592e+6 and timestamp_unix < {timestamp_base} GROUP BY deviceid",
-    ]
-    json_data = request.get_json()
-    timestamp = json_data.get('timestamp')
-    deviceid = json_data.get('deviceid')
-    token = json_data.get('token')
+    mongo_connection = {
+        'uri': "mongodb+srv://admin:6lHqq9LqgwDlninK@cluster0.aqtcyq2.mongodb.net/?retryWrites=true&w=majority",
+        'database': 'kafkastream',
+        'rawdata': 'rawdata',
+        'collection': 'sparkaggregate'
+    }
+
+    try:
+        # Define the dynamic Spark SQL queries to be executed
+        sparksql = [
+            "SELECT COUNT(email) AS email_count_last_24_hours, COUNT(name) AS name_count_last_24_hours, deviceid FROM temp_table WHERE deviceid={deviceid} AND timestamp_unix > {timestamp} - 86400 and timestamp_unix < {timestamp_base} GROUP BY deviceid",
+            "SELECT COUNT(email) AS email_count_last_6_days, COUNT(name) AS name_count_last_6_days, deviceid FROM temp_table WHERE deviceid={deviceid} AND timestamp_unix > {timestamp} - 604800 and timestamp_unix < {timestamp_base} GROUP BY deviceid",
+            "SELECT COUNT(email) AS email_count_last_7_days, COUNT(name) AS name_count_last_7_days, deviceid FROM temp_table WHERE deviceid={deviceid} AND timestamp_unix > {timestamp} - 604800 and timestamp_unix < {timestamp_base} GROUP BY deviceid",
+            "SELECT COUNT(email) AS email_count_last_15_days, COUNT(name) AS name_count_last_15_days, deviceid FROM temp_table WHERE deviceid={deviceid} AND timestamp_unix > {timestamp} - 1296000 and timestamp_unix < {timestamp_base} GROUP BY deviceid",
+            "SELECT COUNT(email) AS email_count_last_45_days, COUNT(name) AS name_count_last_45_days, deviceid FROM temp_table WHERE deviceid={deviceid} AND timestamp_unix > {timestamp} - 3.888e+6 and timestamp_unix < {timestamp_base} GROUP BY deviceid",
+        ]
+        json_data = request.get_json()
+        timestamp = json_data.get('timestamp')
+        deviceid = json_data.get('deviceid')
+        token = json_data.get('token')
+
+        materialize_instance = materialize(mongo_connection, timestamp, "deviceid", deviceid, token, custom_schema.schema, sparksql, partition_column="deviceid")
 
-    materialize_instance = materialize(mongo_connection, timestamp, "deviceid", deviceid, token, custom_schema.schema, sparksql, partition_column="deviceid")
+        aggregated_data_str = materialize_instance.read_data_and_aggregate()
+        aggregated_data = json.loads(aggregated_data_str)
 
-    aggregated_data_str = materialize_instance.read_data_and_aggregate()
-    aggregated_data = json.loads(aggregated_data_str)
+        return jsonify(aggregated_data)
 
-    return jsonify(aggregated_data)
+    except Exception as e:
+        return jsonify({"Result":"No data found","error": str(e)})
 
 if __name__ == '__main__':
     app.run(debug=True, port=5001)
```

### Comparing `featurizerai-1.4.8/src/features/tests/test_pipeline.py` & `featurizerai-1.4.9/src/features/tests/test_pipeline.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,14 +29,16 @@
 
     # Create a new instance of the create_stream class
     featurizerai = create_stream(kafka_connection, mongo_connection, "fake-data_test5", "timestamp")
 
     # Start the Kafka consumer in a separate thread
     featurizerai.start(token)
 
+    featurizerai.stop()
+
     # # Run the consumer for 60 seconds
     # time.sleep(60)
     #
     # # Stop the consumer and wait for the thread to finish
     # featurizerai.stop()
 def main():
     token = authenticate_user()
```

### Comparing `featurizerai-1.4.8/src/featurizerai.egg-info/PKG-INFO` & `featurizerai-1.4.9/src/featurizerai.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurizerai
-Version: 1.4.8
+Version: 1.4.9
 Summary: Python library for Featurizer AI
 Home-page: https://github.com/burakglobal/featurizerai
 Author: Burak
 Author-email: burakgblobal@gmail.com
 Keywords: featurizer,package
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

