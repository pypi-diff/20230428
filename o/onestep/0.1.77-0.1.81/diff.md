# Comparing `tmp/onestep-0.1.77.tar.gz` & `tmp/onestep-0.1.81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onestep-0.1.77.tar", max compression
+gzip compressed data, was "onestep-0.1.81.tar", max compression
```

## Comparing `onestep-0.1.77.tar` & `onestep-0.1.81.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0     1362 2023-04-26 03:26:00.698862 onestep-0.1.77/README.md
--rw-r--r--   0        0        0      704 2023-04-26 03:26:00.698862 onestep-0.1.77/pyproject.toml
--rw-r--r--   0        0        0     1374 2023-04-26 03:26:00.698862 onestep-0.1.77/src/onestep/__init__.py
--rw-r--r--   0        0        0      221 2023-04-26 03:26:00.698862 onestep-0.1.77/src/onestep/broker/__init__.py
--rw-r--r--   0        0        0     4543 2023-04-26 03:26:00.698862 onestep-0.1.77/src/onestep/broker/base.py
--rw-r--r--   0        0        0      957 2023-04-26 03:26:00.698862 onestep-0.1.77/src/onestep/broker/cron.py
--rw-r--r--   0        0        0      151 2023-04-26 03:26:00.698862 onestep-0.1.77/src/onestep/broker/memory.py
--rw-r--r--   0        0        0     2423 2023-04-26 03:26:00.698862 onestep-0.1.77/src/onestep/broker/rabbitmq.py
--rw-r--r--   0        0        0     2144 2023-04-26 03:26:00.698862 onestep-0.1.77/src/onestep/broker/webhook.py
--rw-r--r--   0        0        0      610 2023-04-26 03:26:00.698862 onestep-0.1.77/src/onestep/exception.py
--rw-r--r--   0        0        0     4530 2023-04-26 03:26:00.698862 onestep-0.1.77/src/onestep/message.py
--rw-r--r--   0        0        0      286 2023-04-26 03:26:00.698862 onestep-0.1.77/src/onestep/middleware/__init__.py
--rw-r--r--   0        0        0      521 2023-04-26 03:26:00.698862 onestep-0.1.77/src/onestep/middleware/base.py
--rw-r--r--   0        0        0     2438 2023-04-26 03:26:00.698862 onestep-0.1.77/src/onestep/middleware/config.py
--rw-r--r--   0        0        0     6350 2023-04-26 03:26:00.698862 onestep-0.1.77/src/onestep/onestep.py
--rw-r--r--   0        0        0     2699 2023-04-26 03:26:00.698862 onestep-0.1.77/src/onestep/retry.py
--rw-r--r--   0        0        0      293 2023-04-26 03:26:00.702862 onestep-0.1.77/src/onestep/signal.py
--rw-r--r--   0        0        0      618 2023-04-26 03:26:00.702862 onestep-0.1.77/src/onestep/state.py
--rw-r--r--   0        0        0       36 2023-04-26 03:26:00.702862 onestep-0.1.77/src/onestep/store/__init__.py
--rw-r--r--   0        0        0     4466 2023-04-26 03:26:00.702862 onestep-0.1.77/src/onestep/store/rabbitmq.py
--rw-r--r--   0        0        0     3516 2023-04-26 03:26:00.702862 onestep-0.1.77/src/onestep/worker.py
--rw-r--r--   0        0        0     1993 1970-01-01 00:00:00.000000 onestep-0.1.77/PKG-INFO
+-rw-r--r--   0        0        0     1362 2023-04-28 02:40:02.210281 onestep-0.1.81/README.md
+-rw-r--r--   0        0        0      704 2023-04-28 02:40:02.210281 onestep-0.1.81/pyproject.toml
+-rw-r--r--   0        0        0     1390 2023-04-28 02:40:02.210281 onestep-0.1.81/src/onestep/__init__.py
+-rw-r--r--   0        0        0      414 2023-04-28 02:40:02.210281 onestep-0.1.81/src/onestep/_utils.py
+-rw-r--r--   0        0        0      221 2023-04-28 02:40:02.210281 onestep-0.1.81/src/onestep/broker/__init__.py
+-rw-r--r--   0        0        0     4543 2023-04-28 02:40:02.210281 onestep-0.1.81/src/onestep/broker/base.py
+-rw-r--r--   0        0        0      957 2023-04-28 02:40:02.210281 onestep-0.1.81/src/onestep/broker/cron.py
+-rw-r--r--   0        0        0      151 2023-04-28 02:40:02.210281 onestep-0.1.81/src/onestep/broker/memory.py
+-rw-r--r--   0        0        0     2271 2023-04-28 02:40:02.210281 onestep-0.1.81/src/onestep/broker/rabbitmq.py
+-rw-r--r--   0        0        0     2144 2023-04-28 02:40:02.210281 onestep-0.1.81/src/onestep/broker/webhook.py
+-rw-r--r--   0        0        0      610 2023-04-28 02:40:02.210281 onestep-0.1.81/src/onestep/exception.py
+-rw-r--r--   0        0        0     4543 2023-04-28 02:40:02.210281 onestep-0.1.81/src/onestep/message.py
+-rw-r--r--   0        0        0      286 2023-04-28 02:40:02.210281 onestep-0.1.81/src/onestep/middleware/__init__.py
+-rw-r--r--   0        0        0      521 2023-04-28 02:40:02.210281 onestep-0.1.81/src/onestep/middleware/base.py
+-rw-r--r--   0        0        0     2438 2023-04-28 02:40:02.210281 onestep-0.1.81/src/onestep/middleware/config.py
+-rw-r--r--   0        0        0     6350 2023-04-28 02:40:02.210281 onestep-0.1.81/src/onestep/onestep.py
+-rw-r--r--   0        0        0     2699 2023-04-28 02:40:02.210281 onestep-0.1.81/src/onestep/retry.py
+-rw-r--r--   0        0        0      293 2023-04-28 02:40:02.210281 onestep-0.1.81/src/onestep/signal.py
+-rw-r--r--   0        0        0      618 2023-04-28 02:40:02.210281 onestep-0.1.81/src/onestep/state.py
+-rw-r--r--   0        0        0       86 2023-04-28 02:40:02.210281 onestep-0.1.81/src/onestep/store/__init__.py
+-rw-r--r--   0        0        0     4466 2023-04-28 02:40:02.210281 onestep-0.1.81/src/onestep/store/rabbitmq.py
+-rw-r--r--   0        0        0     3516 2023-04-28 02:40:02.210281 onestep-0.1.81/src/onestep/worker.py
+-rw-r--r--   0        0        0     1993 1970-01-01 00:00:00.000000 onestep-0.1.81/PKG-INFO
```

### Comparing `onestep-0.1.77/README.md` & `onestep-0.1.81/README.md`

 * *Files identical despite different names*

### Comparing `onestep-0.1.77/pyproject.toml` & `onestep-0.1.81/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "onestep"
-version = "0.1.77"
+version = "0.1.81"
 description = ""
 authors = ["miclon <jcnd@163.com>"]
 readme = "README.md"
 packages = [
     { include = 'onestep', from = 'src' }
 ]
```

### Comparing `onestep-0.1.77/src/onestep/__init__.py` & `onestep-0.1.81/src/onestep/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,44 +15,44 @@
 from .exception import (
     StopMiddleware, DropMessage,
     RetryException, RetryViaQueue, RetryViaLocal
 )
 
 __all__ = [
     'step',
-
+    
     # broker
     'BaseBroker',
     'BaseConsumer',
     'BaseLocalBroker',
     'BaseLocalConsumer',
     'MemoryBroker',
     'RabbitMQBroker',
     'WebHookBroker',
     'CronBroker',
-
+    
     # retry
     'BaseRetry',
     'NeverRetry',
     'AlwaysRetry',
     'TimesRetry',
     'RetryIfException',
     'AdvancedRetry',
     # error callback
     'BaseErrorCallback',
     'NackErrorCallBack',
-
+    
     # middleware
     'BaseMiddleware',
     'BaseConfigMiddleware',
     'NacosPublishConfigMiddleware',
     'NacosConsumeConfigMiddleware',
     'RedisPublishConfigMiddleware',
     'RedisConsumeConfigMiddleware',
-
+    
     # exception
     'StopMiddleware',
     'DropMessage',
     'RetryException',
     'RetryViaQueue',
     'RetryViaLocal'
 ]
```

### Comparing `onestep-0.1.77/src/onestep/broker/base.py` & `onestep-0.1.81/src/onestep/broker/base.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.77/src/onestep/broker/cron.py` & `onestep-0.1.81/src/onestep/broker/cron.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.77/src/onestep/broker/rabbitmq.py` & `onestep-0.1.81/src/onestep/broker/rabbitmq.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,31 +33,31 @@
         return RabbitMQConsumer(self.queue)
 
     def publish(self, message: Any):
         self.client.send(self.queue_name, message)
 
     def confirm(self, message: Message):
         """确认消息"""
-        self.client.channel.basic.ack(message.msg.delivery_tag)
+        message.msg.ack()
 
     def reject(self, message: Message):
         """拒绝消息"""
-        self.client.channel.basic.nack(message.msg.delivery_tag, requeue=False)
+        message.msg.reject(requeue=False)
 
     def requeue(self, message: Message, is_source=False):
         """
         重发消息：先拒绝 再 重入
         
         :param message: 消息
         :param is_source: 是否是源消息，True: 使用消息的最新数据重入当前队列，False: 使用消息的最新数据重入当前队列
         """
         if is_source:
-            self.client.channel.basic.nack(message.msg.delivery_tag, requeue=True)
+            message.msg.reject(requeue=True)
         else:
-            self.client.channel.basic.nack(message.msg.delivery_tag, requeue=False)
+            message.msg.reject(requeue=False)
             self.send(message)
 
 
 class RabbitMQConsumer(BaseConsumer):
     def _to_message(self, data: amqpstorm.Message):
         try:
             message = json.loads(data.body)
```

### Comparing `onestep-0.1.77/src/onestep/broker/webhook.py` & `onestep-0.1.81/src/onestep/broker/webhook.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.77/src/onestep/exception.py` & `onestep-0.1.81/src/onestep/exception.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.77/src/onestep/message.py` & `onestep-0.1.81/src/onestep/message.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import json
 import sys
 import time
 import uuid
 from traceback import format_exception, TracebackException
 from typing import Optional, Any, Union
 
+from onestep._utils import catch_error
+
 
 class Extra:
     def __init__(self, task_id=None, publish_time=None, failure_count=0):
         self.task_id = task_id or str(uuid.uuid4())
         self.publish_time = publish_time or round(time.time(), 3)
         self.failure_count = failure_count
     
@@ -105,32 +107,32 @@
                     data['exception'] = str(self.exception)
         
         return data
     
     def to_json(self, include_exception=False) -> str:
         return json.dumps(self.to_dict(include_exception))
     
+    @catch_error()
     def confirm(self):
         """确认消息"""
-        if self.broker:
-            self.broker.confirm(self)
+        self.broker.confirm(self)
     
+    @catch_error()
     def reject(self):
         """拒绝消息"""
-        if self.broker:
-            self.broker.reject(self)
+        self.broker.reject(self)
     
+    @catch_error()
     def requeue(self, is_source=False):
         """
         重发消息：先拒绝 再 重入
         
         :param is_source: 是否是源消息，True: 使用消息的最新数据重入当前队列，False: 使用消息的最新数据重入当前队列
         """
-        if self.broker:
-            self.broker.requeue(self, is_source=is_source)
+        self.broker.requeue(self, is_source=is_source)
     
     def __getattr__(self, item):
         return None
     
     def __delattr__(self, item):
         if hasattr(self, item):
             setattr(self, item, None)
```

### Comparing `onestep-0.1.77/src/onestep/middleware/base.py` & `onestep-0.1.81/src/onestep/middleware/base.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.77/src/onestep/middleware/config.py` & `onestep-0.1.81/src/onestep/middleware/config.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.77/src/onestep/onestep.py` & `onestep-0.1.81/src/onestep/onestep.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.77/src/onestep/retry.py` & `onestep-0.1.81/src/onestep/retry.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.77/src/onestep/state.py` & `onestep-0.1.81/src/onestep/state.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.77/src/onestep/store/rabbitmq.py` & `onestep-0.1.81/src/onestep/store/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.77/src/onestep/worker.py` & `onestep-0.1.81/src/onestep/worker.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.77/PKG-INFO` & `onestep-0.1.81/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onestep
-Version: 0.1.77
+Version: 0.1.81
 Summary: 
 Author: miclon
 Author-email: jcnd@163.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

