# Comparing `tmp/antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.0.tar.gz` & `tmp/antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.0.tar", last modified: Tue Apr 25 09:52:03 2023, max compression
+gzip compressed data, was "dist/antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.1.tar", last modified: Fri Apr 28 10:14:20 2023, max compression
```

## Comparing `antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.0.tar` & `antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 09:52:03.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      600 2023-04-25 09:52:03.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-04-25 09:52:03.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2354 2023-04-25 09:52:03.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      900 2023-04-25 09:52:03.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1086 2023-04-25 09:52:03.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 09:52:03.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.0/antchain_ak_ee637c8293f64104af9686dc12e0cd18.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2354 2023-04-25 09:52:03.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.0/antchain_ak_ee637c8293f64104af9686dc12e0cd18.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      579 2023-04-25 09:52:03.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.0/antchain_ak_ee637c8293f64104af9686dc12e0cd18.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 09:52:03.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.0/antchain_ak_ee637c8293f64104af9686dc12e0cd18.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-04-25 09:52:03.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.0/antchain_ak_ee637c8293f64104af9686dc12e0cd18.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-04-25 09:52:03.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.0/antchain_ak_ee637c8293f64104af9686dc12e0cd18.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 09:52:03.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.0/antchain_sdk_ak_ee637c8293f64104af9686dc12e0cd18/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-25 09:52:03.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.0/antchain_sdk_ak_ee637c8293f64104af9686dc12e0cd18/__init__.py
--rw-r--r--   0 root         (0) root         (0)    47040 2023-04-25 09:52:03.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.0/antchain_sdk_ak_ee637c8293f64104af9686dc12e0cd18/client.py
--rw-r--r--   0 root         (0) root         (0)    43969 2023-04-25 09:52:03.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.0/antchain_sdk_ak_ee637c8293f64104af9686dc12e0cd18/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-25 09:52:03.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2650 2023-04-25 09:52:03.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 10:14:20.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-04-28 10:14:20.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-28 10:14:20.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2354 2023-04-28 10:14:20.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      900 2023-04-28 10:14:20.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1086 2023-04-28 10:14:20.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 10:14:20.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.1/antchain_ak_ee637c8293f64104af9686dc12e0cd18.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2354 2023-04-28 10:14:20.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.1/antchain_ak_ee637c8293f64104af9686dc12e0cd18.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      579 2023-04-28 10:14:20.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.1/antchain_ak_ee637c8293f64104af9686dc12e0cd18.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 10:14:20.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.1/antchain_ak_ee637c8293f64104af9686dc12e0cd18.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-04-28 10:14:20.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.1/antchain_ak_ee637c8293f64104af9686dc12e0cd18.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-04-28 10:14:20.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.1/antchain_ak_ee637c8293f64104af9686dc12e0cd18.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 10:14:20.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.1/antchain_sdk_ak_ee637c8293f64104af9686dc12e0cd18/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-28 10:14:20.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.1/antchain_sdk_ak_ee637c8293f64104af9686dc12e0cd18/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    49422 2023-04-28 10:14:20.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.1/antchain_sdk_ak_ee637c8293f64104af9686dc12e0cd18/client.py
+-rw-r--r--   0 root         (0) root         (0)    46245 2023-04-28 10:14:20.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.1/antchain_sdk_ak_ee637c8293f64104af9686dc12e0cd18/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-28 10:14:20.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2650 2023-04-28 10:14:20.000000 antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.1/setup.py
```

### Comparing `antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.0/LICENSE` & `antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.0/PKG-INFO` & `antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_ak_ee637c8293f64104af9686dc12e0cd18
-Version: 1.0.0
+Version: 1.0.1
 Summary: Ant Chain Ak_ee637c8293f64104af9686dc12e0cd18 SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.0/README-CN.md` & `antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.0/README.md` & `antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.0/antchain_ak_ee637c8293f64104af9686dc12e0cd18.egg-info/PKG-INFO` & `antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.1/antchain_ak_ee637c8293f64104af9686dc12e0cd18.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-ak-ee637c8293f64104af9686dc12e0cd18
-Version: 1.0.0
+Version: 1.0.1
 Summary: Ant Chain Ak_ee637c8293f64104af9686dc12e0cd18 SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.0/antchain_ak_ee637c8293f64104af9686dc12e0cd18.egg-info/SOURCES.txt` & `antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.1/antchain_ak_ee637c8293f64104af9686dc12e0cd18.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.0/antchain_sdk_ak_ee637c8293f64104af9686dc12e0cd18/client.py` & `antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.1/antchain_sdk_ak_ee637c8293f64104af9686dc12e0cd18/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.0.0',
+                    'sdk_version': '1.0.1',
                     '_prod_code': 'ak_ee637c8293f64104af9686dc12e0cd18',
                     '_prod_channel': 'saas'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -235,15 +235,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.0.0',
+                    'sdk_version': '1.0.1',
                     '_prod_code': 'ak_ee637c8293f64104af9686dc12e0cd18',
                     '_prod_channel': 'saas'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -551,14 +551,70 @@
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             ak_ee_637c_8293f_64104af_9686dc_12e_0cd_18_models.RegisterDemoTestBizeventMessageResponse(),
             await self.do_request_async('1.0', 'demo.test.bizevent.message.register', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
+    def query_demo_cjtest_cj_res(
+        self,
+        request: ak_ee_637c_8293f_64104af_9686dc_12e_0cd_18_models.QueryDemoCjtestCjResRequest,
+    ) -> ak_ee_637c_8293f_64104af_9686dc_12e_0cd_18_models.QueryDemoCjtestCjResResponse:
+        """
+        Description: cj test
+        Summary: cj test
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.query_demo_cjtest_cj_res_ex(request, headers, runtime)
+
+    async def query_demo_cjtest_cj_res_async(
+        self,
+        request: ak_ee_637c_8293f_64104af_9686dc_12e_0cd_18_models.QueryDemoCjtestCjResRequest,
+    ) -> ak_ee_637c_8293f_64104af_9686dc_12e_0cd_18_models.QueryDemoCjtestCjResResponse:
+        """
+        Description: cj test
+        Summary: cj test
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.query_demo_cjtest_cj_res_ex_async(request, headers, runtime)
+
+    def query_demo_cjtest_cj_res_ex(
+        self,
+        request: ak_ee_637c_8293f_64104af_9686dc_12e_0cd_18_models.QueryDemoCjtestCjResRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ak_ee_637c_8293f_64104af_9686dc_12e_0cd_18_models.QueryDemoCjtestCjResResponse:
+        """
+        Description: cj test
+        Summary: cj test
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ak_ee_637c_8293f_64104af_9686dc_12e_0cd_18_models.QueryDemoCjtestCjResResponse(),
+            self.do_request('1.0', 'demo.cjtest.cj.res.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def query_demo_cjtest_cj_res_ex_async(
+        self,
+        request: ak_ee_637c_8293f_64104af_9686dc_12e_0cd_18_models.QueryDemoCjtestCjResRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> ak_ee_637c_8293f_64104af_9686dc_12e_0cd_18_models.QueryDemoCjtestCjResResponse:
+        """
+        Description: cj test
+        Summary: cj test
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            ak_ee_637c_8293f_64104af_9686dc_12e_0cd_18_models.QueryDemoCjtestCjResResponse(),
+            await self.do_request_async('1.0', 'demo.cjtest.cj.res.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
     def publish_demo_saas_test_testc(
         self,
         request: ak_ee_637c_8293f_64104af_9686dc_12e_0cd_18_models.PublishDemoSaasTestTestcRequest,
     ) -> ak_ee_637c_8293f_64104af_9686dc_12e_0cd_18_models.PublishDemoSaasTestTestcResponse:
         """
         Description: testc
         Summary: 测试用api
```

### Comparing `antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.0/antchain_sdk_ak_ee637c8293f64104af9686dc12e0cd18/models.py` & `antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.1/antchain_sdk_ak_ee637c8293f64104af9686dc12e0cd18/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -600,14 +600,90 @@
         if m.get('result_code') is not None:
             self.result_code = m.get('result_code')
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
         return self
 
 
+class QueryDemoCjtestCjResRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
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
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        return self
+
+
+class QueryDemoCjtestCjResResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
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
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        return self
+
+
 class PublishDemoSaasTestTestcRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
         name: str = None,
         age: int = None,
```

### Comparing `antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.0/setup.py` & `antchain_ak_ee637c8293f64104af9686dc12e0cd18-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_ak_ee637c8293f64104af9686dc12e0cd18.
 
-Created on 25/04/2023
+Created on 28/04/2023
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_ak_ee637c8293f64104af9686dc12e0cd18"
 NAME = "antchain_ak_ee637c8293f64104af9686dc12e0cd18" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain Ak_ee637c8293f64104af9686dc12e0cd18 SDK Library for Python"
```

