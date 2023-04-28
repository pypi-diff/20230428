# Comparing `tmp/aliyun-python-sdk-dytnsapi-1.1.4.tar.gz` & `tmp/aliyun-python-sdk-dytnsapi-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-dytnsapi-1.1.4.tar", last modified: Wed Mar  1 03:03:51 2023, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-dytnsapi-1.1.5.tar", last modified: Fri Apr 28 05:45:10 2023, max compression
```

## Comparing `aliyun-python-sdk-dytnsapi-1.1.4.tar` & `aliyun-python-sdk-dytnsapi-1.1.5.tar`

### file list

```diff
@@ -1,39 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-01 03:03:51.000000 aliyun-python-sdk-dytnsapi-1.1.4/
--rw-r--r--   0 root         (0) root         (0)      575 2023-03-01 03:03:50.000000 aliyun-python-sdk-dytnsapi-1.1.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2023-03-01 03:03:50.000000 aliyun-python-sdk-dytnsapi-1.1.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1562 2023-03-01 03:03:51.000000 aliyun-python-sdk-dytnsapi-1.1.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      537 2023-03-01 03:03:50.000000 aliyun-python-sdk-dytnsapi-1.1.4/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-01 03:03:51.000000 aliyun-python-sdk-dytnsapi-1.1.4/aliyun_python_sdk_dytnsapi.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1562 2023-03-01 03:03:51.000000 aliyun-python-sdk-dytnsapi-1.1.4/aliyun_python_sdk_dytnsapi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1820 2023-03-01 03:03:51.000000 aliyun-python-sdk-dytnsapi-1.1.4/aliyun_python_sdk_dytnsapi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-01 03:03:51.000000 aliyun-python-sdk-dytnsapi-1.1.4/aliyun_python_sdk_dytnsapi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-03-01 03:03:51.000000 aliyun-python-sdk-dytnsapi-1.1.4/aliyun_python_sdk_dytnsapi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-03-01 03:03:51.000000 aliyun-python-sdk-dytnsapi-1.1.4/aliyun_python_sdk_dytnsapi.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-01 03:03:51.000000 aliyun-python-sdk-dytnsapi-1.1.4/aliyunsdkdytnsapi/
--rw-r--r--   0 root         (0) root         (0)       21 2023-03-01 03:03:50.000000 aliyun-python-sdk-dytnsapi-1.1.4/aliyunsdkdytnsapi/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1087 2023-03-01 03:03:50.000000 aliyun-python-sdk-dytnsapi-1.1.4/aliyunsdkdytnsapi/endpoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-01 03:03:51.000000 aliyun-python-sdk-dytnsapi-1.1.4/aliyunsdkdytnsapi/request/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-01 03:03:50.000000 aliyun-python-sdk-dytnsapi-1.1.4/aliyunsdkdytnsapi/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-01 03:03:51.000000 aliyun-python-sdk-dytnsapi-1.1.4/aliyunsdkdytnsapi/request/v20200217/
--rw-r--r--   0 root         (0) root         (0)     2291 2023-03-01 03:03:50.000000 aliyun-python-sdk-dytnsapi-1.1.4/aliyunsdkdytnsapi/request/v20200217/DescribeEmptyNumberDetectRequest.py
--rw-r--r--   0 root         (0) root         (0)     2452 2023-03-01 03:03:50.000000 aliyun-python-sdk-dytnsapi-1.1.4/aliyunsdkdytnsapi/request/v20200217/DescribeEmptyNumberRequest.py
--rw-r--r--   0 root         (0) root         (0)     2812 2023-03-01 03:03:50.000000 aliyun-python-sdk-dytnsapi-1.1.4/aliyunsdkdytnsapi/request/v20200217/DescribePhoneNumberAnalysisRequest.py
--rw-r--r--   0 root         (0) root         (0)     2136 2023-03-01 03:03:50.000000 aliyun-python-sdk-dytnsapi-1.1.4/aliyunsdkdytnsapi/request/v20200217/DescribePhoneNumberAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2645 2023-03-01 03:03:50.000000 aliyun-python-sdk-dytnsapi-1.1.4/aliyunsdkdytnsapi/request/v20200217/DescribePhoneNumberOnlineTimeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2486 2023-03-01 03:03:50.000000 aliyun-python-sdk-dytnsapi-1.1.4/aliyunsdkdytnsapi/request/v20200217/DescribePhoneNumberOperatorAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2291 2023-03-01 03:03:50.000000 aliyun-python-sdk-dytnsapi-1.1.4/aliyunsdkdytnsapi/request/v20200217/DescribePhoneNumberResaleRequest.py
--rw-r--r--   0 root         (0) root         (0)     2130 2023-03-01 03:03:50.000000 aliyun-python-sdk-dytnsapi-1.1.4/aliyunsdkdytnsapi/request/v20200217/DescribePhoneNumberStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     2653 2023-03-01 03:03:50.000000 aliyun-python-sdk-dytnsapi-1.1.4/aliyunsdkdytnsapi/request/v20200217/DescribePhoneTwiceTelVerifyRequest.py
--rw-r--r--   0 root         (0) root         (0)     2462 2023-03-01 03:03:50.000000 aliyun-python-sdk-dytnsapi-1.1.4/aliyunsdkdytnsapi/request/v20200217/InvalidPhoneNumberFilterRequest.py
--rw-r--r--   0 root         (0) root         (0)     2450 2023-03-01 03:03:50.000000 aliyun-python-sdk-dytnsapi-1.1.4/aliyunsdkdytnsapi/request/v20200217/PhoneNumberEncryptRequest.py
--rw-r--r--   0 root         (0) root         (0)     2468 2023-03-01 03:03:50.000000 aliyun-python-sdk-dytnsapi-1.1.4/aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForAccountRequest.py
--rw-r--r--   0 root         (0) root         (0)     2466 2023-03-01 03:03:50.000000 aliyun-python-sdk-dytnsapi-1.1.4/aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForPublicRequest.py
--rw-r--r--   0 root         (0) root         (0)     2462 2023-03-01 03:03:50.000000 aliyun-python-sdk-dytnsapi-1.1.4/aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForRealRequest.py
--rw-r--r--   0 root         (0) root         (0)     2460 2023-03-01 03:03:50.000000 aliyun-python-sdk-dytnsapi-1.1.4/aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForSmsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2468 2023-03-01 03:03:50.000000 aliyun-python-sdk-dytnsapi-1.1.4/aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForVirtualRequest.py
--rw-r--r--   0 root         (0) root         (0)     2464 2023-03-01 03:03:50.000000 aliyun-python-sdk-dytnsapi-1.1.4/aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForVoiceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2798 2023-03-01 03:03:50.000000 aliyun-python-sdk-dytnsapi-1.1.4/aliyunsdkdytnsapi/request/v20200217/ThreeElementsVerificationRequest.py
--rw-r--r--   0 root         (0) root         (0)     2615 2023-03-01 03:03:50.000000 aliyun-python-sdk-dytnsapi-1.1.4/aliyunsdkdytnsapi/request/v20200217/TwoElementsVerificationRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-01 03:03:50.000000 aliyun-python-sdk-dytnsapi-1.1.4/aliyunsdkdytnsapi/request/v20200217/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2023-03-01 03:03:51.000000 aliyun-python-sdk-dytnsapi-1.1.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2477 2023-03-01 03:03:50.000000 aliyun-python-sdk-dytnsapi-1.1.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 05:45:10.000000 aliyun-python-sdk-dytnsapi-1.1.5/
+-rw-r--r--   0 root         (0) root         (0)      575 2023-04-28 05:45:10.000000 aliyun-python-sdk-dytnsapi-1.1.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2023-04-28 05:45:10.000000 aliyun-python-sdk-dytnsapi-1.1.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1562 2023-04-28 05:45:10.000000 aliyun-python-sdk-dytnsapi-1.1.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      537 2023-04-28 05:45:10.000000 aliyun-python-sdk-dytnsapi-1.1.5/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 05:45:10.000000 aliyun-python-sdk-dytnsapi-1.1.5/aliyun_python_sdk_dytnsapi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1562 2023-04-28 05:45:10.000000 aliyun-python-sdk-dytnsapi-1.1.5/aliyun_python_sdk_dytnsapi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1529 2023-04-28 05:45:10.000000 aliyun-python-sdk-dytnsapi-1.1.5/aliyun_python_sdk_dytnsapi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 05:45:10.000000 aliyun-python-sdk-dytnsapi-1.1.5/aliyun_python_sdk_dytnsapi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-04-28 05:45:10.000000 aliyun-python-sdk-dytnsapi-1.1.5/aliyun_python_sdk_dytnsapi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-04-28 05:45:10.000000 aliyun-python-sdk-dytnsapi-1.1.5/aliyun_python_sdk_dytnsapi.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 05:45:10.000000 aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-28 05:45:10.000000 aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1087 2023-04-28 05:45:10.000000 aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 05:45:10.000000 aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 05:45:10.000000 aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 05:45:10.000000 aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/request/v20200217/
+-rw-r--r--   0 root         (0) root         (0)     2667 2023-04-28 05:45:10.000000 aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/request/v20200217/DescribeEmptyNumberRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2812 2023-04-28 05:45:10.000000 aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/request/v20200217/DescribePhoneNumberAnalysisRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2860 2023-04-28 05:45:10.000000 aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/request/v20200217/DescribePhoneNumberOnlineTimeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2486 2023-04-28 05:45:10.000000 aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/request/v20200217/DescribePhoneNumberOperatorAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2868 2023-04-28 05:45:10.000000 aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/request/v20200217/DescribePhoneTwiceTelVerifyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-04-28 05:45:10.000000 aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/request/v20200217/InvalidPhoneNumberFilterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2450 2023-04-28 05:45:10.000000 aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/request/v20200217/PhoneNumberEncryptRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2683 2023-04-28 05:45:10.000000 aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForAccountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2466 2023-04-28 05:45:10.000000 aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForPublicRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2677 2023-04-28 05:45:10.000000 aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForRealRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2675 2023-04-28 05:45:10.000000 aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForSmsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2683 2023-04-28 05:45:10.000000 aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForVirtualRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2679 2023-04-28 05:45:10.000000 aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForVoiceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3013 2023-04-28 05:45:10.000000 aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/request/v20200217/ThreeElementsVerificationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2830 2023-04-28 05:45:10.000000 aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/request/v20200217/TwoElementsVerificationRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 05:45:10.000000 aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/request/v20200217/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2023-04-28 05:45:10.000000 aliyun-python-sdk-dytnsapi-1.1.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2477 2023-04-28 05:45:10.000000 aliyun-python-sdk-dytnsapi-1.1.5/setup.py
```

### Comparing `aliyun-python-sdk-dytnsapi-1.1.4/LICENSE` & `aliyun-python-sdk-dytnsapi-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dytnsapi-1.1.4/PKG-INFO` & `aliyun-python-sdk-dytnsapi-1.1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-dytnsapi
-Version: 1.1.4
+Version: 1.1.5
 Summary: The dytnsapi module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-dytnsapi
```

### Comparing `aliyun-python-sdk-dytnsapi-1.1.4/README.rst` & `aliyun-python-sdk-dytnsapi-1.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dytnsapi-1.1.4/aliyun_python_sdk_dytnsapi.egg-info/PKG-INFO` & `aliyun-python-sdk-dytnsapi-1.1.5/aliyun_python_sdk_dytnsapi.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-dytnsapi
-Version: 1.1.4
+Version: 1.1.5
 Summary: The dytnsapi module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-dytnsapi
```

### Comparing `aliyun-python-sdk-dytnsapi-1.1.4/aliyun_python_sdk_dytnsapi.egg-info/SOURCES.txt` & `aliyun-python-sdk-dytnsapi-1.1.5/aliyun_python_sdk_dytnsapi.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -7,22 +7,18 @@
 aliyun_python_sdk_dytnsapi.egg-info/SOURCES.txt
 aliyun_python_sdk_dytnsapi.egg-info/dependency_links.txt
 aliyun_python_sdk_dytnsapi.egg-info/requires.txt
 aliyun_python_sdk_dytnsapi.egg-info/top_level.txt
 aliyunsdkdytnsapi/__init__.py
 aliyunsdkdytnsapi/endpoint.py
 aliyunsdkdytnsapi/request/__init__.py
-aliyunsdkdytnsapi/request/v20200217/DescribeEmptyNumberDetectRequest.py
 aliyunsdkdytnsapi/request/v20200217/DescribeEmptyNumberRequest.py
 aliyunsdkdytnsapi/request/v20200217/DescribePhoneNumberAnalysisRequest.py
-aliyunsdkdytnsapi/request/v20200217/DescribePhoneNumberAttributeRequest.py
 aliyunsdkdytnsapi/request/v20200217/DescribePhoneNumberOnlineTimeRequest.py
 aliyunsdkdytnsapi/request/v20200217/DescribePhoneNumberOperatorAttributeRequest.py
-aliyunsdkdytnsapi/request/v20200217/DescribePhoneNumberResaleRequest.py
-aliyunsdkdytnsapi/request/v20200217/DescribePhoneNumberStatusRequest.py
 aliyunsdkdytnsapi/request/v20200217/DescribePhoneTwiceTelVerifyRequest.py
 aliyunsdkdytnsapi/request/v20200217/InvalidPhoneNumberFilterRequest.py
 aliyunsdkdytnsapi/request/v20200217/PhoneNumberEncryptRequest.py
 aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForAccountRequest.py
 aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForPublicRequest.py
 aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForRealRequest.py
 aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForSmsRequest.py
```

### Comparing `aliyun-python-sdk-dytnsapi-1.1.4/aliyunsdkdytnsapi/endpoint.py` & `aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/endpoint.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dytnsapi-1.1.4/aliyunsdkdytnsapi/request/v20200217/DescribeEmptyNumberDetectRequest.py` & `aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/request/v20200217/InvalidPhoneNumberFilterRequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,43 +16,48 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdytnsapi.endpoint import endpoint_data
 
-class DescribeEmptyNumberDetectRequest(RpcRequest):
+class InvalidPhoneNumberFilterRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Dytnsapi', '2020-02-17', 'DescribeEmptyNumberDetect')
+		RpcRequest.__init__(self, 'Dytnsapi', '2020-02-17', 'InvalidPhoneNumberFilter')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
 		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
-	def get_EncryptType(self): # String
-		return self.get_query_params().get('EncryptType')
+	def get_Mask(self): # String
+		return self.get_query_params().get('Mask')
 
-	def set_EncryptType(self, EncryptType):  # String
-		self.add_query_param('EncryptType', EncryptType)
+	def set_Mask(self, Mask):  # String
+		self.add_query_param('Mask', Mask)
 	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
 	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
 		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
 	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self, OwnerId):  # Long
 		self.add_query_param('OwnerId', OwnerId)
-	def get_Phone(self): # String
-		return self.get_query_params().get('Phone')
+	def get_AuthCode(self): # String
+		return self.get_query_params().get('AuthCode')
 
-	def set_Phone(self, Phone):  # String
-		self.add_query_param('Phone', Phone)
+	def set_AuthCode(self, AuthCode):  # String
+		self.add_query_param('AuthCode', AuthCode)
+	def get_InputNumber(self): # String
+		return self.get_query_params().get('InputNumber')
+
+	def set_InputNumber(self, InputNumber):  # String
+		self.add_query_param('InputNumber', InputNumber)
```

### Comparing `aliyun-python-sdk-dytnsapi-1.1.4/aliyunsdkdytnsapi/request/v20200217/DescribeEmptyNumberRequest.py` & `aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/request/v20200217/PhoneNumberEncryptRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdytnsapi.endpoint import endpoint_data
 
-class DescribeEmptyNumberRequest(RpcRequest):
+class PhoneNumberEncryptRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Dytnsapi', '2020-02-17', 'DescribeEmptyNumber')
+		RpcRequest.__init__(self, 'Dytnsapi', '2020-02-17', 'PhoneNumberEncrypt')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-dytnsapi-1.1.4/aliyunsdkdytnsapi/request/v20200217/DescribePhoneNumberAnalysisRequest.py` & `aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/request/v20200217/DescribePhoneNumberAnalysisRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dytnsapi-1.1.4/aliyunsdkdytnsapi/request/v20200217/DescribePhoneNumberAttributeRequest.py` & `aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/request/v20200217/DescribeEmptyNumberRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,38 +16,53 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdytnsapi.endpoint import endpoint_data
 
-class DescribePhoneNumberAttributeRequest(RpcRequest):
+class DescribeEmptyNumberRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Dytnsapi', '2020-02-17', 'DescribePhoneNumberAttribute')
+		RpcRequest.__init__(self, 'Dytnsapi', '2020-02-17', 'DescribeEmptyNumber')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
 		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_ExtendFunction(self): # String
+		return self.get_query_params().get('ExtendFunction')
+
+	def set_ExtendFunction(self, ExtendFunction):  # String
+		self.add_query_param('ExtendFunction', ExtendFunction)
+	def get_Mask(self): # String
+		return self.get_query_params().get('Mask')
+
+	def set_Mask(self, Mask):  # String
+		self.add_query_param('Mask', Mask)
 	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
 	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
 		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
-	def get_PhoneNumber(self): # String
-		return self.get_query_params().get('PhoneNumber')
-
-	def set_PhoneNumber(self, PhoneNumber):  # String
-		self.add_query_param('PhoneNumber', PhoneNumber)
 	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self, OwnerId):  # Long
 		self.add_query_param('OwnerId', OwnerId)
+	def get_AuthCode(self): # String
+		return self.get_query_params().get('AuthCode')
+
+	def set_AuthCode(self, AuthCode):  # String
+		self.add_query_param('AuthCode', AuthCode)
+	def get_InputNumber(self): # String
+		return self.get_query_params().get('InputNumber')
+
+	def set_InputNumber(self, InputNumber):  # String
+		self.add_query_param('InputNumber', InputNumber)
```

### Comparing `aliyun-python-sdk-dytnsapi-1.1.4/aliyunsdkdytnsapi/request/v20200217/DescribePhoneNumberOnlineTimeRequest.py` & `aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/request/v20200217/ThreeElementsVerificationRequest.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,30 +16,40 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdytnsapi.endpoint import endpoint_data
 
-class DescribePhoneNumberOnlineTimeRequest(RpcRequest):
+class ThreeElementsVerificationRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Dytnsapi', '2020-02-17', 'DescribePhoneNumberOnlineTime')
+		RpcRequest.__init__(self, 'Dytnsapi', '2020-02-17', 'ThreeElementsVerification')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
 		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_ExtendFunction(self): # String
+		return self.get_query_params().get('ExtendFunction')
+
+	def set_ExtendFunction(self, ExtendFunction):  # String
+		self.add_query_param('ExtendFunction', ExtendFunction)
+	def get_CertCode(self): # String
+		return self.get_query_params().get('CertCode')
+
+	def set_CertCode(self, CertCode):  # String
+		self.add_query_param('CertCode', CertCode)
 	def get_Mask(self): # String
 		return self.get_query_params().get('Mask')
 
 	def set_Mask(self, Mask):  # String
 		self.add_query_param('Mask', Mask)
 	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
@@ -57,12 +67,12 @@
 	def set_AuthCode(self, AuthCode):  # String
 		self.add_query_param('AuthCode', AuthCode)
 	def get_InputNumber(self): # String
 		return self.get_query_params().get('InputNumber')
 
 	def set_InputNumber(self, InputNumber):  # String
 		self.add_query_param('InputNumber', InputNumber)
-	def get_Carrier(self): # String
-		return self.get_query_params().get('Carrier')
+	def get_Name(self): # String
+		return self.get_query_params().get('Name')
 
-	def set_Carrier(self, Carrier):  # String
-		self.add_query_param('Carrier', Carrier)
+	def set_Name(self, Name):  # String
+		self.add_query_param('Name', Name)
```

### Comparing `aliyun-python-sdk-dytnsapi-1.1.4/aliyunsdkdytnsapi/request/v20200217/DescribePhoneNumberOperatorAttributeRequest.py` & `aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/request/v20200217/DescribePhoneNumberOperatorAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-dytnsapi-1.1.4/aliyunsdkdytnsapi/request/v20200217/DescribePhoneNumberResaleRequest.py` & `aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForVirtualRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,43 +16,53 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdytnsapi.endpoint import endpoint_data
 
-class DescribePhoneNumberResaleRequest(RpcRequest):
+class PhoneNumberStatusForVirtualRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Dytnsapi', '2020-02-17', 'DescribePhoneNumberResale')
+		RpcRequest.__init__(self, 'Dytnsapi', '2020-02-17', 'PhoneNumberStatusForVirtual')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
 		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_ExtendFunction(self): # String
+		return self.get_query_params().get('ExtendFunction')
+
+	def set_ExtendFunction(self, ExtendFunction):  # String
+		self.add_query_param('ExtendFunction', ExtendFunction)
+	def get_Mask(self): # String
+		return self.get_query_params().get('Mask')
+
+	def set_Mask(self, Mask):  # String
+		self.add_query_param('Mask', Mask)
 	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
 	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
 		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
-	def get_PhoneNumber(self): # String
-		return self.get_query_params().get('PhoneNumber')
-
-	def set_PhoneNumber(self, PhoneNumber):  # String
-		self.add_query_param('PhoneNumber', PhoneNumber)
 	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self, OwnerId):  # Long
 		self.add_query_param('OwnerId', OwnerId)
-	def get_Since(self): # String
-		return self.get_query_params().get('Since')
+	def get_AuthCode(self): # String
+		return self.get_query_params().get('AuthCode')
+
+	def set_AuthCode(self, AuthCode):  # String
+		self.add_query_param('AuthCode', AuthCode)
+	def get_InputNumber(self): # String
+		return self.get_query_params().get('InputNumber')
 
-	def set_Since(self, Since):  # String
-		self.add_query_param('Since', Since)
+	def set_InputNumber(self, InputNumber):  # String
+		self.add_query_param('InputNumber', InputNumber)
```

### Comparing `aliyun-python-sdk-dytnsapi-1.1.4/aliyunsdkdytnsapi/request/v20200217/DescribePhoneNumberStatusRequest.py` & `aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForPublicRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,38 +16,48 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdytnsapi.endpoint import endpoint_data
 
-class DescribePhoneNumberStatusRequest(RpcRequest):
+class PhoneNumberStatusForPublicRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Dytnsapi', '2020-02-17', 'DescribePhoneNumberStatus')
+		RpcRequest.__init__(self, 'Dytnsapi', '2020-02-17', 'PhoneNumberStatusForPublic')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
 		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_Mask(self): # String
+		return self.get_query_params().get('Mask')
+
+	def set_Mask(self, Mask):  # String
+		self.add_query_param('Mask', Mask)
 	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
 
 	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
 		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
-	def get_PhoneNumber(self): # String
-		return self.get_query_params().get('PhoneNumber')
-
-	def set_PhoneNumber(self, PhoneNumber):  # String
-		self.add_query_param('PhoneNumber', PhoneNumber)
 	def get_OwnerId(self): # Long
 		return self.get_query_params().get('OwnerId')
 
 	def set_OwnerId(self, OwnerId):  # Long
 		self.add_query_param('OwnerId', OwnerId)
+	def get_AuthCode(self): # String
+		return self.get_query_params().get('AuthCode')
+
+	def set_AuthCode(self, AuthCode):  # String
+		self.add_query_param('AuthCode', AuthCode)
+	def get_InputNumber(self): # String
+		return self.get_query_params().get('InputNumber')
+
+	def set_InputNumber(self, InputNumber):  # String
+		self.add_query_param('InputNumber', InputNumber)
```

### Comparing `aliyun-python-sdk-dytnsapi-1.1.4/aliyunsdkdytnsapi/request/v20200217/DescribePhoneTwiceTelVerifyRequest.py` & `aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForRealRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,35 +16,35 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdytnsapi.endpoint import endpoint_data
 
-class DescribePhoneTwiceTelVerifyRequest(RpcRequest):
+class PhoneNumberStatusForRealRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Dytnsapi', '2020-02-17', 'DescribePhoneTwiceTelVerify')
+		RpcRequest.__init__(self, 'Dytnsapi', '2020-02-17', 'PhoneNumberStatusForReal')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
 		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
-	def get_StartTime(self): # String
-		return self.get_query_params().get('StartTime')
+	def get_ExtendFunction(self): # String
+		return self.get_query_params().get('ExtendFunction')
 
-	def set_StartTime(self, StartTime):  # String
-		self.add_query_param('StartTime', StartTime)
+	def set_ExtendFunction(self, ExtendFunction):  # String
+		self.add_query_param('ExtendFunction', ExtendFunction)
 	def get_Mask(self): # String
 		return self.get_query_params().get('Mask')
 
 	def set_Mask(self, Mask):  # String
 		self.add_query_param('Mask', Mask)
 	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
```

### Comparing `aliyun-python-sdk-dytnsapi-1.1.4/aliyunsdkdytnsapi/request/v20200217/InvalidPhoneNumberFilterRequest.py` & `aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForSmsRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,30 +16,35 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdytnsapi.endpoint import endpoint_data
 
-class InvalidPhoneNumberFilterRequest(RpcRequest):
+class PhoneNumberStatusForSmsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Dytnsapi', '2020-02-17', 'InvalidPhoneNumberFilter')
+		RpcRequest.__init__(self, 'Dytnsapi', '2020-02-17', 'PhoneNumberStatusForSms')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
 		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_ExtendFunction(self): # String
+		return self.get_query_params().get('ExtendFunction')
+
+	def set_ExtendFunction(self, ExtendFunction):  # String
+		self.add_query_param('ExtendFunction', ExtendFunction)
 	def get_Mask(self): # String
 		return self.get_query_params().get('Mask')
 
 	def set_Mask(self, Mask):  # String
 		self.add_query_param('Mask', Mask)
 	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
```

### Comparing `aliyun-python-sdk-dytnsapi-1.1.4/aliyunsdkdytnsapi/request/v20200217/PhoneNumberEncryptRequest.py` & `aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForAccountRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,30 +16,35 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdytnsapi.endpoint import endpoint_data
 
-class PhoneNumberEncryptRequest(RpcRequest):
+class PhoneNumberStatusForAccountRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Dytnsapi', '2020-02-17', 'PhoneNumberEncrypt')
+		RpcRequest.__init__(self, 'Dytnsapi', '2020-02-17', 'PhoneNumberStatusForAccount')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
 		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_ExtendFunction(self): # String
+		return self.get_query_params().get('ExtendFunction')
+
+	def set_ExtendFunction(self, ExtendFunction):  # String
+		self.add_query_param('ExtendFunction', ExtendFunction)
 	def get_Mask(self): # String
 		return self.get_query_params().get('Mask')
 
 	def set_Mask(self, Mask):  # String
 		self.add_query_param('Mask', Mask)
 	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
```

### Comparing `aliyun-python-sdk-dytnsapi-1.1.4/aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForAccountRequest.py` & `aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForVoiceRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,30 +16,35 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdytnsapi.endpoint import endpoint_data
 
-class PhoneNumberStatusForAccountRequest(RpcRequest):
+class PhoneNumberStatusForVoiceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Dytnsapi', '2020-02-17', 'PhoneNumberStatusForAccount')
+		RpcRequest.__init__(self, 'Dytnsapi', '2020-02-17', 'PhoneNumberStatusForVoice')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
 		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_ExtendFunction(self): # String
+		return self.get_query_params().get('ExtendFunction')
+
+	def set_ExtendFunction(self, ExtendFunction):  # String
+		self.add_query_param('ExtendFunction', ExtendFunction)
 	def get_Mask(self): # String
 		return self.get_query_params().get('Mask')
 
 	def set_Mask(self, Mask):  # String
 		self.add_query_param('Mask', Mask)
 	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
```

### Comparing `aliyun-python-sdk-dytnsapi-1.1.4/aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForPublicRequest.py` & `aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/request/v20200217/DescribePhoneTwiceTelVerifyRequest.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,30 +16,40 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdytnsapi.endpoint import endpoint_data
 
-class PhoneNumberStatusForPublicRequest(RpcRequest):
+class DescribePhoneTwiceTelVerifyRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Dytnsapi', '2020-02-17', 'PhoneNumberStatusForPublic')
+		RpcRequest.__init__(self, 'Dytnsapi', '2020-02-17', 'DescribePhoneTwiceTelVerify')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
 		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_StartTime(self): # String
+		return self.get_query_params().get('StartTime')
+
+	def set_StartTime(self, StartTime):  # String
+		self.add_query_param('StartTime', StartTime)
+	def get_ExtendFunction(self): # String
+		return self.get_query_params().get('ExtendFunction')
+
+	def set_ExtendFunction(self, ExtendFunction):  # String
+		self.add_query_param('ExtendFunction', ExtendFunction)
 	def get_Mask(self): # String
 		return self.get_query_params().get('Mask')
 
 	def set_Mask(self, Mask):  # String
 		self.add_query_param('Mask', Mask)
 	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
```

### Comparing `aliyun-python-sdk-dytnsapi-1.1.4/aliyunsdkdytnsapi/request/v20200217/PhoneNumberStatusForSmsRequest.py` & `aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/request/v20200217/TwoElementsVerificationRequest.py`

 * *Files 27% similar despite different names*

```diff
@@ -16,30 +16,35 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdytnsapi.endpoint import endpoint_data
 
-class PhoneNumberStatusForSmsRequest(RpcRequest):
+class TwoElementsVerificationRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Dytnsapi', '2020-02-17', 'PhoneNumberStatusForSms')
+		RpcRequest.__init__(self, 'Dytnsapi', '2020-02-17', 'TwoElementsVerification')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
 		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
+	def get_ExtendFunction(self): # String
+		return self.get_query_params().get('ExtendFunction')
+
+	def set_ExtendFunction(self, ExtendFunction):  # String
+		self.add_query_param('ExtendFunction', ExtendFunction)
 	def get_Mask(self): # String
 		return self.get_query_params().get('Mask')
 
 	def set_Mask(self, Mask):  # String
 		self.add_query_param('Mask', Mask)
 	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
@@ -57,7 +62,12 @@
 	def set_AuthCode(self, AuthCode):  # String
 		self.add_query_param('AuthCode', AuthCode)
 	def get_InputNumber(self): # String
 		return self.get_query_params().get('InputNumber')
 
 	def set_InputNumber(self, InputNumber):  # String
 		self.add_query_param('InputNumber', InputNumber)
+	def get_Name(self): # String
+		return self.get_query_params().get('Name')
+
+	def set_Name(self, Name):  # String
+		self.add_query_param('Name', Name)
```

### Comparing `aliyun-python-sdk-dytnsapi-1.1.4/aliyunsdkdytnsapi/request/v20200217/ThreeElementsVerificationRequest.py` & `aliyun-python-sdk-dytnsapi-1.1.5/aliyunsdkdytnsapi/request/v20200217/DescribePhoneNumberOnlineTimeRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,35 +16,35 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkdytnsapi.endpoint import endpoint_data
 
-class ThreeElementsVerificationRequest(RpcRequest):
+class DescribePhoneNumberOnlineTimeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Dytnsapi', '2020-02-17', 'ThreeElementsVerification')
+		RpcRequest.__init__(self, 'Dytnsapi', '2020-02-17', 'DescribePhoneNumberOnlineTime')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 	def get_ResourceOwnerId(self): # Long
 		return self.get_query_params().get('ResourceOwnerId')
 
 	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
 		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
-	def get_CertCode(self): # String
-		return self.get_query_params().get('CertCode')
+	def get_ExtendFunction(self): # String
+		return self.get_query_params().get('ExtendFunction')
 
-	def set_CertCode(self, CertCode):  # String
-		self.add_query_param('CertCode', CertCode)
+	def set_ExtendFunction(self, ExtendFunction):  # String
+		self.add_query_param('ExtendFunction', ExtendFunction)
 	def get_Mask(self): # String
 		return self.get_query_params().get('Mask')
 
 	def set_Mask(self, Mask):  # String
 		self.add_query_param('Mask', Mask)
 	def get_ResourceOwnerAccount(self): # String
 		return self.get_query_params().get('ResourceOwnerAccount')
@@ -62,12 +62,12 @@
 	def set_AuthCode(self, AuthCode):  # String
 		self.add_query_param('AuthCode', AuthCode)
 	def get_InputNumber(self): # String
 		return self.get_query_params().get('InputNumber')
 
 	def set_InputNumber(self, InputNumber):  # String
 		self.add_query_param('InputNumber', InputNumber)
-	def get_Name(self): # String
-		return self.get_query_params().get('Name')
+	def get_Carrier(self): # String
+		return self.get_query_params().get('Carrier')
 
-	def set_Name(self, Name):  # String
-		self.add_query_param('Name', Name)
+	def set_Carrier(self, Carrier):  # String
+		self.add_query_param('Carrier', Carrier)
```

### Comparing `aliyun-python-sdk-dytnsapi-1.1.4/setup.py` & `aliyun-python-sdk-dytnsapi-1.1.5/setup.py`

 * *Files identical despite different names*

