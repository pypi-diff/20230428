# Comparing `tmp/xia_user-0.1.8-cp39-none-win_amd64.whl.zip` & `tmp/xia_user-0.1.9-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 427046 bytes, number of entries: 9
--rw-r--r--  2.0 unx      330 b- defN 23-Mar-27 19:38 xia_user/__init__.py
--rw-r--r--  2.0 unx   256000 b- defN 23-Mar-27 19:42 xia_user/messages.cp39-win_amd64.pyd
--rw-r--r--  2.0 unx   379392 b- defN 23-Mar-27 19:41 xia_user/role_matrix.cp39-win_amd64.pyd
--rw-r--r--  2.0 unx   449536 b- defN 23-Mar-27 19:40 xia_user/user.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      152 b- defN 23-Mar-27 19:42 xia_user-0.1.8.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      713 b- defN 23-Mar-27 19:42 xia_user-0.1.8.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Mar-27 19:42 xia_user-0.1.8.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Mar-27 19:42 xia_user-0.1.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      752 b- defN 23-Mar-27 19:42 xia_user-0.1.8.dist-info/RECORD
-9 files, 1086983 bytes uncompressed, 425750 bytes compressed:  60.8%
+Zip file size: 427488 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      330 b- defN 23-Mar-27 19:47 xia_user/__init__.py
+-rw-r--r--  2.0 unx   256000 b- defN 23-Mar-27 19:52 xia_user/messages.cp39-win_amd64.pyd
+-rw-r--r--  2.0 unx   379392 b- defN 23-Mar-27 19:51 xia_user/role_matrix.cp39-win_amd64.pyd
+-rw-r--r--  2.0 unx   451072 b- defN 23-Mar-27 19:50 xia_user/user.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 unx      152 b- defN 23-Mar-27 19:52 xia_user-0.1.9.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      713 b- defN 23-Mar-27 19:52 xia_user-0.1.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Mar-27 19:52 xia_user-0.1.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Mar-27 19:52 xia_user-0.1.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      752 b- defN 23-Mar-27 19:52 xia_user-0.1.9.dist-info/RECORD
+9 files, 1088519 bytes uncompressed, 426192 bytes compressed:  60.8%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: xia_user/role_matrix.cp39-win_amd64.pyd
 Comment: 
 
 Filename: xia_user/user.cp39-win_amd64.pyd
 Comment: 
 
-Filename: xia_user-0.1.8.dist-info/LICENSE.txt
+Filename: xia_user-0.1.9.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_user-0.1.8.dist-info/METADATA
+Filename: xia_user-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: xia_user-0.1.8.dist-info/WHEEL
+Filename: xia_user-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: xia_user-0.1.8.dist-info/top_level.txt
+Filename: xia_user-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_user-0.1.8.dist-info/RECORD
+Filename: xia_user-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_user/__init__.py

```diff
@@ -6,8 +6,8 @@
 __all__ = [
     "UserBasicInfo", "AppNameField",
     "User", "UserRoles", "ApiInfo", "ApiKey",
     "RoleMatrix", "RoleContent",
 ]
 
 
-__version__ = "0.1.8"
+__version__ = "0.1.9"
```

## Comparing `xia_user-0.1.8.dist-info/METADATA` & `xia_user-0.1.9.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-user
-Version: 0.1.8
+Version: 0.1.9
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-user/0.1.8/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-user/0.1.9/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

