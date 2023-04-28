# Comparing `tmp/YOMAPI-0.1.4.tar.gz` & `tmp/YOMAPI-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/YOMAPI-0.1.4.tar", last modified: Thu Mar 16 12:43:23 2023, max compression
+gzip compressed data, was "dist/YOMAPI-0.1.6.tar", last modified: Fri Apr 28 12:39:49 2023, max compression
```

## Comparing `YOMAPI-0.1.4.tar` & `YOMAPI-0.1.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-16 12:43:23.000000 YOMAPI-0.1.4/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-03-16 12:43:23.000000 YOMAPI-0.1.4/YOMAPI/
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)    38435 2023-03-16 12:43:12.000000 YOMAPI-0.1.4/YOMAPI/YOMAPI.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)       68 2023-03-16 12:43:12.000000 YOMAPI-0.1.4/YOMAPI/__init__.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)       39 2023-03-16 12:43:12.000000 YOMAPI-0.1.4/setup.cfg
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)      922 2023-03-16 12:43:12.000000 YOMAPI-0.1.4/setup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      701 2023-03-16 12:43:23.000000 YOMAPI-0.1.4/PKG-INFO
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-28 12:39:49.000000 YOMAPI-0.1.6/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-28 12:39:49.000000 YOMAPI-0.1.6/YOMAPI/
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)    39250 2023-04-28 12:39:39.000000 YOMAPI-0.1.6/YOMAPI/YOMAPI.py
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)       68 2023-04-28 12:39:39.000000 YOMAPI-0.1.6/YOMAPI/__init__.py
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)       39 2023-04-28 12:39:39.000000 YOMAPI-0.1.6/setup.cfg
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)      922 2023-04-28 12:39:39.000000 YOMAPI-0.1.6/setup.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      701 2023-04-28 12:39:49.000000 YOMAPI-0.1.6/PKG-INFO
```

### Comparing `YOMAPI-0.1.4/YOMAPI/YOMAPI.py` & `YOMAPI-0.1.6/YOMAPI/YOMAPI.py`

 * *Files 2% similar despite different names*

```diff
@@ -513,23 +513,26 @@
     def update_bulk_segments(
         self,
         batch,
         fields_not_to_be_updated,
         token,
         sync_job_id=None,
         from_integration=None,
-        filter_keys=None
+        filter_keys=None,
+        segment_type=None,
     ):
         path = self.url + '/api/v2/segments/bulk'
         session = self.__build_session(token)
         try:
             body = {
                 'data': batch,
-                'fieldsNotToBeUpdated': fields_not_to_be_updated
+                'fieldsNotToBeUpdated': fields_not_to_be_updated,
             }
+            if segment_type:
+                body['type'] = segment_type
             if sync_job_id:
                 body['syncJobId'] = sync_job_id
             if from_integration:
                 body['fromIntegration'] = from_integration
             if filter_keys:
                 body['filterKeys'] = filter_keys
 
@@ -560,24 +563,27 @@
     def update_bulk_user_segments(
         self,
         batch,
         fields_not_to_be_updated,
         token,
         sync_job_id=None,
         from_integration=None,
-        filter_keys=None
+        filter_keys=None,
+        segment_type=None,
     ):
         path = self.url + '/api/v2/segments/user-segments/bulk'
         session = self.__build_session(token)
 
         try:
             body = {
                 'data': batch,
                 'fieldsNotToBeUpdated': fields_not_to_be_updated
             }
+            if segment_type:
+                body['type'] = segment_type
             if sync_job_id:
                 body['syncJobId'] = sync_job_id
             if from_integration:
                 body['fromIntegration'] = from_integration
             if filter_keys:
                 body['filterKeys'] = filter_keys
             response = session.put(path, json.dumps(body))
@@ -601,31 +607,35 @@
             response = session.post(path, json.dumps(body))
             response = json.loads(response.content.decode('utf-8'))
             return response
         except Exception as error:
             raise ApiResponseError(path, str(error))
 
 
-    def bulk_clean_segments(self, job_id, token=None):
+    def bulk_clean_segments(self, job_id, token=None, segment_type=None):
         path = self.url + f'/api/v2/segments/segments/delete-not-by-sync-job/{job_id}'
         self.logger.info('Sending segments delete for job id {}'.format(job_id))
         try:
             session = self.__build_session(token)
+            if segment_type:
+                path += f'?type={segment_type}'
             response = session.delete(path)
             self.logger.info((response.status_code, response.json()))
             return response
         except Exception as error:
             raise ApiResponseError(path, str(error))
 
 
-    def bulk_clean_user_segments(self, job_id, token=None):
+    def bulk_clean_user_segments(self, job_id, token=None, segment_type=None):
         path = self.url + f'/api/v2/segments/user-segments/delete-not-by-sync-job/{job_id}'
         self.logger.info('Sending user segments delete for job id {}'.format(job_id))
         try:
             session = self.__build_session(token)
+            if segment_type:
+                path += f'?type={segment_type}'
             response = session.delete(path)
             self.logger.info((response.status_code, response.json()))
             return response
         except Exception as error:
             raise ApiResponseError(path, str(error))
 
 
@@ -1015,25 +1025,37 @@
             if input_params:
                 if 'parent' in input_params: params['parent'] = input_params['parent']
             response = session.get(path, params=params)
             return (response.status_code, response.json())
         except Exception as error:
             raise ApiResponseError(path, str(error))
 
-    def get_categories(self, token, input_params=None):
+    def get_categories(self, token=None, input_params=None):
         current_page = 0
         total_pages = float('inf')
-        products = []
+        categories = []
         while(current_page < total_pages):
             current_page += 1
             status, response = self.__get_categories_page(page=current_page, limit=100, token=token, input_params=input_params)
-            products += response['docs']
+            categories += response['docs']
             total_pages = response['pages']
             self.logger.info('Sending categories query for page {}/{}'.format(current_page, total_pages))
-        return products
+        return categories
+    
+    def update_bulk_categories(self, batch, token):
+        path = self.url + '/api/v2/categories/bulk'
+        session = self.__build_session(token)
+        try:
+            body = {
+                'data': batch,
+            }
+            response = session.put(path, json.dumps(body))
+            return response
+        except Exception as error:
+            raise ApiResponseError(path, str(error))
 
     """
     Configuration Endpoints
     """
 
     def get_configuration(self, name, token=None):
         path = self.url_v3 + '/api/v3/admin/data-import/integration-config/name'
```

### Comparing `YOMAPI-0.1.4/setup.py` & `YOMAPI-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from distutils.core import setup
 setup(
   name = 'YOMAPI',
   packages = ['YOMAPI'],
-  version = '0.1.4',
+  version = '0.1.6',
   license='MIT',
   description = 'A PACKAGE TO USE THE SAME YOM API INTERFACE FROM YOM INTEGRATIONS',
   author = 'Camilo Jiménez',
   author_email = 'camilo@youorder.me',
   url = 'https://github.com/user/reponame',
   # download_url = 'https://github.com/user/reponame/archive/v_01.tar.gz', 
   keywords = ['YOM-INTEGRATIONS'],   # Keywords that define your package best
```

### Comparing `YOMAPI-0.1.4/PKG-INFO` & `YOMAPI-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: YOMAPI
-Version: 0.1.4
+Version: 0.1.6
 Summary: A PACKAGE TO USE THE SAME YOM API INTERFACE FROM YOM INTEGRATIONS
 Home-page: https://github.com/user/reponame
 Author: Camilo Jiménez
 Author-email: camilo@youorder.me
 License: MIT
 Description: UNKNOWN
 Keywords: YOM-INTEGRATIONS
```

