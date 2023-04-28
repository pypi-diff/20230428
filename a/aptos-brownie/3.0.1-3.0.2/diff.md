# Comparing `tmp/aptos_brownie-3.0.1-py3-none-any.whl.zip` & `tmp/aptos_brownie-3.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 7546 bytes, number of entries: 5
--rw-r--r--  2.0 unx    34123 b- defN 23-Apr-28 08:31 aptos_brownie.py
--rw-r--r--  2.0 unx      891 b- defN 23-Apr-28 08:32 aptos_brownie-3.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-28 08:32 aptos_brownie-3.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 23-Apr-28 08:32 aptos_brownie-3.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      395 b- defN 23-Apr-28 08:32 aptos_brownie-3.0.1.dist-info/RECORD
-5 files, 35515 bytes uncompressed, 6808 bytes compressed:  80.8%
+Zip file size: 7612 bytes, number of entries: 5
+-rw-r--r--  2.0 unx    34213 b- defN 23-Apr-28 08:43 aptos_brownie.py
+-rw-r--r--  2.0 unx      911 b- defN 23-Apr-28 09:49 aptos_brownie-3.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-28 09:49 aptos_brownie-3.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 23-Apr-28 09:49 aptos_brownie-3.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      395 b- defN 23-Apr-28 09:49 aptos_brownie-3.0.2.dist-info/RECORD
+5 files, 35625 bytes uncompressed, 6874 bytes compressed:  80.7%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: aptos_brownie.py
 Comment: 
 
-Filename: aptos_brownie-3.0.1.dist-info/METADATA
+Filename: aptos_brownie-3.0.2.dist-info/METADATA
 Comment: 
 
-Filename: aptos_brownie-3.0.1.dist-info/WHEEL
+Filename: aptos_brownie-3.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: aptos_brownie-3.0.1.dist-info/top_level.txt
+Filename: aptos_brownie-3.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: aptos_brownie-3.0.1.dist-info/RECORD
+Filename: aptos_brownie-3.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aptos_brownie.py

```diff
@@ -754,33 +754,41 @@
                          ):
         if isinstance(account_addr, str):
             account_addr = AccountAddress.from_hex(account_addr)
         return self.rest_client.account_resource(account_addr, resource_type)
 
     def account_resources(self,
                           account_addr: Union[str, AccountAddress],
-                          limit=None
+                          limit=None,
+                          cursor=None
                           ):
         if isinstance(account_addr, str):
             account_addr = AccountAddress.from_hex(account_addr)
-        if limit is None:
-            response = self.rest_client.client.get(
-                f"{self.rest_client.base_url}/accounts/{account_addr}/resources"
-            )
-            is_limit = False
-        else:
-            response = self.rest_client.client.get(
-                f"{self.rest_client.base_url}/accounts/{account_addr}/resources?limit={int(limit)}"
-            )
-            is_limit = True
+        data = []
+        is_cursor = False
+        if cursor is not None:
+            data.append(f"start={cursor}")
+            is_cursor = True
+
+        if limit is not None:
+            data.append(f"limit={int(limit)}")
+            is_cursor = True
+
+        if len(data):
+            data = "?" + "&".join(data)
+
+        response = self.rest_client.client.get(
+            f"{self.rest_client.base_url}/accounts/{account_addr}/resources{data}"
+        )
+
         if response.status_code == 404:
             return None
         if response.status_code >= 400:
             raise ApiError(f"{response.text} - {account_addr}", response.status_code)
-        if is_limit:
+        if is_cursor:
             return response.json(), response.headers.get('x-aptos-cursor', None)
         else:
             return response.json()
 
     def register_coin(self, asset_id):
         """Register the receiver account to receive transfers for the new coin."""
```

## Comparing `aptos_brownie-3.0.1.dist-info/METADATA` & `aptos_brownie-3.0.2.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: aptos-brownie
-Version: 3.0.1
+Version: 3.0.2
 Summary: Aptos Package Tool
 Home-page: https://github.com/OmniBTC/OmniSwap/blob/main/utils
 Author: DaiWei
 Author-email: dw1253464613@gmail.com
 License: MIT
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: System :: Logging
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
@@ -19,7 +20,9 @@
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Requires-Dist: aptos-sdk
 Requires-Dist: pyyaml
 Requires-Dist: toml
 
 This is an aptos python tool to quickly implement aptos calls
+
+
```

