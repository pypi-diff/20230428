# Comparing `tmp/oauth2-client-1.4.1.tar.gz` & `tmp/oauth2-client-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/oauth2-client-1.4.1.tar", last modified: Thu Apr 27 21:01:42 2023, max compression
+gzip compressed data, was "dist/oauth2-client-1.4.2.tar", last modified: Fri Apr 28 12:55:27 2023, max compression
```

## Comparing `oauth2-client-1.4.1.tar` & `oauth2-client-1.4.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 21:01:42.000000 oauth2-client-1.4.1/
--rw-rw-r--   0 root         (0) root         (0)    11347 2022-12-03 11:03:06.000000 oauth2-client-1.4.1/LICENSE
--rw-rw-r--   0 root         (0) root         (0)       38 2022-12-03 11:03:06.000000 oauth2-client-1.4.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     7870 2023-04-27 21:01:42.000000 oauth2-client-1.4.1/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     7184 2023-02-02 15:04:57.000000 oauth2-client-1.4.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 21:01:42.000000 oauth2-client-1.4.1/main/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 21:01:42.000000 oauth2-client-1.4.1/main/oauth2_client/
--rw-rw-r--   0 root         (0) root         (0)       22 2023-04-27 21:00:33.000000 oauth2-client-1.4.1/main/oauth2_client/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    13047 2023-04-27 21:00:22.000000 oauth2-client-1.4.1/main/oauth2_client/credentials_manager.py
--rw-rw-r--   0 root         (0) root         (0)     2324 2022-12-03 11:03:06.000000 oauth2-client-1.4.1/main/oauth2_client/http_server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 21:01:42.000000 oauth2-client-1.4.1/oauth2_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7870 2023-04-27 21:01:42.000000 oauth2-client-1.4.1/oauth2_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      383 2023-04-27 21:01:42.000000 oauth2-client-1.4.1/oauth2_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 21:01:42.000000 oauth2-client-1.4.1/oauth2_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 21:01:42.000000 oauth2-client-1.4.1/oauth2_client.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       16 2023-04-27 21:01:42.000000 oauth2-client-1.4.1/oauth2_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-04-27 21:01:42.000000 oauth2-client-1.4.1/oauth2_client.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)       15 2022-12-03 11:03:06.000000 oauth2-client-1.4.1/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-27 21:01:42.000000 oauth2-client-1.4.1/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1567 2023-02-02 14:51:28.000000 oauth2-client-1.4.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 12:55:27.000000 oauth2-client-1.4.2/
+-rw-rw-r--   0 root         (0) root         (0)    11347 2022-12-03 11:03:06.000000 oauth2-client-1.4.2/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)       38 2022-12-03 11:03:06.000000 oauth2-client-1.4.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     7870 2023-04-28 12:55:27.000000 oauth2-client-1.4.2/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     7184 2023-02-02 15:04:57.000000 oauth2-client-1.4.2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 12:55:27.000000 oauth2-client-1.4.2/main/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 12:55:27.000000 oauth2-client-1.4.2/main/oauth2_client/
+-rw-rw-r--   0 root         (0) root         (0)       22 2023-04-28 12:53:28.000000 oauth2-client-1.4.2/main/oauth2_client/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    13055 2023-04-28 12:52:05.000000 oauth2-client-1.4.2/main/oauth2_client/credentials_manager.py
+-rw-rw-r--   0 root         (0) root         (0)     2324 2022-12-03 11:03:06.000000 oauth2-client-1.4.2/main/oauth2_client/http_server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 12:55:27.000000 oauth2-client-1.4.2/oauth2_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7870 2023-04-28 12:55:27.000000 oauth2-client-1.4.2/oauth2_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      383 2023-04-28 12:55:27.000000 oauth2-client-1.4.2/oauth2_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 12:55:27.000000 oauth2-client-1.4.2/oauth2_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 12:55:02.000000 oauth2-client-1.4.2/oauth2_client.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       16 2023-04-28 12:55:27.000000 oauth2-client-1.4.2/oauth2_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-04-28 12:55:27.000000 oauth2-client-1.4.2/oauth2_client.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)       15 2022-12-03 11:03:06.000000 oauth2-client-1.4.2/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-28 12:55:27.000000 oauth2-client-1.4.2/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1567 2023-02-02 14:51:28.000000 oauth2-client-1.4.2/setup.py
```

### Comparing `oauth2-client-1.4.1/LICENSE` & `oauth2-client-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `oauth2-client-1.4.1/PKG-INFO` & `oauth2-client-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oauth2-client
-Version: 1.4.1
+Version: 1.4.2
 Summary: A client library for OAuth2
 Home-page: http://github.com/antechrestos/OAuth2Client
 Author: Benjamin Einaudi
 Author-email: antechrestos@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `oauth2-client-1.4.1/README.rst` & `oauth2-client-1.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `oauth2-client-1.4.1/main/oauth2_client/credentials_manager.py` & `oauth2-client-1.4.2/main/oauth2_client/credentials_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,20 +30,25 @@
                  scopes: list,
                  verify: bool = True):
         self.authorize_service = authorize_service
         self.token_service = token_service
         self.client_id = client_id
         self.client_secret = client_secret
         self.scopes = scopes
-        self.auth = (
-            base64.b64encode(bytes('%s:%s' % (self.client_id, self.client_secret), 'UTF-8')).decode('UTF-8')
-            if self.client_secret else None
-        )
         self.verify = verify
 
+    @property
+    def authorization_header(self):
+        return 'Basic %s' % base64.b64encode(bytes('%s:%s' % (self.client_id, self.client_secret), 'UTF-8'))\
+            .decode('UTF-8')
+
+    @property
+    def public_api(self):
+        return self.client_secret is None
+
 
 class AuthorizeResponseCallback(dict):
     def __init__(self, *args, **kwargs):
         super(AuthorizeResponseCallback, self).__init__(*args, **kwargs)
         self.response = Event()
 
     def wait(self, timeout: Optional[float] = None):
@@ -183,19 +188,18 @@
                 _logger.debug('refresh_token - unauthorized - cleaning token')
                 self._session = None
                 self.refresh_token = None
             raise err
 
     def _token_request(self, request_parameters: dict, refresh_token_mandatory: bool):
         headers = self._token_request_headers(request_parameters['grant_type'])
-        if self.service_information.auth:
-            headers['Authorization'] = 'Basic %s' % self.service_information.auth
-        else:
+        if self.service_information.public_api:
             request_parameters["client_id"] = self.service_information.client_id
-            request_parameters["client_secret"] = self.service_information.client_secret
+        else:
+            headers['Authorization'] = self.service_information.authorization_header
         response = requests.post(self.service_information.token_service,
                                  data=request_parameters,
                                  headers=headers,
                                  proxies=self.proxies,
                                  verify=self.service_information.verify)
         if response.status_code != HTTPStatus.OK.value:
             CredentialManager._handle_bad_response(response)
```

### Comparing `oauth2-client-1.4.1/main/oauth2_client/http_server.py` & `oauth2-client-1.4.2/main/oauth2_client/http_server.py`

 * *Files identical despite different names*

### Comparing `oauth2-client-1.4.1/oauth2_client.egg-info/PKG-INFO` & `oauth2-client-1.4.2/oauth2_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oauth2-client
-Version: 1.4.1
+Version: 1.4.2
 Summary: A client library for OAuth2
 Home-page: http://github.com/antechrestos/OAuth2Client
 Author: Benjamin Einaudi
 Author-email: antechrestos@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `oauth2-client-1.4.1/setup.py` & `oauth2-client-1.4.2/setup.py`

 * *Files identical despite different names*

