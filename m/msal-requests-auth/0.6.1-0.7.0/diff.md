# Comparing `tmp/msal_requests_auth-0.6.1.tar.gz` & `tmp/msal_requests_auth-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msal_requests_auth-0.6.1.tar", last modified: Fri Dec  9 22:12:15 2022, max compression
+gzip compressed data, was "msal_requests_auth-0.7.0.tar", last modified: Fri Apr 28 19:32:48 2023, max compression
```

## Comparing `msal_requests_auth-0.6.1.tar` & `msal_requests_auth-0.7.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 22:12:15.851232 msal_requests_auth-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2022-12-09 22:12:02.000000 msal_requests_auth-0.6.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2022-12-09 22:12:02.000000 msal_requests_auth-0.6.1/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2022-12-09 22:12:02.000000 msal_requests_auth-0.6.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2022-12-09 22:12:02.000000 msal_requests_auth-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      130 2022-12-09 22:12:02.000000 msal_requests_auth-0.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5444 2022-12-09 22:12:15.855232 msal_requests_auth-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4333 2022-12-09 22:12:02.000000 msal_requests_auth-0.6.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 22:12:15.851232 msal_requests_auth-0.6.1/msal_requests_auth/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2022-12-09 22:12:02.000000 msal_requests_auth-0.6.1/msal_requests_auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2022-12-09 22:12:02.000000 msal_requests_auth-0.6.1/msal_requests_auth/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 22:12:15.851232 msal_requests_auth-0.6.1/msal_requests_auth/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2022-12-09 22:12:02.000000 msal_requests_auth-0.6.1/msal_requests_auth/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2022-12-09 22:12:02.000000 msal_requests_auth-0.6.1/msal_requests_auth/auth/base_auth_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2022-12-09 22:12:02.000000 msal_requests_auth-0.6.1/msal_requests_auth/auth/client_credential.py
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2022-12-09 22:12:02.000000 msal_requests_auth-0.6.1/msal_requests_auth/auth/device_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2022-12-09 22:12:02.000000 msal_requests_auth-0.6.1/msal_requests_auth/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2022-12-09 22:12:02.000000 msal_requests_auth-0.6.1/msal_requests_auth/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-09 22:12:02.000000 msal_requests_auth-0.6.1/msal_requests_auth/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 22:12:15.851232 msal_requests_auth-0.6.1/msal_requests_auth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5444 2022-12-09 22:12:15.000000 msal_requests_auth-0.6.1/msal_requests_auth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      755 2022-12-09 22:12:15.000000 msal_requests_auth-0.6.1/msal_requests_auth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-09 22:12:15.000000 msal_requests_auth-0.6.1/msal_requests_auth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-09 22:12:15.000000 msal_requests_auth-0.6.1/msal_requests_auth.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      118 2022-12-09 22:12:15.000000 msal_requests_auth-0.6.1/msal_requests_auth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2022-12-09 22:12:15.000000 msal_requests_auth-0.6.1/msal_requests_auth.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2022-12-09 22:12:15.855232 msal_requests_auth-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       60 2022-12-09 22:12:02.000000 msal_requests_auth-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 22:12:15.851232 msal_requests_auth-0.6.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2022-12-09 22:12:02.000000 msal_requests_auth-0.6.1/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2022-12-09 22:12:02.000000 msal_requests_auth-0.6.1/test/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2022-12-09 22:12:02.000000 msal_requests_auth-0.6.1/test/test_client_credential.py
--rw-r--r--   0 runner    (1001) docker     (123)     6334 2022-12-09 22:12:02.000000 msal_requests_auth-0.6.1/test/test_devide_code.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:32:48.649364 msal_requests_auth-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-04-28 19:32:32.000000 msal_requests_auth-0.7.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-04-28 19:32:32.000000 msal_requests_auth-0.7.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-04-28 19:32:32.000000 msal_requests_auth-0.7.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-28 19:32:32.000000 msal_requests_auth-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-28 19:32:32.000000 msal_requests_auth-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-04-28 19:32:48.649364 msal_requests_auth-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-04-28 19:32:32.000000 msal_requests_auth-0.7.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:32:48.649364 msal_requests_auth-0.7.0/msal_requests_auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-28 19:32:32.000000 msal_requests_auth-0.7.0/msal_requests_auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-28 19:32:32.000000 msal_requests_auth-0.7.0/msal_requests_auth/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:32:48.649364 msal_requests_auth-0.7.0/msal_requests_auth/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-28 19:32:32.000000 msal_requests_auth-0.7.0/msal_requests_auth/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-04-28 19:32:32.000000 msal_requests_auth-0.7.0/msal_requests_auth/auth/base_auth_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-04-28 19:32:32.000000 msal_requests_auth-0.7.0/msal_requests_auth/auth/client_credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-04-28 19:32:32.000000 msal_requests_auth-0.7.0/msal_requests_auth/auth/device_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-04-28 19:32:32.000000 msal_requests_auth-0.7.0/msal_requests_auth/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-28 19:32:32.000000 msal_requests_auth-0.7.0/msal_requests_auth/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 19:32:32.000000 msal_requests_auth-0.7.0/msal_requests_auth/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:32:48.649364 msal_requests_auth-0.7.0/msal_requests_auth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-04-28 19:32:48.000000 msal_requests_auth-0.7.0/msal_requests_auth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-28 19:32:48.000000 msal_requests_auth-0.7.0/msal_requests_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 19:32:48.000000 msal_requests_auth-0.7.0/msal_requests_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 19:32:48.000000 msal_requests_auth-0.7.0/msal_requests_auth.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-28 19:32:48.000000 msal_requests_auth-0.7.0/msal_requests_auth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-28 19:32:48.000000 msal_requests_auth-0.7.0/msal_requests_auth.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-28 19:32:48.649364 msal_requests_auth-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-28 19:32:32.000000 msal_requests_auth-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 19:32:48.649364 msal_requests_auth-0.7.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-28 19:32:32.000000 msal_requests_auth-0.7.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-04-28 19:32:32.000000 msal_requests_auth-0.7.0/test/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-04-28 19:32:32.000000 msal_requests_auth-0.7.0/test/test_client_credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6334 2023-04-28 19:32:32.000000 msal_requests_auth-0.7.0/test/test_devide_code.py
```

### Comparing `msal_requests_auth-0.6.1/AUTHORS.rst` & `msal_requests_auth-0.7.0/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `msal_requests_auth-0.6.1/CODE_OF_CONDUCT.rst` & `msal_requests_auth-0.7.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `msal_requests_auth-0.6.1/CONTRIBUTING.rst` & `msal_requests_auth-0.7.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `msal_requests_auth-0.6.1/LICENSE` & `msal_requests_auth-0.7.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2021, Corteva Agriscience™
+Copyright (c) 2021-2023, Corteva Agriscience™
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
```

### Comparing `msal_requests_auth-0.6.1/PKG-INFO` & `msal_requests_auth-0.7.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msal_requests_auth
-Version: 0.6.1
+Version: 0.7.0
 Summary: Authentication using python requests and MSAL
 Home-page: https://github.com/corteva/msal-requests-auth
 Download-URL: http://python.org/pypi/msal-requests-auth
 Author: msal_requests_auth Contributors
 Author-email: alansnow21@gmail.com
 License: BSD License
 Keywords: msal,requests
@@ -20,14 +20,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
+Provides-Extra: keyring
 Provides-Extra: dev
 Provides-Extra: all
 License-File: LICENSE
 
 ==================
 msal-requests-auth
 ==================
@@ -85,28 +86,28 @@
 
 .. note:: By default, `DeviceCodeAuth` copys the code to your clipboard and opens a webbrowser.
           To disable, either set `headless=True` when initializing `DeviceCodeAuth`
           or set the environment variable `MSAL_REQUESTS_AUTH_HEADLESS` to `true`.
 
 - New in version 0.2.0: headless
 - New in version 0.6.0: MSAL_REQUESTS_AUTH_HEADLESS environment variable
-
+- New in version 0.7.0: KeyringTokenCache
 
 .. code-block:: python
 
     import requests
     import msal
     from msal_requests_auth.auth import DeviceCodeAuth
-    from msal_requests_auth.cache import SimpleTokenCache
+    from msal_requests_auth.cache import KeyringTokenCache
 
     client_id = "<client ID from Azure AD>"
     tenant_id = "<tenant ID from Azure AD>"
     application_id = "<client ID of application you want to get a token for from Azure AD>"
 
-    with SimpleTokenCache() as token_cache:
+    with KeyringTokenCache() as token_cache:
         app = msal.PublicClientApplication(
             client_id,
             authority=f"https://login.microsoftonline.com/{tenant_id}/",
             token_cache=token_cache,
         )
         auth = DeviceCodeAuth(
             client=app,
```

### Comparing `msal_requests_auth-0.6.1/README.rst` & `msal_requests_auth-0.7.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -55,28 +55,28 @@
 
 .. note:: By default, `DeviceCodeAuth` copys the code to your clipboard and opens a webbrowser.
           To disable, either set `headless=True` when initializing `DeviceCodeAuth`
           or set the environment variable `MSAL_REQUESTS_AUTH_HEADLESS` to `true`.
 
 - New in version 0.2.0: headless
 - New in version 0.6.0: MSAL_REQUESTS_AUTH_HEADLESS environment variable
-
+- New in version 0.7.0: KeyringTokenCache
 
 .. code-block:: python
 
     import requests
     import msal
     from msal_requests_auth.auth import DeviceCodeAuth
-    from msal_requests_auth.cache import SimpleTokenCache
+    from msal_requests_auth.cache import KeyringTokenCache
 
     client_id = "<client ID from Azure AD>"
     tenant_id = "<tenant ID from Azure AD>"
     application_id = "<client ID of application you want to get a token for from Azure AD>"
 
-    with SimpleTokenCache() as token_cache:
+    with KeyringTokenCache() as token_cache:
         app = msal.PublicClientApplication(
             client_id,
             authority=f"https://login.microsoftonline.com/{tenant_id}/",
             token_cache=token_cache,
         )
         auth = DeviceCodeAuth(
             client=app,
```

### Comparing `msal_requests_auth-0.6.1/msal_requests_auth/auth/base_auth_client.py` & `msal_requests_auth-0.7.0/msal_requests_auth/auth/base_auth_client.py`

 * *Files identical despite different names*

### Comparing `msal_requests_auth-0.6.1/msal_requests_auth/auth/client_credential.py` & `msal_requests_auth-0.7.0/msal_requests_auth/auth/client_credential.py`

 * *Files identical despite different names*

### Comparing `msal_requests_auth-0.6.1/msal_requests_auth/auth/device_code.py` & `msal_requests_auth-0.7.0/msal_requests_auth/auth/device_code.py`

 * *Files identical despite different names*

### Comparing `msal_requests_auth-0.6.1/msal_requests_auth/cache.py` & `msal_requests_auth-0.7.0/msal_requests_auth/cache.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,43 @@
 """
 Based on:
 https://msal-python.readthedocs.io/en/latest/#msal.SerializableTokenCache
 """
 import os
+from abc import ABC, abstractmethod
 from pathlib import Path
 from typing import Union
 
 from appdirs import user_cache_dir
 from msal import SerializableTokenCache
 
 
-class SimpleTokenCache(SerializableTokenCache):
+class _BaseTokenCache(ABC, SerializableTokenCache):
+    """
+    Base class for a token cache
+    """
+
+    @abstractmethod
+    def write_cache(self) -> None:
+        """
+        Write cache if needed.
+        """
+        raise NotImplementedError
+
+    def __del__(self):
+        self.write_cache()
+
+    def __enter__(self):
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        self.write_cache()
+
+
+class SimpleTokenCache(_BaseTokenCache):
     """
     Provides a simple token cache for users to
     persist the cache across sessions.
 
     .. versionadded:: 0.4.0
 
     """
@@ -42,15 +65,47 @@
     def write_cache(self) -> None:
         """
         Write cache to disk if needed.
         """
         if self.has_state_changed:
             self.cache_file.write_text(self.serialize())
 
-    def __del__(self):
-        self.write_cache()
 
-    def __enter__(self):
-        return self
+def _import_keyring():
+    """
+    Method to import keyring with error message
+    """
+    try:
+        import keyring
+    except ModuleNotFoundError as error:
+        raise ModuleNotFoundError(
+            "Please install msal_requests_auth with the "
+            "'keyring' extra: msal_requests_auth[keyring]."
+        ) from error
+    return keyring
 
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        self.write_cache()
+
+class KeyringTokenCache(_BaseTokenCache):
+    """
+    Provides a token cache for users to
+    persist the cache across sessions using keyring.
+
+    .. versionadded:: 0.7.0
+
+    .. note:: Requires keyring to be installed. The 'keyring'
+              extra can be used for that (msal_requests_auth[keyring]).
+    """
+
+    def __init__(self) -> None:
+        super().__init__()
+        token_cache = _import_keyring().get_password("__msal_requests_auth__", "token")
+        if token_cache is not None:
+            self.deserialize(token_cache)
+
+    def write_cache(self) -> None:
+        """
+        Write cache to keyring if needed.
+        """
+        if self.has_state_changed:
+            _import_keyring().set_password(
+                "__msal_requests_auth__", "token", self.serialize()
+            )
```

### Comparing `msal_requests_auth-0.6.1/msal_requests_auth.egg-info/PKG-INFO` & `msal_requests_auth-0.7.0/msal_requests_auth.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msal-requests-auth
-Version: 0.6.1
+Version: 0.7.0
 Summary: Authentication using python requests and MSAL
 Home-page: https://github.com/corteva/msal-requests-auth
 Download-URL: http://python.org/pypi/msal-requests-auth
 Author: msal_requests_auth Contributors
 Author-email: alansnow21@gmail.com
 License: BSD License
 Keywords: msal,requests
@@ -20,14 +20,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
+Provides-Extra: keyring
 Provides-Extra: dev
 Provides-Extra: all
 License-File: LICENSE
 
 ==================
 msal-requests-auth
 ==================
@@ -85,28 +86,28 @@
 
 .. note:: By default, `DeviceCodeAuth` copys the code to your clipboard and opens a webbrowser.
           To disable, either set `headless=True` when initializing `DeviceCodeAuth`
           or set the environment variable `MSAL_REQUESTS_AUTH_HEADLESS` to `true`.
 
 - New in version 0.2.0: headless
 - New in version 0.6.0: MSAL_REQUESTS_AUTH_HEADLESS environment variable
-
+- New in version 0.7.0: KeyringTokenCache
 
 .. code-block:: python
 
     import requests
     import msal
     from msal_requests_auth.auth import DeviceCodeAuth
-    from msal_requests_auth.cache import SimpleTokenCache
+    from msal_requests_auth.cache import KeyringTokenCache
 
     client_id = "<client ID from Azure AD>"
     tenant_id = "<tenant ID from Azure AD>"
     application_id = "<client ID of application you want to get a token for from Azure AD>"
 
-    with SimpleTokenCache() as token_cache:
+    with KeyringTokenCache() as token_cache:
         app = msal.PublicClientApplication(
             client_id,
             authority=f"https://login.microsoftonline.com/{tenant_id}/",
             token_cache=token_cache,
         )
         auth = DeviceCodeAuth(
             client=app,
```

### Comparing `msal_requests_auth-0.6.1/msal_requests_auth.egg-info/SOURCES.txt` & `msal_requests_auth-0.7.0/msal_requests_auth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `msal_requests_auth-0.6.1/setup.cfg` & `msal_requests_auth-0.7.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -42,19 +42,22 @@
 msal_requests_auth = 
 	py.typed
 
 [options.packages.find]
 include = msal_requests_auth*
 
 [options.extras_require]
+keyring = 
+	keyring
 dev = 
 	pytest
 	pytest-cov
 	pre-commit
 	pylint
 all = 
+	%(keyring)s
 	%(dev)s
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `msal_requests_auth-0.6.1/test/test_client_credential.py` & `msal_requests_auth-0.7.0/test/test_client_credential.py`

 * *Files identical despite different names*

### Comparing `msal_requests_auth-0.6.1/test/test_devide_code.py` & `msal_requests_auth-0.7.0/test/test_devide_code.py`

 * *Files identical despite different names*

