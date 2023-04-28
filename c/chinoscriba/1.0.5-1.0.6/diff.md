# Comparing `tmp/chinoscriba-1.0.5.tar.gz` & `tmp/chinoscriba-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chinoscriba-1.0.5.tar", last modified: Wed Apr 19 10:22:02 2023, max compression
+gzip compressed data, was "chinoscriba-1.0.6.tar", last modified: Fri Apr 28 12:14:25 2023, max compression
```

## Comparing `chinoscriba-1.0.5.tar` & `chinoscriba-1.0.6.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 10:22:02.387193 chinoscriba-1.0.5/
--rw-r--r--   0 root         (0) root         (0)     3621 2023-04-19 10:22:02.387193 chinoscriba-1.0.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3181 2022-08-24 15:25:53.000000 chinoscriba-1.0.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 10:22:02.383192 chinoscriba-1.0.5/chinoscriba/
--rw-r--r--   0 root         (0) root         (0)     1377 2023-04-19 10:22:02.000000 chinoscriba-1.0.5/chinoscriba/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 10:22:02.387193 chinoscriba-1.0.5/chinoscriba/api/
--rw-r--r--   0 root         (0) root         (0)      277 2023-04-19 10:22:02.000000 chinoscriba-1.0.5/chinoscriba/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8189 2023-04-19 10:22:01.000000 chinoscriba-1.0.5/chinoscriba/api/blocks_api.py
--rw-r--r--   0 root         (0) root         (0)    25311 2023-04-19 10:22:01.000000 chinoscriba-1.0.5/chinoscriba/api/events_api.py
--rw-r--r--   0 root         (0) root         (0)    25634 2023-04-19 10:22:01.000000 chinoscriba-1.0.5/chinoscriba/api/logs_api.py
--rw-r--r--   0 root         (0) root         (0)     7718 2023-04-19 10:22:01.000000 chinoscriba-1.0.5/chinoscriba/api/stats_api.py
--rw-r--r--   0 root         (0) root         (0)    24814 2023-04-19 10:22:02.000000 chinoscriba-1.0.5/chinoscriba/api_client.py
--rw-r--r--   0 root         (0) root         (0)     8796 2023-04-19 10:22:02.000000 chinoscriba-1.0.5/chinoscriba/configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 10:22:02.387193 chinoscriba-1.0.5/chinoscriba/models/
--rw-r--r--   0 root         (0) root         (0)     1041 2023-04-19 10:22:02.000000 chinoscriba-1.0.5/chinoscriba/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14568 2023-04-19 10:22:00.000000 chinoscriba-1.0.5/chinoscriba/models/audit_log.py
--rw-r--r--   0 root         (0) root         (0)    11485 2023-04-19 10:22:00.000000 chinoscriba-1.0.5/chinoscriba/models/block.py
--rw-r--r--   0 root         (0) root         (0)     7000 2023-04-19 10:22:01.000000 chinoscriba-1.0.5/chinoscriba/models/event.py
--rw-r--r--   0 root         (0) root         (0)     5253 2023-04-19 10:22:01.000000 chinoscriba-1.0.5/chinoscriba/models/inline_response200.py
--rw-r--r--   0 root         (0) root         (0)     5273 2023-04-19 10:22:01.000000 chinoscriba-1.0.5/chinoscriba/models/inline_response2001.py
--rw-r--r--   0 root         (0) root         (0)     5267 2023-04-19 10:22:01.000000 chinoscriba-1.0.5/chinoscriba/models/inline_response2002.py
--rw-rw-rw-   0 root         (0) root         (0)     5150 2022-08-24 15:25:53.000000 chinoscriba-1.0.5/chinoscriba/models/inline_response200_bis.py
--rw-r--r--   0 root         (0) root         (0)    16827 2023-04-19 10:22:01.000000 chinoscriba-1.0.5/chinoscriba/models/log.py
--rw-r--r--   0 root         (0) root         (0)     3362 2023-04-19 10:22:01.000000 chinoscriba-1.0.5/chinoscriba/models/multi_audit_log_serializer_output.py
--rw-r--r--   0 root         (0) root         (0)     3803 2023-04-19 10:22:01.000000 chinoscriba-1.0.5/chinoscriba/models/search_request.py
--rw-r--r--   0 root         (0) root         (0)     4075 2023-04-19 10:22:01.000000 chinoscriba-1.0.5/chinoscriba/models/sort_rule.py
--rw-r--r--   0 root         (0) root         (0)     8028 2023-04-19 10:22:01.000000 chinoscriba-1.0.5/chinoscriba/models/stat.py
--rw-rw-rw-   0 root         (0) root         (0)    13815 2023-04-19 09:49:35.000000 chinoscriba-1.0.5/chinoscriba/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 10:22:02.387193 chinoscriba-1.0.5/chinoscriba.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3621 2023-04-19 10:22:02.000000 chinoscriba-1.0.5/chinoscriba.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      959 2023-04-19 10:22:02.000000 chinoscriba-1.0.5/chinoscriba.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 10:22:02.000000 chinoscriba-1.0.5/chinoscriba.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       48 2023-04-19 10:22:02.000000 chinoscriba-1.0.5/chinoscriba.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-04-19 10:22:02.000000 chinoscriba-1.0.5/chinoscriba.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-19 10:22:02.387193 chinoscriba-1.0.5/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1318 2023-04-19 10:22:02.000000 chinoscriba-1.0.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 10:22:02.387193 chinoscriba-1.0.5/test/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-24 15:25:53.000000 chinoscriba-1.0.5/test/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18730 2022-08-24 15:25:53.000000 chinoscriba-1.0.5/test/test_default_api.py
--rw-rw-rw-   0 root         (0) root         (0)     1316 2022-08-24 15:25:53.000000 chinoscriba-1.0.5/test/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 12:14:25.362982 chinoscriba-1.0.6/
+-rw-r--r--   0 root         (0) root         (0)     4195 2023-04-28 12:14:25.362982 chinoscriba-1.0.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3755 2023-04-27 16:58:59.000000 chinoscriba-1.0.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 12:14:25.358981 chinoscriba-1.0.6/chinoscriba/
+-rw-r--r--   0 root         (0) root         (0)     1377 2023-04-28 12:14:24.000000 chinoscriba-1.0.6/chinoscriba/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 12:14:25.358981 chinoscriba-1.0.6/chinoscriba/api/
+-rw-r--r--   0 root         (0) root         (0)      277 2023-04-28 12:14:24.000000 chinoscriba-1.0.6/chinoscriba/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8189 2023-04-28 12:14:24.000000 chinoscriba-1.0.6/chinoscriba/api/blocks_api.py
+-rw-r--r--   0 root         (0) root         (0)    25311 2023-04-28 12:14:24.000000 chinoscriba-1.0.6/chinoscriba/api/events_api.py
+-rw-r--r--   0 root         (0) root         (0)    25634 2023-04-28 12:14:24.000000 chinoscriba-1.0.6/chinoscriba/api/logs_api.py
+-rw-r--r--   0 root         (0) root         (0)     7718 2023-04-28 12:14:24.000000 chinoscriba-1.0.6/chinoscriba/api/stats_api.py
+-rw-r--r--   0 root         (0) root         (0)    24814 2023-04-28 12:14:25.000000 chinoscriba-1.0.6/chinoscriba/api_client.py
+-rw-r--r--   0 root         (0) root         (0)     8796 2023-04-28 12:14:24.000000 chinoscriba-1.0.6/chinoscriba/configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 12:14:25.362982 chinoscriba-1.0.6/chinoscriba/models/
+-rw-r--r--   0 root         (0) root         (0)     1041 2023-04-28 12:14:24.000000 chinoscriba-1.0.6/chinoscriba/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14568 2023-04-28 12:14:24.000000 chinoscriba-1.0.6/chinoscriba/models/audit_log.py
+-rw-r--r--   0 root         (0) root         (0)    11485 2023-04-28 12:14:24.000000 chinoscriba-1.0.6/chinoscriba/models/block.py
+-rw-r--r--   0 root         (0) root         (0)     7000 2023-04-28 12:14:24.000000 chinoscriba-1.0.6/chinoscriba/models/event.py
+-rw-r--r--   0 root         (0) root         (0)     5253 2023-04-28 12:14:24.000000 chinoscriba-1.0.6/chinoscriba/models/inline_response200.py
+-rw-r--r--   0 root         (0) root         (0)     5273 2023-04-28 12:14:24.000000 chinoscriba-1.0.6/chinoscriba/models/inline_response2001.py
+-rw-r--r--   0 root         (0) root         (0)     5267 2023-04-28 12:14:24.000000 chinoscriba-1.0.6/chinoscriba/models/inline_response2002.py
+-rw-rw-rw-   0 root         (0) root         (0)     5150 2022-08-24 15:25:53.000000 chinoscriba-1.0.6/chinoscriba/models/inline_response200_bis.py
+-rw-r--r--   0 root         (0) root         (0)    16827 2023-04-28 12:14:24.000000 chinoscriba-1.0.6/chinoscriba/models/log.py
+-rw-r--r--   0 root         (0) root         (0)     3362 2023-04-28 12:14:24.000000 chinoscriba-1.0.6/chinoscriba/models/multi_audit_log_serializer_output.py
+-rw-r--r--   0 root         (0) root         (0)     3803 2023-04-28 12:14:24.000000 chinoscriba-1.0.6/chinoscriba/models/search_request.py
+-rw-r--r--   0 root         (0) root         (0)     4075 2023-04-28 12:14:24.000000 chinoscriba-1.0.6/chinoscriba/models/sort_rule.py
+-rw-r--r--   0 root         (0) root         (0)     8028 2023-04-28 12:14:24.000000 chinoscriba-1.0.6/chinoscriba/models/stat.py
+-rw-rw-rw-   0 root         (0) root         (0)    14078 2023-04-27 16:58:59.000000 chinoscriba-1.0.6/chinoscriba/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 12:14:25.358981 chinoscriba-1.0.6/chinoscriba.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4195 2023-04-28 12:14:25.000000 chinoscriba-1.0.6/chinoscriba.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      959 2023-04-28 12:14:25.000000 chinoscriba-1.0.6/chinoscriba.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 12:14:25.000000 chinoscriba-1.0.6/chinoscriba.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2023-04-28 12:14:25.000000 chinoscriba-1.0.6/chinoscriba.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-04-28 12:14:25.000000 chinoscriba-1.0.6/chinoscriba.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-28 12:14:25.362982 chinoscriba-1.0.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1318 2023-04-28 12:14:25.000000 chinoscriba-1.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 12:14:25.362982 chinoscriba-1.0.6/test/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-24 15:25:53.000000 chinoscriba-1.0.6/test/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18730 2022-08-24 15:25:53.000000 chinoscriba-1.0.6/test/test_default_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1316 2022-08-24 15:25:53.000000 chinoscriba-1.0.6/test/utils.py
```

### Comparing `chinoscriba-1.0.5/PKG-INFO` & `chinoscriba-1.0.6/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: chinoscriba
-Version: 1.0.5
-Summary: Chino.io Scriba SDK Python
-Home-page: https://www.chino.io
-Author-email: 
-License: UNKNOWN
-Keywords: Chino.io Scriba API
-Platform: UNKNOWN
-Classifier: Topic :: Software Development
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-
 Chino.io :: Scriba Documentation: the Application Programming Interface
 
 This Python package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:
 
 - API version: v1
 - Package version: 1.0.0
 - Build package: io.swagger.codegen.v3.generators.python.PythonClientCodegen
@@ -39,77 +24,87 @@
 from pprint import pprint
 
 # Configure HTTP basic authorization: Basic
 configuration = chinoscriba.Configuration()
 configuration.username = 'customer_id'
 configuration.password = 'customer_key'
 
-# create an instance of the API class
-api_instance = chinoscriba.DefaultApi(chinoscriba.ApiClient(configuration))
+# create an instance of the API classes
+logs_api = chinoscriba.LogsApi(chinoscriba.ApiClient(configuration))
+stats_api = chinoscriba.StatsApi(chinoscriba.ApiClient(configuration))
+blocks_api = chinoscriba.BlocksApi(chinoscriba.ApiClient(configuration))
+
 limit = 56 # int | Number of results to return per page
 offset = 0 # int | The initial index from which to return the results
 
 
 # # Audit logs # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # 
 
 # Create a new Log
 body = chinoscriba.AuditLog() # AuditLog | 
 try:
-    api_response = api_instance.logs_create(body)
+    api_response = logs_api.logs_create(body)
     pprint(api_response)
 except ApiException as e:
     print("Exception when calling DefaultApi->logs_create: %s\n" % e)
 
 
 # Create multiple Logs (bulk)
 body = [chinoscriba.AuditLog()] # list[AuditLog] | 
 try:
-    api_response = api_instance.logs_multiple(body)
+    api_response = logs_api.logs_multiple(body)
     pprint(api_response)
 except ApiException as e:
     print("Exception when calling DefaultApi->logs_multiple: %s\n" % e)
 
 try:
     # List all Logs
-    api_response = api_instance.logs_list(limit=limit, offset=offset)
+    api_response = logs_api.logs_list(limit=limit, offset=offset)
     pprint(api_response)
 except ApiException as e:
     print("Exception when calling DefaultApi->logs_list: %s\n" % e)
 
 try:
     # Search by query
-    api_response = api_instance.logs_search(body, limit=limit, offset=offset)
+    api_response = logs_api.logs_search(body, limit=limit, offset=offset)
     pprint(api_response)
 except ApiException as e:
     print("Exception when calling DefaultApi->logs_search: %s\n" % e)
 
+# # Stats # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # 
+    
 try:
     # Retrieve customer statistics
-    api_response = api_instance.stats_read()
+    api_response = stats_api.stats_read()
     pprint(api_response)
 except ApiException as e:
     print("Exception when calling DefaultApi->stats_read: %s\n" % e)
 
 
 # # Exporter # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # 
 
 try:
     # List exportable Blocks
-    api_response = api_instance.exported_list(limit=limit, offset=offset)
+    api_response = blocks_api.exported_list(limit=limit, offset=offset)
     pprint(api_response)
 except ApiException as e:
     print("Exception when calling DefaultApi->exported_list: %s\n" % e)
 
 
 # Export a Block
 block_id = "" # string | ID of the Block to download
 try:
-    api_instance.exported_read(block_id)
+    # NOTE: due to an issue in a third-party library, this only works with 
+    #  '_preload_content' disabled. This will bypass the malfunctioning code
+    #  and return directly the HTTPResponse, which contains the zip file bytes
+    #  in the 'data' attribute.
+    res = blocks_api.exported_read(block_id, _preload_content=False)
+    zip_bytes = res.data  # You can read this using python library 'zipfile'.
 except ApiException as e:
-    print("Exception when calling DefaultApi->exported_read: %s\n" % e)
+    print("Exception when calling BlocksApi->exported_read: %s\n" % e)
 
 ```
 
 ## Changelog
 
 ### [next] - unreleased
 - fixed events' tests
@@ -119,9 +114,7 @@
 - added support for new events endpoints
 - removed unique class `DefaultApi` in favour of specific classes based on
   endpoint semantic groups: `LogApi`, `BlockApi`, `EventsApi`, `StatsApi`
 
 ### [1.0.1] - 2021-01-15
 - `DefaultApi` class which manages logs (create, list, search) and block
    downloads
-
-
```

### Comparing `chinoscriba-1.0.5/chinoscriba/__init__.py` & `chinoscriba-1.0.6/chinoscriba/__init__.py`

 * *Files identical despite different names*

### Comparing `chinoscriba-1.0.5/chinoscriba/api/blocks_api.py` & `chinoscriba-1.0.6/chinoscriba/api/blocks_api.py`

 * *Files identical despite different names*

### Comparing `chinoscriba-1.0.5/chinoscriba/api/events_api.py` & `chinoscriba-1.0.6/chinoscriba/api/events_api.py`

 * *Files identical despite different names*

### Comparing `chinoscriba-1.0.5/chinoscriba/api/logs_api.py` & `chinoscriba-1.0.6/chinoscriba/api/logs_api.py`

 * *Files identical despite different names*

### Comparing `chinoscriba-1.0.5/chinoscriba/api/stats_api.py` & `chinoscriba-1.0.6/chinoscriba/api/stats_api.py`

 * *Files identical despite different names*

### Comparing `chinoscriba-1.0.5/chinoscriba/api_client.py` & `chinoscriba-1.0.6/chinoscriba/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         self.pool = ThreadPool()
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'Swagger-Codegen/1.0.5/python'
+        self.user_agent = 'Swagger-Codegen/1.0.6/python'
 
     def __del__(self):
         self.pool.close()
         self.pool.join()
 
     @property
     def user_agent(self):
```

### Comparing `chinoscriba-1.0.5/chinoscriba/configuration.py` & `chinoscriba-1.0.6/chinoscriba/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -257,9 +257,9 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: v1\n"\
-               "SDK Package Version: 1.0.5".\
+               "SDK Package Version: 1.0.6".\
                format(env=sys.platform, pyversion=sys.version)
```

### Comparing `chinoscriba-1.0.5/chinoscriba/models/__init__.py` & `chinoscriba-1.0.6/chinoscriba/models/__init__.py`

 * *Files identical despite different names*

### Comparing `chinoscriba-1.0.5/chinoscriba/models/audit_log.py` & `chinoscriba-1.0.6/chinoscriba/models/audit_log.py`

 * *Files identical despite different names*

### Comparing `chinoscriba-1.0.5/chinoscriba/models/block.py` & `chinoscriba-1.0.6/chinoscriba/models/block.py`

 * *Files identical despite different names*

### Comparing `chinoscriba-1.0.5/chinoscriba/models/event.py` & `chinoscriba-1.0.6/chinoscriba/models/event.py`

 * *Files identical despite different names*

### Comparing `chinoscriba-1.0.5/chinoscriba/models/inline_response200.py` & `chinoscriba-1.0.6/chinoscriba/models/inline_response200.py`

 * *Files identical despite different names*

### Comparing `chinoscriba-1.0.5/chinoscriba/models/inline_response2001.py` & `chinoscriba-1.0.6/chinoscriba/models/inline_response2001.py`

 * *Files identical despite different names*

### Comparing `chinoscriba-1.0.5/chinoscriba/models/inline_response2002.py` & `chinoscriba-1.0.6/chinoscriba/models/inline_response2002.py`

 * *Files identical despite different names*

### Comparing `chinoscriba-1.0.5/chinoscriba/models/inline_response200_bis.py` & `chinoscriba-1.0.6/chinoscriba/models/inline_response200_bis.py`

 * *Files identical despite different names*

### Comparing `chinoscriba-1.0.5/chinoscriba/models/log.py` & `chinoscriba-1.0.6/chinoscriba/models/log.py`

 * *Files identical despite different names*

### Comparing `chinoscriba-1.0.5/chinoscriba/models/multi_audit_log_serializer_output.py` & `chinoscriba-1.0.6/chinoscriba/models/multi_audit_log_serializer_output.py`

 * *Files identical despite different names*

### Comparing `chinoscriba-1.0.5/chinoscriba/models/search_request.py` & `chinoscriba-1.0.6/chinoscriba/models/search_request.py`

 * *Files identical despite different names*

### Comparing `chinoscriba-1.0.5/chinoscriba/models/sort_rule.py` & `chinoscriba-1.0.6/chinoscriba/models/sort_rule.py`

 * *Files identical despite different names*

### Comparing `chinoscriba-1.0.5/chinoscriba/models/stat.py` & `chinoscriba-1.0.6/chinoscriba/models/stat.py`

 * *Files identical despite different names*

### Comparing `chinoscriba-1.0.5/chinoscriba/rest.py` & `chinoscriba-1.0.6/chinoscriba/rest.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from __future__ import absolute_import
 
 import io
 import json
 import logging
 import re
 import ssl
+import warnings
 
 import certifi
 # python 2 and python 3 compatibility library
 import six
 from six.moves.urllib.parse import urlencode
 
 try:
@@ -223,16 +224,20 @@
             try:
                 # In the python 3, the response.data is bytes.
                 # we need to decode it to string.
                 if six.PY3:
                     r.data = r.data.decode('utf8')
             except UnicodeDecodeError:
                 content_type = r.getheader("Content-Type", None)
-                if 'application/zip' in content_type:
-                    pass  # allow zip content to be passed as bytes
+                if 'application/zip' in content_type.lower():
+                    # Warn about incorrect call params
+                    msg = "This endpoint returned a ZIP archive. You may need "
+                    msg += "to call this method with '_preload_content=False' "
+                    msg += "to read the file bytes."
+                    warnings.warn(msg)
                 else:
                     raise
 
             # log response body
             logger.debug("response body: %s", r.data)
 
         if not 200 <= r.status <= 299:
```

### Comparing `chinoscriba-1.0.5/chinoscriba.egg-info/PKG-INFO` & `chinoscriba-1.0.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chinoscriba
-Version: 1.0.5
+Version: 1.0.6
 Summary: Chino.io Scriba SDK Python
 Home-page: https://www.chino.io
 Author-email: 
 License: UNKNOWN
 Keywords: Chino.io Scriba API
 Platform: UNKNOWN
 Classifier: Topic :: Software Development
@@ -39,77 +39,87 @@
 from pprint import pprint
 
 # Configure HTTP basic authorization: Basic
 configuration = chinoscriba.Configuration()
 configuration.username = 'customer_id'
 configuration.password = 'customer_key'
 
-# create an instance of the API class
-api_instance = chinoscriba.DefaultApi(chinoscriba.ApiClient(configuration))
+# create an instance of the API classes
+logs_api = chinoscriba.LogsApi(chinoscriba.ApiClient(configuration))
+stats_api = chinoscriba.StatsApi(chinoscriba.ApiClient(configuration))
+blocks_api = chinoscriba.BlocksApi(chinoscriba.ApiClient(configuration))
+
 limit = 56 # int | Number of results to return per page
 offset = 0 # int | The initial index from which to return the results
 
 
 # # Audit logs # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # 
 
 # Create a new Log
 body = chinoscriba.AuditLog() # AuditLog | 
 try:
-    api_response = api_instance.logs_create(body)
+    api_response = logs_api.logs_create(body)
     pprint(api_response)
 except ApiException as e:
     print("Exception when calling DefaultApi->logs_create: %s\n" % e)
 
 
 # Create multiple Logs (bulk)
 body = [chinoscriba.AuditLog()] # list[AuditLog] | 
 try:
-    api_response = api_instance.logs_multiple(body)
+    api_response = logs_api.logs_multiple(body)
     pprint(api_response)
 except ApiException as e:
     print("Exception when calling DefaultApi->logs_multiple: %s\n" % e)
 
 try:
     # List all Logs
-    api_response = api_instance.logs_list(limit=limit, offset=offset)
+    api_response = logs_api.logs_list(limit=limit, offset=offset)
     pprint(api_response)
 except ApiException as e:
     print("Exception when calling DefaultApi->logs_list: %s\n" % e)
 
 try:
     # Search by query
-    api_response = api_instance.logs_search(body, limit=limit, offset=offset)
+    api_response = logs_api.logs_search(body, limit=limit, offset=offset)
     pprint(api_response)
 except ApiException as e:
     print("Exception when calling DefaultApi->logs_search: %s\n" % e)
 
+# # Stats # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # 
+    
 try:
     # Retrieve customer statistics
-    api_response = api_instance.stats_read()
+    api_response = stats_api.stats_read()
     pprint(api_response)
 except ApiException as e:
     print("Exception when calling DefaultApi->stats_read: %s\n" % e)
 
 
 # # Exporter # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # 
 
 try:
     # List exportable Blocks
-    api_response = api_instance.exported_list(limit=limit, offset=offset)
+    api_response = blocks_api.exported_list(limit=limit, offset=offset)
     pprint(api_response)
 except ApiException as e:
     print("Exception when calling DefaultApi->exported_list: %s\n" % e)
 
 
 # Export a Block
 block_id = "" # string | ID of the Block to download
 try:
-    api_instance.exported_read(block_id)
+    # NOTE: due to an issue in a third-party library, this only works with 
+    #  '_preload_content' disabled. This will bypass the malfunctioning code
+    #  and return directly the HTTPResponse, which contains the zip file bytes
+    #  in the 'data' attribute.
+    res = blocks_api.exported_read(block_id, _preload_content=False)
+    zip_bytes = res.data  # You can read this using python library 'zipfile'.
 except ApiException as e:
-    print("Exception when calling DefaultApi->exported_read: %s\n" % e)
+    print("Exception when calling BlocksApi->exported_read: %s\n" % e)
 
 ```
 
 ## Changelog
 
 ### [next] - unreleased
 - fixed events' tests
```

### Comparing `chinoscriba-1.0.5/chinoscriba.egg-info/SOURCES.txt` & `chinoscriba-1.0.6/chinoscriba.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chinoscriba-1.0.5/setup.py` & `chinoscriba-1.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 
 here = path.abspath(path.dirname(__file__))
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 NAME = "chinoscriba"
-VERSION = "1.0.5"
+VERSION = "1.0.6"
 
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `chinoscriba-1.0.5/test/test_default_api.py` & `chinoscriba-1.0.6/test/test_default_api.py`

 * *Files identical despite different names*

### Comparing `chinoscriba-1.0.5/test/utils.py` & `chinoscriba-1.0.6/test/utils.py`

 * *Files identical despite different names*

