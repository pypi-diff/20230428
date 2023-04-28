# Comparing `tmp/alibabacloud_computenestsupplier20210521-1.1.2.tar.gz` & `tmp/alibabacloud_computenestsupplier20210521-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_computenestsupplier20210521-1.1.2.tar", last modified: Mon Feb  6 08:13:01 2023, max compression
+gzip compressed data, was "dist/alibabacloud_computenestsupplier20210521-1.2.0.tar", last modified: Fri Apr 28 07:45:17 2023, max compression
```

## Comparing `alibabacloud_computenestsupplier20210521-1.1.2.tar` & `alibabacloud_computenestsupplier20210521-1.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 08:13:01.000000 alibabacloud_computenestsupplier20210521-1.1.2/
--rw-r--r--   0 root         (0) root         (0)      195 2023-02-06 08:13:01.000000 alibabacloud_computenestsupplier20210521-1.1.2/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-02-06 08:13:01.000000 alibabacloud_computenestsupplier20210521-1.1.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-02-06 08:13:01.000000 alibabacloud_computenestsupplier20210521-1.1.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2424 2023-02-06 08:13:01.000000 alibabacloud_computenestsupplier20210521-1.1.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1070 2023-02-06 08:13:01.000000 alibabacloud_computenestsupplier20210521-1.1.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1155 2023-02-06 08:13:01.000000 alibabacloud_computenestsupplier20210521-1.1.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 08:13:01.000000 alibabacloud_computenestsupplier20210521-1.1.2/alibabacloud_computenestsupplier20210521/
--rw-r--r--   0 root         (0) root         (0)       21 2023-02-06 08:13:01.000000 alibabacloud_computenestsupplier20210521-1.1.2/alibabacloud_computenestsupplier20210521/__init__.py
--rw-r--r--   0 root         (0) root         (0)    38737 2023-02-06 08:13:01.000000 alibabacloud_computenestsupplier20210521-1.1.2/alibabacloud_computenestsupplier20210521/client.py
--rw-r--r--   0 root         (0) root         (0)   116070 2023-02-06 08:13:01.000000 alibabacloud_computenestsupplier20210521-1.1.2/alibabacloud_computenestsupplier20210521/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-06 08:13:01.000000 alibabacloud_computenestsupplier20210521-1.1.2/alibabacloud_computenestsupplier20210521.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2424 2023-02-06 08:13:01.000000 alibabacloud_computenestsupplier20210521-1.1.2/alibabacloud_computenestsupplier20210521.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      548 2023-02-06 08:13:01.000000 alibabacloud_computenestsupplier20210521-1.1.2/alibabacloud_computenestsupplier20210521.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-06 08:13:01.000000 alibabacloud_computenestsupplier20210521-1.1.2/alibabacloud_computenestsupplier20210521.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-02-06 08:13:01.000000 alibabacloud_computenestsupplier20210521-1.1.2/alibabacloud_computenestsupplier20210521.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       41 2023-02-06 08:13:01.000000 alibabacloud_computenestsupplier20210521-1.1.2/alibabacloud_computenestsupplier20210521.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-02-06 08:13:01.000000 alibabacloud_computenestsupplier20210521-1.1.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2690 2023-02-06 08:13:01.000000 alibabacloud_computenestsupplier20210521-1.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:45:17.000000 alibabacloud_computenestsupplier20210521-1.2.0/
+-rw-r--r--   0 root         (0) root         (0)      259 2023-04-28 07:45:17.000000 alibabacloud_computenestsupplier20210521-1.2.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-04-28 07:45:17.000000 alibabacloud_computenestsupplier20210521-1.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-04-28 07:45:17.000000 alibabacloud_computenestsupplier20210521-1.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2424 2023-04-28 07:45:17.000000 alibabacloud_computenestsupplier20210521-1.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1070 2023-04-28 07:45:17.000000 alibabacloud_computenestsupplier20210521-1.2.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1155 2023-04-28 07:45:17.000000 alibabacloud_computenestsupplier20210521-1.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:45:17.000000 alibabacloud_computenestsupplier20210521-1.2.0/alibabacloud_computenestsupplier20210521/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-28 07:45:17.000000 alibabacloud_computenestsupplier20210521-1.2.0/alibabacloud_computenestsupplier20210521/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    54641 2023-04-28 07:45:17.000000 alibabacloud_computenestsupplier20210521-1.2.0/alibabacloud_computenestsupplier20210521/client.py
+-rw-r--r--   0 root         (0) root         (0)   153003 2023-04-28 07:45:17.000000 alibabacloud_computenestsupplier20210521-1.2.0/alibabacloud_computenestsupplier20210521/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 07:45:17.000000 alibabacloud_computenestsupplier20210521-1.2.0/alibabacloud_computenestsupplier20210521.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2424 2023-04-28 07:45:17.000000 alibabacloud_computenestsupplier20210521-1.2.0/alibabacloud_computenestsupplier20210521.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      548 2023-04-28 07:45:17.000000 alibabacloud_computenestsupplier20210521-1.2.0/alibabacloud_computenestsupplier20210521.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 07:45:17.000000 alibabacloud_computenestsupplier20210521-1.2.0/alibabacloud_computenestsupplier20210521.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-04-28 07:45:17.000000 alibabacloud_computenestsupplier20210521-1.2.0/alibabacloud_computenestsupplier20210521.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       41 2023-04-28 07:45:17.000000 alibabacloud_computenestsupplier20210521-1.2.0/alibabacloud_computenestsupplier20210521.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-28 07:45:17.000000 alibabacloud_computenestsupplier20210521-1.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2690 2023-04-28 07:45:17.000000 alibabacloud_computenestsupplier20210521-1.2.0/setup.py
```

### Comparing `alibabacloud_computenestsupplier20210521-1.1.2/LICENSE` & `alibabacloud_computenestsupplier20210521-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_computenestsupplier20210521-1.1.2/PKG-INFO` & `alibabacloud_computenestsupplier20210521-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_computenestsupplier20210521
-Version: 1.1.2
+Version: 1.2.0
 Summary: Alibaba Cloud ComputeNestSupplier (20210521) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_computenestsupplier20210521-1.1.2/README-CN.md` & `alibabacloud_computenestsupplier20210521-1.2.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_computenestsupplier20210521-1.1.2/README.md` & `alibabacloud_computenestsupplier20210521-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_computenestsupplier20210521-1.1.2/alibabacloud_computenestsupplier20210521/client.py` & `alibabacloud_computenestsupplier20210521-1.2.0/alibabacloud_computenestsupplier20210521/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -139,14 +139,160 @@
     async def create_artifact_async(
         self,
         request: compute_nest_supplier_20210521_models.CreateArtifactRequest,
     ) -> compute_nest_supplier_20210521_models.CreateArtifactResponse:
         runtime = util_models.RuntimeOptions()
         return await self.create_artifact_with_options_async(request, runtime)
 
+    def create_service_with_options(
+        self,
+        request: compute_nest_supplier_20210521_models.CreateServiceRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> compute_nest_supplier_20210521_models.CreateServiceResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.alarm_metadata):
+            query['AlarmMetadata'] = request.alarm_metadata
+        if not UtilClient.is_unset(request.approval_type):
+            query['ApprovalType'] = request.approval_type
+        if not UtilClient.is_unset(request.client_token):
+            query['ClientToken'] = request.client_token
+        if not UtilClient.is_unset(request.deploy_metadata):
+            query['DeployMetadata'] = request.deploy_metadata
+        if not UtilClient.is_unset(request.deploy_type):
+            query['DeployType'] = request.deploy_type
+        if not UtilClient.is_unset(request.duration):
+            query['Duration'] = request.duration
+        if not UtilClient.is_unset(request.is_support_operated):
+            query['IsSupportOperated'] = request.is_support_operated
+        if not UtilClient.is_unset(request.license_metadata):
+            query['LicenseMetadata'] = request.license_metadata
+        if not UtilClient.is_unset(request.operation_metadata):
+            query['OperationMetadata'] = request.operation_metadata
+        if not UtilClient.is_unset(request.policy_names):
+            query['PolicyNames'] = request.policy_names
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.service_id):
+            query['ServiceId'] = request.service_id
+        if not UtilClient.is_unset(request.service_info):
+            query['ServiceInfo'] = request.service_info
+        if not UtilClient.is_unset(request.service_type):
+            query['ServiceType'] = request.service_type
+        if not UtilClient.is_unset(request.share_type):
+            query['ShareType'] = request.share_type
+        if not UtilClient.is_unset(request.tag):
+            query['Tag'] = request.tag
+        if not UtilClient.is_unset(request.tenant_type):
+            query['TenantType'] = request.tenant_type
+        if not UtilClient.is_unset(request.trial_duration):
+            query['TrialDuration'] = request.trial_duration
+        if not UtilClient.is_unset(request.upgrade_metadata):
+            query['UpgradeMetadata'] = request.upgrade_metadata
+        if not UtilClient.is_unset(request.version_name):
+            query['VersionName'] = request.version_name
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='CreateService',
+            version='2021-05-21',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            compute_nest_supplier_20210521_models.CreateServiceResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def create_service_with_options_async(
+        self,
+        request: compute_nest_supplier_20210521_models.CreateServiceRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> compute_nest_supplier_20210521_models.CreateServiceResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.alarm_metadata):
+            query['AlarmMetadata'] = request.alarm_metadata
+        if not UtilClient.is_unset(request.approval_type):
+            query['ApprovalType'] = request.approval_type
+        if not UtilClient.is_unset(request.client_token):
+            query['ClientToken'] = request.client_token
+        if not UtilClient.is_unset(request.deploy_metadata):
+            query['DeployMetadata'] = request.deploy_metadata
+        if not UtilClient.is_unset(request.deploy_type):
+            query['DeployType'] = request.deploy_type
+        if not UtilClient.is_unset(request.duration):
+            query['Duration'] = request.duration
+        if not UtilClient.is_unset(request.is_support_operated):
+            query['IsSupportOperated'] = request.is_support_operated
+        if not UtilClient.is_unset(request.license_metadata):
+            query['LicenseMetadata'] = request.license_metadata
+        if not UtilClient.is_unset(request.operation_metadata):
+            query['OperationMetadata'] = request.operation_metadata
+        if not UtilClient.is_unset(request.policy_names):
+            query['PolicyNames'] = request.policy_names
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.service_id):
+            query['ServiceId'] = request.service_id
+        if not UtilClient.is_unset(request.service_info):
+            query['ServiceInfo'] = request.service_info
+        if not UtilClient.is_unset(request.service_type):
+            query['ServiceType'] = request.service_type
+        if not UtilClient.is_unset(request.share_type):
+            query['ShareType'] = request.share_type
+        if not UtilClient.is_unset(request.tag):
+            query['Tag'] = request.tag
+        if not UtilClient.is_unset(request.tenant_type):
+            query['TenantType'] = request.tenant_type
+        if not UtilClient.is_unset(request.trial_duration):
+            query['TrialDuration'] = request.trial_duration
+        if not UtilClient.is_unset(request.upgrade_metadata):
+            query['UpgradeMetadata'] = request.upgrade_metadata
+        if not UtilClient.is_unset(request.version_name):
+            query['VersionName'] = request.version_name
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='CreateService',
+            version='2021-05-21',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            compute_nest_supplier_20210521_models.CreateServiceResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def create_service(
+        self,
+        request: compute_nest_supplier_20210521_models.CreateServiceRequest,
+    ) -> compute_nest_supplier_20210521_models.CreateServiceResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.create_service_with_options(request, runtime)
+
+    async def create_service_async(
+        self,
+        request: compute_nest_supplier_20210521_models.CreateServiceRequest,
+    ) -> compute_nest_supplier_20210521_models.CreateServiceResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.create_service_with_options_async(request, runtime)
+
     def delete_artifact_with_options(
         self,
         request: compute_nest_supplier_20210521_models.DeleteArtifactRequest,
         runtime: util_models.RuntimeOptions,
     ) -> compute_nest_supplier_20210521_models.DeleteArtifactResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -361,14 +507,116 @@
     async def get_artifact_repository_credentials_async(
         self,
         request: compute_nest_supplier_20210521_models.GetArtifactRepositoryCredentialsRequest,
     ) -> compute_nest_supplier_20210521_models.GetArtifactRepositoryCredentialsResponse:
         runtime = util_models.RuntimeOptions()
         return await self.get_artifact_repository_credentials_with_options_async(request, runtime)
 
+    def get_service_estimate_cost_with_options(
+        self,
+        tmp_req: compute_nest_supplier_20210521_models.GetServiceEstimateCostRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> compute_nest_supplier_20210521_models.GetServiceEstimateCostResponse:
+        UtilClient.validate_model(tmp_req)
+        request = compute_nest_supplier_20210521_models.GetServiceEstimateCostShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.parameters):
+            request.parameters_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.parameters, 'Parameters', 'json')
+        query = {}
+        if not UtilClient.is_unset(request.client_token):
+            query['ClientToken'] = request.client_token
+        if not UtilClient.is_unset(request.parameters_shrink):
+            query['Parameters'] = request.parameters_shrink
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.service_id):
+            query['ServiceId'] = request.service_id
+        if not UtilClient.is_unset(request.service_instance_id):
+            query['ServiceInstanceId'] = request.service_instance_id
+        if not UtilClient.is_unset(request.service_version):
+            query['ServiceVersion'] = request.service_version
+        if not UtilClient.is_unset(request.template_name):
+            query['TemplateName'] = request.template_name
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetServiceEstimateCost',
+            version='2021-05-21',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            compute_nest_supplier_20210521_models.GetServiceEstimateCostResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def get_service_estimate_cost_with_options_async(
+        self,
+        tmp_req: compute_nest_supplier_20210521_models.GetServiceEstimateCostRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> compute_nest_supplier_20210521_models.GetServiceEstimateCostResponse:
+        UtilClient.validate_model(tmp_req)
+        request = compute_nest_supplier_20210521_models.GetServiceEstimateCostShrinkRequest()
+        OpenApiUtilClient.convert(tmp_req, request)
+        if not UtilClient.is_unset(tmp_req.parameters):
+            request.parameters_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.parameters, 'Parameters', 'json')
+        query = {}
+        if not UtilClient.is_unset(request.client_token):
+            query['ClientToken'] = request.client_token
+        if not UtilClient.is_unset(request.parameters_shrink):
+            query['Parameters'] = request.parameters_shrink
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.service_id):
+            query['ServiceId'] = request.service_id
+        if not UtilClient.is_unset(request.service_instance_id):
+            query['ServiceInstanceId'] = request.service_instance_id
+        if not UtilClient.is_unset(request.service_version):
+            query['ServiceVersion'] = request.service_version
+        if not UtilClient.is_unset(request.template_name):
+            query['TemplateName'] = request.template_name
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetServiceEstimateCost',
+            version='2021-05-21',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            compute_nest_supplier_20210521_models.GetServiceEstimateCostResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def get_service_estimate_cost(
+        self,
+        request: compute_nest_supplier_20210521_models.GetServiceEstimateCostRequest,
+    ) -> compute_nest_supplier_20210521_models.GetServiceEstimateCostResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.get_service_estimate_cost_with_options(request, runtime)
+
+    async def get_service_estimate_cost_async(
+        self,
+        request: compute_nest_supplier_20210521_models.GetServiceEstimateCostRequest,
+    ) -> compute_nest_supplier_20210521_models.GetServiceEstimateCostResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.get_service_estimate_cost_with_options_async(request, runtime)
+
     def get_service_instance_with_options(
         self,
         request: compute_nest_supplier_20210521_models.GetServiceInstanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> compute_nest_supplier_20210521_models.GetServiceInstanceResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -606,14 +854,16 @@
             query['Filter'] = request.filter
         if not UtilClient.is_unset(request.max_results):
             query['MaxResults'] = request.max_results
         if not UtilClient.is_unset(request.next_token):
             query['NextToken'] = request.next_token
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.show_deleted):
+            query['ShowDeleted'] = request.show_deleted
         if not UtilClient.is_unset(request.tag):
             query['Tag'] = request.tag
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListServiceInstances',
@@ -642,14 +892,16 @@
             query['Filter'] = request.filter
         if not UtilClient.is_unset(request.max_results):
             query['MaxResults'] = request.max_results
         if not UtilClient.is_unset(request.next_token):
             query['NextToken'] = request.next_token
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.show_deleted):
+            query['ShowDeleted'] = request.show_deleted
         if not UtilClient.is_unset(request.tag):
             query['Tag'] = request.tag
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListServiceInstances',
@@ -755,14 +1007,104 @@
     async def list_service_usages_async(
         self,
         request: compute_nest_supplier_20210521_models.ListServiceUsagesRequest,
     ) -> compute_nest_supplier_20210521_models.ListServiceUsagesResponse:
         runtime = util_models.RuntimeOptions()
         return await self.list_service_usages_with_options_async(request, runtime)
 
+    def list_services_with_options(
+        self,
+        request: compute_nest_supplier_20210521_models.ListServicesRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> compute_nest_supplier_20210521_models.ListServicesResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.all_versions):
+            query['AllVersions'] = request.all_versions
+        if not UtilClient.is_unset(request.filter):
+            query['Filter'] = request.filter
+        if not UtilClient.is_unset(request.max_results):
+            query['MaxResults'] = request.max_results
+        if not UtilClient.is_unset(request.next_token):
+            query['NextToken'] = request.next_token
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.tag):
+            query['Tag'] = request.tag
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListServices',
+            version='2021-05-21',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            compute_nest_supplier_20210521_models.ListServicesResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def list_services_with_options_async(
+        self,
+        request: compute_nest_supplier_20210521_models.ListServicesRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> compute_nest_supplier_20210521_models.ListServicesResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.all_versions):
+            query['AllVersions'] = request.all_versions
+        if not UtilClient.is_unset(request.filter):
+            query['Filter'] = request.filter
+        if not UtilClient.is_unset(request.max_results):
+            query['MaxResults'] = request.max_results
+        if not UtilClient.is_unset(request.next_token):
+            query['NextToken'] = request.next_token
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.tag):
+            query['Tag'] = request.tag
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListServices',
+            version='2021-05-21',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            compute_nest_supplier_20210521_models.ListServicesResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def list_services(
+        self,
+        request: compute_nest_supplier_20210521_models.ListServicesRequest,
+    ) -> compute_nest_supplier_20210521_models.ListServicesResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.list_services_with_options(request, runtime)
+
+    async def list_services_async(
+        self,
+        request: compute_nest_supplier_20210521_models.ListServicesRequest,
+    ) -> compute_nest_supplier_20210521_models.ListServicesResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.list_services_with_options_async(request, runtime)
+
     def release_artifact_with_options(
         self,
         request: compute_nest_supplier_20210521_models.ReleaseArtifactRequest,
         runtime: util_models.RuntimeOptions,
     ) -> compute_nest_supplier_20210521_models.ReleaseArtifactResponse:
         UtilClient.validate_model(request)
         query = {}
```

### Comparing `alibabacloud_computenestsupplier20210521-1.1.2/alibabacloud_computenestsupplier20210521/models.py` & `alibabacloud_computenestsupplier20210521-1.2.0/alibabacloud_computenestsupplier20210521/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # This file is auto-generated, don't edit it. Thanks.
 from Tea.model import TeaModel
-from typing import List, Dict
+from typing import List, Dict, Any
 
 
 class CreateArtifactRequestArtifactProperty(TeaModel):
     def __init__(
         self,
         commodity_code: str = None,
         commodity_version: str = None,
@@ -328,14 +328,339 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CreateArtifactResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class CreateServiceRequestServiceInfo(TeaModel):
+    def __init__(
+        self,
+        image: str = None,
+        locale: str = None,
+        name: str = None,
+        short_description: str = None,
+    ):
+        self.image = image
+        self.locale = locale
+        self.name = name
+        self.short_description = short_description
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
+        if self.image is not None:
+            result['Image'] = self.image
+        if self.locale is not None:
+            result['Locale'] = self.locale
+        if self.name is not None:
+            result['Name'] = self.name
+        if self.short_description is not None:
+            result['ShortDescription'] = self.short_description
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Image') is not None:
+            self.image = m.get('Image')
+        if m.get('Locale') is not None:
+            self.locale = m.get('Locale')
+        if m.get('Name') is not None:
+            self.name = m.get('Name')
+        if m.get('ShortDescription') is not None:
+            self.short_description = m.get('ShortDescription')
+        return self
+
+
+class CreateServiceRequestTag(TeaModel):
+    def __init__(
+        self,
+        key: str = None,
+        value: str = None,
+    ):
+        self.key = key
+        self.value = value
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
+        if self.key is not None:
+            result['Key'] = self.key
+        if self.value is not None:
+            result['Value'] = self.value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Key') is not None:
+            self.key = m.get('Key')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
+class CreateServiceRequest(TeaModel):
+    def __init__(
+        self,
+        alarm_metadata: str = None,
+        approval_type: str = None,
+        client_token: str = None,
+        deploy_metadata: str = None,
+        deploy_type: str = None,
+        duration: int = None,
+        is_support_operated: bool = None,
+        license_metadata: str = None,
+        operation_metadata: str = None,
+        policy_names: str = None,
+        region_id: str = None,
+        service_id: str = None,
+        service_info: List[CreateServiceRequestServiceInfo] = None,
+        service_type: str = None,
+        share_type: str = None,
+        tag: List[CreateServiceRequestTag] = None,
+        tenant_type: str = None,
+        trial_duration: int = None,
+        upgrade_metadata: str = None,
+        version_name: str = None,
+    ):
+        self.alarm_metadata = alarm_metadata
+        self.approval_type = approval_type
+        self.client_token = client_token
+        self.deploy_metadata = deploy_metadata
+        self.deploy_type = deploy_type
+        self.duration = duration
+        self.is_support_operated = is_support_operated
+        self.license_metadata = license_metadata
+        self.operation_metadata = operation_metadata
+        self.policy_names = policy_names
+        self.region_id = region_id
+        self.service_id = service_id
+        self.service_info = service_info
+        self.service_type = service_type
+        self.share_type = share_type
+        self.tag = tag
+        self.tenant_type = tenant_type
+        self.trial_duration = trial_duration
+        self.upgrade_metadata = upgrade_metadata
+        self.version_name = version_name
+
+    def validate(self):
+        if self.service_info:
+            for k in self.service_info:
+                if k:
+                    k.validate()
+        if self.tag:
+            for k in self.tag:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.alarm_metadata is not None:
+            result['AlarmMetadata'] = self.alarm_metadata
+        if self.approval_type is not None:
+            result['ApprovalType'] = self.approval_type
+        if self.client_token is not None:
+            result['ClientToken'] = self.client_token
+        if self.deploy_metadata is not None:
+            result['DeployMetadata'] = self.deploy_metadata
+        if self.deploy_type is not None:
+            result['DeployType'] = self.deploy_type
+        if self.duration is not None:
+            result['Duration'] = self.duration
+        if self.is_support_operated is not None:
+            result['IsSupportOperated'] = self.is_support_operated
+        if self.license_metadata is not None:
+            result['LicenseMetadata'] = self.license_metadata
+        if self.operation_metadata is not None:
+            result['OperationMetadata'] = self.operation_metadata
+        if self.policy_names is not None:
+            result['PolicyNames'] = self.policy_names
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.service_id is not None:
+            result['ServiceId'] = self.service_id
+        result['ServiceInfo'] = []
+        if self.service_info is not None:
+            for k in self.service_info:
+                result['ServiceInfo'].append(k.to_map() if k else None)
+        if self.service_type is not None:
+            result['ServiceType'] = self.service_type
+        if self.share_type is not None:
+            result['ShareType'] = self.share_type
+        result['Tag'] = []
+        if self.tag is not None:
+            for k in self.tag:
+                result['Tag'].append(k.to_map() if k else None)
+        if self.tenant_type is not None:
+            result['TenantType'] = self.tenant_type
+        if self.trial_duration is not None:
+            result['TrialDuration'] = self.trial_duration
+        if self.upgrade_metadata is not None:
+            result['UpgradeMetadata'] = self.upgrade_metadata
+        if self.version_name is not None:
+            result['VersionName'] = self.version_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AlarmMetadata') is not None:
+            self.alarm_metadata = m.get('AlarmMetadata')
+        if m.get('ApprovalType') is not None:
+            self.approval_type = m.get('ApprovalType')
+        if m.get('ClientToken') is not None:
+            self.client_token = m.get('ClientToken')
+        if m.get('DeployMetadata') is not None:
+            self.deploy_metadata = m.get('DeployMetadata')
+        if m.get('DeployType') is not None:
+            self.deploy_type = m.get('DeployType')
+        if m.get('Duration') is not None:
+            self.duration = m.get('Duration')
+        if m.get('IsSupportOperated') is not None:
+            self.is_support_operated = m.get('IsSupportOperated')
+        if m.get('LicenseMetadata') is not None:
+            self.license_metadata = m.get('LicenseMetadata')
+        if m.get('OperationMetadata') is not None:
+            self.operation_metadata = m.get('OperationMetadata')
+        if m.get('PolicyNames') is not None:
+            self.policy_names = m.get('PolicyNames')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('ServiceId') is not None:
+            self.service_id = m.get('ServiceId')
+        self.service_info = []
+        if m.get('ServiceInfo') is not None:
+            for k in m.get('ServiceInfo'):
+                temp_model = CreateServiceRequestServiceInfo()
+                self.service_info.append(temp_model.from_map(k))
+        if m.get('ServiceType') is not None:
+            self.service_type = m.get('ServiceType')
+        if m.get('ShareType') is not None:
+            self.share_type = m.get('ShareType')
+        self.tag = []
+        if m.get('Tag') is not None:
+            for k in m.get('Tag'):
+                temp_model = CreateServiceRequestTag()
+                self.tag.append(temp_model.from_map(k))
+        if m.get('TenantType') is not None:
+            self.tenant_type = m.get('TenantType')
+        if m.get('TrialDuration') is not None:
+            self.trial_duration = m.get('TrialDuration')
+        if m.get('UpgradeMetadata') is not None:
+            self.upgrade_metadata = m.get('UpgradeMetadata')
+        if m.get('VersionName') is not None:
+            self.version_name = m.get('VersionName')
+        return self
+
+
+class CreateServiceResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+        service_id: str = None,
+        status: str = None,
+        version: str = None,
+    ):
+        self.request_id = request_id
+        self.service_id = service_id
+        self.status = status
+        self.version = version
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
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.service_id is not None:
+            result['ServiceId'] = self.service_id
+        if self.status is not None:
+            result['Status'] = self.status
+        if self.version is not None:
+            result['Version'] = self.version
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('ServiceId') is not None:
+            self.service_id = m.get('ServiceId')
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
+        if m.get('Version') is not None:
+            self.version = m.get('Version')
+        return self
+
+
+class CreateServiceResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: CreateServiceResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
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
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = CreateServiceResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class DeleteArtifactRequest(TeaModel):
     def __init__(
         self,
         artifact_id: str = None,
         artifact_version: str = None,
     ):
         self.artifact_id = artifact_id
@@ -831,14 +1156,217 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GetArtifactRepositoryCredentialsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GetServiceEstimateCostRequest(TeaModel):
+    def __init__(
+        self,
+        client_token: str = None,
+        parameters: Dict[str, Any] = None,
+        region_id: str = None,
+        service_id: str = None,
+        service_instance_id: str = None,
+        service_version: str = None,
+        template_name: str = None,
+    ):
+        self.client_token = client_token
+        self.parameters = parameters
+        self.region_id = region_id
+        self.service_id = service_id
+        self.service_instance_id = service_instance_id
+        self.service_version = service_version
+        self.template_name = template_name
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
+        if self.client_token is not None:
+            result['ClientToken'] = self.client_token
+        if self.parameters is not None:
+            result['Parameters'] = self.parameters
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.service_id is not None:
+            result['ServiceId'] = self.service_id
+        if self.service_instance_id is not None:
+            result['ServiceInstanceId'] = self.service_instance_id
+        if self.service_version is not None:
+            result['ServiceVersion'] = self.service_version
+        if self.template_name is not None:
+            result['TemplateName'] = self.template_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ClientToken') is not None:
+            self.client_token = m.get('ClientToken')
+        if m.get('Parameters') is not None:
+            self.parameters = m.get('Parameters')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('ServiceId') is not None:
+            self.service_id = m.get('ServiceId')
+        if m.get('ServiceInstanceId') is not None:
+            self.service_instance_id = m.get('ServiceInstanceId')
+        if m.get('ServiceVersion') is not None:
+            self.service_version = m.get('ServiceVersion')
+        if m.get('TemplateName') is not None:
+            self.template_name = m.get('TemplateName')
+        return self
+
+
+class GetServiceEstimateCostShrinkRequest(TeaModel):
+    def __init__(
+        self,
+        client_token: str = None,
+        parameters_shrink: str = None,
+        region_id: str = None,
+        service_id: str = None,
+        service_instance_id: str = None,
+        service_version: str = None,
+        template_name: str = None,
+    ):
+        self.client_token = client_token
+        self.parameters_shrink = parameters_shrink
+        self.region_id = region_id
+        self.service_id = service_id
+        self.service_instance_id = service_instance_id
+        self.service_version = service_version
+        self.template_name = template_name
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
+        if self.client_token is not None:
+            result['ClientToken'] = self.client_token
+        if self.parameters_shrink is not None:
+            result['Parameters'] = self.parameters_shrink
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.service_id is not None:
+            result['ServiceId'] = self.service_id
+        if self.service_instance_id is not None:
+            result['ServiceInstanceId'] = self.service_instance_id
+        if self.service_version is not None:
+            result['ServiceVersion'] = self.service_version
+        if self.template_name is not None:
+            result['TemplateName'] = self.template_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ClientToken') is not None:
+            self.client_token = m.get('ClientToken')
+        if m.get('Parameters') is not None:
+            self.parameters_shrink = m.get('Parameters')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('ServiceId') is not None:
+            self.service_id = m.get('ServiceId')
+        if m.get('ServiceInstanceId') is not None:
+            self.service_instance_id = m.get('ServiceInstanceId')
+        if m.get('ServiceVersion') is not None:
+            self.service_version = m.get('ServiceVersion')
+        if m.get('TemplateName') is not None:
+            self.template_name = m.get('TemplateName')
+        return self
+
+
+class GetServiceEstimateCostResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+        resources: Dict[str, Any] = None,
+    ):
+        self.request_id = request_id
+        self.resources = resources
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
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.resources is not None:
+            result['Resources'] = self.resources
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('Resources') is not None:
+            self.resources = m.get('Resources')
+        return self
+
+
+class GetServiceEstimateCostResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GetServiceEstimateCostResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
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
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = GetServiceEstimateCostResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class GetServiceInstanceRequest(TeaModel):
     def __init__(
         self,
         region_id: str = None,
         service_instance_id: str = None,
     ):
         self.region_id = region_id
@@ -867,21 +1395,23 @@
             self.service_instance_id = m.get('ServiceInstanceId')
         return self
 
 
 class GetServiceInstanceResponseBodyNetworkConfigPrivateVpcConnectionsConnectionConfigs(TeaModel):
     def __init__(
         self,
+        domain_name: str = None,
         endpoint_ips: List[str] = None,
         ingress_endpoint_status: str = None,
         network_service_status: str = None,
         security_groups: List[str] = None,
         v_switches: List[str] = None,
         vpc_id: str = None,
     ):
+        self.domain_name = domain_name
         self.endpoint_ips = endpoint_ips
         self.ingress_endpoint_status = ingress_endpoint_status
         self.network_service_status = network_service_status
         self.security_groups = security_groups
         self.v_switches = v_switches
         self.vpc_id = vpc_id
 
@@ -890,14 +1420,16 @@
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.domain_name is not None:
+            result['DomainName'] = self.domain_name
         if self.endpoint_ips is not None:
             result['EndpointIps'] = self.endpoint_ips
         if self.ingress_endpoint_status is not None:
             result['IngressEndpointStatus'] = self.ingress_endpoint_status
         if self.network_service_status is not None:
             result['NetworkServiceStatus'] = self.network_service_status
         if self.security_groups is not None:
@@ -906,14 +1438,16 @@
             result['VSwitches'] = self.v_switches
         if self.vpc_id is not None:
             result['VpcId'] = self.vpc_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('DomainName') is not None:
+            self.domain_name = m.get('DomainName')
         if m.get('EndpointIps') is not None:
             self.endpoint_ips = m.get('EndpointIps')
         if m.get('IngressEndpointStatus') is not None:
             self.ingress_endpoint_status = m.get('IngressEndpointStatus')
         if m.get('NetworkServiceStatus') is not None:
             self.network_service_status = m.get('NetworkServiceStatus')
         if m.get('SecurityGroups') is not None:
@@ -1128,28 +1662,30 @@
         service_id: str = None,
         service_infos: List[GetServiceInstanceResponseBodyServiceServiceInfos] = None,
         service_product_url: str = None,
         service_type: str = None,
         status: str = None,
         supplier_name: str = None,
         supplier_url: str = None,
+        upgradable_service_versions: List[str] = None,
         version: str = None,
         version_name: str = None,
     ):
         self.deploy_metadata = deploy_metadata
         self.deploy_type = deploy_type
         self.publish_time = publish_time
         self.service_doc_url = service_doc_url
         self.service_id = service_id
         self.service_infos = service_infos
         self.service_product_url = service_product_url
         self.service_type = service_type
         self.status = status
         self.supplier_name = supplier_name
         self.supplier_url = supplier_url
+        self.upgradable_service_versions = upgradable_service_versions
         self.version = version
         self.version_name = version_name
 
     def validate(self):
         if self.service_infos:
             for k in self.service_infos:
                 if k:
@@ -1181,14 +1717,16 @@
             result['ServiceType'] = self.service_type
         if self.status is not None:
             result['Status'] = self.status
         if self.supplier_name is not None:
             result['SupplierName'] = self.supplier_name
         if self.supplier_url is not None:
             result['SupplierUrl'] = self.supplier_url
+        if self.upgradable_service_versions is not None:
+            result['UpgradableServiceVersions'] = self.upgradable_service_versions
         if self.version is not None:
             result['Version'] = self.version
         if self.version_name is not None:
             result['VersionName'] = self.version_name
         return result
 
     def from_map(self, m: dict = None):
@@ -1214,14 +1752,16 @@
             self.service_type = m.get('ServiceType')
         if m.get('Status') is not None:
             self.status = m.get('Status')
         if m.get('SupplierName') is not None:
             self.supplier_name = m.get('SupplierName')
         if m.get('SupplierUrl') is not None:
             self.supplier_url = m.get('SupplierUrl')
+        if m.get('UpgradableServiceVersions') is not None:
+            self.upgradable_service_versions = m.get('UpgradableServiceVersions')
         if m.get('Version') is not None:
             self.version = m.get('Version')
         if m.get('VersionName') is not None:
             self.version_name = m.get('VersionName')
         return self
 
 
@@ -1259,26 +1799,28 @@
 
 
 class GetServiceInstanceResponseBody(TeaModel):
     def __init__(
         self,
         create_time: str = None,
         enable_instance_ops: bool = None,
+        enable_user_prometheus: str = None,
         end_time: str = None,
         is_operated: bool = None,
         license_metadata: str = None,
         name: str = None,
         network_config: GetServiceInstanceResponseBodyNetworkConfig = None,
         operated_service_instance_id: str = None,
         operation_end_time: str = None,
         operation_start_time: str = None,
         outputs: str = None,
         parameters: str = None,
         pay_type: str = None,
         progress: int = None,
+        rd_account_login_url: str = None,
         request_id: str = None,
         resources: str = None,
         service: GetServiceInstanceResponseBodyService = None,
         service_instance_id: str = None,
         service_type: str = None,
         source: str = None,
         status: str = None,
@@ -1287,26 +1829,28 @@
         tags: List[GetServiceInstanceResponseBodyTags] = None,
         template_name: str = None,
         update_time: str = None,
         user_id: int = None,
     ):
         self.create_time = create_time
         self.enable_instance_ops = enable_instance_ops
+        self.enable_user_prometheus = enable_user_prometheus
         self.end_time = end_time
         self.is_operated = is_operated
         self.license_metadata = license_metadata
         self.name = name
         self.network_config = network_config
         self.operated_service_instance_id = operated_service_instance_id
         self.operation_end_time = operation_end_time
         self.operation_start_time = operation_start_time
         self.outputs = outputs
         self.parameters = parameters
         self.pay_type = pay_type
         self.progress = progress
+        self.rd_account_login_url = rd_account_login_url
         self.request_id = request_id
         self.resources = resources
         self.service = service
         self.service_instance_id = service_instance_id
         self.service_type = service_type
         self.source = source
         self.status = status
@@ -1333,14 +1877,16 @@
             return _map
 
         result = dict()
         if self.create_time is not None:
             result['CreateTime'] = self.create_time
         if self.enable_instance_ops is not None:
             result['EnableInstanceOps'] = self.enable_instance_ops
+        if self.enable_user_prometheus is not None:
+            result['EnableUserPrometheus'] = self.enable_user_prometheus
         if self.end_time is not None:
             result['EndTime'] = self.end_time
         if self.is_operated is not None:
             result['IsOperated'] = self.is_operated
         if self.license_metadata is not None:
             result['LicenseMetadata'] = self.license_metadata
         if self.name is not None:
@@ -1357,14 +1903,16 @@
             result['Outputs'] = self.outputs
         if self.parameters is not None:
             result['Parameters'] = self.parameters
         if self.pay_type is not None:
             result['PayType'] = self.pay_type
         if self.progress is not None:
             result['Progress'] = self.progress
+        if self.rd_account_login_url is not None:
+            result['RdAccountLoginUrl'] = self.rd_account_login_url
         if self.request_id is not None:
             result['RequestId'] = self.request_id
         if self.resources is not None:
             result['Resources'] = self.resources
         if self.service is not None:
             result['Service'] = self.service.to_map()
         if self.service_instance_id is not None:
@@ -1393,14 +1941,16 @@
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('CreateTime') is not None:
             self.create_time = m.get('CreateTime')
         if m.get('EnableInstanceOps') is not None:
             self.enable_instance_ops = m.get('EnableInstanceOps')
+        if m.get('EnableUserPrometheus') is not None:
+            self.enable_user_prometheus = m.get('EnableUserPrometheus')
         if m.get('EndTime') is not None:
             self.end_time = m.get('EndTime')
         if m.get('IsOperated') is not None:
             self.is_operated = m.get('IsOperated')
         if m.get('LicenseMetadata') is not None:
             self.license_metadata = m.get('LicenseMetadata')
         if m.get('Name') is not None:
@@ -1418,14 +1968,16 @@
             self.outputs = m.get('Outputs')
         if m.get('Parameters') is not None:
             self.parameters = m.get('Parameters')
         if m.get('PayType') is not None:
             self.pay_type = m.get('PayType')
         if m.get('Progress') is not None:
             self.progress = m.get('Progress')
+        if m.get('RdAccountLoginUrl') is not None:
+            self.rd_account_login_url = m.get('RdAccountLoginUrl')
         if m.get('RequestId') is not None:
             self.request_id = m.get('RequestId')
         if m.get('Resources') is not None:
             self.resources = m.get('Resources')
         if m.get('Service') is not None:
             temp_model = GetServiceInstanceResponseBodyService()
             self.service = temp_model.from_map(m['Service'])
@@ -2055,20 +2607,22 @@
 class ListServiceInstancesRequest(TeaModel):
     def __init__(
         self,
         filter: List[ListServiceInstancesRequestFilter] = None,
         max_results: str = None,
         next_token: str = None,
         region_id: str = None,
+        show_deleted: bool = None,
         tag: List[ListServiceInstancesRequestTag] = None,
     ):
         self.filter = filter
         self.max_results = max_results
         self.next_token = next_token
         self.region_id = region_id
+        self.show_deleted = show_deleted
         self.tag = tag
 
     def validate(self):
         if self.filter:
             for k in self.filter:
                 if k:
                     k.validate()
@@ -2089,14 +2643,16 @@
                 result['Filter'].append(k.to_map() if k else None)
         if self.max_results is not None:
             result['MaxResults'] = self.max_results
         if self.next_token is not None:
             result['NextToken'] = self.next_token
         if self.region_id is not None:
             result['RegionId'] = self.region_id
+        if self.show_deleted is not None:
+            result['ShowDeleted'] = self.show_deleted
         result['Tag'] = []
         if self.tag is not None:
             for k in self.tag:
                 result['Tag'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
@@ -2108,14 +2664,16 @@
                 self.filter.append(temp_model.from_map(k))
         if m.get('MaxResults') is not None:
             self.max_results = m.get('MaxResults')
         if m.get('NextToken') is not None:
             self.next_token = m.get('NextToken')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
+        if m.get('ShowDeleted') is not None:
+            self.show_deleted = m.get('ShowDeleted')
         self.tag = []
         if m.get('Tag') is not None:
             for k in m.get('Tag'):
                 temp_model = ListServiceInstancesRequestTag()
                 self.tag.append(temp_model.from_map(k))
         return self
 
@@ -2166,26 +2724,28 @@
 
 
 class ListServiceInstancesResponseBodyServiceInstancesService(TeaModel):
     def __init__(
         self,
         deploy_metadata: str = None,
         deploy_type: str = None,
+        enable_private_vpc_connection: bool = None,
         publish_time: str = None,
         service_id: str = None,
         service_infos: List[ListServiceInstancesResponseBodyServiceInstancesServiceServiceInfos] = None,
         service_type: str = None,
         status: str = None,
         supplier_name: str = None,
         supplier_url: str = None,
         version: str = None,
         version_name: str = None,
     ):
         self.deploy_metadata = deploy_metadata
         self.deploy_type = deploy_type
+        self.enable_private_vpc_connection = enable_private_vpc_connection
         self.publish_time = publish_time
         self.service_id = service_id
         self.service_infos = service_infos
         self.service_type = service_type
         self.status = status
         self.supplier_name = supplier_name
         self.supplier_url = supplier_url
@@ -2204,14 +2764,16 @@
             return _map
 
         result = dict()
         if self.deploy_metadata is not None:
             result['DeployMetadata'] = self.deploy_metadata
         if self.deploy_type is not None:
             result['DeployType'] = self.deploy_type
+        if self.enable_private_vpc_connection is not None:
+            result['EnablePrivateVpcConnection'] = self.enable_private_vpc_connection
         if self.publish_time is not None:
             result['PublishTime'] = self.publish_time
         if self.service_id is not None:
             result['ServiceId'] = self.service_id
         result['ServiceInfos'] = []
         if self.service_infos is not None:
             for k in self.service_infos:
@@ -2232,14 +2794,16 @@
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('DeployMetadata') is not None:
             self.deploy_metadata = m.get('DeployMetadata')
         if m.get('DeployType') is not None:
             self.deploy_type = m.get('DeployType')
+        if m.get('EnablePrivateVpcConnection') is not None:
+            self.enable_private_vpc_connection = m.get('EnablePrivateVpcConnection')
         if m.get('PublishTime') is not None:
             self.publish_time = m.get('PublishTime')
         if m.get('ServiceId') is not None:
             self.service_id = m.get('ServiceId')
         self.service_infos = []
         if m.get('ServiceInfos') is not None:
             for k in m.get('ServiceInfos'):
@@ -2879,14 +3443,511 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ListServiceUsagesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ListServicesRequestFilter(TeaModel):
+    def __init__(
+        self,
+        name: str = None,
+        value: List[str] = None,
+    ):
+        self.name = name
+        self.value = value
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
+        if self.name is not None:
+            result['Name'] = self.name
+        if self.value is not None:
+            result['Value'] = self.value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Name') is not None:
+            self.name = m.get('Name')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
+class ListServicesRequestTag(TeaModel):
+    def __init__(
+        self,
+        key: str = None,
+        value: str = None,
+    ):
+        self.key = key
+        self.value = value
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
+        if self.key is not None:
+            result['Key'] = self.key
+        if self.value is not None:
+            result['Value'] = self.value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Key') is not None:
+            self.key = m.get('Key')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
+class ListServicesRequest(TeaModel):
+    def __init__(
+        self,
+        all_versions: bool = None,
+        filter: List[ListServicesRequestFilter] = None,
+        max_results: str = None,
+        next_token: str = None,
+        region_id: str = None,
+        tag: List[ListServicesRequestTag] = None,
+    ):
+        self.all_versions = all_versions
+        self.filter = filter
+        self.max_results = max_results
+        self.next_token = next_token
+        self.region_id = region_id
+        self.tag = tag
+
+    def validate(self):
+        if self.filter:
+            for k in self.filter:
+                if k:
+                    k.validate()
+        if self.tag:
+            for k in self.tag:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.all_versions is not None:
+            result['AllVersions'] = self.all_versions
+        result['Filter'] = []
+        if self.filter is not None:
+            for k in self.filter:
+                result['Filter'].append(k.to_map() if k else None)
+        if self.max_results is not None:
+            result['MaxResults'] = self.max_results
+        if self.next_token is not None:
+            result['NextToken'] = self.next_token
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        result['Tag'] = []
+        if self.tag is not None:
+            for k in self.tag:
+                result['Tag'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('AllVersions') is not None:
+            self.all_versions = m.get('AllVersions')
+        self.filter = []
+        if m.get('Filter') is not None:
+            for k in m.get('Filter'):
+                temp_model = ListServicesRequestFilter()
+                self.filter.append(temp_model.from_map(k))
+        if m.get('MaxResults') is not None:
+            self.max_results = m.get('MaxResults')
+        if m.get('NextToken') is not None:
+            self.next_token = m.get('NextToken')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        self.tag = []
+        if m.get('Tag') is not None:
+            for k in m.get('Tag'):
+                temp_model = ListServicesRequestTag()
+                self.tag.append(temp_model.from_map(k))
+        return self
+
+
+class ListServicesResponseBodyServicesServiceInfos(TeaModel):
+    def __init__(
+        self,
+        image: str = None,
+        locale: str = None,
+        name: str = None,
+        short_description: str = None,
+    ):
+        self.image = image
+        self.locale = locale
+        self.name = name
+        self.short_description = short_description
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
+        if self.image is not None:
+            result['Image'] = self.image
+        if self.locale is not None:
+            result['Locale'] = self.locale
+        if self.name is not None:
+            result['Name'] = self.name
+        if self.short_description is not None:
+            result['ShortDescription'] = self.short_description
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Image') is not None:
+            self.image = m.get('Image')
+        if m.get('Locale') is not None:
+            self.locale = m.get('Locale')
+        if m.get('Name') is not None:
+            self.name = m.get('Name')
+        if m.get('ShortDescription') is not None:
+            self.short_description = m.get('ShortDescription')
+        return self
+
+
+class ListServicesResponseBodyServicesTags(TeaModel):
+    def __init__(
+        self,
+        key: str = None,
+        value: str = None,
+    ):
+        self.key = key
+        self.value = value
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
+        if self.key is not None:
+            result['Key'] = self.key
+        if self.value is not None:
+            result['Value'] = self.value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('Key') is not None:
+            self.key = m.get('Key')
+        if m.get('Value') is not None:
+            self.value = m.get('Value')
+        return self
+
+
+class ListServicesResponseBodyServices(TeaModel):
+    def __init__(
+        self,
+        approval_type: str = None,
+        artifact_id: str = None,
+        artifact_version: str = None,
+        commodity_code: str = None,
+        create_time: str = None,
+        default_version: bool = None,
+        deploy_type: str = None,
+        publish_time: str = None,
+        relation_type: str = None,
+        service_id: str = None,
+        service_infos: List[ListServicesResponseBodyServicesServiceInfos] = None,
+        service_type: str = None,
+        share_type: str = None,
+        source_image: str = None,
+        status: str = None,
+        supplier_name: str = None,
+        supplier_url: str = None,
+        tags: List[ListServicesResponseBodyServicesTags] = None,
+        tenant_type: str = None,
+        trial_type: str = None,
+        update_time: str = None,
+        version: str = None,
+        version_name: str = None,
+    ):
+        self.approval_type = approval_type
+        self.artifact_id = artifact_id
+        self.artifact_version = artifact_version
+        self.commodity_code = commodity_code
+        self.create_time = create_time
+        self.default_version = default_version
+        self.deploy_type = deploy_type
+        self.publish_time = publish_time
+        self.relation_type = relation_type
+        self.service_id = service_id
+        self.service_infos = service_infos
+        self.service_type = service_type
+        self.share_type = share_type
+        self.source_image = source_image
+        self.status = status
+        self.supplier_name = supplier_name
+        self.supplier_url = supplier_url
+        self.tags = tags
+        self.tenant_type = tenant_type
+        self.trial_type = trial_type
+        self.update_time = update_time
+        self.version = version
+        self.version_name = version_name
+
+    def validate(self):
+        if self.service_infos:
+            for k in self.service_infos:
+                if k:
+                    k.validate()
+        if self.tags:
+            for k in self.tags:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.approval_type is not None:
+            result['ApprovalType'] = self.approval_type
+        if self.artifact_id is not None:
+            result['ArtifactId'] = self.artifact_id
+        if self.artifact_version is not None:
+            result['ArtifactVersion'] = self.artifact_version
+        if self.commodity_code is not None:
+            result['CommodityCode'] = self.commodity_code
+        if self.create_time is not None:
+            result['CreateTime'] = self.create_time
+        if self.default_version is not None:
+            result['DefaultVersion'] = self.default_version
+        if self.deploy_type is not None:
+            result['DeployType'] = self.deploy_type
+        if self.publish_time is not None:
+            result['PublishTime'] = self.publish_time
+        if self.relation_type is not None:
+            result['RelationType'] = self.relation_type
+        if self.service_id is not None:
+            result['ServiceId'] = self.service_id
+        result['ServiceInfos'] = []
+        if self.service_infos is not None:
+            for k in self.service_infos:
+                result['ServiceInfos'].append(k.to_map() if k else None)
+        if self.service_type is not None:
+            result['ServiceType'] = self.service_type
+        if self.share_type is not None:
+            result['ShareType'] = self.share_type
+        if self.source_image is not None:
+            result['SourceImage'] = self.source_image
+        if self.status is not None:
+            result['Status'] = self.status
+        if self.supplier_name is not None:
+            result['SupplierName'] = self.supplier_name
+        if self.supplier_url is not None:
+            result['SupplierUrl'] = self.supplier_url
+        result['Tags'] = []
+        if self.tags is not None:
+            for k in self.tags:
+                result['Tags'].append(k.to_map() if k else None)
+        if self.tenant_type is not None:
+            result['TenantType'] = self.tenant_type
+        if self.trial_type is not None:
+            result['TrialType'] = self.trial_type
+        if self.update_time is not None:
+            result['UpdateTime'] = self.update_time
+        if self.version is not None:
+            result['Version'] = self.version
+        if self.version_name is not None:
+            result['VersionName'] = self.version_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('ApprovalType') is not None:
+            self.approval_type = m.get('ApprovalType')
+        if m.get('ArtifactId') is not None:
+            self.artifact_id = m.get('ArtifactId')
+        if m.get('ArtifactVersion') is not None:
+            self.artifact_version = m.get('ArtifactVersion')
+        if m.get('CommodityCode') is not None:
+            self.commodity_code = m.get('CommodityCode')
+        if m.get('CreateTime') is not None:
+            self.create_time = m.get('CreateTime')
+        if m.get('DefaultVersion') is not None:
+            self.default_version = m.get('DefaultVersion')
+        if m.get('DeployType') is not None:
+            self.deploy_type = m.get('DeployType')
+        if m.get('PublishTime') is not None:
+            self.publish_time = m.get('PublishTime')
+        if m.get('RelationType') is not None:
+            self.relation_type = m.get('RelationType')
+        if m.get('ServiceId') is not None:
+            self.service_id = m.get('ServiceId')
+        self.service_infos = []
+        if m.get('ServiceInfos') is not None:
+            for k in m.get('ServiceInfos'):
+                temp_model = ListServicesResponseBodyServicesServiceInfos()
+                self.service_infos.append(temp_model.from_map(k))
+        if m.get('ServiceType') is not None:
+            self.service_type = m.get('ServiceType')
+        if m.get('ShareType') is not None:
+            self.share_type = m.get('ShareType')
+        if m.get('SourceImage') is not None:
+            self.source_image = m.get('SourceImage')
+        if m.get('Status') is not None:
+            self.status = m.get('Status')
+        if m.get('SupplierName') is not None:
+            self.supplier_name = m.get('SupplierName')
+        if m.get('SupplierUrl') is not None:
+            self.supplier_url = m.get('SupplierUrl')
+        self.tags = []
+        if m.get('Tags') is not None:
+            for k in m.get('Tags'):
+                temp_model = ListServicesResponseBodyServicesTags()
+                self.tags.append(temp_model.from_map(k))
+        if m.get('TenantType') is not None:
+            self.tenant_type = m.get('TenantType')
+        if m.get('TrialType') is not None:
+            self.trial_type = m.get('TrialType')
+        if m.get('UpdateTime') is not None:
+            self.update_time = m.get('UpdateTime')
+        if m.get('Version') is not None:
+            self.version = m.get('Version')
+        if m.get('VersionName') is not None:
+            self.version_name = m.get('VersionName')
+        return self
+
+
+class ListServicesResponseBody(TeaModel):
+    def __init__(
+        self,
+        max_results: int = None,
+        next_token: str = None,
+        request_id: str = None,
+        services: List[ListServicesResponseBodyServices] = None,
+        total_count: str = None,
+    ):
+        self.max_results = max_results
+        self.next_token = next_token
+        self.request_id = request_id
+        self.services = services
+        self.total_count = total_count
+
+    def validate(self):
+        if self.services:
+            for k in self.services:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.max_results is not None:
+            result['MaxResults'] = self.max_results
+        if self.next_token is not None:
+            result['NextToken'] = self.next_token
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        result['Services'] = []
+        if self.services is not None:
+            for k in self.services:
+                result['Services'].append(k.to_map() if k else None)
+        if self.total_count is not None:
+            result['TotalCount'] = self.total_count
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('MaxResults') is not None:
+            self.max_results = m.get('MaxResults')
+        if m.get('NextToken') is not None:
+            self.next_token = m.get('NextToken')
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        self.services = []
+        if m.get('Services') is not None:
+            for k in m.get('Services'):
+                temp_model = ListServicesResponseBodyServices()
+                self.services.append(temp_model.from_map(k))
+        if m.get('TotalCount') is not None:
+            self.total_count = m.get('TotalCount')
+        return self
+
+
+class ListServicesResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ListServicesResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        self.validate_required(self.headers, 'headers')
+        self.validate_required(self.status_code, 'status_code')
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
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ListServicesResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class ReleaseArtifactRequest(TeaModel):
     def __init__(
         self,
         artifact_id: str = None,
     ):
         self.artifact_id = artifact_id
```

### Comparing `alibabacloud_computenestsupplier20210521-1.1.2/alibabacloud_computenestsupplier20210521.egg-info/PKG-INFO` & `alibabacloud_computenestsupplier20210521-1.2.0/alibabacloud_computenestsupplier20210521.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-computenestsupplier20210521
-Version: 1.1.2
+Version: 1.2.0
 Summary: Alibaba Cloud ComputeNestSupplier (20210521) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_computenestsupplier20210521-1.1.2/alibabacloud_computenestsupplier20210521.egg-info/SOURCES.txt` & `alibabacloud_computenestsupplier20210521-1.2.0/alibabacloud_computenestsupplier20210521.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud_computenestsupplier20210521-1.1.2/setup.py` & `alibabacloud_computenestsupplier20210521-1.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_computenestsupplier20210521.
 
-Created on 06/02/2023
+Created on 28/04/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_computenestsupplier20210521"
 NAME = "alibabacloud_computenestsupplier20210521" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud ComputeNestSupplier (20210521) SDK Library for Python"
```

