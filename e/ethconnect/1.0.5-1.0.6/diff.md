# Comparing `tmp/ethconnect-1.0.5.tar.gz` & `tmp/ethconnect-1.0.6.tar.gz`

## Comparing `ethconnect-1.0.5.tar` & `ethconnect-1.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 ethconnect-1.0.5/src/ethconnect/Account.py
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 ethconnect-1.0.5/src/ethconnect/EllipticCurve.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 ethconnect-1.0.5/src/ethconnect/EthAccount.py
--rw-r--r--   0        0        0    11003 2020-02-02 00:00:00.000000 ethconnect-1.0.5/src/ethconnect/EthConnect.py
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 ethconnect-1.0.5/src/ethconnect/EthTransaction.py
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 ethconnect-1.0.5/src/ethconnect/Keyring.py
--rw-r--r--   0        0        0    12153 2020-02-02 00:00:00.000000 ethconnect-1.0.5/src/ethconnect/ZymbitEthKeyring.py
--rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 ethconnect-1.0.5/src/ethconnect/ZymbitKeyringManager.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 ethconnect-1.0.5/src/ethconnect/__init__.py
--rw-r--r--   0        0        0    11245 2020-02-02 00:00:00.000000 ethconnect-1.0.5/tests/ABI.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ethconnect-1.0.5/tests/__init__.py
--rw-r--r--   0        0        0    17056 2020-02-02 00:00:00.000000 ethconnect-1.0.5/tests/bytecode.txt
--rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 ethconnect-1.0.5/tests/test_eth_account.py
--rw-r--r--   0        0        0     3947 2020-02-02 00:00:00.000000 ethconnect-1.0.5/tests/test_eth_connect.py
--rw-r--r--   0        0        0     4203 2020-02-02 00:00:00.000000 ethconnect-1.0.5/tests/test_zymbit_eth_keyring.py
--rw-r--r--   0        0        0     3175 2020-02-02 00:00:00.000000 ethconnect-1.0.5/tests/test_zymbit_keyring_manager.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 ethconnect-1.0.5/.gitignore
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 ethconnect-1.0.5/LICENSE.md
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 ethconnect-1.0.5/README.md
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 ethconnect-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 ethconnect-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 ethconnect-1.0.6/src/ethconnect/Account.py
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 ethconnect-1.0.6/src/ethconnect/EllipticCurve.py
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 ethconnect-1.0.6/src/ethconnect/EthAccount.py
+-rw-r--r--   0        0        0    11003 2020-02-02 00:00:00.000000 ethconnect-1.0.6/src/ethconnect/EthConnect.py
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 ethconnect-1.0.6/src/ethconnect/EthTransaction.py
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 ethconnect-1.0.6/src/ethconnect/Keyring.py
+-rw-r--r--   0        0        0    12153 2020-02-02 00:00:00.000000 ethconnect-1.0.6/src/ethconnect/ZymbitEthKeyring.py
+-rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 ethconnect-1.0.6/src/ethconnect/ZymbitKeyringManager.py
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 ethconnect-1.0.6/src/ethconnect/__init__.py
+-rw-r--r--   0        0        0    11245 2020-02-02 00:00:00.000000 ethconnect-1.0.6/tests/ABI.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ethconnect-1.0.6/tests/__init__.py
+-rw-r--r--   0        0        0    17056 2020-02-02 00:00:00.000000 ethconnect-1.0.6/tests/bytecode.txt
+-rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 ethconnect-1.0.6/tests/test_eth_account.py
+-rw-r--r--   0        0        0     3856 2020-02-02 00:00:00.000000 ethconnect-1.0.6/tests/test_eth_connect.py
+-rw-r--r--   0        0        0     4068 2020-02-02 00:00:00.000000 ethconnect-1.0.6/tests/test_zymbit_eth_keyring.py
+-rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 ethconnect-1.0.6/tests/test_zymbit_keyring_manager.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 ethconnect-1.0.6/.gitignore
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 ethconnect-1.0.6/LICENSE.md
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 ethconnect-1.0.6/README.md
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 ethconnect-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 ethconnect-1.0.6/PKG-INFO
```

### Comparing `ethconnect-1.0.5/src/ethconnect/EthAccount.py` & `ethconnect-1.0.6/src/ethconnect/EthAccount.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 
 class EthAccount(Account):
     def __init__(self, path: str, address: str, slot: int) -> None:
         self.path = path
         self.address = address
         self.slot = slot
 
+        if not self.is_valid_account():
+            raise ValueError("Must provide a valid path, address, and slot")
+
     def serialize(self) -> dict:
         return {
             "path": self.path,
             "address": self.address,
             "slot": self.slot
         }
```

### Comparing `ethconnect-1.0.5/src/ethconnect/EthConnect.py` & `ethconnect-1.0.6/src/ethconnect/EthConnect.py`

 * *Files identical despite different names*

### Comparing `ethconnect-1.0.5/src/ethconnect/EthTransaction.py` & `ethconnect-1.0.6/src/ethconnect/EthTransaction.py`

 * *Files identical despite different names*

### Comparing `ethconnect-1.0.5/src/ethconnect/Keyring.py` & `ethconnect-1.0.6/src/ethconnect/Keyring.py`

 * *Files identical despite different names*

### Comparing `ethconnect-1.0.5/src/ethconnect/ZymbitEthKeyring.py` & `ethconnect-1.0.6/src/ethconnect/ZymbitEthKeyring.py`

 * *Files identical despite different names*

### Comparing `ethconnect-1.0.5/src/ethconnect/ZymbitKeyringManager.py` & `ethconnect-1.0.6/src/ethconnect/ZymbitKeyringManager.py`

 * *Files identical despite different names*

### Comparing `ethconnect-1.0.5/src/ethconnect/__init__.py` & `ethconnect-1.0.6/src/ethconnect/__init__.py`

 * *Files identical despite different names*

### Comparing `ethconnect-1.0.5/tests/ABI.json` & `ethconnect-1.0.6/tests/ABI.json`

 * *Files identical despite different names*

### Comparing `ethconnect-1.0.5/tests/bytecode.txt` & `ethconnect-1.0.6/tests/bytecode.txt`

 * *Files identical despite different names*

### Comparing `ethconnect-1.0.5/tests/test_eth_account.py` & `ethconnect-1.0.6/tests/test_eth_account.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import unittest
 from unittest.mock import MagicMock
 import sys
-sys.path.append('../src/ethconnect')
-from Account import Account
-from EthAccount import EthAccount
+from ethconnect import Account, EthAccount
 import zymkey
 import binascii
 from web3 import Web3
 
 class TestEthAccount(unittest.TestCase):
 
     def test_init(self):
```

### Comparing `ethconnect-1.0.5/tests/test_eth_connect.py` & `ethconnect-1.0.6/tests/test_eth_connect.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 import unittest
 from unittest.mock import Mock
 import sys
 import zymkey
 import time
-sys.path.append('../src/ethconnect')
-from EthConnect import EthConnect
-from EthTransaction import EthTransaction, SignedEthTransaction
-from ZymbitEthKeyring import ZymbitEthKeyring
+from ethconnect import EthConnect, EthTransaction, SignedEthTransaction, ZymbitEthKeyring
 from Crypto.Hash import keccak, SHA256
 
 class TestEthConnect(unittest.TestCase):
 
     @classmethod
     def setUpClass(cls):
         slots: list[int] = zymkey.client.get_slot_alloc_list()[0]
```

### Comparing `ethconnect-1.0.5/tests/test_zymbit_eth_keyring.py` & `ethconnect-1.0.6/tests/test_zymbit_eth_keyring.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,14 @@
 import unittest
 from unittest.mock import patch
 from Crypto.Hash import SHA256, keccak
 from typing import List
 import sys
 import zymkey
-sys.path.append('../src/ethconnect')
-from Keyring import Keyring
-from EthAccount import EthAccount
-from EllipticCurve import EllipticCurve
-from EthTransaction import EthTransaction, SignedEthTransaction
-from ZymbitEthKeyring import ZymbitEthKeyring
+from ethconnect import Keyring, EthAccount, EllipticCurve, EthTransaction, SignedEthTransaction, ZymbitEthKeyring
 
 
 class TestZymbitEthKeyring(unittest.TestCase):
 
     @classmethod
     def setUpClass(cls):
         slots: list[int] = zymkey.client.get_slot_alloc_list()[0]
```

### Comparing `ethconnect-1.0.5/tests/test_zymbit_keyring_manager.py` & `ethconnect-1.0.6/tests/test_zymbit_keyring_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 import unittest
 from typing import Type
 import zymkey
 import sys
-sys.path.append('../src/ethconnect')
-from Keyring import Keyring
-from ZymbitEthKeyring import ZymbitEthKeyring
-from ZymbitKeyringManager import ZymbitKeyringManager
+from ethconnect import Keyring, ZymbitEthKeyring, ZymbitKeyringManager
 
 
 class ZymbitEthKeyringTest(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
         # create a zymbit keyring manager instance
         cls.keyring_manager = ZymbitKeyringManager()
```

### Comparing `ethconnect-1.0.5/LICENSE.md` & `ethconnect-1.0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ethconnect-1.0.5/README.md` & `ethconnect-1.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# ETH-Connect Python API
+# ETH-Connect Python SDK
 
 ## Overview
 
-Ethereum accounts, signatures, and transactions have an additional layer of complexity over traditional cryptographic keys and signatures. [Zymbit](https://www.zymbit.com/)'s ETH-Connect API aims to abstract away this complexity, enabling you to seamlessly integrate with Ethereum and EVM compatible chains without having to deal with their technical intricacies.
+Ethereum accounts, signatures, and transactions have an additional layer of complexity over traditional cryptographic keys and signatures. [Zymbit](https://www.zymbit.com/)'s ETH-Connect SDK aims to abstract away this complexity, enabling you to seamlessly integrate with Ethereum and EVM compatible chains without having to deal with their technical intricacies.
 
 **NOTE:** Only compatible with [HSM6](https://www.zymbit.com/hsm6/), [SCM](https://www.zymbit.com/scm/), and [SEN](https://www.zymbit.com/secure-compute-node/)
 
 ## Installation
 
 ```
 pip install ethconnect
```

### Comparing `ethconnect-1.0.5/pyproject.toml` & `ethconnect-1.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ethconnect"
-version = "1.0.5"
+version = "1.0.6"
 authors = [
   { name="Shivaansh Kapoor", email="shiv@zymbit.com" },
 ]
-description = "ETH-Connect Python API"
+description = "ETH-Connect Python SDK"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `ethconnect-1.0.5/PKG-INFO` & `ethconnect-1.0.6/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: ethconnect
-Version: 1.0.5
-Summary: ETH-Connect Python API
+Version: 1.0.6
+Summary: ETH-Connect Python SDK
 Project-URL: Homepage, https://github.com/Zymbit-Wallet/ETH-Connect-PY
 Author-email: Shivaansh Kapoor <shiv@zymbit.com>
 License-File: LICENSE.md
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
-# ETH-Connect Python API
+# ETH-Connect Python SDK
 
 ## Overview
 
-Ethereum accounts, signatures, and transactions have an additional layer of complexity over traditional cryptographic keys and signatures. [Zymbit](https://www.zymbit.com/)'s ETH-Connect API aims to abstract away this complexity, enabling you to seamlessly integrate with Ethereum and EVM compatible chains without having to deal with their technical intricacies.
+Ethereum accounts, signatures, and transactions have an additional layer of complexity over traditional cryptographic keys and signatures. [Zymbit](https://www.zymbit.com/)'s ETH-Connect SDK aims to abstract away this complexity, enabling you to seamlessly integrate with Ethereum and EVM compatible chains without having to deal with their technical intricacies.
 
 **NOTE:** Only compatible with [HSM6](https://www.zymbit.com/hsm6/), [SCM](https://www.zymbit.com/scm/), and [SEN](https://www.zymbit.com/secure-compute-node/)
 
 ## Installation
 
 ```
 pip install ethconnect
```

