# Comparing `tmp/citizenk-0.1.21.tar.gz` & `tmp/citizenk-0.1.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citizenk-0.1.21.tar", max compression
+gzip compressed data, was "citizenk-0.1.22.tar", max compression
```

## Comparing `citizenk-0.1.21.tar` & `citizenk-0.1.22.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      310 2023-03-29 19:05:43.686872 citizenk-0.1.21/citizenk/__init__.py
--rw-r--r--   0        0        0     3788 2023-03-29 19:05:42.121589 citizenk-0.1.21/citizenk/agent.py
--rw-r--r--   0        0        0    17717 2023-03-31 08:50:09.117648 citizenk-0.1.21/citizenk/citizenk.py
--rw-r--r--   0        0        0    20513 2023-03-31 08:37:43.679744 citizenk-0.1.21/citizenk/kafka_adapter.py
--rw-r--r--   0        0        0     1715 2023-03-21 12:34:01.052758 citizenk-0.1.21/citizenk/murmur2.py
--rw-r--r--   0        0        0     4800 2023-03-31 07:11:57.561185 citizenk-0.1.21/citizenk/topic.py
--rw-r--r--   0        0        0      413 2023-03-26 13:09:50.145208 citizenk-0.1.21/citizenk/utils.py
--rw-r--r--   0        0        0     1497 2023-03-31 08:50:30.937788 citizenk-0.1.21/pyproject.toml
--rw-r--r--   0        0        0      870 2023-03-31 08:50:37.022984 citizenk-0.1.21/setup.py
--rw-r--r--   0        0        0     1083 2023-03-31 08:50:37.023419 citizenk-0.1.21/PKG-INFO
+-rw-r--r--   0        0        0      310 2023-04-04 18:14:45.297052 citizenk-0.1.22/citizenk/__init__.py
+-rw-r--r--   0        0        0     3788 2023-04-04 18:14:45.297131 citizenk-0.1.22/citizenk/agent.py
+-rw-r--r--   0        0        0    18077 2023-04-28 07:38:42.095328 citizenk-0.1.22/citizenk/citizenk.py
+-rw-r--r--   0        0        0    20509 2023-04-04 18:14:45.297447 citizenk-0.1.22/citizenk/kafka_adapter.py
+-rw-r--r--   0        0        0     1715 2023-04-04 18:14:45.297535 citizenk-0.1.22/citizenk/murmur2.py
+-rw-r--r--   0        0        0     4802 2023-04-04 18:14:45.297629 citizenk-0.1.22/citizenk/topic.py
+-rw-r--r--   0        0        0      413 2023-04-04 18:14:45.297697 citizenk-0.1.22/citizenk/utils.py
+-rw-r--r--   0        0        0     1522 2023-04-28 07:41:45.960993 citizenk-0.1.22/pyproject.toml
+-rw-r--r--   0        0        0      870 2023-04-28 07:41:51.038426 citizenk-0.1.22/setup.py
+-rw-r--r--   0        0        0     1083 2023-04-28 07:41:51.038681 citizenk-0.1.22/PKG-INFO
```

### Comparing `citizenk-0.1.21/citizenk/agent.py` & `citizenk-0.1.22/citizenk/agent.py`

 * *Files identical despite different names*

### Comparing `citizenk-0.1.21/citizenk/citizenk.py` & `citizenk-0.1.22/citizenk/citizenk.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,29 +38,31 @@
         app_name: str,
         app_type: AppType = AppType.SOURCE,
         consumer_group_init_offset: str = "latest",
         schema_registry_url: Optional[str] = None,
         auto_generate_apis: bool = True,
         max_processing_cycle_ms: int = 5 * 1000,
         api_router_prefix: str = "",
+        api_port: Optional[int] = None,
         *args,
         **kwargs,
     ):
         super().__init__(*args, **kwargs)
         self.app_name = app_name
         self.app_type = app_type
         self.kafka_config = kafka_config
         self.consumer_group_init_offset = consumer_group_init_offset
         self.schema_registry_url = schema_registry_url
         self.auto_generate_apis = auto_generate_apis
         self.max_processing_cycle_ms = max_processing_cycle_ms
         self.api_router_prefix = api_router_prefix
+        self.api_port = api_port
         self.producer = None
         self.consumer = None
-        self.started = datetime.utcnow()
+        self._started = datetime.utcnow()
 
         self.total_batch_size = 0
         self.consumer_topics = set()
         self.topics = {}
         self.agents = {}
         self.main_consumer_loop_task = None
         self.monitor_loop_task = None
@@ -96,15 +98,15 @@
             assignments = {}
             lag = {}
             if self.consumer is not None:
                 hosts = self.consumer.get_group_members()
                 assignments = self.consumer.assigned_partitions
                 lag = self.consumer.get_group_lag()
             return {
-                "started": self.started,
+                "started": self._started,
                 "app": {
                     "name": self.app_name,
                     "title": self.title,
                     "description": self.description,
                     "version": self.version,
                 },
                 "topics": {
@@ -338,20 +340,21 @@
                 self, agent_name, f, topics, batch_size, return_type, websocket_route
             )
             logger.debug("Adding agent %s %s", agent_name, topics)
             return wrapper
 
         return decorator
 
-    def topic_router(self,topic: Topic,match_info: str) -> Callable:
+    def topic_router(self, topic: Topic, match_info: str) -> Callable:
         """
         routes the request to the right worker based on topic, key:
         assumes default partitioner... Used mainly for statefule services where
         Each worker holds some state / key
         """
+
         def decorator(f):
             @wraps(f)
             async def wrapper(*args, **kwargs):
                 if self.consumer is None or self.consumer.consumer_group_name is None:
                     raise CitizenKError(
                         "Topic routing doesn't make sense without a consumer group"
                     )
@@ -389,15 +392,17 @@
                 if topic.name in self.consumer.assigned_partitions:
                     if partition_id in self.consumer.assigned_partitions[topic.name]:
                         return await f(*args, **kwargs)
 
                 members = self.consumer.get_group_members()
                 host = members.get((topic.name, partition_id), None)
                 if host is None:
-                    raise CitizenKError(f"Can't find a host for this request {topic.name}/{partition_id}")
+                    raise CitizenKError(
+                        f"Can't find a host for this request {topic.name}/{partition_id}"
+                    )
 
                 # Route the request to the host
                 request = kwargs["request"]
                 params = dict(request.query_params)
                 if "citizenk_stop_propogate" in params:
                     return await f(*args, **kwargs)
                 params["citizenk_stop_propogate"] = True
@@ -410,15 +415,15 @@
                         headers=request.headers.raw,
                         params=params,
                         content=await request.body(),
                         timeout=10.0,
                     )
                     try:
                         return r.json()
-                    except  json.JSONDecodeError:
+                    except json.JSONDecodeError:
                         return r.text
 
             return wrapper
 
         return decorator
 
     def broadcast_router(self) -> Callable:
@@ -451,14 +456,18 @@
                     return await f(*args, **kwargs)
                 params["citizenk_stop_propogate"] = True
 
                 response = {}
                 async with httpx.AsyncClient() as client:
                     for host in hosts:
                         url = httpx.URL(str(request.url)).copy_with(host=host)
+                        # Mainly used for testing purposes
+                        if self.api_port != None:
+                            url = url.copy_with(port=self.api_port)
+                        logger.debug("Broadcast to %s",url)
                         r = await client.request(
                             method=request.method,
                             url=url,
                             headers=request.headers.raw,
                             params=params,
                             content=await request.body(),
                             timeout=10.0,
```

### Comparing `citizenk-0.1.21/citizenk/kafka_adapter.py` & `citizenk-0.1.22/citizenk/kafka_adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 import subprocess
 import sys
 import tempfile
 from collections import defaultdict
 from dataclasses import dataclass
 from enum import Enum
-from typing import Any, Dict, List, Optional, Union, Tuple
+from typing import Any, Dict, List, Optional, Tuple, Union
 
 import certifi
 from confluent_kafka import (
     Consumer,
     KafkaError,
     KafkaException,
     Message,
@@ -276,15 +276,15 @@
             return []
 
         for p in committed:
             if p.offset > 0:
                 group_topics.add(p.topic)
         return list(group_topics)
 
-    def get_group_lag(self) -> Dict[str,int]:
+    def get_group_lag(self) -> Dict[str, int]:
         """Get the total lag of the group for each topic"""
         group_topics = defaultdict(int)
         if self.role != KafkaRole.CONSUMER or self.consumer_group_name is None:
             return group_topics
 
         partitions = self.get_all_broker_partitions()
         try:
@@ -378,15 +378,15 @@
         else:
             logger.debug(
                 "Successfully deleted offsets for group %s topic %s", group, topic
             )
         os.remove(temp_config_filename)
         return error_code
 
-    def delete_old_offsets_for_group(self)  -> int:
+    def delete_old_offsets_for_group(self) -> int:
         if self.role != KafkaRole.CONSUMER:
             return 0
         if not self.consumer_started:
             return 0
         if self.consumer_group_name is None:
             return 0
         # Check if the consumer group has unwanted topics if so, delete them
@@ -435,15 +435,15 @@
             else:
                 self.connection.assign(source_partitions)
         self.consumer_topics = topics
         self.consumer_started = True
         logger.debug("Finished setting up consumer, and starting consuming")
 
     @staticmethod
-    def messages_to_dict(messages: List[Message]) -> List[Dict[str,Any]]:
+    def messages_to_dict(messages: List[Message]) -> List[Dict[str, Any]]:
         try:
             return [
                 {
                     "topic": m.topic(),
                     "key": m.key().decode("utf-8") if m.key() is not None else None,
                     "value": json.loads(m.value()),
                     "partition": m.partition(),
@@ -467,24 +467,25 @@
             else:
                 self._on_kafka_error(error)
             self.topic_stats[msg.topic()] += 1
         logger.debug("Consumed %s Kafka messages", len(msgs))
         return msgs
 
     def produce(
-        self, topic: str, value: Any, key: Optional[Any] = None, partition: int = -1, headers: Optional[Dict[str,bytes]] = None
+        self,
+        topic: str,
+        value: Any,
+        key: Optional[Any] = None,
+        partition: int = -1,
+        headers: Optional[Dict[str, bytes]] = None,
     ):
         """Produce a message to the given topic"""
         self.topic_stats[topic] += 1
         self.connection.produce(
-            topic,
-            value=value,
-            key=key,
-            partition=partition,
-            headers=headers
+            topic, value=value, key=key, partition=partition, headers=headers
         )
 
     def _on_kafka_commit(self, err: KafkaError, partitions: List[TopicPartition]):
         logger.debug("Kafka committed %s %s", err, partitions)
 
     def _on_kafka_stats(self, json_str: str):
         self.last_stats = json.loads(json_str)
@@ -504,15 +505,15 @@
             self.assigned_partitions[p.topic].discard(p.partition)
 
     def _on_kafka_lost(self, consumer, partitions: List[TopicPartition]):
         logger.info("Group rebalancing. Partitions lost %s", partitions)
         for p in partitions:
             self.assigned_partitions[p.topic].discard(p.partition)
 
-    def get_topic_stats(self) -> Dict[str,int]:
+    def get_topic_stats(self) -> Dict[str, int]:
         result = self.topic_stats
         self.topic_stats = defaultdict(int)
         return result
 
     def messages_in_queue(self) -> int:
         if self.role != KafkaRole.PRODUCER:
             return 0
```

### Comparing `citizenk-0.1.21/citizenk/murmur2.py` & `citizenk-0.1.22/citizenk/murmur2.py`

 * *Files identical despite different names*

### Comparing `citizenk-0.1.21/citizenk/topic.py` & `citizenk-0.1.22/citizenk/topic.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     def __init__(
         self,
         app: CitizenK,
         name: str,
         value_type: BaseModel,
         topic_dir: TopicDir = TopicDir.INPUT,
         subject_name: str | None = None,
-        partitioner: Callable[[str | bytes],int] = None
+        partitioner: Callable[[str | bytes], int] = None,
     ):
         self.app = app
         self.name = name
         self.value_type = value_type
         self.topic_dir = topic_dir
         self.subject_name = (
             f"{name}-value".lower() if subject_name is None else subject_name
@@ -93,15 +93,15 @@
                 return False
         if not isinstance(value, BaseModel):
             raise CitizenKError("Value should be a pydantic model", value)
         if not isinstance(key, (str, bytes)):
             raise CitizenKError("Key should be a either a str or bytes", key)
         if self.partitioner is not None and partition == -1:
             partition = self.partitioner(key)
-        # TODO: Add schmea to headers
+        # TODO: Add schema to headers
         self.app.producer.produce(
             topic=self.name, value=value.json(), key=key, partition=partition
         )
         return True
 
     def manage_schema(self):
         """Handle schema registry registration and validation"""
```

### Comparing `citizenk-0.1.21/pyproject.toml` & `citizenk-0.1.22/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "citizenk"
-version = "0.1.21"
+version = "0.1.22"
 description = "An async Kafka Python Framework based on FastAPI and Confluent Kafka"
 authors = ["Valerann <info@valerann.com>"]
 maintainers = ["Valerann <info@valerann.com>"]
 license = "Apache-2.0"
 homepage = "https://pypi.org/user/valerann/"
 repository = "https://github.com/Valerann/citizenk"
 keywords = ["kafka", "fastapi"]
@@ -30,14 +30,15 @@
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.3"
 assertpy = "^1.1"
 pytest-xdist = "^2.5.0"
 pytest-mock = "^3.8.2"
 pytest-asyncio = "^0.21.0"
 websocket-client = "^1.5.1"
+pytest-dotenv = "^0.5.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
     py36 = true
```

### Comparing `citizenk-0.1.21/setup.py` & `citizenk-0.1.22/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'fastapi-utils>=0.2.1,<0.3.0',
  'fastapi>=0.92.0,<0.93.0',
  'httpx>=0.23.3,<0.24.0',
  'websockets>=10.4,<11.0']
 
 setup_kwargs = {
     'name': 'citizenk',
-    'version': '0.1.21',
+    'version': '0.1.22',
     'description': 'An async Kafka Python Framework based on FastAPI and Confluent Kafka',
     'long_description': None,
     'author': 'Valerann',
     'author_email': 'info@valerann.com',
     'maintainer': 'Valerann',
     'maintainer_email': 'info@valerann.com',
     'url': 'https://pypi.org/user/valerann/',
```

### Comparing `citizenk-0.1.21/PKG-INFO` & `citizenk-0.1.22/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citizenk
-Version: 0.1.21
+Version: 0.1.22
 Summary: An async Kafka Python Framework based on FastAPI and Confluent Kafka
 Home-page: https://pypi.org/user/valerann/
 License: Apache-2.0
 Keywords: kafka,fastapi
 Author: Valerann
 Author-email: info@valerann.com
 Maintainer: Valerann
```

