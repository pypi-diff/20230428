# Comparing `tmp/whitson_tool_helper-0.1.1.tar.gz` & `tmp/whitson_tool_helper-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whitson_tool_helper-0.1.1.tar", last modified: Thu Apr 27 15:53:20 2023, max compression
+gzip compressed data, was "whitson_tool_helper-0.1.2.tar", last modified: Fri Apr 28 08:44:24 2023, max compression
```

## Comparing `whitson_tool_helper-0.1.1.tar` & `whitson_tool_helper-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxr-xr-x   0 tuedachu  (1000) tuedachu  (1000)        0 2023-04-27 15:53:20.839941 whitson_tool_helper-0.1.1/
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      404 2023-04-27 15:53:20.839941 whitson_tool_helper-0.1.1/PKG-INFO
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      705 2023-04-27 15:53:15.000000 whitson_tool_helper-0.1.1/pyproject.toml
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)       38 2023-04-27 15:53:20.839941 whitson_tool_helper-0.1.1/setup.cfg
-drwxr-xr-x   0 tuedachu  (1000) tuedachu  (1000)        0 2023-04-27 15:53:20.839941 whitson_tool_helper-0.1.1/src/
-drwxr-xr-x   0 tuedachu  (1000) tuedachu  (1000)        0 2023-04-27 15:53:20.839941 whitson_tool_helper-0.1.1/src/whitson_tool_helper/
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      107 2023-04-26 09:24:26.000000 whitson_tool_helper-0.1.1/src/whitson_tool_helper/__init__.py
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)       66 2023-04-26 13:22:55.000000 whitson_tool_helper-0.1.1/src/whitson_tool_helper/logger.py
-drwxr-xr-x   0 tuedachu  (1000) tuedachu  (1000)        0 2023-04-27 15:53:20.839941 whitson_tool_helper-0.1.1/src/whitson_tool_helper/messaging/
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      370 2023-04-26 13:32:24.000000 whitson_tool_helper-0.1.1/src/whitson_tool_helper/messaging/aux.py
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)     2988 2023-04-27 15:14:46.000000 whitson_tool_helper-0.1.1/src/whitson_tool_helper/messaging/main.py
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)     4403 2023-04-26 14:33:47.000000 whitson_tool_helper-0.1.1/src/whitson_tool_helper/messaging/pubsub.py
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)     3969 2023-04-27 13:40:01.000000 whitson_tool_helper-0.1.1/src/whitson_tool_helper/messaging/rabbitmq.py
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      574 2023-04-26 07:15:11.000000 whitson_tool_helper-0.1.1/src/whitson_tool_helper/timeout.py
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      704 2023-04-26 12:52:42.000000 whitson_tool_helper-0.1.1/src/whitson_tool_helper/whitson_exceptions.py
-drwxr-xr-x   0 tuedachu  (1000) tuedachu  (1000)        0 2023-04-27 15:53:20.839941 whitson_tool_helper-0.1.1/src/whitson_tool_helper.egg-info/
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      138 2023-04-26 12:44:58.000000 whitson_tool_helper-0.1.1/src/whitson_tool_helper.egg-info/.SOURCES.txt.~undo-tree~
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      404 2023-04-27 15:53:20.000000 whitson_tool_helper-0.1.1/src/whitson_tool_helper.egg-info/PKG-INFO
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      630 2023-04-27 15:53:20.000000 whitson_tool_helper-0.1.1/src/whitson_tool_helper.egg-info/SOURCES.txt
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)        1 2023-04-27 15:53:20.000000 whitson_tool_helper-0.1.1/src/whitson_tool_helper.egg-info/dependency_links.txt
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      116 2023-04-27 15:53:20.000000 whitson_tool_helper-0.1.1/src/whitson_tool_helper.egg-info/requires.txt
--rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)       20 2023-04-27 15:53:20.000000 whitson_tool_helper-0.1.1/src/whitson_tool_helper.egg-info/top_level.txt
+drwxr-xr-x   0 tuedachu  (1000) tuedachu  (1000)        0 2023-04-28 08:44:24.399978 whitson_tool_helper-0.1.2/
+-rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      404 2023-04-28 08:44:24.389978 whitson_tool_helper-0.1.2/PKG-INFO
+-rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      705 2023-04-28 08:44:18.000000 whitson_tool_helper-0.1.2/pyproject.toml
+-rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)       38 2023-04-28 08:44:24.399978 whitson_tool_helper-0.1.2/setup.cfg
+drwxr-xr-x   0 tuedachu  (1000) tuedachu  (1000)        0 2023-04-28 08:44:24.389978 whitson_tool_helper-0.1.2/src/
+drwxr-xr-x   0 tuedachu  (1000) tuedachu  (1000)        0 2023-04-28 08:44:24.389978 whitson_tool_helper-0.1.2/src/whitson_tool_helper/
+-rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      107 2023-04-26 09:24:26.000000 whitson_tool_helper-0.1.2/src/whitson_tool_helper/__init__.py
+-rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)       66 2023-04-26 13:22:55.000000 whitson_tool_helper-0.1.2/src/whitson_tool_helper/logger.py
+drwxr-xr-x   0 tuedachu  (1000) tuedachu  (1000)        0 2023-04-28 08:44:24.389978 whitson_tool_helper-0.1.2/src/whitson_tool_helper/messaging/
+-rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      370 2023-04-26 13:32:24.000000 whitson_tool_helper-0.1.2/src/whitson_tool_helper/messaging/aux.py
+-rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)     2738 2023-04-28 08:39:14.000000 whitson_tool_helper-0.1.2/src/whitson_tool_helper/messaging/main.py
+-rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)     4403 2023-04-26 14:33:47.000000 whitson_tool_helper-0.1.2/src/whitson_tool_helper/messaging/pubsub.py
+-rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)     3494 2023-04-28 08:40:03.000000 whitson_tool_helper-0.1.2/src/whitson_tool_helper/messaging/rabbitmq.py
+-rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      574 2023-04-26 07:15:11.000000 whitson_tool_helper-0.1.2/src/whitson_tool_helper/timeout.py
+-rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      704 2023-04-26 12:52:42.000000 whitson_tool_helper-0.1.2/src/whitson_tool_helper/whitson_exceptions.py
+drwxr-xr-x   0 tuedachu  (1000) tuedachu  (1000)        0 2023-04-28 08:44:24.389978 whitson_tool_helper-0.1.2/src/whitson_tool_helper.egg-info/
+-rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      404 2023-04-28 08:44:24.000000 whitson_tool_helper-0.1.2/src/whitson_tool_helper.egg-info/PKG-INFO
+-rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      572 2023-04-28 08:44:24.000000 whitson_tool_helper-0.1.2/src/whitson_tool_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)        1 2023-04-28 08:44:24.000000 whitson_tool_helper-0.1.2/src/whitson_tool_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)      116 2023-04-28 08:44:24.000000 whitson_tool_helper-0.1.2/src/whitson_tool_helper.egg-info/requires.txt
+-rw-r--r--   0 tuedachu  (1000) tuedachu  (1000)       20 2023-04-28 08:44:24.000000 whitson_tool_helper-0.1.2/src/whitson_tool_helper.egg-info/top_level.txt
```

### Comparing `whitson_tool_helper-0.1.1/pyproject.toml` & `whitson_tool_helper-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "whitson_tool_helper"
-version =  "0.1.1"
+version =  "0.1.2"
 authors = [
   { name="Markus Blytt", email="blytt@whitson.com" },
   { name="Jason Hu", email="jason@whitson.com" },
   { name="Arnaud Hoffmann", email="arnaud@whitson.com" },
 ]
 description = "A Toolbox for whitson cloud software solutions"
 dependencies = ["pika==1.3.1", "google-auth==2.16.0","google-cloud-pubsub==2.14.0", "google-cloud-storage==2.7.0","google-cloud-logging==3.5.0"]
```

### Comparing `whitson_tool_helper-0.1.1/src/whitson_tool_helper/messaging/main.py` & `whitson_tool_helper-0.1.2/src/whitson_tool_helper/messaging/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,21 +31,17 @@
             self._consumer = rabbitmq.RabbitMQConsumer(process_function)
         else:
             raise MessagingSystemNotSupportedError(messaging_system)
 
         self._messaging_system = messaging_system
 
     def work(self):
-        restart = False
         while True:
             LOGGER.info("Connecting to server...")
             try:
-                if restart and self._messaging_system == MessagingSystem.rabbitmq:
-                    print("Reopening connection...")
-                    self._consumer.reopen_connection()
                 self._consumer.work()
             except KeyboardInterrupt:
                 LOGGER.info("Keyboard interrupt!")
                 LOGGER.info("Consumer shut down!")
                 sys.exit()
             except ChannelClosedByBroker as e:
                 LOGGER.error("-- RABBITMQ ACCESS REFUSED --")
@@ -53,15 +49,14 @@
                 sys.exit()
             except Exception as e:
                 LOGGER.error("-- UNKNOWN ERROR ENCOUNTERED --")
                 LOGGER.error(e)
             finally:
                 if self._messaging_system == MessagingSystem.rabbitmq:
                     self._consumer.connection.close()
-                    restart = True
                 LOGGER.warning("Restarting worker")
 
 
 class Publisher:
     def __init__(self, messaging_system: MessagingSystem, exchange: str = None):
         if messaging_system == MessagingSystem.pubsub:
             from whitson_tool_helper.messaging import pubsub
```

### Comparing `whitson_tool_helper-0.1.1/src/whitson_tool_helper/messaging/pubsub.py` & `whitson_tool_helper-0.1.2/src/whitson_tool_helper/messaging/pubsub.py`

 * *Files identical despite different names*

### Comparing `whitson_tool_helper-0.1.1/src/whitson_tool_helper/messaging/rabbitmq.py` & `whitson_tool_helper-0.1.2/src/whitson_tool_helper/messaging/rabbitmq.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,27 +54,14 @@
             process_function(data=msg["data"], meta_data=msg["meta_data"])
             LOGGER.info("  ---  SUCCESS  ---  ")
             ch.basic_ack(delivery_tag=method.delivery_tag)
             LOGGER.info(f"Listening to {method.routing_key} ...")
 
         self.channel.basic_consume(queue=subscription, on_message_callback=callback)
 
-    def reopen_connection(self):
-        parameters = get_rabbitmq_params()
-        self.connection = pika.BlockingConnection(parameters)
-        self.channel = self.connection.channel()
-        subscription = os.getenv("MESSAGING_SUBSCRIPTION")
-        self.channel.queue_declare(
-            queue=subscription,
-            durable=True,
-            arguments={"x-max-priority": 100, "x-queue-type": "classic"},
-        )
-
-        self.channel.basic_qos(prefetch_count=1)
-
     def work(self):
         self.channel.start_consuming()
 
 
 class RabbitMQPublisher:
     def __init__(self, exchange):
         self.parameters = get_rabbitmq_params()
```

### Comparing `whitson_tool_helper-0.1.1/src/whitson_tool_helper/timeout.py` & `whitson_tool_helper-0.1.2/src/whitson_tool_helper/timeout.py`

 * *Files identical despite different names*

### Comparing `whitson_tool_helper-0.1.1/src/whitson_tool_helper/whitson_exceptions.py` & `whitson_tool_helper-0.1.2/src/whitson_tool_helper/whitson_exceptions.py`

 * *Files identical despite different names*

### Comparing `whitson_tool_helper-0.1.1/src/whitson_tool_helper.egg-info/SOURCES.txt` & `whitson_tool_helper-0.1.2/src/whitson_tool_helper.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 pyproject.toml
 src/whitson_tool_helper/__init__.py
 src/whitson_tool_helper/logger.py
 src/whitson_tool_helper/timeout.py
 src/whitson_tool_helper/whitson_exceptions.py
-src/whitson_tool_helper.egg-info/.SOURCES.txt.~undo-tree~
 src/whitson_tool_helper.egg-info/PKG-INFO
 src/whitson_tool_helper.egg-info/SOURCES.txt
 src/whitson_tool_helper.egg-info/dependency_links.txt
 src/whitson_tool_helper.egg-info/requires.txt
 src/whitson_tool_helper.egg-info/top_level.txt
 src/whitson_tool_helper/messaging/aux.py
 src/whitson_tool_helper/messaging/main.py
```

