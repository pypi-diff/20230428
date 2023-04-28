# Comparing `tmp/pyattest-0.0.8.tar.gz` & `tmp/pyattest-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyattest-0.0.8.tar", last modified: Wed Sep 15 14:48:19 2021, max compression
+gzip compressed data, was "dist/pyattest-0.0.9.tar", last modified: Mon Sep 27 13:36:26 2021, max compression
```

## Comparing `pyattest-0.0.8.tar` & `pyattest-0.0.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 lab       (1000) lab       (1000)        0 2021-09-15 14:48:19.361833 pyattest-0.0.8/
--rw-rw-r--   0 lab       (1000) lab       (1000)     1064 2021-01-22 10:45:45.000000 pyattest-0.0.8/LICENSE
--rw-rw-r--   0 lab       (1000) lab       (1000)       60 2021-01-22 10:45:45.000000 pyattest-0.0.8/MANIFEST.in
--rw-rw-r--   0 lab       (1000) lab       (1000)     2951 2021-09-15 14:48:19.361833 pyattest-0.0.8/PKG-INFO
--rw-rw-r--   0 lab       (1000) lab       (1000)     1890 2021-04-01 07:22:59.000000 pyattest-0.0.8/README.md
-drwxrwxr-x   0 lab       (1000) lab       (1000)        0 2021-09-15 14:48:19.361833 pyattest-0.0.8/pyattest/
--rw-rw-r--   0 lab       (1000) lab       (1000)        0 2021-01-14 17:06:25.000000 pyattest-0.0.8/pyattest/__init__.py
--rw-rw-r--   0 lab       (1000) lab       (1000)       63 2021-09-15 14:47:52.000000 pyattest-0.0.8/pyattest/__version__.py
--rw-rw-r--   0 lab       (1000) lab       (1000)     1039 2021-09-15 14:47:44.000000 pyattest-0.0.8/pyattest/assertion.py
--rw-rw-r--   0 lab       (1000) lab       (1000)      896 2021-09-15 14:47:44.000000 pyattest-0.0.8/pyattest/attestation.py
-drwxrwxr-x   0 lab       (1000) lab       (1000)        0 2021-09-15 14:48:19.361833 pyattest-0.0.8/pyattest/configs/
--rw-rw-r--   0 lab       (1000) lab       (1000)        0 2021-04-01 09:54:33.000000 pyattest-0.0.8/pyattest/configs/__init__.py
--rw-rw-r--   0 lab       (1000) lab       (1000)     1194 2021-09-15 14:47:44.000000 pyattest-0.0.8/pyattest/configs/apple.py
--rw-rw-r--   0 lab       (1000) lab       (1000)      256 2021-09-15 14:47:44.000000 pyattest-0.0.8/pyattest/configs/config.py
--rw-rw-r--   0 lab       (1000) lab       (1000)      886 2021-09-15 14:47:44.000000 pyattest-0.0.8/pyattest/configs/google.py
--rw-rw-r--   0 lab       (1000) lab       (1000)      705 2021-09-14 13:55:35.000000 pyattest-0.0.8/pyattest/exceptions.py
-drwxrwxr-x   0 lab       (1000) lab       (1000)        0 2021-09-15 14:48:19.361833 pyattest-0.0.8/pyattest/testutils/
--rw-rw-r--   0 lab       (1000) lab       (1000)        0 2021-09-14 07:55:39.000000 pyattest-0.0.8/pyattest/testutils/__init__.py
-drwxrwxr-x   0 lab       (1000) lab       (1000)        0 2021-09-15 14:48:19.361833 pyattest-0.0.8/pyattest/testutils/factories/
--rw-rw-r--   0 lab       (1000) lab       (1000)        0 2021-09-14 07:55:39.000000 pyattest-0.0.8/pyattest/testutils/factories/__init__.py
-drwxrwxr-x   0 lab       (1000) lab       (1000)        0 2021-09-15 14:48:19.361833 pyattest-0.0.8/pyattest/testutils/factories/attestation/
--rw-rw-r--   0 lab       (1000) lab       (1000)        0 2021-09-14 07:55:39.000000 pyattest-0.0.8/pyattest/testutils/factories/attestation/__init__.py
--rw-rw-r--   0 lab       (1000) lab       (1000)     3265 2021-09-14 09:48:29.000000 pyattest-0.0.8/pyattest/testutils/factories/attestation/apple.py
--rw-rw-r--   0 lab       (1000) lab       (1000)     2765 2021-09-14 09:48:51.000000 pyattest-0.0.8/pyattest/testutils/factories/attestation/google.py
--rw-rw-r--   0 lab       (1000) lab       (1000)     1708 2021-09-14 07:55:39.000000 pyattest-0.0.8/pyattest/testutils/factories/certificates.py
-drwxrwxr-x   0 lab       (1000) lab       (1000)        0 2021-09-15 14:48:19.361833 pyattest-0.0.8/pyattest/verifiers/
--rw-rw-r--   0 lab       (1000) lab       (1000)        0 2021-04-01 09:54:33.000000 pyattest-0.0.8/pyattest/verifiers/__init__.py
--rw-rw-r--   0 lab       (1000) lab       (1000)     1360 2021-09-15 14:47:44.000000 pyattest-0.0.8/pyattest/verifiers/apple_assertion.py
--rw-rw-r--   0 lab       (1000) lab       (1000)     7502 2021-09-15 14:47:44.000000 pyattest-0.0.8/pyattest/verifiers/apple_attestation.py
--rw-rw-r--   0 lab       (1000) lab       (1000)      246 2021-09-15 14:47:44.000000 pyattest-0.0.8/pyattest/verifiers/assertion.py
--rw-rw-r--   0 lab       (1000) lab       (1000)      260 2021-09-15 14:47:44.000000 pyattest-0.0.8/pyattest/verifiers/attestation.py
--rw-rw-r--   0 lab       (1000) lab       (1000)      146 2021-09-15 14:47:44.000000 pyattest-0.0.8/pyattest/verifiers/google_assertion.py
--rw-rw-r--   0 lab       (1000) lab       (1000)     4724 2021-09-15 14:47:44.000000 pyattest-0.0.8/pyattest/verifiers/google_attestation.py
-drwxrwxr-x   0 lab       (1000) lab       (1000)        0 2021-09-15 14:48:19.361833 pyattest-0.0.8/pyattest.egg-info/
--rw-rw-r--   0 lab       (1000) lab       (1000)     2951 2021-09-15 14:48:19.000000 pyattest-0.0.8/pyattest.egg-info/PKG-INFO
--rw-rw-r--   0 lab       (1000) lab       (1000)      946 2021-09-15 14:48:19.000000 pyattest-0.0.8/pyattest.egg-info/SOURCES.txt
--rw-rw-r--   0 lab       (1000) lab       (1000)        1 2021-09-15 14:48:19.000000 pyattest-0.0.8/pyattest.egg-info/dependency_links.txt
--rw-rw-r--   0 lab       (1000) lab       (1000)       39 2021-09-15 14:48:19.000000 pyattest-0.0.8/pyattest.egg-info/requires.txt
--rw-rw-r--   0 lab       (1000) lab       (1000)        9 2021-09-15 14:48:19.000000 pyattest-0.0.8/pyattest.egg-info/top_level.txt
--rw-rw-r--   0 lab       (1000) lab       (1000)       38 2021-09-15 14:48:19.361833 pyattest-0.0.8/setup.cfg
--rw-rw-r--   0 lab       (1000) lab       (1000)     3127 2021-09-14 09:46:42.000000 pyattest-0.0.8/setup.py
+drwxrwxr-x   0 lab       (1000) lab       (1000)        0 2021-09-27 13:36:26.883540 pyattest-0.0.9/
+-rw-rw-r--   0 lab       (1000) lab       (1000)     1064 2021-01-22 10:45:45.000000 pyattest-0.0.9/LICENSE
+-rw-rw-r--   0 lab       (1000) lab       (1000)       60 2021-01-22 10:45:45.000000 pyattest-0.0.9/MANIFEST.in
+-rw-rw-r--   0 lab       (1000) lab       (1000)     2951 2021-09-27 13:36:26.883540 pyattest-0.0.9/PKG-INFO
+-rw-rw-r--   0 lab       (1000) lab       (1000)     1890 2021-04-01 07:22:59.000000 pyattest-0.0.9/README.md
+drwxrwxr-x   0 lab       (1000) lab       (1000)        0 2021-09-27 13:36:26.879540 pyattest-0.0.9/pyattest/
+-rw-rw-r--   0 lab       (1000) lab       (1000)        0 2021-01-14 17:06:25.000000 pyattest-0.0.9/pyattest/__init__.py
+-rw-rw-r--   0 lab       (1000) lab       (1000)       63 2021-09-27 13:35:38.000000 pyattest-0.0.9/pyattest/__version__.py
+-rw-rw-r--   0 lab       (1000) lab       (1000)      986 2021-09-27 13:34:27.000000 pyattest-0.0.9/pyattest/assertion.py
+-rw-rw-r--   0 lab       (1000) lab       (1000)      896 2021-09-15 14:47:44.000000 pyattest-0.0.9/pyattest/attestation.py
+drwxrwxr-x   0 lab       (1000) lab       (1000)        0 2021-09-27 13:36:26.879540 pyattest-0.0.9/pyattest/configs/
+-rw-rw-r--   0 lab       (1000) lab       (1000)        0 2021-04-01 09:54:33.000000 pyattest-0.0.9/pyattest/configs/__init__.py
+-rw-rw-r--   0 lab       (1000) lab       (1000)     1194 2021-09-15 14:47:44.000000 pyattest-0.0.9/pyattest/configs/apple.py
+-rw-rw-r--   0 lab       (1000) lab       (1000)      256 2021-09-15 14:47:44.000000 pyattest-0.0.9/pyattest/configs/config.py
+-rw-rw-r--   0 lab       (1000) lab       (1000)      886 2021-09-15 14:47:44.000000 pyattest-0.0.9/pyattest/configs/google.py
+-rw-rw-r--   0 lab       (1000) lab       (1000)      705 2021-09-14 13:55:35.000000 pyattest-0.0.9/pyattest/exceptions.py
+drwxrwxr-x   0 lab       (1000) lab       (1000)        0 2021-09-27 13:36:26.883540 pyattest-0.0.9/pyattest/testutils/
+-rw-rw-r--   0 lab       (1000) lab       (1000)        0 2021-09-14 07:55:39.000000 pyattest-0.0.9/pyattest/testutils/__init__.py
+drwxrwxr-x   0 lab       (1000) lab       (1000)        0 2021-09-27 13:36:26.883540 pyattest-0.0.9/pyattest/testutils/factories/
+-rw-rw-r--   0 lab       (1000) lab       (1000)        0 2021-09-14 07:55:39.000000 pyattest-0.0.9/pyattest/testutils/factories/__init__.py
+drwxrwxr-x   0 lab       (1000) lab       (1000)        0 2021-09-27 13:36:26.883540 pyattest-0.0.9/pyattest/testutils/factories/attestation/
+-rw-rw-r--   0 lab       (1000) lab       (1000)        0 2021-09-14 07:55:39.000000 pyattest-0.0.9/pyattest/testutils/factories/attestation/__init__.py
+-rw-rw-r--   0 lab       (1000) lab       (1000)     3265 2021-09-14 09:48:29.000000 pyattest-0.0.9/pyattest/testutils/factories/attestation/apple.py
+-rw-rw-r--   0 lab       (1000) lab       (1000)     2765 2021-09-14 09:48:51.000000 pyattest-0.0.9/pyattest/testutils/factories/attestation/google.py
+-rw-rw-r--   0 lab       (1000) lab       (1000)     1708 2021-09-14 07:55:39.000000 pyattest-0.0.9/pyattest/testutils/factories/certificates.py
+drwxrwxr-x   0 lab       (1000) lab       (1000)        0 2021-09-27 13:36:26.883540 pyattest-0.0.9/pyattest/verifiers/
+-rw-rw-r--   0 lab       (1000) lab       (1000)        0 2021-04-01 09:54:33.000000 pyattest-0.0.9/pyattest/verifiers/__init__.py
+-rw-rw-r--   0 lab       (1000) lab       (1000)     1304 2021-09-27 13:27:05.000000 pyattest-0.0.9/pyattest/verifiers/apple_assertion.py
+-rw-rw-r--   0 lab       (1000) lab       (1000)     7502 2021-09-15 14:47:44.000000 pyattest-0.0.9/pyattest/verifiers/apple_attestation.py
+-rw-rw-r--   0 lab       (1000) lab       (1000)      246 2021-09-15 14:47:44.000000 pyattest-0.0.9/pyattest/verifiers/assertion.py
+-rw-rw-r--   0 lab       (1000) lab       (1000)      260 2021-09-15 14:47:44.000000 pyattest-0.0.9/pyattest/verifiers/attestation.py
+-rw-rw-r--   0 lab       (1000) lab       (1000)      362 2021-09-27 13:29:38.000000 pyattest-0.0.9/pyattest/verifiers/google_assertion.py
+-rw-rw-r--   0 lab       (1000) lab       (1000)     4724 2021-09-15 14:47:44.000000 pyattest-0.0.9/pyattest/verifiers/google_attestation.py
+drwxrwxr-x   0 lab       (1000) lab       (1000)        0 2021-09-27 13:36:26.879540 pyattest-0.0.9/pyattest.egg-info/
+-rw-rw-r--   0 lab       (1000) lab       (1000)     2951 2021-09-27 13:36:26.000000 pyattest-0.0.9/pyattest.egg-info/PKG-INFO
+-rw-rw-r--   0 lab       (1000) lab       (1000)      946 2021-09-27 13:36:26.000000 pyattest-0.0.9/pyattest.egg-info/SOURCES.txt
+-rw-rw-r--   0 lab       (1000) lab       (1000)        1 2021-09-27 13:36:26.000000 pyattest-0.0.9/pyattest.egg-info/dependency_links.txt
+-rw-rw-r--   0 lab       (1000) lab       (1000)       39 2021-09-27 13:36:26.000000 pyattest-0.0.9/pyattest.egg-info/requires.txt
+-rw-rw-r--   0 lab       (1000) lab       (1000)        9 2021-09-27 13:36:26.000000 pyattest-0.0.9/pyattest.egg-info/top_level.txt
+-rw-rw-r--   0 lab       (1000) lab       (1000)       38 2021-09-27 13:36:26.883540 pyattest-0.0.9/setup.cfg
+-rw-rw-r--   0 lab       (1000) lab       (1000)     3127 2021-09-14 09:46:42.000000 pyattest-0.0.9/setup.py
```

### Comparing `pyattest-0.0.8/LICENSE` & `pyattest-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyattest-0.0.8/PKG-INFO` & `pyattest-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyattest
-Version: 0.0.8
+Version: 0.0.9
 Summary: UNKNOWN
 Home-page: https://github.com/dreipol/pyattest
 Author: dreipol
 Author-email: dev@dreipol.ch
 License: MIT
 Description: 
         # pyattest
```

### Comparing `pyattest-0.0.8/README.md` & `pyattest-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pyattest-0.0.8/pyattest/assertion.py` & `pyattest-0.0.9/pyattest/assertion.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-from hashlib import sha256
-from typing import Union
-
 from cryptography.hazmat.primitives.asymmetric.ec import EllipticCurvePublicKey
 
 from pyattest.configs.config import Config
 from pyattest.exceptions import PyAttestException
 
 
 class Assertion:
```

### Comparing `pyattest-0.0.8/pyattest/attestation.py` & `pyattest-0.0.9/pyattest/attestation.py`

 * *Files identical despite different names*

### Comparing `pyattest-0.0.8/pyattest/configs/apple.py` & `pyattest-0.0.9/pyattest/configs/apple.py`

 * *Files identical despite different names*

### Comparing `pyattest-0.0.8/pyattest/configs/google.py` & `pyattest-0.0.9/pyattest/configs/google.py`

 * *Files identical despite different names*

### Comparing `pyattest-0.0.8/pyattest/exceptions.py` & `pyattest-0.0.9/pyattest/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyattest-0.0.8/pyattest/testutils/factories/attestation/apple.py` & `pyattest-0.0.9/pyattest/testutils/factories/attestation/apple.py`

 * *Files identical despite different names*

### Comparing `pyattest-0.0.8/pyattest/testutils/factories/attestation/google.py` & `pyattest-0.0.9/pyattest/testutils/factories/attestation/google.py`

 * *Files identical despite different names*

### Comparing `pyattest-0.0.8/pyattest/testutils/factories/certificates.py` & `pyattest-0.0.9/pyattest/testutils/factories/certificates.py`

 * *Files identical despite different names*

### Comparing `pyattest-0.0.8/pyattest/verifiers/apple_assertion.py` & `pyattest-0.0.9/pyattest/verifiers/apple_assertion.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,16 +16,14 @@
         """
         unpacked = self.unpack(self.assertion.raw)
         authenticator_data = unpacked['authenticator_data']
         nonce = sha256(authenticator_data + self.assertion.expected_hash).digest()
 
         self.assertion.public_key.verify(unpacked['raw']['signature'], nonce, ECDSA(hashes.SHA256()))
 
-        # cls.verify_app_id(unpacked['rp_id'], config)
-
     @staticmethod
     def unpack(raw: bytes) -> dict:
         """ Extract in `verify` method mentioned relevant data from cbor encoded raw bytes input. """
         raw = cbor_decode(raw)
 
         return {
             'raw': raw,
```

### Comparing `pyattest-0.0.8/pyattest/verifiers/apple_attestation.py` & `pyattest-0.0.9/pyattest/verifiers/apple_attestation.py`

 * *Files identical despite different names*

### Comparing `pyattest-0.0.8/pyattest/verifiers/google_attestation.py` & `pyattest-0.0.9/pyattest/verifiers/google_attestation.py`

 * *Files identical despite different names*

### Comparing `pyattest-0.0.8/pyattest.egg-info/PKG-INFO` & `pyattest-0.0.9/pyattest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyattest
-Version: 0.0.8
+Version: 0.0.9
 Summary: UNKNOWN
 Home-page: https://github.com/dreipol/pyattest
 Author: dreipol
 Author-email: dev@dreipol.ch
 License: MIT
 Description: 
         # pyattest
```

### Comparing `pyattest-0.0.8/pyattest.egg-info/SOURCES.txt` & `pyattest-0.0.9/pyattest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyattest-0.0.8/setup.py` & `pyattest-0.0.9/setup.py`

 * *Files identical despite different names*

