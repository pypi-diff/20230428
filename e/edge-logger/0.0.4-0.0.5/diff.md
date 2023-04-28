# Comparing `tmp/edge_logger-0.0.4.tar.gz` & `tmp/edge_logger-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edge_logger-0.0.4.tar", max compression
+gzip compressed data, was "edge_logger-0.0.5.tar", max compression
```

## Comparing `edge_logger-0.0.4.tar` & `edge_logger-0.0.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-04-16 19:59:55.248252 edge_logger-0.0.4/LICENSE
--rw-r--r--   0        0        0        0 2023-04-17 03:01:06.502367 edge_logger-0.0.4/README.md
--rw-r--r--   0        0        0        0 2023-04-16 20:07:03.564649 edge_logger-0.0.4/edge_logger/__init__.py
--rw-r--r--   0        0        0     5325 2023-04-27 03:18:19.983133 edge_logger-0.0.4/edge_logger/edge_logger.py
--rw-r--r--   0        0        0      380 2023-04-27 03:23:08.613589 edge_logger-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      480 1970-01-01 00:00:00.000000 edge_logger-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-16 19:59:55.248252 edge_logger-0.0.5/LICENSE
+-rw-r--r--   0        0        0        0 2023-04-17 03:01:06.502367 edge_logger-0.0.5/README.md
+-rw-r--r--   0        0        0        0 2023-04-16 20:07:03.564649 edge_logger-0.0.5/edge_logger/__init__.py
+-rw-r--r--   0        0        0     5700 2023-04-28 06:17:30.970678 edge_logger-0.0.5/edge_logger/edge_logger.py
+-rw-r--r--   0        0        0      380 2023-04-28 06:26:05.689175 edge_logger-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      480 1970-01-01 00:00:00.000000 edge_logger-0.0.5/PKG-INFO
```

### Comparing `edge_logger-0.0.4/LICENSE` & `edge_logger-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `edge_logger-0.0.4/edge_logger/edge_logger.py` & `edge_logger-0.0.5/edge_logger/edge_logger.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     def __init__(self, url: str):
         """
         Initializes the custom http handler
         Parameters:
             url (str): The URL that the logs will be sent to
         """
         self.url = url
-        #self.token = token
+        # self.token = token
 
         # sets up a session with the server
         self.MAX_POOLSIZE = 100
         self.session = session = requests.Session()
         session.headers.update({
             'Content-Type': 'application/json'
         })
@@ -34,29 +34,39 @@
             ),
             pool_connections=self.MAX_POOLSIZE,
             pool_maxsize=self.MAX_POOLSIZE
         ))
 
         super().__init__()
 
-    def emit_process_entry(self, record):
-        json_log = self.format(record)
+    def emit_process_entry(self, json_log):
+        # Send the POST request with the JSON data and headers
         response = self.session.post(self.url, data=json_log)
         return response
 
     def emit(self, record):
         """
         This function gets called when a log event gets emitted. It receives a
         record, formats it and sends it to the url
         Parameters:
             record: a log record
         """
-        # self.emit_process_entry(record)
+        json_log = self.format(record)
         with concurrent.futures.ProcessPoolExecutor() as executor:
-            future = executor.submit(self.emit_process_entry, record)
+            future = executor.submit(emit_entry_process_out, json_log, self.url)
+            ret = future.result()
+            print(ret)
+        # self.emit_process_entry(record)
+
+
+def emit_entry_process_out(json_log, url):
+    # Send the POST request with the JSON data and headers
+    headers = {'Content-Type': 'application/json'}
+    response = requests.post(url, data=json_log, headers=headers)
+    return response
 
 
 class JsonFormatter(logging.Formatter):
 
     def __init__(self, indent=False):
         super().__init__()
         self._indent = indent
```

