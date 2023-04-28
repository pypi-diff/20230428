# Comparing `tmp/patchwork-client-kafka-0.1.4.tar.gz` & `tmp/patchwork-client-kafka-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/patchwork-client-kafka-0.1.4.tar", last modified: Wed Mar  1 19:11:41 2023, max compression
+gzip compressed data, was "dist/patchwork-client-kafka-0.1.5.tar", last modified: Fri Apr 28 15:24:53 2023, max compression
```

## Comparing `patchwork-client-kafka-0.1.4.tar` & `patchwork-client-kafka-0.1.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-01 19:11:41.000000 patchwork-client-kafka-0.1.4/
--rw-rw-rw-   0 root         (0) root         (0)     1056 2023-03-01 19:11:28.000000 patchwork-client-kafka-0.1.4/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       58 2023-03-01 19:11:28.000000 patchwork-client-kafka-0.1.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1032 2023-03-01 19:11:41.000000 patchwork-client-kafka-0.1.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      316 2023-03-01 19:11:28.000000 patchwork-client-kafka-0.1.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-01 19:11:41.000000 patchwork-client-kafka-0.1.4/int/
--rw-rw-rw-   0 root         (0) root         (0)     2410 2023-03-01 19:11:28.000000 patchwork-client-kafka-0.1.4/int/test_integration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-01 19:11:41.000000 patchwork-client-kafka-0.1.4/patchwork/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-01 19:11:41.000000 patchwork-client-kafka-0.1.4/patchwork/client/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-01 19:11:41.000000 patchwork-client-kafka-0.1.4/patchwork/client/kafka/
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-03-01 19:11:28.000000 patchwork-client-kafka-0.1.4/patchwork/client/kafka/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3623 2023-03-01 19:11:28.000000 patchwork-client-kafka-0.1.4/patchwork/client/kafka/common.py
--rw-rw-rw-   0 root         (0) root         (0)     9749 2023-03-01 19:11:28.000000 patchwork-client-kafka-0.1.4/patchwork/client/kafka/publisher.py
--rw-rw-rw-   0 root         (0) root         (0)    18187 2023-03-01 19:11:28.000000 patchwork-client-kafka-0.1.4/patchwork/client/kafka/subscriber.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-01 19:11:41.000000 patchwork-client-kafka-0.1.4/patchwork_client_kafka.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1032 2023-03-01 19:11:41.000000 patchwork-client-kafka-0.1.4/patchwork_client_kafka.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      556 2023-03-01 19:11:41.000000 patchwork-client-kafka-0.1.4/patchwork_client_kafka.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-01 19:11:41.000000 patchwork-client-kafka-0.1.4/patchwork_client_kafka.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-01 19:11:41.000000 patchwork-client-kafka-0.1.4/patchwork_client_kafka.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       52 2023-03-01 19:11:41.000000 patchwork-client-kafka-0.1.4/patchwork_client_kafka.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-03-01 19:11:41.000000 patchwork-client-kafka-0.1.4/patchwork_client_kafka.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       51 2023-03-01 19:11:28.000000 patchwork-client-kafka-0.1.4/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-01 19:11:41.000000 patchwork-client-kafka-0.1.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1676 2023-03-01 19:11:28.000000 patchwork-client-kafka-0.1.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-01 19:11:41.000000 patchwork-client-kafka-0.1.4/tests/
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-03-01 19:11:28.000000 patchwork-client-kafka-0.1.4/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      314 2023-03-01 19:11:28.000000 patchwork-client-kafka-0.1.4/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)       51 2023-03-01 19:11:28.000000 patchwork-client-kafka-0.1.4/tests/test_clientkafka.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 15:24:53.000000 patchwork-client-kafka-0.1.5/
+-rw-rw-rw-   0 root         (0) root         (0)     1056 2023-04-28 15:24:39.000000 patchwork-client-kafka-0.1.5/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       58 2023-04-28 15:24:39.000000 patchwork-client-kafka-0.1.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1032 2023-04-28 15:24:53.000000 patchwork-client-kafka-0.1.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      316 2023-04-28 15:24:39.000000 patchwork-client-kafka-0.1.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 15:24:53.000000 patchwork-client-kafka-0.1.5/int/
+-rw-rw-rw-   0 root         (0) root         (0)     2410 2023-04-28 15:24:39.000000 patchwork-client-kafka-0.1.5/int/test_integration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 15:24:53.000000 patchwork-client-kafka-0.1.5/patchwork/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 15:24:53.000000 patchwork-client-kafka-0.1.5/patchwork/client/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 15:24:53.000000 patchwork-client-kafka-0.1.5/patchwork/client/kafka/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-04-28 15:24:39.000000 patchwork-client-kafka-0.1.5/patchwork/client/kafka/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3623 2023-04-28 15:24:39.000000 patchwork-client-kafka-0.1.5/patchwork/client/kafka/common.py
+-rw-rw-rw-   0 root         (0) root         (0)     9749 2023-04-28 15:24:39.000000 patchwork-client-kafka-0.1.5/patchwork/client/kafka/publisher.py
+-rw-rw-rw-   0 root         (0) root         (0)    18195 2023-04-28 15:24:39.000000 patchwork-client-kafka-0.1.5/patchwork/client/kafka/subscriber.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 15:24:53.000000 patchwork-client-kafka-0.1.5/patchwork_client_kafka.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1032 2023-04-28 15:24:53.000000 patchwork-client-kafka-0.1.5/patchwork_client_kafka.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      556 2023-04-28 15:24:53.000000 patchwork-client-kafka-0.1.5/patchwork_client_kafka.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 15:24:53.000000 patchwork-client-kafka-0.1.5/patchwork_client_kafka.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 15:24:53.000000 patchwork-client-kafka-0.1.5/patchwork_client_kafka.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       52 2023-04-28 15:24:53.000000 patchwork-client-kafka-0.1.5/patchwork_client_kafka.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-04-28 15:24:53.000000 patchwork-client-kafka-0.1.5/patchwork_client_kafka.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       51 2023-04-28 15:24:39.000000 patchwork-client-kafka-0.1.5/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-28 15:24:53.000000 patchwork-client-kafka-0.1.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1676 2023-04-28 15:24:39.000000 patchwork-client-kafka-0.1.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 15:24:53.000000 patchwork-client-kafka-0.1.5/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-04-28 15:24:39.000000 patchwork-client-kafka-0.1.5/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      314 2023-04-28 15:24:39.000000 patchwork-client-kafka-0.1.5/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)       51 2023-04-28 15:24:39.000000 patchwork-client-kafka-0.1.5/tests/test_clientkafka.py
```

### Comparing `patchwork-client-kafka-0.1.4/LICENSE` & `patchwork-client-kafka-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `patchwork-client-kafka-0.1.4/PKG-INFO` & `patchwork-client-kafka-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: patchwork-client-kafka
-Version: 0.1.4
+Version: 0.1.5
 Summary: Kafka client for Patchwork - The distributed asynchronous microframework
 Home-page: 
 Author: Pawel Pecio
 Author-email: 
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `patchwork-client-kafka-0.1.4/int/test_integration.py` & `patchwork-client-kafka-0.1.5/int/test_integration.py`

 * *Files identical despite different names*

### Comparing `patchwork-client-kafka-0.1.4/patchwork/client/kafka/common.py` & `patchwork-client-kafka-0.1.5/patchwork/client/kafka/common.py`

 * *Files identical despite different names*

### Comparing `patchwork-client-kafka-0.1.4/patchwork/client/kafka/publisher.py` & `patchwork-client-kafka-0.1.5/patchwork/client/kafka/publisher.py`

 * *Files identical despite different names*

### Comparing `patchwork-client-kafka-0.1.4/patchwork/client/kafka/subscriber.py` & `patchwork-client-kafka-0.1.5/patchwork/client/kafka/subscriber.py`

 * *Files 0% similar despite different names*

```diff
@@ -297,15 +297,15 @@
                 # this TP has already a task in process, so there is no tasks to fetch
                 # on partitions which are not in process (were prioritized above)
                 self.consumer.seek(tp, msg.offset)
                 try:
                     # wait until something resumed or short period, so if something arrives at
                     # not in process TP it will be processed
                     await asyncio.wait_for(self._resumed.wait(), timeout=0.250)
-                except TimeoutError:
+                except asyncio.TimeoutError:
                     pass
                 else:
                     self._resumed.clear()
                 continue
 
             try:
                 # wait for getter no longer then half pool interval
```

### Comparing `patchwork-client-kafka-0.1.4/patchwork_client_kafka.egg-info/PKG-INFO` & `patchwork-client-kafka-0.1.5/patchwork_client_kafka.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: patchwork-client-kafka
-Version: 0.1.4
+Version: 0.1.5
 Summary: Kafka client for Patchwork - The distributed asynchronous microframework
 Home-page: 
 Author: Pawel Pecio
 Author-email: 
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `patchwork-client-kafka-0.1.4/patchwork_client_kafka.egg-info/SOURCES.txt` & `patchwork-client-kafka-0.1.5/patchwork_client_kafka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `patchwork-client-kafka-0.1.4/setup.py` & `patchwork-client-kafka-0.1.5/setup.py`

 * *Files identical despite different names*

