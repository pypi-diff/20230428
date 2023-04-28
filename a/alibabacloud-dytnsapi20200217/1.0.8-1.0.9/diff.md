# Comparing `tmp/alibabacloud_dytnsapi20200217-1.0.8.tar.gz` & `tmp/alibabacloud_dytnsapi20200217-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dytnsapi20200217-1.0.8.tar", last modified: Wed Dec 15 02:28:59 2021, max compression
+gzip compressed data, was "dist/alibabacloud_dytnsapi20200217-1.0.9.tar", last modified: Mon Mar 21 03:12:08 2022, max compression
```

## Comparing `alibabacloud_dytnsapi20200217-1.0.8.tar` & `alibabacloud_dytnsapi20200217-1.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-15 02:28:59.000000 alibabacloud_dytnsapi20200217-1.0.8/
--rw-r--r--   0 root         (0) root         (0)      450 2021-12-15 02:28:59.000000 alibabacloud_dytnsapi20200217-1.0.8/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2021-12-15 02:28:59.000000 alibabacloud_dytnsapi20200217-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2021-12-15 02:28:59.000000 alibabacloud_dytnsapi20200217-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2358 2021-12-15 02:28:59.000000 alibabacloud_dytnsapi20200217-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1037 2021-12-15 02:28:59.000000 alibabacloud_dytnsapi20200217-1.0.8/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1122 2021-12-15 02:28:59.000000 alibabacloud_dytnsapi20200217-1.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-15 02:28:59.000000 alibabacloud_dytnsapi20200217-1.0.8/alibabacloud_dytnsapi20200217/
--rw-r--r--   0 root         (0) root         (0)       21 2021-12-15 02:28:59.000000 alibabacloud_dytnsapi20200217-1.0.8/alibabacloud_dytnsapi20200217/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18953 2021-12-15 02:28:59.000000 alibabacloud_dytnsapi20200217-1.0.8/alibabacloud_dytnsapi20200217/client.py
--rw-r--r--   0 root         (0) root         (0)    28789 2021-12-15 02:28:59.000000 alibabacloud_dytnsapi20200217-1.0.8/alibabacloud_dytnsapi20200217/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-15 02:28:59.000000 alibabacloud_dytnsapi20200217-1.0.8/alibabacloud_dytnsapi20200217.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2358 2021-12-15 02:28:59.000000 alibabacloud_dytnsapi20200217-1.0.8/alibabacloud_dytnsapi20200217.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      460 2021-12-15 02:28:59.000000 alibabacloud_dytnsapi20200217-1.0.8/alibabacloud_dytnsapi20200217.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-12-15 02:28:59.000000 alibabacloud_dytnsapi20200217-1.0.8/alibabacloud_dytnsapi20200217.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2021-12-15 02:28:59.000000 alibabacloud_dytnsapi20200217-1.0.8/alibabacloud_dytnsapi20200217.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2021-12-15 02:28:59.000000 alibabacloud_dytnsapi20200217-1.0.8/alibabacloud_dytnsapi20200217.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2021-12-15 02:28:59.000000 alibabacloud_dytnsapi20200217-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2635 2021-12-15 02:28:59.000000 alibabacloud_dytnsapi20200217-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-21 03:12:08.000000 alibabacloud_dytnsapi20200217-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)      519 2022-03-21 03:12:07.000000 alibabacloud_dytnsapi20200217-1.0.9/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2022-03-21 03:12:07.000000 alibabacloud_dytnsapi20200217-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2022-03-21 03:12:07.000000 alibabacloud_dytnsapi20200217-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2358 2022-03-21 03:12:08.000000 alibabacloud_dytnsapi20200217-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1037 2022-03-21 03:12:07.000000 alibabacloud_dytnsapi20200217-1.0.9/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1122 2022-03-21 03:12:07.000000 alibabacloud_dytnsapi20200217-1.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-21 03:12:08.000000 alibabacloud_dytnsapi20200217-1.0.9/alibabacloud_dytnsapi20200217/
+-rw-r--r--   0 root         (0) root         (0)       21 2022-03-21 03:12:07.000000 alibabacloud_dytnsapi20200217-1.0.9/alibabacloud_dytnsapi20200217/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26409 2022-03-21 03:12:07.000000 alibabacloud_dytnsapi20200217-1.0.9/alibabacloud_dytnsapi20200217/client.py
+-rw-r--r--   0 root         (0) root         (0)    34192 2022-03-21 03:12:07.000000 alibabacloud_dytnsapi20200217-1.0.9/alibabacloud_dytnsapi20200217/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-21 03:12:08.000000 alibabacloud_dytnsapi20200217-1.0.9/alibabacloud_dytnsapi20200217.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2358 2022-03-21 03:12:07.000000 alibabacloud_dytnsapi20200217-1.0.9/alibabacloud_dytnsapi20200217.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      460 2022-03-21 03:12:07.000000 alibabacloud_dytnsapi20200217-1.0.9/alibabacloud_dytnsapi20200217.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-03-21 03:12:07.000000 alibabacloud_dytnsapi20200217-1.0.9/alibabacloud_dytnsapi20200217.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2022-03-21 03:12:07.000000 alibabacloud_dytnsapi20200217-1.0.9/alibabacloud_dytnsapi20200217.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2022-03-21 03:12:07.000000 alibabacloud_dytnsapi20200217-1.0.9/alibabacloud_dytnsapi20200217.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2022-03-21 03:12:08.000000 alibabacloud_dytnsapi20200217-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2635 2022-03-21 03:12:07.000000 alibabacloud_dytnsapi20200217-1.0.9/setup.py
```

### Comparing `alibabacloud_dytnsapi20200217-1.0.8/LICENSE` & `alibabacloud_dytnsapi20200217-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dytnsapi20200217-1.0.8/PKG-INFO` & `alibabacloud_dytnsapi20200217-1.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dytnsapi20200217
-Version: 1.0.8
+Version: 1.0.9
 Summary: Alibaba Cloud Dytnsapi (20200217) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dytnsapi20200217-1.0.8/README-CN.md` & `alibabacloud_dytnsapi20200217-1.0.9/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dytnsapi20200217-1.0.8/README.md` & `alibabacloud_dytnsapi20200217-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dytnsapi20200217-1.0.8/alibabacloud_dytnsapi20200217/client.py` & `alibabacloud_dytnsapi20200217-1.0.9/alibabacloud_dytnsapi20200217/client.py`

 * *Files 27% similar despite different names*

```diff
@@ -44,19 +44,24 @@
     def describe_empty_number_detect_with_options(
         self,
         request: dytnsapi_20200217_models.DescribeEmptyNumberDetectRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dytnsapi_20200217_models.DescribeEmptyNumberDetectResponse:
         UtilClient.validate_model(request)
         query = {}
-        query['EncryptType'] = request.encrypt_type
-        query['OwnerId'] = request.owner_id
-        query['Phone'] = request.phone
-        query['ResourceOwnerAccount'] = request.resource_owner_account
-        query['ResourceOwnerId'] = request.resource_owner_id
+        if not UtilClient.is_unset(request.encrypt_type):
+            query['EncryptType'] = request.encrypt_type
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.phone):
+            query['Phone'] = request.phone
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
+        if not UtilClient.is_unset(request.resource_owner_id):
+            query['ResourceOwnerId'] = request.resource_owner_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeEmptyNumberDetect',
             version='2020-02-17',
             protocol='HTTPS',
@@ -75,19 +80,24 @@
     async def describe_empty_number_detect_with_options_async(
         self,
         request: dytnsapi_20200217_models.DescribeEmptyNumberDetectRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dytnsapi_20200217_models.DescribeEmptyNumberDetectResponse:
         UtilClient.validate_model(request)
         query = {}
-        query['EncryptType'] = request.encrypt_type
-        query['OwnerId'] = request.owner_id
-        query['Phone'] = request.phone
-        query['ResourceOwnerAccount'] = request.resource_owner_account
-        query['ResourceOwnerId'] = request.resource_owner_id
+        if not UtilClient.is_unset(request.encrypt_type):
+            query['EncryptType'] = request.encrypt_type
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.phone):
+            query['Phone'] = request.phone
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
+        if not UtilClient.is_unset(request.resource_owner_id):
+            query['ResourceOwnerId'] = request.resource_owner_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribeEmptyNumberDetect',
             version='2020-02-17',
             protocol='HTTPS',
@@ -120,22 +130,30 @@
     def describe_phone_number_analysis_with_options(
         self,
         request: dytnsapi_20200217_models.DescribePhoneNumberAnalysisRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dytnsapi_20200217_models.DescribePhoneNumberAnalysisResponse:
         UtilClient.validate_model(request)
         query = {}
-        query['AuthCode'] = request.auth_code
-        query['InputNumber'] = request.input_number
-        query['Mask'] = request.mask
-        query['NumberType'] = request.number_type
-        query['OwnerId'] = request.owner_id
-        query['Rate'] = request.rate
-        query['ResourceOwnerAccount'] = request.resource_owner_account
-        query['ResourceOwnerId'] = request.resource_owner_id
+        if not UtilClient.is_unset(request.auth_code):
+            query['AuthCode'] = request.auth_code
+        if not UtilClient.is_unset(request.input_number):
+            query['InputNumber'] = request.input_number
+        if not UtilClient.is_unset(request.mask):
+            query['Mask'] = request.mask
+        if not UtilClient.is_unset(request.number_type):
+            query['NumberType'] = request.number_type
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.rate):
+            query['Rate'] = request.rate
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
+        if not UtilClient.is_unset(request.resource_owner_id):
+            query['ResourceOwnerId'] = request.resource_owner_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribePhoneNumberAnalysis',
             version='2020-02-17',
             protocol='HTTPS',
@@ -154,22 +172,30 @@
     async def describe_phone_number_analysis_with_options_async(
         self,
         request: dytnsapi_20200217_models.DescribePhoneNumberAnalysisRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dytnsapi_20200217_models.DescribePhoneNumberAnalysisResponse:
         UtilClient.validate_model(request)
         query = {}
-        query['AuthCode'] = request.auth_code
-        query['InputNumber'] = request.input_number
-        query['Mask'] = request.mask
-        query['NumberType'] = request.number_type
-        query['OwnerId'] = request.owner_id
-        query['Rate'] = request.rate
-        query['ResourceOwnerAccount'] = request.resource_owner_account
-        query['ResourceOwnerId'] = request.resource_owner_id
+        if not UtilClient.is_unset(request.auth_code):
+            query['AuthCode'] = request.auth_code
+        if not UtilClient.is_unset(request.input_number):
+            query['InputNumber'] = request.input_number
+        if not UtilClient.is_unset(request.mask):
+            query['Mask'] = request.mask
+        if not UtilClient.is_unset(request.number_type):
+            query['NumberType'] = request.number_type
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.rate):
+            query['Rate'] = request.rate
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
+        if not UtilClient.is_unset(request.resource_owner_id):
+            query['ResourceOwnerId'] = request.resource_owner_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribePhoneNumberAnalysis',
             version='2020-02-17',
             protocol='HTTPS',
@@ -202,18 +228,22 @@
     def describe_phone_number_attribute_with_options(
         self,
         request: dytnsapi_20200217_models.DescribePhoneNumberAttributeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dytnsapi_20200217_models.DescribePhoneNumberAttributeResponse:
         UtilClient.validate_model(request)
         query = {}
-        query['OwnerId'] = request.owner_id
-        query['PhoneNumber'] = request.phone_number
-        query['ResourceOwnerAccount'] = request.resource_owner_account
-        query['ResourceOwnerId'] = request.resource_owner_id
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.phone_number):
+            query['PhoneNumber'] = request.phone_number
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
+        if not UtilClient.is_unset(request.resource_owner_id):
+            query['ResourceOwnerId'] = request.resource_owner_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribePhoneNumberAttribute',
             version='2020-02-17',
             protocol='HTTPS',
@@ -232,18 +262,22 @@
     async def describe_phone_number_attribute_with_options_async(
         self,
         request: dytnsapi_20200217_models.DescribePhoneNumberAttributeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dytnsapi_20200217_models.DescribePhoneNumberAttributeResponse:
         UtilClient.validate_model(request)
         query = {}
-        query['OwnerId'] = request.owner_id
-        query['PhoneNumber'] = request.phone_number
-        query['ResourceOwnerAccount'] = request.resource_owner_account
-        query['ResourceOwnerId'] = request.resource_owner_id
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.phone_number):
+            query['PhoneNumber'] = request.phone_number
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
+        if not UtilClient.is_unset(request.resource_owner_id):
+            query['ResourceOwnerId'] = request.resource_owner_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribePhoneNumberAttribute',
             version='2020-02-17',
             protocol='HTTPS',
@@ -269,26 +303,125 @@
     async def describe_phone_number_attribute_async(
         self,
         request: dytnsapi_20200217_models.DescribePhoneNumberAttributeRequest,
     ) -> dytnsapi_20200217_models.DescribePhoneNumberAttributeResponse:
         runtime = util_models.RuntimeOptions()
         return await self.describe_phone_number_attribute_with_options_async(request, runtime)
 
+    def describe_phone_number_online_time_with_options(
+        self,
+        request: dytnsapi_20200217_models.DescribePhoneNumberOnlineTimeRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dytnsapi_20200217_models.DescribePhoneNumberOnlineTimeResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.auth_code):
+            query['AuthCode'] = request.auth_code
+        if not UtilClient.is_unset(request.carrier):
+            query['Carrier'] = request.carrier
+        if not UtilClient.is_unset(request.input_number):
+            query['InputNumber'] = request.input_number
+        if not UtilClient.is_unset(request.mask):
+            query['Mask'] = request.mask
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
+        if not UtilClient.is_unset(request.resource_owner_id):
+            query['ResourceOwnerId'] = request.resource_owner_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribePhoneNumberOnlineTime',
+            version='2020-02-17',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dytnsapi_20200217_models.DescribePhoneNumberOnlineTimeResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def describe_phone_number_online_time_with_options_async(
+        self,
+        request: dytnsapi_20200217_models.DescribePhoneNumberOnlineTimeRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> dytnsapi_20200217_models.DescribePhoneNumberOnlineTimeResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.auth_code):
+            query['AuthCode'] = request.auth_code
+        if not UtilClient.is_unset(request.carrier):
+            query['Carrier'] = request.carrier
+        if not UtilClient.is_unset(request.input_number):
+            query['InputNumber'] = request.input_number
+        if not UtilClient.is_unset(request.mask):
+            query['Mask'] = request.mask
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
+        if not UtilClient.is_unset(request.resource_owner_id):
+            query['ResourceOwnerId'] = request.resource_owner_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribePhoneNumberOnlineTime',
+            version='2020-02-17',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dytnsapi_20200217_models.DescribePhoneNumberOnlineTimeResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def describe_phone_number_online_time(
+        self,
+        request: dytnsapi_20200217_models.DescribePhoneNumberOnlineTimeRequest,
+    ) -> dytnsapi_20200217_models.DescribePhoneNumberOnlineTimeResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.describe_phone_number_online_time_with_options(request, runtime)
+
+    async def describe_phone_number_online_time_async(
+        self,
+        request: dytnsapi_20200217_models.DescribePhoneNumberOnlineTimeRequest,
+    ) -> dytnsapi_20200217_models.DescribePhoneNumberOnlineTimeResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.describe_phone_number_online_time_with_options_async(request, runtime)
+
     def describe_phone_number_resale_with_options(
         self,
         request: dytnsapi_20200217_models.DescribePhoneNumberResaleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dytnsapi_20200217_models.DescribePhoneNumberResaleResponse:
         UtilClient.validate_model(request)
         query = {}
-        query['OwnerId'] = request.owner_id
-        query['PhoneNumber'] = request.phone_number
-        query['ResourceOwnerAccount'] = request.resource_owner_account
-        query['ResourceOwnerId'] = request.resource_owner_id
-        query['Since'] = request.since
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.phone_number):
+            query['PhoneNumber'] = request.phone_number
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
+        if not UtilClient.is_unset(request.resource_owner_id):
+            query['ResourceOwnerId'] = request.resource_owner_id
+        if not UtilClient.is_unset(request.since):
+            query['Since'] = request.since
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribePhoneNumberResale',
             version='2020-02-17',
             protocol='HTTPS',
@@ -307,19 +440,24 @@
     async def describe_phone_number_resale_with_options_async(
         self,
         request: dytnsapi_20200217_models.DescribePhoneNumberResaleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dytnsapi_20200217_models.DescribePhoneNumberResaleResponse:
         UtilClient.validate_model(request)
         query = {}
-        query['OwnerId'] = request.owner_id
-        query['PhoneNumber'] = request.phone_number
-        query['ResourceOwnerAccount'] = request.resource_owner_account
-        query['ResourceOwnerId'] = request.resource_owner_id
-        query['Since'] = request.since
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.phone_number):
+            query['PhoneNumber'] = request.phone_number
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
+        if not UtilClient.is_unset(request.resource_owner_id):
+            query['ResourceOwnerId'] = request.resource_owner_id
+        if not UtilClient.is_unset(request.since):
+            query['Since'] = request.since
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribePhoneNumberResale',
             version='2020-02-17',
             protocol='HTTPS',
@@ -352,18 +490,22 @@
     def describe_phone_number_status_with_options(
         self,
         request: dytnsapi_20200217_models.DescribePhoneNumberStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dytnsapi_20200217_models.DescribePhoneNumberStatusResponse:
         UtilClient.validate_model(request)
         query = {}
-        query['OwnerId'] = request.owner_id
-        query['PhoneNumber'] = request.phone_number
-        query['ResourceOwnerAccount'] = request.resource_owner_account
-        query['ResourceOwnerId'] = request.resource_owner_id
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.phone_number):
+            query['PhoneNumber'] = request.phone_number
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
+        if not UtilClient.is_unset(request.resource_owner_id):
+            query['ResourceOwnerId'] = request.resource_owner_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribePhoneNumberStatus',
             version='2020-02-17',
             protocol='HTTPS',
@@ -382,18 +524,22 @@
     async def describe_phone_number_status_with_options_async(
         self,
         request: dytnsapi_20200217_models.DescribePhoneNumberStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dytnsapi_20200217_models.DescribePhoneNumberStatusResponse:
         UtilClient.validate_model(request)
         query = {}
-        query['OwnerId'] = request.owner_id
-        query['PhoneNumber'] = request.phone_number
-        query['ResourceOwnerAccount'] = request.resource_owner_account
-        query['ResourceOwnerId'] = request.resource_owner_id
+        if not UtilClient.is_unset(request.owner_id):
+            query['OwnerId'] = request.owner_id
+        if not UtilClient.is_unset(request.phone_number):
+            query['PhoneNumber'] = request.phone_number
+        if not UtilClient.is_unset(request.resource_owner_account):
+            query['ResourceOwnerAccount'] = request.resource_owner_account
+        if not UtilClient.is_unset(request.resource_owner_id):
+            query['ResourceOwnerId'] = request.resource_owner_id
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='DescribePhoneNumberStatus',
             version='2020-02-17',
             protocol='HTTPS',
```

### Comparing `alibabacloud_dytnsapi20200217-1.0.8/alibabacloud_dytnsapi20200217/models.py` & `alibabacloud_dytnsapi20200217-1.0.9/alibabacloud_dytnsapi20200217/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -552,14 +552,188 @@
             self.headers = m.get('headers')
         if m.get('body') is not None:
             temp_model = DescribePhoneNumberAttributeResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DescribePhoneNumberOnlineTimeRequest(TeaModel):
+    def __init__(
+        self,
+        auth_code: str = None,
+        carrier: str = None,
+        input_number: str = None,
+        mask: str = None,
+        owner_id: int = None,
+        resource_owner_account: str = None,
+        resource_owner_id: int = None,
+    ):
+        self.auth_code = auth_code
+        self.carrier = carrier
+        self.input_number = input_number
+        self.mask = mask
+        self.owner_id = owner_id
+        self.resource_owner_account = resource_owner_account
+        self.resource_owner_id = resource_owner_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_code is not None:
+            result['AuthCode'] = self.auth_code
+        if self.carrier is not None:
+            result['Carrier'] = self.carrier
+        if self.input_number is not None:
+            result['InputNumber'] = self.input_number
+        if self.mask is not None:
+            result['Mask'] = self.mask
+        if self.owner_id is not None:
+            result['OwnerId'] = self.owner_id
+        if self.resource_owner_account is not None:
+            result['ResourceOwnerAccount'] = self.resource_owner_account
+        if self.resource_owner_id is not None:
+            result['ResourceOwnerId'] = self.resource_owner_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AuthCode') is not None:
+            self.auth_code = m.get('AuthCode')
+        if m.get('Carrier') is not None:
+            self.carrier = m.get('Carrier')
+        if m.get('InputNumber') is not None:
+            self.input_number = m.get('InputNumber')
+        if m.get('Mask') is not None:
+            self.mask = m.get('Mask')
+        if m.get('OwnerId') is not None:
+            self.owner_id = m.get('OwnerId')
+        if m.get('ResourceOwnerAccount') is not None:
+            self.resource_owner_account = m.get('ResourceOwnerAccount')
+        if m.get('ResourceOwnerId') is not None:
+            self.resource_owner_id = m.get('ResourceOwnerId')
+        return self
+
+
+class DescribePhoneNumberOnlineTimeResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        verify_result: str = None,
+    ):
+        self.verify_result = verify_result
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.verify_result is not None:
+            result['VerifyResult'] = self.verify_result
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('VerifyResult') is not None:
+            self.verify_result = m.get('VerifyResult')
+        return self
+
+
+class DescribePhoneNumberOnlineTimeResponseBody(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        data: DescribePhoneNumberOnlineTimeResponseBodyData = None,
+        message: str = None,
+        request_id: str = None,
+    ):
+        self.code = code
+        self.data = data
+        self.message = message
+        self.request_id = request_id
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code is not None:
+            result['Code'] = self.code
+        if self.data is not None:
+            result['Data'] = self.data.to_map()
+        if self.message is not None:
+            result['Message'] = self.message
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Code') is not None:
+            self.code = m.get('Code')
+        if m.get('Data') is not None:
+            temp_model = DescribePhoneNumberOnlineTimeResponseBodyData()
+            self.data = temp_model.from_map(m['Data'])
+        if m.get('Message') is not None:
+            self.message = m.get('Message')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class DescribePhoneNumberOnlineTimeResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        body: DescribePhoneNumberOnlineTimeResponseBody = None,
+    ):
+        self.headers = headers
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.body, 'body')
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('body') is not None:
+            temp_model = DescribePhoneNumberOnlineTimeResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class DescribePhoneNumberResaleRequest(TeaModel):
     def __init__(
         self,
         owner_id: int = None,
         phone_number: str = None,
         resource_owner_account: str = None,
         resource_owner_id: int = None,
```

### Comparing `alibabacloud_dytnsapi20200217-1.0.8/alibabacloud_dytnsapi20200217.egg-info/PKG-INFO` & `alibabacloud_dytnsapi20200217-1.0.9/alibabacloud_dytnsapi20200217.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dytnsapi20200217
-Version: 1.0.8
+Version: 1.0.9
 Summary: Alibaba Cloud Dytnsapi (20200217) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dytnsapi20200217-1.0.8/setup.py` & `alibabacloud_dytnsapi20200217-1.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dytnsapi20200217.
 
-Created on 15/12/2021
+Created on 21/03/2022
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dytnsapi20200217"
 NAME = "alibabacloud_dytnsapi20200217" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Dytnsapi (20200217) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "alibabacloud_tea_util>=0.3.5, <1.0.0",
-    "alibabacloud_tea_openapi>=0.3.0, <1.0.0",
+    "alibabacloud_tea_openapi>=0.3.1, <1.0.0",
     "alibabacloud_openapi_util>=0.1.6, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
```

