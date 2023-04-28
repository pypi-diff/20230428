# Comparing `tmp/django-dreiattest-0.0.8.tar.gz` & `tmp/django-dreiattest-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-dreiattest-0.0.8.tar", last modified: Wed Apr 21 16:22:01 2021, max compression
+gzip compressed data, was "django-dreiattest-0.0.9.tar", last modified: Mon Apr 26 14:34:32 2021, max compression
```

## Comparing `django-dreiattest-0.0.8.tar` & `django-dreiattest-0.0.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 samuelbichsel   (501) staff       (20)        0 2021-04-21 16:22:01.297888 django-dreiattest-0.0.8/
--rw-r--r--   0 samuelbichsel   (501) staff       (20)     1064 2021-04-13 15:27:50.000000 django-dreiattest-0.0.8/LICENSE
--rw-r--r--   0 samuelbichsel   (501) staff       (20)       62 2021-04-13 15:27:50.000000 django-dreiattest-0.0.8/MANIFEST.in
--rw-r--r--   0 samuelbichsel   (501) staff       (20)     2167 2021-04-21 16:22:01.297629 django-dreiattest-0.0.8/PKG-INFO
--rw-r--r--   0 samuelbichsel   (501) staff       (20)     1192 2021-04-13 15:27:50.000000 django-dreiattest-0.0.8/README.md
-drwxr-xr-x   0 samuelbichsel   (501) staff       (20)        0 2021-04-21 16:22:01.287590 django-dreiattest-0.0.8/django_dreiattest.egg-info/
--rw-r--r--   0 samuelbichsel   (501) staff       (20)     2167 2021-04-21 16:22:01.000000 django-dreiattest-0.0.8/django_dreiattest.egg-info/PKG-INFO
--rw-r--r--   0 samuelbichsel   (501) staff       (20)      748 2021-04-21 16:22:01.000000 django-dreiattest-0.0.8/django_dreiattest.egg-info/SOURCES.txt
--rw-r--r--   0 samuelbichsel   (501) staff       (20)        1 2021-04-21 16:22:01.000000 django-dreiattest-0.0.8/django_dreiattest.egg-info/dependency_links.txt
--rw-r--r--   0 samuelbichsel   (501) staff       (20)       11 2021-04-21 16:22:01.000000 django-dreiattest-0.0.8/django_dreiattest.egg-info/top_level.txt
-drwxr-xr-x   0 samuelbichsel   (501) staff       (20)        0 2021-04-21 16:22:01.294984 django-dreiattest-0.0.8/dreiattest/
--rw-r--r--   0 samuelbichsel   (501) staff       (20)       56 2021-04-13 15:27:50.000000 django-dreiattest-0.0.8/dreiattest/__init__.py
--rw-r--r--   0 samuelbichsel   (501) staff       (20)       63 2021-04-21 16:19:37.000000 django-dreiattest-0.0.8/dreiattest/__version__.py
--rw-r--r--   0 samuelbichsel   (501) staff       (20)       95 2021-04-13 15:27:50.000000 django-dreiattest-0.0.8/dreiattest/apps.py
--rw-r--r--   0 samuelbichsel   (501) staff       (20)     1826 2021-04-21 06:49:37.000000 django-dreiattest-0.0.8/dreiattest/decorators.py
--rw-r--r--   0 samuelbichsel   (501) staff       (20)     1925 2021-04-13 16:28:25.000000 django-dreiattest-0.0.8/dreiattest/device_session.py
--rw-r--r--   0 samuelbichsel   (501) staff       (20)      234 2021-04-13 15:27:50.000000 django-dreiattest-0.0.8/dreiattest/exceptions.py
--rw-r--r--   0 samuelbichsel   (501) staff       (20)     1516 2021-04-21 15:20:23.000000 django-dreiattest-0.0.8/dreiattest/helpers.py
--rw-r--r--   0 samuelbichsel   (501) staff       (20)     2373 2021-04-13 16:28:25.000000 django-dreiattest-0.0.8/dreiattest/key.py
--rw-r--r--   0 samuelbichsel   (501) staff       (20)       57 2021-04-21 12:41:24.000000 django-dreiattest-0.0.8/dreiattest/logging.py
-drwxr-xr-x   0 samuelbichsel   (501) staff       (20)        0 2021-04-21 16:22:01.297299 django-dreiattest-0.0.8/dreiattest/migrations/
--rw-r--r--   0 samuelbichsel   (501) staff       (20)     1912 2021-04-13 15:27:50.000000 django-dreiattest-0.0.8/dreiattest/migrations/0001_initial.py
--rw-r--r--   0 samuelbichsel   (501) staff       (20)     1244 2021-04-13 15:27:50.000000 django-dreiattest-0.0.8/dreiattest/migrations/0002_auto_20210225_0949.py
--rw-r--r--   0 samuelbichsel   (501) staff       (20)      538 2021-04-13 15:27:50.000000 django-dreiattest-0.0.8/dreiattest/migrations/0003_auto_20210225_1008.py
--rw-r--r--   0 samuelbichsel   (501) staff       (20)      512 2021-04-13 15:27:50.000000 django-dreiattest-0.0.8/dreiattest/migrations/0004_auto_20210225_1246.py
--rw-r--r--   0 samuelbichsel   (501) staff       (20)        0 2021-04-13 15:27:50.000000 django-dreiattest-0.0.8/dreiattest/migrations/__init__.py
--rw-r--r--   0 samuelbichsel   (501) staff       (20)     1902 2021-04-20 13:19:52.000000 django-dreiattest-0.0.8/dreiattest/models.py
--rw-r--r--   0 samuelbichsel   (501) staff       (20)     1118 2021-04-13 16:28:25.000000 django-dreiattest-0.0.8/dreiattest/nonce.py
--rw-r--r--   0 samuelbichsel   (501) staff       (20)      658 2021-04-21 07:52:27.000000 django-dreiattest-0.0.8/dreiattest/settings.py
--rw-r--r--   0 samuelbichsel   (501) staff       (20)      327 2021-04-13 15:27:50.000000 django-dreiattest-0.0.8/dreiattest/urls.py
--rw-r--r--   0 samuelbichsel   (501) staff       (20)     1976 2021-04-13 16:28:25.000000 django-dreiattest-0.0.8/dreiattest/views.py
--rw-r--r--   0 samuelbichsel   (501) staff       (20)      100 2021-04-21 09:26:49.000000 django-dreiattest-0.0.8/pyproject.toml
--rw-r--r--   0 samuelbichsel   (501) staff       (20)       38 2021-04-21 16:22:01.298010 django-dreiattest-0.0.8/setup.cfg
--rw-r--r--   0 samuelbichsel   (501) staff       (20)     2939 2021-04-13 15:27:50.000000 django-dreiattest-0.0.8/setup.py
+drwxr-xr-x   0 samuelbichsel   (501) staff       (20)        0 2021-04-26 14:34:32.979477 django-dreiattest-0.0.9/
+-rw-r--r--   0 samuelbichsel   (501) staff       (20)     1064 2021-04-13 15:27:50.000000 django-dreiattest-0.0.9/LICENSE
+-rw-r--r--   0 samuelbichsel   (501) staff       (20)       62 2021-04-13 15:27:50.000000 django-dreiattest-0.0.9/MANIFEST.in
+-rw-r--r--   0 samuelbichsel   (501) staff       (20)     2167 2021-04-26 14:34:32.979189 django-dreiattest-0.0.9/PKG-INFO
+-rw-r--r--   0 samuelbichsel   (501) staff       (20)     1192 2021-04-13 15:27:50.000000 django-dreiattest-0.0.9/README.md
+drwxr-xr-x   0 samuelbichsel   (501) staff       (20)        0 2021-04-26 14:34:32.973177 django-dreiattest-0.0.9/django_dreiattest.egg-info/
+-rw-r--r--   0 samuelbichsel   (501) staff       (20)     2167 2021-04-26 14:34:32.000000 django-dreiattest-0.0.9/django_dreiattest.egg-info/PKG-INFO
+-rw-r--r--   0 samuelbichsel   (501) staff       (20)      748 2021-04-26 14:34:32.000000 django-dreiattest-0.0.9/django_dreiattest.egg-info/SOURCES.txt
+-rw-r--r--   0 samuelbichsel   (501) staff       (20)        1 2021-04-26 14:34:32.000000 django-dreiattest-0.0.9/django_dreiattest.egg-info/dependency_links.txt
+-rw-r--r--   0 samuelbichsel   (501) staff       (20)       11 2021-04-26 14:34:32.000000 django-dreiattest-0.0.9/django_dreiattest.egg-info/top_level.txt
+drwxr-xr-x   0 samuelbichsel   (501) staff       (20)        0 2021-04-26 14:34:32.977373 django-dreiattest-0.0.9/dreiattest/
+-rw-r--r--   0 samuelbichsel   (501) staff       (20)       56 2021-04-13 15:27:50.000000 django-dreiattest-0.0.9/dreiattest/__init__.py
+-rw-r--r--   0 samuelbichsel   (501) staff       (20)       63 2021-04-26 14:33:47.000000 django-dreiattest-0.0.9/dreiattest/__version__.py
+-rw-r--r--   0 samuelbichsel   (501) staff       (20)       95 2021-04-13 15:27:50.000000 django-dreiattest-0.0.9/dreiattest/apps.py
+-rw-r--r--   0 samuelbichsel   (501) staff       (20)     1826 2021-04-21 06:49:37.000000 django-dreiattest-0.0.9/dreiattest/decorators.py
+-rw-r--r--   0 samuelbichsel   (501) staff       (20)     1925 2021-04-13 16:28:25.000000 django-dreiattest-0.0.9/dreiattest/device_session.py
+-rw-r--r--   0 samuelbichsel   (501) staff       (20)      234 2021-04-13 15:27:50.000000 django-dreiattest-0.0.9/dreiattest/exceptions.py
+-rw-r--r--   0 samuelbichsel   (501) staff       (20)     1516 2021-04-21 15:20:23.000000 django-dreiattest-0.0.9/dreiattest/helpers.py
+-rw-r--r--   0 samuelbichsel   (501) staff       (20)     2373 2021-04-13 16:28:25.000000 django-dreiattest-0.0.9/dreiattest/key.py
+-rw-r--r--   0 samuelbichsel   (501) staff       (20)       57 2021-04-21 12:41:24.000000 django-dreiattest-0.0.9/dreiattest/logging.py
+drwxr-xr-x   0 samuelbichsel   (501) staff       (20)        0 2021-04-26 14:34:32.978859 django-dreiattest-0.0.9/dreiattest/migrations/
+-rw-r--r--   0 samuelbichsel   (501) staff       (20)     1912 2021-04-13 15:27:50.000000 django-dreiattest-0.0.9/dreiattest/migrations/0001_initial.py
+-rw-r--r--   0 samuelbichsel   (501) staff       (20)     1244 2021-04-13 15:27:50.000000 django-dreiattest-0.0.9/dreiattest/migrations/0002_auto_20210225_0949.py
+-rw-r--r--   0 samuelbichsel   (501) staff       (20)      538 2021-04-13 15:27:50.000000 django-dreiattest-0.0.9/dreiattest/migrations/0003_auto_20210225_1008.py
+-rw-r--r--   0 samuelbichsel   (501) staff       (20)      512 2021-04-13 15:27:50.000000 django-dreiattest-0.0.9/dreiattest/migrations/0004_auto_20210225_1246.py
+-rw-r--r--   0 samuelbichsel   (501) staff       (20)        0 2021-04-13 15:27:50.000000 django-dreiattest-0.0.9/dreiattest/migrations/__init__.py
+-rw-r--r--   0 samuelbichsel   (501) staff       (20)     2266 2021-04-26 13:45:55.000000 django-dreiattest-0.0.9/dreiattest/models.py
+-rw-r--r--   0 samuelbichsel   (501) staff       (20)     1118 2021-04-13 16:28:25.000000 django-dreiattest-0.0.9/dreiattest/nonce.py
+-rw-r--r--   0 samuelbichsel   (501) staff       (20)      658 2021-04-21 07:52:27.000000 django-dreiattest-0.0.9/dreiattest/settings.py
+-rw-r--r--   0 samuelbichsel   (501) staff       (20)      327 2021-04-13 15:27:50.000000 django-dreiattest-0.0.9/dreiattest/urls.py
+-rw-r--r--   0 samuelbichsel   (501) staff       (20)     1977 2021-04-26 13:37:18.000000 django-dreiattest-0.0.9/dreiattest/views.py
+-rw-r--r--   0 samuelbichsel   (501) staff       (20)      100 2021-04-21 09:26:49.000000 django-dreiattest-0.0.9/pyproject.toml
+-rw-r--r--   0 samuelbichsel   (501) staff       (20)       38 2021-04-26 14:34:32.979573 django-dreiattest-0.0.9/setup.cfg
+-rw-r--r--   0 samuelbichsel   (501) staff       (20)     2939 2021-04-13 15:27:50.000000 django-dreiattest-0.0.9/setup.py
```

### Comparing `django-dreiattest-0.0.8/LICENSE` & `django-dreiattest-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django-dreiattest-0.0.8/PKG-INFO` & `django-dreiattest-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-dreiattest
-Version: 0.0.8
+Version: 0.0.9
 Summary: UNKNOWN
 Home-page: https://github.com/dreipol/django-dreiattest
 Author: dreipol
 Author-email: dev@dreipol.ch
 License: MIT
 Description: 
         # django-dreiattest
```

### Comparing `django-dreiattest-0.0.8/README.md` & `django-dreiattest-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `django-dreiattest-0.0.8/django_dreiattest.egg-info/PKG-INFO` & `django-dreiattest-0.0.9/django_dreiattest.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-dreiattest
-Version: 0.0.8
+Version: 0.0.9
 Summary: UNKNOWN
 Home-page: https://github.com/dreipol/django-dreiattest
 Author: dreipol
 Author-email: dev@dreipol.ch
 License: MIT
 Description: 
         # django-dreiattest
```

### Comparing `django-dreiattest-0.0.8/django_dreiattest.egg-info/SOURCES.txt` & `django-dreiattest-0.0.9/django_dreiattest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-dreiattest-0.0.8/dreiattest/decorators.py` & `django-dreiattest-0.0.9/dreiattest/decorators.py`

 * *Files identical despite different names*

### Comparing `django-dreiattest-0.0.8/dreiattest/device_session.py` & `django-dreiattest-0.0.9/dreiattest/device_session.py`

 * *Files identical despite different names*

### Comparing `django-dreiattest-0.0.8/dreiattest/helpers.py` & `django-dreiattest-0.0.9/dreiattest/helpers.py`

 * *Files identical despite different names*

### Comparing `django-dreiattest-0.0.8/dreiattest/key.py` & `django-dreiattest-0.0.9/dreiattest/key.py`

 * *Files identical despite different names*

### Comparing `django-dreiattest-0.0.8/dreiattest/migrations/0001_initial.py` & `django-dreiattest-0.0.9/dreiattest/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-dreiattest-0.0.8/dreiattest/migrations/0002_auto_20210225_0949.py` & `django-dreiattest-0.0.9/dreiattest/migrations/0002_auto_20210225_0949.py`

 * *Files identical despite different names*

### Comparing `django-dreiattest-0.0.8/dreiattest/migrations/0003_auto_20210225_1008.py` & `django-dreiattest-0.0.9/dreiattest/migrations/0003_auto_20210225_1008.py`

 * *Files identical despite different names*

### Comparing `django-dreiattest-0.0.8/dreiattest/migrations/0004_auto_20210225_1246.py` & `django-dreiattest-0.0.9/dreiattest/migrations/0004_auto_20210225_1246.py`

 * *Files identical despite different names*

### Comparing `django-dreiattest-0.0.8/dreiattest/models.py` & `django-dreiattest-0.0.9/dreiattest/models.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,24 @@
+import base64
 from datetime import datetime
-
 from cryptography.hazmat.primitives.asymmetric.ec import ECDSA
 from django.db.models import Model, CharField, UUIDField, DateTimeField, ForeignKey, PROTECT, TextField
 from cryptography.hazmat.primitives.serialization.base import load_pem_public_key
 from cryptography.hazmat._types import _PUBLIC_KEY_TYPES
 from cryptography.hazmat.primitives import hashes
+from . import settings as dreiattest_settings
 
 from cryptography.hazmat.primitives.asymmetric import (
     dsa,
     ec,
     ed25519,
     ed448,
     rsa,
 )
+from pyattest.configs.apple import AppleConfig
 from pyattest.verifiers.apple import AppleVerifier
 
 
 class DeviceSession(Model):
     user_id = CharField(max_length=255, null=True)
     session_id = UUIDField(unique=True)
     created_at = DateTimeField(auto_now_add=True)
@@ -52,8 +54,12 @@
     def load_pem(self) -> _PUBLIC_KEY_TYPES:
         return load_pem_public_key(self.public_key.encode())
 
     def verify(self, signature_header: bytes, nonce: bytes) -> None:
         pem_key = self.load_pem()
 
         if isinstance(pem_key, ec.EllipticCurvePublicKey):
-            AppleVerifier.verify_assertion(signature_header, nonce, pem_key)
+            config = AppleConfig(key_id=base64.b64decode(self.public_key_id),
+                                 app_id=dreiattest_settings.DREIATTEST_APPLE_APPID,
+                                 production=dreiattest_settings.DREIATTEST_PRODUCTION)
+
+            AppleVerifier.verify_assertion(signature_header, nonce, pem_key, config)
```

### Comparing `django-dreiattest-0.0.8/dreiattest/nonce.py` & `django-dreiattest-0.0.9/dreiattest/nonce.py`

 * *Files identical despite different names*

### Comparing `django-dreiattest-0.0.8/dreiattest/settings.py` & `django-dreiattest-0.0.9/dreiattest/settings.py`

 * *Files identical despite different names*

### Comparing `django-dreiattest-0.0.8/dreiattest/views.py` & `django-dreiattest-0.0.9/dreiattest/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from django.core.handlers.wsgi import WSGIRequest
 from django.http import JsonResponse
 from django.views.decorators.csrf import csrf_exempt
 from django.views.decorators.http import require_http_methods
 from pyattest.exceptions import PyAttestException
 
+from dreiattest.device_session import device_session_from_request
 from dreiattest.exceptions import InvalidHeaderException, InvalidPayloadException
 from dreiattest.key import key_from_request
 from dreiattest.nonce import create_nonce, nonce_from_request
-from dreiattest.device_session import device_session_from_request
 
 
 @require_http_methods(['GET'])
 def nonce(request: WSGIRequest):
     """
     Request a nonce to create the attestation on the device. The Dreiattest-Uid header needs to be set
     with a valid device session id. The server will persist the nonce and persist it with the given uid.
@@ -19,15 +19,15 @@
     try:
         device_session = device_session_from_request(request)
     except InvalidHeaderException:
         return JsonResponse({'error': 'Invalid or missing Dreiattest-Uid header.'})
 
     nonce = create_nonce(device_session)
 
-    return JsonResponse({'nonce': nonce.value})
+    return JsonResponse(nonce.value, safe=False)
 
 
 @require_http_methods(['POST'])
 @csrf_exempt
 def key(request: WSGIRequest):
     """ Store a public key belonging to a user in the database. Upcoming requests can be signed with said key. """
     try:
```

### Comparing `django-dreiattest-0.0.8/setup.py` & `django-dreiattest-0.0.9/setup.py`

 * *Files identical despite different names*

