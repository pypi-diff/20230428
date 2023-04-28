# Comparing `tmp/edx-enterprise-subsidy-client-0.2.6.tar.gz` & `tmp/edx-enterprise-subsidy-client-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-enterprise-subsidy-client-0.2.6.tar", last modified: Thu Apr 27 16:48:13 2023, max compression
+gzip compressed data, was "edx-enterprise-subsidy-client-0.3.0.tar", last modified: Fri Apr 28 18:46:58 2023, max compression
```

## Comparing `edx-enterprise-subsidy-client-0.2.6.tar` & `edx-enterprise-subsidy-client-0.3.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:48:13.586901 edx-enterprise-subsidy-client-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (122)     1341 2023-04-27 16:48:06.000000 edx-enterprise-subsidy-client-0.2.6/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    34523 2023-04-27 16:48:06.000000 edx-enterprise-subsidy-client-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-04-27 16:48:06.000000 edx-enterprise-subsidy-client-0.2.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      224 2023-04-27 16:48:06.000000 edx-enterprise-subsidy-client-0.2.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     8365 2023-04-27 16:48:13.586901 edx-enterprise-subsidy-client-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6341 2023-04-27 16:48:06.000000 edx-enterprise-subsidy-client-0.2.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:48:13.582901 edx-enterprise-subsidy-client-0.2.6/edx_enterprise_subsidy_client/
--rw-r--r--   0 runner    (1001) docker     (122)      140 2023-04-27 16:48:06.000000 edx-enterprise-subsidy-client-0.2.6/edx_enterprise_subsidy_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6785 2023-04-27 16:48:06.000000 edx-enterprise-subsidy-client-0.2.6/edx_enterprise_subsidy_client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:48:13.586901 edx-enterprise-subsidy-client-0.2.6/edx_enterprise_subsidy_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     8365 2023-04-27 16:48:13.000000 edx-enterprise-subsidy-client-0.2.6/edx_enterprise_subsidy_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      544 2023-04-27 16:48:13.000000 edx-enterprise-subsidy-client-0.2.6/edx_enterprise_subsidy_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-27 16:48:13.000000 edx-enterprise-subsidy-client-0.2.6/edx_enterprise_subsidy_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-27 16:48:13.000000 edx-enterprise-subsidy-client-0.2.6/edx_enterprise_subsidy_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-04-27 16:48:13.000000 edx-enterprise-subsidy-client-0.2.6/edx_enterprise_subsidy_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-04-27 16:48:13.000000 edx-enterprise-subsidy-client-0.2.6/edx_enterprise_subsidy_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:48:13.586901 edx-enterprise-subsidy-client-0.2.6/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)       86 2023-04-27 16:48:06.000000 edx-enterprise-subsidy-client-0.2.6/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      561 2023-04-27 16:48:06.000000 edx-enterprise-subsidy-client-0.2.6/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      208 2023-04-27 16:48:13.586901 edx-enterprise-subsidy-client-0.2.6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     5111 2023-04-27 16:48:06.000000 edx-enterprise-subsidy-client-0.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-27 16:48:13.586901 edx-enterprise-subsidy-client-0.2.6/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     1257 2023-04-27 16:48:06.000000 edx-enterprise-subsidy-client-0.2.6/tests/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 18:46:58.758784 edx-enterprise-subsidy-client-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1410 2023-04-28 18:46:53.000000 edx-enterprise-subsidy-client-0.3.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    34523 2023-04-28 18:46:53.000000 edx-enterprise-subsidy-client-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-04-28 18:46:53.000000 edx-enterprise-subsidy-client-0.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      224 2023-04-28 18:46:53.000000 edx-enterprise-subsidy-client-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     8434 2023-04-28 18:46:58.758784 edx-enterprise-subsidy-client-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6341 2023-04-28 18:46:53.000000 edx-enterprise-subsidy-client-0.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 18:46:58.754784 edx-enterprise-subsidy-client-0.3.0/edx_enterprise_subsidy_client/
+-rw-r--r--   0 runner    (1001) docker     (122)      140 2023-04-28 18:46:53.000000 edx-enterprise-subsidy-client-0.3.0/edx_enterprise_subsidy_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9715 2023-04-28 18:46:53.000000 edx-enterprise-subsidy-client-0.3.0/edx_enterprise_subsidy_client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 18:46:58.758784 edx-enterprise-subsidy-client-0.3.0/edx_enterprise_subsidy_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     8434 2023-04-28 18:46:58.000000 edx-enterprise-subsidy-client-0.3.0/edx_enterprise_subsidy_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      544 2023-04-28 18:46:58.000000 edx-enterprise-subsidy-client-0.3.0/edx_enterprise_subsidy_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-28 18:46:58.000000 edx-enterprise-subsidy-client-0.3.0/edx_enterprise_subsidy_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-28 18:46:58.000000 edx-enterprise-subsidy-client-0.3.0/edx_enterprise_subsidy_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-04-28 18:46:58.000000 edx-enterprise-subsidy-client-0.3.0/edx_enterprise_subsidy_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-04-28 18:46:58.000000 edx-enterprise-subsidy-client-0.3.0/edx_enterprise_subsidy_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 18:46:58.758784 edx-enterprise-subsidy-client-0.3.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)       86 2023-04-28 18:46:53.000000 edx-enterprise-subsidy-client-0.3.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-04-28 18:46:53.000000 edx-enterprise-subsidy-client-0.3.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      208 2023-04-28 18:46:58.758784 edx-enterprise-subsidy-client-0.3.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5111 2023-04-28 18:46:53.000000 edx-enterprise-subsidy-client-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 18:46:58.758784 edx-enterprise-subsidy-client-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     1257 2023-04-28 18:46:53.000000 edx-enterprise-subsidy-client-0.3.0/tests/test_client.py
```

### Comparing `edx-enterprise-subsidy-client-0.2.6/CHANGELOG.rst` & `edx-enterprise-subsidy-client-0.3.0/CHANGELOG.rst`

 * *Files 7% similar despite different names*

```diff
@@ -13,14 +13,18 @@
 
 Unreleased
 **********
 
 * Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
   deprecated
 
+[0.3.0]
+*******
+* feat: add new client for v2 transaction endpoint.
+
 [0.2.6]
 *******
 * feat: transaction endpoint accepts `lms_user_id` instead of `learner_id`
 
 [0.2.5]
 *******
 * feat: redemption metadata.
```

### Comparing `edx-enterprise-subsidy-client-0.2.6/LICENSE` & `edx-enterprise-subsidy-client-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edx-enterprise-subsidy-client-0.2.6/LICENSE.txt` & `edx-enterprise-subsidy-client-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-subsidy-client-0.2.6/PKG-INFO` & `edx-enterprise-subsidy-client-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-enterprise-subsidy-client
-Version: 0.2.6
+Version: 0.3.0
 Summary: Client for interacting with the enterprise-subsidy service.
 Home-page: https://github.com/openedx/edx-enterprise-subsidy-client
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -223,14 +223,18 @@
 
 Unreleased
 **********
 
 * Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
   deprecated
 
+[0.3.0]
+*******
+* feat: add new client for v2 transaction endpoint.
+
 [0.2.6]
 *******
 * feat: transaction endpoint accepts `lms_user_id` instead of `learner_id`
 
 [0.2.5]
 *******
 * feat: redemption metadata.
```

### Comparing `edx-enterprise-subsidy-client-0.2.6/README.rst` & `edx-enterprise-subsidy-client-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `edx-enterprise-subsidy-client-0.2.6/edx_enterprise_subsidy_client/client.py` & `edx-enterprise-subsidy-client-0.3.0/edx_enterprise_subsidy_client/client.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,28 +6,48 @@
 import requests
 from django.conf import settings
 from edx_rest_api_client.client import OAuthAPIClient
 
 logger = logging.getLogger(__name__)
 
 
+class EnterpriseSubsidyAPIClientException(Exception):
+    """
+    A general exception to represent non-http errors
+    arising during Subsidy API client usage.
+    """
+
+
+def get_enterprise_subsidy_api_client(version=1):
+    """
+    Helper to get a versioned client.
+    """
+    assert version in [1, 2]
+    if version == 1:
+        return EnterpriseSubsidyAPIClient()
+    if version == 2:
+        return EnterpriseSubsidyAPIClientV2()
+    raise EnterpriseSubsidyAPIClientException(f'{version} is not a valid version!')
+
+
 class EnterpriseSubsidyAPIClient:
     """
     API client for calls to the enterprise-subsidy service.
 
     To use this within your service, ensure the service's settings contain the following vars:
     OAUTH2_PROVIDER_URL=backend-service-oauth-provider-url
     BACKEND_SERVICE_EDX_OAUTH2_KEY=your-services-application-key
     BACKEND_SERVICE_EDX_OAUTH2_SECRET=your-services-application-secret
     ENTERPRISE_SUBSIDY_URL=enterprise-subsidy-service-base-url
     """
-    API_BASE_URL = settings.ENTERPRISE_SUBSIDY_URL.strip('/') + '/api/v1/'
-    SUBSIDIES_ENDPOINT = API_BASE_URL + 'subsidies/'
-    TRANSACTIONS_ENDPOINT = API_BASE_URL + 'transactions/'
-    CONTENT_METADATA_ENDPOINT = API_BASE_URL + 'content-metadata/'
+    API_BASE_URL = settings.ENTERPRISE_SUBSIDY_URL.strip('/') + '/api/'
+    V1_BASE_URL = API_BASE_URL + 'v1/'
+    SUBSIDIES_ENDPOINT = V1_BASE_URL + 'subsidies/'
+    TRANSACTIONS_ENDPOINT = V1_BASE_URL + 'transactions/'
+    CONTENT_METADATA_ENDPOINT = V1_BASE_URL + 'content-metadata/'
 
     def __init__(self):
         """
         Initializes the OAuthAPIClient instance.
         """
         self.client = OAuthAPIClient(
             settings.OAUTH2_PROVIDER_URL,
@@ -185,7 +205,65 @@
         }
         response = self.client.get(
             self.SUBSIDIES_ENDPOINT + f'{subsidy_uuid}/can_redeem/',
             params=query_params,
         )
         response.raise_for_status()
         return response.json()
+
+
+class EnterpriseSubsidyAPIClientV2(EnterpriseSubsidyAPIClient):  # pylint: disable=abstract-method
+    """
+    API client for calls to the enterprise-subsidy service.  Supports v2 transaction
+    admin list and create actions.
+
+    To use this within your service, ensure the service's settings contain the following vars:
+    OAUTH2_PROVIDER_URL=backend-service-oauth-provider-url
+    BACKEND_SERVICE_EDX_OAUTH2_KEY=your-services-application-key
+    BACKEND_SERVICE_EDX_OAUTH2_SECRET=your-services-application-secret
+    ENTERPRISE_SUBSIDY_URL=enterprise-subsidy-service-base-url
+    """
+    V2_BASE_URL = EnterpriseSubsidyAPIClient.API_BASE_URL + 'v2/'
+    TRANSACTIONS_LIST_ENDPOINT = V2_BASE_URL + 'subsidies/{subsidy_uuid}/transactions/'
+
+    def list_subsidy_transactions(
+        self, subsidy_uuid, include_aggregates=True,
+        lms_user_id=None, content_key=None,
+        subsidy_access_policy_uuid=None,
+    ):
+        """
+        List transactions in a subsidy with admin- or operator-level permissions.
+        """
+        query_params = {}
+        if include_aggregates:
+            query_params['include_aggregates'] = include_aggregates
+        if lms_user_id:
+            query_params['lms_user_id'] = lms_user_id
+        if content_key:
+            query_params['content_key'] = content_key
+        if subsidy_access_policy_uuid:
+            query_params['subsidy_access_policy_uuid'] = str(subsidy_access_policy_uuid)
+
+        response = self.client.get(
+            self.TRANSACTIONS_LIST_ENDPOINT.format(subsidy_uuid),
+            params=query_params,
+        )
+        response.raise_for_status()
+        return response.json()
+
+    def create_subsidy_transaction(self, subsidy_uuid, lms_user_id, content_key, subsidy_access_policy_uuid, metadata):
+        """
+        Creates a transaction in the given subsidy, requires operator-level permissions.
+        """
+        request_payload = {
+            'subsidy_uuid': str(subsidy_uuid),
+            'lms_user_id': lms_user_id,
+            'content_key': content_key,
+            'subsidy_access_policy_uuid': str(subsidy_access_policy_uuid),
+            'metadata': metadata,
+        }
+        response = self.client.post(
+            self.TRANSACTIONS_LIST_ENDPOINT.format(subsidy_uuid),
+            json=request_payload,
+        )
+        response.raise_for_status()
+        return response.json()
```

### Comparing `edx-enterprise-subsidy-client-0.2.6/edx_enterprise_subsidy_client.egg-info/PKG-INFO` & `edx-enterprise-subsidy-client-0.3.0/edx_enterprise_subsidy_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-enterprise-subsidy-client
-Version: 0.2.6
+Version: 0.3.0
 Summary: Client for interacting with the enterprise-subsidy service.
 Home-page: https://github.com/openedx/edx-enterprise-subsidy-client
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -223,14 +223,18 @@
 
 Unreleased
 **********
 
 * Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
   deprecated
 
+[0.3.0]
+*******
+* feat: add new client for v2 transaction endpoint.
+
 [0.2.6]
 *******
 * feat: transaction endpoint accepts `lms_user_id` instead of `learner_id`
 
 [0.2.5]
 *******
 * feat: redemption metadata.
```

### Comparing `edx-enterprise-subsidy-client-0.2.6/edx_enterprise_subsidy_client.egg-info/SOURCES.txt` & `edx-enterprise-subsidy-client-0.3.0/edx_enterprise_subsidy_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-subsidy-client-0.2.6/requirements/constraints.txt` & `edx-enterprise-subsidy-client-0.3.0/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `edx-enterprise-subsidy-client-0.2.6/setup.py` & `edx-enterprise-subsidy-client-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `edx-enterprise-subsidy-client-0.2.6/tests/test_client.py` & `edx-enterprise-subsidy-client-0.3.0/tests/test_client.py`

 * *Files identical despite different names*

