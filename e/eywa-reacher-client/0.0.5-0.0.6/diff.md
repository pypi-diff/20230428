# Comparing `tmp/eywa-reacher-client-0.0.5.tar.gz` & `tmp/eywa-reacher-client-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eywa-reacher-client-0.0.5.tar", last modified: Wed Mar 29 17:41:23 2023, max compression
+gzip compressed data, was "eywa-reacher-client-0.0.6.tar", last modified: Fri Apr 28 13:56:07 2023, max compression
```

## Comparing `eywa-reacher-client-0.0.5.tar` & `eywa-reacher-client-0.0.6.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rw-r--r--   0        0        0     6148 2022-04-15 15:13:21.951104 eywa-reacher-client-0.0.5/.DS_Store
--rw-r--r--   0        0        0     1080 2023-02-17 10:08:38.060538 eywa-reacher-client-0.0.5/LICENSE
--rw-r--r--   0        0        0      121 2022-04-15 15:13:21.951239 eywa-reacher-client-0.0.5/README.md
--rw-r--r--   0        0        0        0 2022-04-15 15:13:21.951363 eywa-reacher-client-0.0.5/examples/__init__.py
--rw-r--r--   0        0        0      742 2023-02-23 12:16:33.603767 eywa-reacher-client-0.0.5/examples/graphql.py
--rw-r--r--   0        0        0      668 2023-02-17 10:08:38.063044 eywa-reacher-client-0.0.5/examples/raw_graphql.py
--rw-r--r--   0        0        0      584 2023-02-17 10:08:38.064690 eywa-reacher-client-0.0.5/examples/webdriver.py
--rw-r--r--   0        0        0      414 2023-03-29 17:36:05.426403 eywa-reacher-client-0.0.5/pyproject.toml
--rw-r--r--   0        0        0    13358 2023-03-29 17:41:15.419091 eywa-reacher-client-0.0.5/src/eywa.py
--rw-r--r--   0        0        0      392 1970-01-01 00:00:00.000000 eywa-reacher-client-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     6148 2022-04-15 15:13:21.951104 eywa-reacher-client-0.0.6/.DS_Store
+-rw-r--r--   0        0        0     1080 2023-02-17 10:08:38.060538 eywa-reacher-client-0.0.6/LICENSE
+-rw-r--r--   0        0        0      121 2022-04-15 15:13:21.951239 eywa-reacher-client-0.0.6/README.md
+-rw-r--r--   0        0        0        0 2022-04-15 15:13:21.951363 eywa-reacher-client-0.0.6/examples/__init__.py
+-rw-r--r--   0        0        0       25 2023-03-29 17:54:52.518026 eywa-reacher-client-0.0.6/examples/config.txt
+-rw-r--r--   0        0        0       78 2023-03-29 17:54:52.518895 eywa-reacher-client-0.0.6/examples/echo.py
+-rw-r--r--   0        0        0      745 2023-04-28 13:52:46.149280 eywa-reacher-client-0.0.6/examples/graphql.py
+-rw-r--r--   0        0        0      668 2023-02-17 10:08:38.063044 eywa-reacher-client-0.0.6/examples/raw_graphql.py
+-rw-r--r--   0        0        0      584 2023-02-17 10:08:38.064690 eywa-reacher-client-0.0.6/examples/webdriver.py
+-rw-r--r--   0        0        0      414 2023-04-28 13:54:11.756101 eywa-reacher-client-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0    13604 2023-04-28 13:54:10.405821 eywa-reacher-client-0.0.6/src/eywa.py
+-rw-r--r--   0        0        0      392 1970-01-01 00:00:00.000000 eywa-reacher-client-0.0.6/PKG-INFO
```

### Comparing `eywa-reacher-client-0.0.5/.DS_Store` & `eywa-reacher-client-0.0.6/.DS_Store`

 * *Files identical despite different names*

### Comparing `eywa-reacher-client-0.0.5/LICENSE` & `eywa-reacher-client-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `eywa-reacher-client-0.0.5/examples/graphql.py` & `eywa-reacher-client-0.0.6/examples/graphql.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,14 @@
     "customer-subsidy-input": {
         "ban": "527624975",
         "first-name": "f_name",
         "last-name": "l_name",
         "ticket-id": "17.02.2023 13:08/38975209909/",
         "category": "217812"
         }
-    }})
+    }}, 2)
 
 print('Response:\n' + str(response))
 
 
 # {"jsonrpc":"2.0","id":0,"result":100} 
 # {"jsonrpc":"2.0","id":0,"error": {"code": -32602, "message": "Fucker"}}
```

### Comparing `eywa-reacher-client-0.0.5/examples/raw_graphql.py` & `eywa-reacher-client-0.0.6/examples/raw_graphql.py`

 * *Files identical despite different names*

### Comparing `eywa-reacher-client-0.0.5/examples/webdriver.py` & `eywa-reacher-client-0.0.6/examples/webdriver.py`

 * *Files identical despite different names*

### Comparing `eywa-reacher-client-0.0.5/src/eywa.py` & `eywa-reacher-client-0.0.6/src/eywa.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """EYWA Reacher client"""
 
 __author__ = "Robert Gersak"
 __email__ = "r.gersak@gmail.com"
 __license__ = "MIT"
 __status__ = "Development"
-__version__ = "0.0.5"
+__version__ = "0.0.6"
 
 
 import time
 import datetime
 import json
 import sys
 import threading
@@ -126,21 +126,23 @@
 
     def __del__(self):
         connection = getattr(self, "_line", None)
         if connection:
             connection.stop()
 
     @classmethod
-    def request(cls, method, params):
+    def request(cls, method, params, timeout = None):
         # check if the call is a notification
         eywa = EYWA()
         # create a new id for requests expecting a response
         eywa._i += 1
         id = eywa._i
 
+        now = time.time();
+
         # store an empty result for the meantime
         eywa._results[id] = EMPTY_RESULT
 
         # create the request
         req = generate_request(method, id=id, params=params)
         eywa._write(req)
 
@@ -150,15 +152,18 @@
             if eywa._results[id] != EMPTY_RESULT:
                 result = eywa._results[id]
                 del eywa._results[id]
                 if isinstance(result, Exception):
                    raise result
                 else:
                     return result
-            time.sleep(0.1)
+            elif timeout is not None  and time.time() - now > timeout:
+                raise ValueError('EYWA silent error. Timeout occured for:\n' + req)
+            else:
+                time.sleep(0.1)
 
     @classmethod
     def notify(cls, method, data = None):
         eywa = EYWA()
         req = generate_request(method, None, data)
         eywa._write(req)
 
@@ -523,11 +528,11 @@
     EYWA.notify("task.update",{"status":status})
 
 
 def return_task():
     EYWA.notify("task.return")
     sys.exit(0)
 
-def graphql(query):
-    return EYWA.request("eywa.datasets.graphql", query)
+def graphql(query, timeout = None):
+    return EYWA.request("eywa.datasets.graphql", query, timeout)
 
 eywa = EYWA()
```

