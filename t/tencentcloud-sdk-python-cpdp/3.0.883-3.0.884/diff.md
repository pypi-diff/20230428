# Comparing `tmp/tencentcloud-sdk-python-cpdp-3.0.883.tar.gz` & `tmp/tencentcloud-sdk-python-cpdp-3.0.884.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cpdp-3.0.883.tar", last modified: Thu Apr 27 00:26:15 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cpdp-3.0.884.tar", last modified: Fri Apr 28 02:10:06 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cpdp-3.0.883.tar` & `tencentcloud-sdk-python-cpdp-3.0.884.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:26:15.000000 tencentcloud-sdk-python-cpdp-3.0.883/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:26:15.000000 tencentcloud-sdk-python-cpdp-3.0.883/tencentcloud_sdk_python_cpdp.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 00:26:15.000000 tencentcloud-sdk-python-cpdp-3.0.883/tencentcloud_sdk_python_cpdp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-04-27 00:26:15.000000 tencentcloud-sdk-python-cpdp-3.0.883/tencentcloud_sdk_python_cpdp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-04-27 00:26:15.000000 tencentcloud-sdk-python-cpdp-3.0.883/tencentcloud_sdk_python_cpdp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-27 00:26:15.000000 tencentcloud-sdk-python-cpdp-3.0.883/tencentcloud_sdk_python_cpdp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      740 2023-04-27 00:26:15.000000 tencentcloud-sdk-python-cpdp-3.0.883/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:26:15.000000 tencentcloud-sdk-python-cpdp-3.0.883/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-27 00:26:15.000000 tencentcloud-sdk-python-cpdp-3.0.883/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:26:15.000000 tencentcloud-sdk-python-cpdp-3.0.883/tencentcloud/cpdp/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 00:26:15.000000 tencentcloud-sdk-python-cpdp-3.0.883/tencentcloud/cpdp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:26:15.000000 tencentcloud-sdk-python-cpdp-3.0.883/tencentcloud/cpdp/v20190820/
--rw-r--r--   0 root         (0) root         (0)   208899 2023-04-27 00:26:15.000000 tencentcloud-sdk-python-cpdp-3.0.883/tencentcloud/cpdp/v20190820/cpdp_client.py
--rw-r--r--   0 root         (0) root         (0)    19183 2023-04-27 00:26:15.000000 tencentcloud-sdk-python-cpdp-3.0.883/tencentcloud/cpdp/v20190820/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 00:26:15.000000 tencentcloud-sdk-python-cpdp-3.0.883/tencentcloud/cpdp/v20190820/__init__.py
--rw-r--r--   0 root         (0) root         (0)  1213614 2023-04-27 00:26:15.000000 tencentcloud-sdk-python-cpdp-3.0.883/tencentcloud/cpdp/v20190820/models.py
--rw-r--r--   0 root         (0) root         (0)     1664 2023-04-27 00:26:15.000000 tencentcloud-sdk-python-cpdp-3.0.883/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-04-27 00:26:15.000000 tencentcloud-sdk-python-cpdp-3.0.883/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-27 00:26:15.000000 tencentcloud-sdk-python-cpdp-3.0.883/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:10:06.000000 tencentcloud-sdk-python-cpdp-3.0.884/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:10:06.000000 tencentcloud-sdk-python-cpdp-3.0.884/tencentcloud_sdk_python_cpdp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 02:10:06.000000 tencentcloud-sdk-python-cpdp-3.0.884/tencentcloud_sdk_python_cpdp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-04-28 02:10:06.000000 tencentcloud-sdk-python-cpdp-3.0.884/tencentcloud_sdk_python_cpdp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-04-28 02:10:06.000000 tencentcloud-sdk-python-cpdp-3.0.884/tencentcloud_sdk_python_cpdp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-28 02:10:06.000000 tencentcloud-sdk-python-cpdp-3.0.884/tencentcloud_sdk_python_cpdp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      740 2023-04-28 02:10:06.000000 tencentcloud-sdk-python-cpdp-3.0.884/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:10:06.000000 tencentcloud-sdk-python-cpdp-3.0.884/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-28 02:10:06.000000 tencentcloud-sdk-python-cpdp-3.0.884/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:10:06.000000 tencentcloud-sdk-python-cpdp-3.0.884/tencentcloud/cpdp/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 02:10:06.000000 tencentcloud-sdk-python-cpdp-3.0.884/tencentcloud/cpdp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:10:06.000000 tencentcloud-sdk-python-cpdp-3.0.884/tencentcloud/cpdp/v20190820/
+-rw-r--r--   0 root         (0) root         (0)   208899 2023-04-28 02:10:06.000000 tencentcloud-sdk-python-cpdp-3.0.884/tencentcloud/cpdp/v20190820/cpdp_client.py
+-rw-r--r--   0 root         (0) root         (0)    19183 2023-04-28 02:10:06.000000 tencentcloud-sdk-python-cpdp-3.0.884/tencentcloud/cpdp/v20190820/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 02:10:06.000000 tencentcloud-sdk-python-cpdp-3.0.884/tencentcloud/cpdp/v20190820/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  1213952 2023-04-28 02:10:06.000000 tencentcloud-sdk-python-cpdp-3.0.884/tencentcloud/cpdp/v20190820/models.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-04-28 02:10:06.000000 tencentcloud-sdk-python-cpdp-3.0.884/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-04-28 02:10:06.000000 tencentcloud-sdk-python-cpdp-3.0.884/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-28 02:10:06.000000 tencentcloud-sdk-python-cpdp-3.0.884/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cpdp-3.0.883/tencentcloud_sdk_python_cpdp.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cpdp-3.0.884/tencentcloud_sdk_python_cpdp.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cpdp
-Version: 3.0.883
+Version: 3.0.884
 Summary: Tencent Cloud Cpdp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cpdp-3.0.883/README.rst` & `tencentcloud-sdk-python-cpdp-3.0.884/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cpdp-3.0.883/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cpdp-3.0.884/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.883'
+__version__ = '3.0.884'
```

### Comparing `tencentcloud-sdk-python-cpdp-3.0.883/tencentcloud/cpdp/v20190820/cpdp_client.py` & `tencentcloud-sdk-python-cpdp-3.0.884/tencentcloud/cpdp/v20190820/cpdp_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cpdp-3.0.883/tencentcloud/cpdp/v20190820/errorcodes.py` & `tencentcloud-sdk-python-cpdp-3.0.884/tencentcloud/cpdp/v20190820/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cpdp-3.0.883/tencentcloud/cpdp/v20190820/models.py` & `tencentcloud-sdk-python-cpdp-3.0.884/tencentcloud/cpdp/v20190820/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -16047,14 +16047,17 @@
         :type AdditionalTaxSum: str
         :param AdditionalTaxItem: 附加税税项。格式为JSON格式
 注意：此字段可能返回 null，表示取不到有效值。
         :type AdditionalTaxItem: str
         :param FailReason: 失败原因。当Status为FAILED时，改字段为失败的原因。
 注意：此字段可能返回 null，表示取不到有效值。
         :type FailReason: str
+        :param FundingAccountSubType: 资金账户字类型: WECHATPAY_ACCOUNT 微信零钱, BANK_ACCOUNT 银行卡
+注意：此字段可能返回 null，表示取不到有效值。
+        :type FundingAccountSubType: str
         """
         self.IncomeType = None
         self.AmountBeforeTax = None
         self.AmountAfterTax = None
         self.Tax = None
         self.OutOrderId = None
         self.OrderId = None
@@ -16067,14 +16070,15 @@
         self.OutUserId = None
         self.ChannelOrderId = None
         self.Vat = None
         self.IndividualIncomeTax = None
         self.AdditionalTaxSum = None
         self.AdditionalTaxItem = None
         self.FailReason = None
+        self.FundingAccountSubType = None
 
 
     def _deserialize(self, params):
         self.IncomeType = params.get("IncomeType")
         self.AmountBeforeTax = params.get("AmountBeforeTax")
         self.AmountAfterTax = params.get("AmountAfterTax")
         self.Tax = params.get("Tax")
@@ -16089,14 +16093,15 @@
         self.OutUserId = params.get("OutUserId")
         self.ChannelOrderId = params.get("ChannelOrderId")
         self.Vat = params.get("Vat")
         self.IndividualIncomeTax = params.get("IndividualIncomeTax")
         self.AdditionalTaxSum = params.get("AdditionalTaxSum")
         self.AdditionalTaxItem = params.get("AdditionalTaxItem")
         self.FailReason = params.get("FailReason")
+        self.FundingAccountSubType = params.get("FundingAccountSubType")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-cpdp-3.0.883/PKG-INFO` & `tencentcloud-sdk-python-cpdp-3.0.884/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cpdp
-Version: 3.0.883
+Version: 3.0.884
 Summary: Tencent Cloud Cpdp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cpdp-3.0.883/setup.py` & `tencentcloud-sdk-python-cpdp-3.0.884/setup.py`

 * *Files identical despite different names*

