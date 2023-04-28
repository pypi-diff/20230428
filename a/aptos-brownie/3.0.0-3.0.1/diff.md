# Comparing `tmp/aptos_brownie-3.0.0-py3-none-any.whl.zip` & `tmp/aptos_brownie-3.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 7462 bytes, number of entries: 5
--rw-r--r--  2.0 unx    33691 b- defN 23-Apr-12 05:13 aptos_brownie.py
--rw-r--r--  2.0 unx      891 b- defN 23-Apr-12 05:14 aptos_brownie-3.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-12 05:14 aptos_brownie-3.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 23-Apr-12 05:14 aptos_brownie-3.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      395 b- defN 23-Apr-12 05:14 aptos_brownie-3.0.0.dist-info/RECORD
-5 files, 35083 bytes uncompressed, 6724 bytes compressed:  80.8%
+Zip file size: 7546 bytes, number of entries: 5
+-rw-r--r--  2.0 unx    34123 b- defN 23-Apr-28 08:31 aptos_brownie.py
+-rw-r--r--  2.0 unx      891 b- defN 23-Apr-28 08:32 aptos_brownie-3.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-28 08:32 aptos_brownie-3.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 23-Apr-28 08:32 aptos_brownie-3.0.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      395 b- defN 23-Apr-28 08:32 aptos_brownie-3.0.1.dist-info/RECORD
+5 files, 35515 bytes uncompressed, 6808 bytes compressed:  80.8%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: aptos_brownie.py
 Comment: 
 
-Filename: aptos_brownie-3.0.0.dist-info/METADATA
+Filename: aptos_brownie-3.0.1.dist-info/METADATA
 Comment: 
 
-Filename: aptos_brownie-3.0.0.dist-info/WHEEL
+Filename: aptos_brownie-3.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: aptos_brownie-3.0.0.dist-info/top_level.txt
+Filename: aptos_brownie-3.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: aptos_brownie-3.0.0.dist-info/RECORD
+Filename: aptos_brownie-3.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aptos_brownie.py

```diff
@@ -754,25 +754,36 @@
                          ):
         if isinstance(account_addr, str):
             account_addr = AccountAddress.from_hex(account_addr)
         return self.rest_client.account_resource(account_addr, resource_type)
 
     def account_resources(self,
                           account_addr: Union[str, AccountAddress],
+                          limit=None
                           ):
         if isinstance(account_addr, str):
             account_addr = AccountAddress.from_hex(account_addr)
-        response = self.rest_client.client.get(
-            f"{self.rest_client.base_url}/accounts/{account_addr}/resources"
-        )
+        if limit is None:
+            response = self.rest_client.client.get(
+                f"{self.rest_client.base_url}/accounts/{account_addr}/resources"
+            )
+            is_limit = False
+        else:
+            response = self.rest_client.client.get(
+                f"{self.rest_client.base_url}/accounts/{account_addr}/resources?limit={int(limit)}"
+            )
+            is_limit = True
         if response.status_code == 404:
             return None
         if response.status_code >= 400:
             raise ApiError(f"{response.text} - {account_addr}", response.status_code)
-        return response.json()
+        if is_limit:
+            return response.json(), response.headers.get('x-aptos-cursor', None)
+        else:
+            return response.json()
 
     def register_coin(self, asset_id):
         """Register the receiver account to receive transfers for the new coin."""
 
         payload = EntryFunction.natural(
             "0x1::managed_coin",
             "register",
```

## Comparing `aptos_brownie-3.0.0.dist-info/METADATA` & `aptos_brownie-3.0.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aptos-brownie
-Version: 3.0.0
+Version: 3.0.1
 Summary: Aptos Package Tool
 Home-page: https://github.com/OmniBTC/OmniSwap/blob/main/utils
 Author: DaiWei
 Author-email: dw1253464613@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

