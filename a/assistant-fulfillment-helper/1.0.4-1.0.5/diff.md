# Comparing `tmp/assistant-fulfillment-helper-1.0.4.tar.gz` & `tmp/assistant-fulfillment-helper-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assistant-fulfillment-helper-1.0.4.tar", last modified: Thu Dec 29 16:29:13 2022, max compression
+gzip compressed data, was "assistant-fulfillment-helper-1.0.5.tar", last modified: Fri Apr 28 19:22:46 2023, max compression
```

## Comparing `assistant-fulfillment-helper-1.0.4.tar` & `assistant-fulfillment-helper-1.0.5.tar`

### file list

```diff
@@ -1,38 +1,41 @@
-drwxrwxr-x   0 alisson   (1000) alisson   (1000)        0 2022-12-29 16:29:13.654264 assistant-fulfillment-helper-1.0.4/
--rw-rw-r--   0 alisson   (1000) alisson   (1000)     1101 2022-12-26 15:25:59.000000 assistant-fulfillment-helper-1.0.4/LICENSE
--rw-rw-r--   0 alisson   (1000) alisson   (1000)     9487 2022-12-29 16:29:13.654264 assistant-fulfillment-helper-1.0.4/PKG-INFO
--rw-rw-r--   0 alisson   (1000) alisson   (1000)     7797 2022-12-27 17:32:05.000000 assistant-fulfillment-helper-1.0.4/README.md
-drwxrwxr-x   0 alisson   (1000) alisson   (1000)        0 2022-12-29 16:29:13.650264 assistant-fulfillment-helper-1.0.4/assistant_fulfillment_helper/
--rw-rw-r--   0 alisson   (1000) alisson   (1000)      130 2022-12-27 15:22:03.000000 assistant-fulfillment-helper-1.0.4/assistant_fulfillment_helper/__init__.py
-drwxrwxr-x   0 alisson   (1000) alisson   (1000)        0 2022-12-29 16:29:13.650264 assistant-fulfillment-helper-1.0.4/assistant_fulfillment_helper/app/
--rw-rw-r--   0 alisson   (1000) alisson   (1000)      300 2022-12-23 19:55:50.000000 assistant-fulfillment-helper-1.0.4/assistant_fulfillment_helper/app/__init__.py
--rw-rw-r--   0 alisson   (1000) alisson   (1000)      443 2022-12-27 16:55:40.000000 assistant-fulfillment-helper-1.0.4/assistant_fulfillment_helper/app/auth_helper.py
-drwxrwxr-x   0 alisson   (1000) alisson   (1000)        0 2022-12-29 16:29:13.654264 assistant-fulfillment-helper-1.0.4/assistant_fulfillment_helper/app/controllers/
--rw-rw-r--   0 alisson   (1000) alisson   (1000)     2497 2022-12-29 14:59:40.000000 assistant-fulfillment-helper-1.0.4/assistant_fulfillment_helper/app/controllers/fulfillment_intent.py
--rw-rw-r--   0 alisson   (1000) alisson   (1000)      239 2022-12-23 21:12:45.000000 assistant-fulfillment-helper-1.0.4/assistant_fulfillment_helper/app/controllers/fulfillment_server.py
-drwxrwxr-x   0 alisson   (1000) alisson   (1000)        0 2022-12-29 16:29:13.654264 assistant-fulfillment-helper-1.0.4/assistant_fulfillment_helper/app/exceptions/
--rw-rw-r--   0 alisson   (1000) alisson   (1000)      376 2022-12-23 18:55:46.000000 assistant-fulfillment-helper-1.0.4/assistant_fulfillment_helper/app/exceptions/duplicated_intent_node_exception.py
--rw-rw-r--   0 alisson   (1000) alisson   (1000)      443 2022-12-27 14:25:44.000000 assistant-fulfillment-helper-1.0.4/assistant_fulfillment_helper/app/exceptions/intent_callback_not_found_exception.py
--rw-rw-r--   0 alisson   (1000) alisson   (1000)      412 2022-12-23 18:49:59.000000 assistant-fulfillment-helper-1.0.4/assistant_fulfillment_helper/app/exceptions/intent_empty_params_exception.py
--rw-rw-r--   0 alisson   (1000) alisson   (1000)      399 2022-12-23 19:34:07.000000 assistant-fulfillment-helper-1.0.4/assistant_fulfillment_helper/app/exceptions/intent_invalid_callback_exception.py
--rw-rw-r--   0 alisson   (1000) alisson   (1000)      410 2022-12-23 18:50:07.000000 assistant-fulfillment-helper-1.0.4/assistant_fulfillment_helper/app/exceptions/intent_missing_params_exception.py
--rw-rw-r--   0 alisson   (1000) alisson   (1000)      421 2022-12-23 22:00:25.000000 assistant-fulfillment-helper-1.0.4/assistant_fulfillment_helper/app/exceptions/intent_response_instance_exception.py
--rw-rw-r--   0 alisson   (1000) alisson   (1000)      428 2022-12-27 14:28:24.000000 assistant-fulfillment-helper-1.0.4/assistant_fulfillment_helper/app/exceptions/invalid_webhook_token_exception.py
-drwxrwxr-x   0 alisson   (1000) alisson   (1000)        0 2022-12-29 16:29:13.654264 assistant-fulfillment-helper-1.0.4/assistant_fulfillment_helper/app/responses/
--rw-rw-r--   0 alisson   (1000) alisson   (1000)      327 2022-12-26 20:20:24.000000 assistant-fulfillment-helper-1.0.4/assistant_fulfillment_helper/app/responses/fulfillment_helper_response.py
--rw-rw-r--   0 alisson   (1000) alisson   (1000)     5734 2022-12-28 22:04:44.000000 assistant-fulfillment-helper-1.0.4/assistant_fulfillment_helper/app/routes.py
--rw-rw-r--   0 alisson   (1000) alisson   (1000)      745 2022-12-23 22:58:15.000000 assistant-fulfillment-helper-1.0.4/assistant_fulfillment_helper/fulfillment_helper.py
--rw-rw-r--   0 alisson   (1000) alisson   (1000)      129 2022-12-23 21:11:10.000000 assistant-fulfillment-helper-1.0.4/assistant_fulfillment_helper/server.py
-drwxrwxr-x   0 alisson   (1000) alisson   (1000)        0 2022-12-29 16:29:13.650264 assistant-fulfillment-helper-1.0.4/assistant_fulfillment_helper.egg-info/
--rw-rw-r--   0 alisson   (1000) alisson   (1000)     9487 2022-12-29 16:29:13.000000 assistant-fulfillment-helper-1.0.4/assistant_fulfillment_helper.egg-info/PKG-INFO
--rw-rw-r--   0 alisson   (1000) alisson   (1000)     1455 2022-12-29 16:29:13.000000 assistant-fulfillment-helper-1.0.4/assistant_fulfillment_helper.egg-info/SOURCES.txt
--rw-rw-r--   0 alisson   (1000) alisson   (1000)        1 2022-12-29 16:29:13.000000 assistant-fulfillment-helper-1.0.4/assistant_fulfillment_helper.egg-info/dependency_links.txt
--rw-rw-r--   0 alisson   (1000) alisson   (1000)      353 2022-12-29 16:29:13.000000 assistant-fulfillment-helper-1.0.4/assistant_fulfillment_helper.egg-info/requires.txt
--rw-rw-r--   0 alisson   (1000) alisson   (1000)       29 2022-12-29 16:29:13.000000 assistant-fulfillment-helper-1.0.4/assistant_fulfillment_helper.egg-info/top_level.txt
--rw-rw-r--   0 alisson   (1000) alisson   (1000)       38 2022-12-29 16:29:13.654264 assistant-fulfillment-helper-1.0.4/setup.cfg
--rw-rw-r--   0 alisson   (1000) alisson   (1000)     1392 2022-12-29 16:29:10.000000 assistant-fulfillment-helper-1.0.4/setup.py
-drwxrwxr-x   0 alisson   (1000) alisson   (1000)        0 2022-12-29 16:29:13.654264 assistant-fulfillment-helper-1.0.4/test/
--rw-rw-r--   0 alisson   (1000) alisson   (1000)     1421 2022-12-29 15:25:02.000000 assistant-fulfillment-helper-1.0.4/test/test_fulfillment_helper.py
--rw-rw-r--   0 alisson   (1000) alisson   (1000)     1430 2022-12-29 16:11:06.000000 assistant-fulfillment-helper-1.0.4/test/test_fulfillment_helper_response.py
--rw-rw-r--   0 alisson   (1000) alisson   (1000)     6308 2022-12-29 15:14:17.000000 assistant-fulfillment-helper-1.0.4/test/test_fulfillment_intent.py
--rw-rw-r--   0 alisson   (1000) alisson   (1000)     4432 2022-12-28 22:18:52.000000 assistant-fulfillment-helper-1.0.4/test/test_webhook_request.py
+drwxrwxr-x   0 alisson   (1000) alisson   (1000)        0 2023-04-28 19:22:46.858353 assistant-fulfillment-helper-1.0.5/
+-rw-rw-r--   0 alisson   (1000) alisson   (1000)     1101 2023-04-19 19:03:45.000000 assistant-fulfillment-helper-1.0.5/LICENSE
+-rw-rw-r--   0 alisson   (1000) alisson   (1000)    12826 2023-04-28 19:22:46.858353 assistant-fulfillment-helper-1.0.5/PKG-INFO
+-rw-rw-r--   0 alisson   (1000) alisson   (1000)    10584 2023-04-28 18:57:58.000000 assistant-fulfillment-helper-1.0.5/README.md
+drwxrwxr-x   0 alisson   (1000) alisson   (1000)        0 2023-04-28 19:22:46.854354 assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper/
+-rw-rw-r--   0 alisson   (1000) alisson   (1000)      186 2023-04-27 13:22:02.000000 assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper/__init__.py
+drwxrwxr-x   0 alisson   (1000) alisson   (1000)        0 2023-04-28 19:22:46.854354 assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper/app/
+drwxrwxr-x   0 alisson   (1000) alisson   (1000)        0 2023-04-28 19:22:46.854354 assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper/app/controllers/
+-rw-rw-r--   0 alisson   (1000) alisson   (1000)     1097 2023-04-27 19:23:01.000000 assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper/app/controllers/auth_controller.py
+-rw-rw-r--   0 alisson   (1000) alisson   (1000)     4725 2023-04-28 18:04:35.000000 assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper/app/controllers/webhook_controller.py
+drwxrwxr-x   0 alisson   (1000) alisson   (1000)        0 2023-04-28 19:22:46.854354 assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper/app/data/
+-rw-rw-r--   0 alisson   (1000) alisson   (1000)      815 2023-04-27 19:34:51.000000 assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper/app/data/token_data.py
+-rw-rw-r--   0 alisson   (1000) alisson   (1000)     2930 2023-04-27 19:55:12.000000 assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper/app/data/webhook_data.py
+drwxrwxr-x   0 alisson   (1000) alisson   (1000)        0 2023-04-28 19:22:46.854354 assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper/app/exceptions/
+-rw-rw-r--   0 alisson   (1000) alisson   (1000)      376 2023-04-26 22:02:12.000000 assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper/app/exceptions/__init__.py
+-rw-rw-r--   0 alisson   (1000) alisson   (1000)      392 2023-04-26 21:14:54.000000 assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper/app/exceptions/duplicated_intent_node_exception.py
+-rw-rw-r--   0 alisson   (1000) alisson   (1000)      443 2023-04-26 21:41:14.000000 assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper/app/exceptions/intent_callback_not_found_exception.py
+-rw-rw-r--   0 alisson   (1000) alisson   (1000)      421 2023-04-26 21:48:21.000000 assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper/app/exceptions/intent_response_instance_exception.py
+-rw-rw-r--   0 alisson   (1000) alisson   (1000)      428 2023-04-26 21:41:29.000000 assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper/app/exceptions/invalid_webhook_token_exception.py
+-rw-rw-r--   0 alisson   (1000) alisson   (1000)      379 2023-04-26 20:40:51.000000 assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper/app/exceptions/webhook_not_found_exception.py
+drwxrwxr-x   0 alisson   (1000) alisson   (1000)        0 2023-04-28 19:22:46.854354 assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper/app/models/
+-rw-rw-r--   0 alisson   (1000) alisson   (1000)      274 2023-04-28 18:03:40.000000 assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper/app/models/intent_model.py
+drwxrwxr-x   0 alisson   (1000) alisson   (1000)        0 2023-04-28 19:22:46.854354 assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper/app/responses/
+-rw-rw-r--   0 alisson   (1000) alisson   (1000)      384 2023-04-27 19:56:30.000000 assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper/app/responses/fulfillment_helper_response.py
+drwxrwxr-x   0 alisson   (1000) alisson   (1000)        0 2023-04-28 19:22:46.858353 assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper/app/server/
+-rw-rw-r--   0 alisson   (1000) alisson   (1000)      187 2023-04-27 17:57:58.000000 assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper/app/server/__init__.py
+-rw-rw-r--   0 alisson   (1000) alisson   (1000)      777 2023-04-27 20:04:17.000000 assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper/app/server/fulfillment_server.py
+-rw-rw-r--   0 alisson   (1000) alisson   (1000)     1052 2023-04-27 20:08:21.000000 assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper/app/server/routes.py
+-rw-rw-r--   0 alisson   (1000) alisson   (1000)     3289 2023-04-28 18:04:06.000000 assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper/fulfillment_helper.py
+drwxrwxr-x   0 alisson   (1000) alisson   (1000)        0 2023-04-28 19:22:46.854354 assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper.egg-info/
+-rw-rw-r--   0 alisson   (1000) alisson   (1000)    12826 2023-04-28 19:22:46.000000 assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper.egg-info/PKG-INFO
+-rw-rw-r--   0 alisson   (1000) alisson   (1000)     1465 2023-04-28 19:22:46.000000 assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper.egg-info/SOURCES.txt
+-rw-rw-r--   0 alisson   (1000) alisson   (1000)        1 2023-04-28 19:22:46.000000 assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper.egg-info/dependency_links.txt
+-rw-rw-r--   0 alisson   (1000) alisson   (1000)      353 2023-04-28 19:22:46.000000 assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper.egg-info/requires.txt
+-rw-rw-r--   0 alisson   (1000) alisson   (1000)       29 2023-04-28 19:22:46.000000 assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper.egg-info/top_level.txt
+-rw-rw-r--   0 alisson   (1000) alisson   (1000)       38 2023-04-28 19:22:46.858353 assistant-fulfillment-helper-1.0.5/setup.cfg
+-rw-rw-r--   0 alisson   (1000) alisson   (1000)     1543 2023-04-28 19:21:30.000000 assistant-fulfillment-helper-1.0.5/setup.py
+drwxrwxr-x   0 alisson   (1000) alisson   (1000)        0 2023-04-28 19:22:46.858353 assistant-fulfillment-helper-1.0.5/test/
+-rw-rw-r--   0 alisson   (1000) alisson   (1000)     2261 2023-04-27 18:53:31.000000 assistant-fulfillment-helper-1.0.5/test/test_fulfillment_helper.py
+-rw-rw-r--   0 alisson   (1000) alisson   (1000)     1430 2023-04-19 19:03:45.000000 assistant-fulfillment-helper-1.0.5/test/test_fulfillment_helper_response.py
+-rw-rw-r--   0 alisson   (1000) alisson   (1000)    10126 2023-04-28 18:09:38.000000 assistant-fulfillment-helper-1.0.5/test/test_webhook_request.py
```

### Comparing `assistant-fulfillment-helper-1.0.4/LICENSE` & `assistant-fulfillment-helper-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `assistant-fulfillment-helper-1.0.4/assistant_fulfillment_helper/app/controllers/fulfillment_intent.py` & `assistant-fulfillment-helper-1.0.5/test/test_fulfillment_helper.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,59 +1,64 @@
-from assistant_fulfillment_helper.app.exceptions.duplicated_intent_node_exception import DuplicatedIntentNodeException
-from assistant_fulfillment_helper.app.exceptions.intent_empty_params_exception import IntentEmptyParamException
-from assistant_fulfillment_helper.app.exceptions.intent_missing_params_exception import IntentMissingParamException
-from assistant_fulfillment_helper.app.exceptions.intent_invalid_callback_exception import IntentInvalidCallbackException
-from assistant_fulfillment_helper.app.exceptions.intent_callback_not_found_exception import IntentCallbackNotFoundException
-from assistant_fulfillment_helper.app.exceptions.invalid_webhook_token_exception import InvalidWebhookTokenException
-
-class FulfillmentIntent:
-
-    __intents = []
-
-    @staticmethod
-    def __validate_intent(intent_data:dict):
-        """
-            Check if this intent is valid
-        """
-        mandatory_params = [
-            'callback', 
-            'webhook_token',
-            'node_name'
-        ]
-
-        for param in mandatory_params:
-            if param not in intent_data:
-                raise IntentMissingParamException(param)
-            if intent_data[param] == False or intent_data[param] == '':
-                raise IntentEmptyParamException(param)
-            if param == 'callback' and callable(intent_data[param]) == False:
-                raise IntentInvalidCallbackException(intent_data['node_name'])
-        FulfillmentIntent.__intent_node_exists(intent_data)
-
-    @staticmethod
-    def __intent_node_exists(intent_node:dict):
-        """
-            Check if this intent is duplicated
-        """
-        for intent in FulfillmentIntent.__intents:
-            if intent['node_name'] == intent_node['node_name']:
-                raise DuplicatedIntentNodeException(intent['node_name'])
-
-    @staticmethod
-    def define(intent_data:dict):
-        """
-            Define a new intent to the intents list
-        """
-        FulfillmentIntent.__validate_intent(intent_data)
-        FulfillmentIntent.__intents.append(intent_data)
-
-    @staticmethod
-    def get(intent_name:str, webhook_token:str):
-        """
-            Get a intent by name
-        """
-        for intent in FulfillmentIntent.__intents:
-            if intent['node_name'] == intent_name:
-                if intent['webhook_token'] == webhook_token:
-                    return intent
-                raise InvalidWebhookTokenException(intent_name)
-        raise IntentCallbackNotFoundException(intent_name)
+from mock import MagicMock
+from test.mocks import constants
+from assistant_fulfillment_helper.fulfillment_helper import FulfillmentHelper
+from assistant_fulfillment_helper.app.responses.fulfillment_helper_response import FulfillmentHelperResponse
+from assistant_fulfillment_helper.app.server.fulfillment_server import FulfillmentServer
+from assistant_fulfillment_helper.app.data.webhook_data import WebhookData
+from assistant_fulfillment_helper.app.models.intent_model import IntentModel
+
+FulfillmentServer.run = MagicMock()
+
+class TestFulfillmentHelper:
+
+    def test_recovery_intent(self):
+        node_name = 'test_define_new_intent'
+        path_name = 'test_path'
+
+        fh = FulfillmentHelper()
+        @fh.intent(path_name, node=node_name, token=constants.FAKE_TOKEN)
+        def callback_test(args:dict):
+            return FulfillmentHelperResponse(
+                message=constants.FAKE_SUCCESS_MESSAGE
+            )
+    
+        assert WebhookData.load_intent(
+            _webhook = WebhookData.get(path_name),
+            intent_name=node_name,
+            intent_token=constants.FAKE_TOKEN
+        ) == IntentModel(
+            callback = callback_test,
+            webhook_token = constants.FAKE_TOKEN,
+            node_name = node_name
+        )
+
+    def test_recovery_intent_deprecated(self):
+        node_name = 'test_define_new_intent'
+        def callback_test(args:dict):
+            return FulfillmentHelperResponse(
+                message=constants.FAKE_SUCCESS_MESSAGE
+            )
+        
+        fh = FulfillmentHelper()
+        fh.registerIntent(
+            callback=callback_test,
+            webhook_token=constants.FAKE_TOKEN,
+            node_name=node_name
+        )
+    
+        assert WebhookData.load_intent(
+            _webhook = WebhookData.get('fh_default_path'),
+            intent_name=node_name,
+            intent_token=constants.FAKE_TOKEN
+        ) == IntentModel(
+            callback = callback_test,
+            webhook_token = constants.FAKE_TOKEN,
+            node_name = node_name
+        )
+
+    def test_start_server(self):
+        fh = FulfillmentHelper()
+        assert fh.start(
+            debug=True,
+            host="123.456.789.012",
+            port=1000
+        ) == None # None == no errors
```

### Comparing `assistant-fulfillment-helper-1.0.4/assistant_fulfillment_helper.egg-info/SOURCES.txt` & `assistant-fulfillment-helper-1.0.5/assistant_fulfillment_helper.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 LICENSE
 README.md
 setup.py
 assistant_fulfillment_helper/__init__.py
 assistant_fulfillment_helper/fulfillment_helper.py
-assistant_fulfillment_helper/server.py
 assistant_fulfillment_helper.egg-info/PKG-INFO
 assistant_fulfillment_helper.egg-info/SOURCES.txt
 assistant_fulfillment_helper.egg-info/dependency_links.txt
 assistant_fulfillment_helper.egg-info/requires.txt
 assistant_fulfillment_helper.egg-info/top_level.txt
-assistant_fulfillment_helper/app/__init__.py
-assistant_fulfillment_helper/app/auth_helper.py
-assistant_fulfillment_helper/app/routes.py
-assistant_fulfillment_helper/app/controllers/fulfillment_intent.py
-assistant_fulfillment_helper/app/controllers/fulfillment_server.py
+assistant_fulfillment_helper/app/controllers/auth_controller.py
+assistant_fulfillment_helper/app/controllers/webhook_controller.py
+assistant_fulfillment_helper/app/data/token_data.py
+assistant_fulfillment_helper/app/data/webhook_data.py
+assistant_fulfillment_helper/app/exceptions/__init__.py
 assistant_fulfillment_helper/app/exceptions/duplicated_intent_node_exception.py
 assistant_fulfillment_helper/app/exceptions/intent_callback_not_found_exception.py
-assistant_fulfillment_helper/app/exceptions/intent_empty_params_exception.py
-assistant_fulfillment_helper/app/exceptions/intent_invalid_callback_exception.py
-assistant_fulfillment_helper/app/exceptions/intent_missing_params_exception.py
 assistant_fulfillment_helper/app/exceptions/intent_response_instance_exception.py
 assistant_fulfillment_helper/app/exceptions/invalid_webhook_token_exception.py
+assistant_fulfillment_helper/app/exceptions/webhook_not_found_exception.py
+assistant_fulfillment_helper/app/models/intent_model.py
 assistant_fulfillment_helper/app/responses/fulfillment_helper_response.py
+assistant_fulfillment_helper/app/server/__init__.py
+assistant_fulfillment_helper/app/server/fulfillment_server.py
+assistant_fulfillment_helper/app/server/routes.py
 test/test_fulfillment_helper.py
 test/test_fulfillment_helper_response.py
-test/test_fulfillment_intent.py
 test/test_webhook_request.py
```

### Comparing `assistant-fulfillment-helper-1.0.4/setup.py` & `assistant-fulfillment-helper-1.0.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,25 +27,28 @@
     'zope.event==4.6',
     'zope.interface==5.5.2'
 ]
 
 setup(
     name='assistant-fulfillment-helper',
     author="TotvsLabs",
-    version='1.0.4',
+    version='1.0.5',
     author_email='info@totvslabs.com',
     python_requires='>=3.7',
     description="Assistant Fulfillment Helper Server",
     long_description=readme,
     long_description_content_type="text/markdown",
     install_requires=requirements,
     include_package_data=True,
     keywords='assistant fulfillment helper carol totvs carolina carolapp',
     packages=[
         'assistant_fulfillment_helper',
         'assistant_fulfillment_helper.app',
         'assistant_fulfillment_helper.app.controllers',
+        'assistant_fulfillment_helper.app.data',
         'assistant_fulfillment_helper.app.exceptions',
-        'assistant_fulfillment_helper.app.responses'
+        'assistant_fulfillment_helper.app.models',
+        'assistant_fulfillment_helper.app.responses',
+        'assistant_fulfillment_helper.app.server'
     ],
     url='https://github.com/totvslabs/assistant-fulfillment-helper'
 )
```

### Comparing `assistant-fulfillment-helper-1.0.4/test/test_fulfillment_helper_response.py` & `assistant-fulfillment-helper-1.0.5/test/test_fulfillment_helper_response.py`

 * *Files identical despite different names*

