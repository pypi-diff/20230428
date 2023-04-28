# Comparing `tmp/tencentcloud-sdk-python-waf-3.0.883.tar.gz` & `tmp/tencentcloud-sdk-python-waf-3.0.884.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-waf-3.0.883.tar", last modified: Thu Apr 27 01:03:33 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-waf-3.0.884.tar", last modified: Fri Apr 28 02:47:43 2023, max compression
```

## Comparing `tencentcloud-sdk-python-waf-3.0.883.tar` & `tencentcloud-sdk-python-waf-3.0.884.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 01:03:33.000000 tencentcloud-sdk-python-waf-3.0.883/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-27 01:03:33.000000 tencentcloud-sdk-python-waf-3.0.883/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 01:03:33.000000 tencentcloud-sdk-python-waf-3.0.883/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 01:03:33.000000 tencentcloud-sdk-python-waf-3.0.883/tencentcloud/waf/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 01:03:33.000000 tencentcloud-sdk-python-waf-3.0.883/tencentcloud/waf/v20180125/
--rw-r--r--   0 root         (0) root         (0)    46564 2023-04-27 01:03:33.000000 tencentcloud-sdk-python-waf-3.0.883/tencentcloud/waf/v20180125/waf_client.py
--rw-r--r--   0 root         (0) root         (0)     2146 2023-04-27 01:03:33.000000 tencentcloud-sdk-python-waf-3.0.883/tencentcloud/waf/v20180125/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 01:03:33.000000 tencentcloud-sdk-python-waf-3.0.883/tencentcloud/waf/v20180125/__init__.py
--rw-r--r--   0 root         (0) root         (0)   179442 2023-04-27 01:03:33.000000 tencentcloud-sdk-python-waf-3.0.883/tencentcloud/waf/v20180125/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 01:03:33.000000 tencentcloud-sdk-python-waf-3.0.883/tencentcloud/waf/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-27 01:03:33.000000 tencentcloud-sdk-python-waf-3.0.883/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-27 01:03:33.000000 tencentcloud-sdk-python-waf-3.0.883/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-27 01:03:33.000000 tencentcloud-sdk-python-waf-3.0.883/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-27 01:03:33.000000 tencentcloud-sdk-python-waf-3.0.883/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 01:03:33.000000 tencentcloud-sdk-python-waf-3.0.883/tencentcloud_sdk_python_waf.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 01:03:33.000000 tencentcloud-sdk-python-waf-3.0.883/tencentcloud_sdk_python_waf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-27 01:03:33.000000 tencentcloud-sdk-python-waf-3.0.883/tencentcloud_sdk_python_waf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-27 01:03:33.000000 tencentcloud-sdk-python-waf-3.0.883/tencentcloud_sdk_python_waf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-27 01:03:33.000000 tencentcloud-sdk-python-waf-3.0.883/tencentcloud_sdk_python_waf.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:47:43.000000 tencentcloud-sdk-python-waf-3.0.884/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-28 02:47:43.000000 tencentcloud-sdk-python-waf-3.0.884/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:47:43.000000 tencentcloud-sdk-python-waf-3.0.884/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:47:43.000000 tencentcloud-sdk-python-waf-3.0.884/tencentcloud/waf/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:47:43.000000 tencentcloud-sdk-python-waf-3.0.884/tencentcloud/waf/v20180125/
+-rw-r--r--   0 root         (0) root         (0)    46564 2023-04-28 02:47:43.000000 tencentcloud-sdk-python-waf-3.0.884/tencentcloud/waf/v20180125/waf_client.py
+-rw-r--r--   0 root         (0) root         (0)     2419 2023-04-28 02:47:43.000000 tencentcloud-sdk-python-waf-3.0.884/tencentcloud/waf/v20180125/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 02:47:43.000000 tencentcloud-sdk-python-waf-3.0.884/tencentcloud/waf/v20180125/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   180081 2023-04-28 02:47:43.000000 tencentcloud-sdk-python-waf-3.0.884/tencentcloud/waf/v20180125/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 02:47:43.000000 tencentcloud-sdk-python-waf-3.0.884/tencentcloud/waf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-28 02:47:43.000000 tencentcloud-sdk-python-waf-3.0.884/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-28 02:47:43.000000 tencentcloud-sdk-python-waf-3.0.884/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-28 02:47:43.000000 tencentcloud-sdk-python-waf-3.0.884/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-28 02:47:43.000000 tencentcloud-sdk-python-waf-3.0.884/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:47:43.000000 tencentcloud-sdk-python-waf-3.0.884/tencentcloud_sdk_python_waf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 02:47:43.000000 tencentcloud-sdk-python-waf-3.0.884/tencentcloud_sdk_python_waf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-28 02:47:43.000000 tencentcloud-sdk-python-waf-3.0.884/tencentcloud_sdk_python_waf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-28 02:47:43.000000 tencentcloud-sdk-python-waf-3.0.884/tencentcloud_sdk_python_waf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-28 02:47:43.000000 tencentcloud-sdk-python-waf-3.0.884/tencentcloud_sdk_python_waf.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-waf-3.0.883/README.rst` & `tencentcloud-sdk-python-waf-3.0.884/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-waf-3.0.883/tencentcloud/waf/v20180125/waf_client.py` & `tencentcloud-sdk-python-waf-3.0.884/tencentcloud/waf/v20180125/waf_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-waf-3.0.883/tencentcloud/waf/v20180125/errorcodes.py` & `tencentcloud-sdk-python-waf-3.0.884/tencentcloud/waf/v20180125/errorcodes.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,17 +22,26 @@
 
 # 操作失败。
 FAILEDOPERATION = 'FailedOperation'
 
 # CLS内部错误。
 FAILEDOPERATION_CLSINTERNALERROR = 'FailedOperation.CLSInternalError'
 
+# 操作Mysql数据库失败
+FAILEDOPERATION_MYSQLDBOPERATIONFAILED = 'FailedOperation.MysqlDBOperationFailed'
+
+# 操作Redis数据库失败
+FAILEDOPERATION_REDISOPERATIONFAILED = 'FailedOperation.RedisOperationFailed'
+
 # 内部错误。
 INTERNALERROR = 'InternalError'
 
+# DBErr
+INTERNALERROR_DBERR = 'InternalError.DBErr'
+
 # 参数错误。
 INVALIDPARAMETER = 'InvalidParameter'
 
 # 证书内容非法。
 INVALIDPARAMETER_INVALIDCERTIFICATE = 'InvalidParameter.InvalidCertificate'
 
 # 根据ID查询证书失败。
```

### Comparing `tencentcloud-sdk-python-waf-3.0.883/tencentcloud/waf/v20180125/models.py` & `tencentcloud-sdk-python-waf-3.0.884/tencentcloud/waf/v20180125/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -874,34 +874,39 @@
         :type InquireNum: int
         :param UsedNum: 使用数量
 注意：此字段可能返回 null，表示取不到有效值。
         :type UsedNum: int
         :param Type: 子产品code
 注意：此字段可能返回 null，表示取不到有效值。
         :type Type: str
+        :param RenewFlag: 续费标志	
+注意：此字段可能返回 null，表示取不到有效值。
+        :type RenewFlag: int
         """
         self.ResourceIds = None
         self.Status = None
         self.Region = None
         self.BeginTime = None
         self.EndTime = None
         self.InquireNum = None
         self.UsedNum = None
         self.Type = None
+        self.RenewFlag = None
 
 
     def _deserialize(self, params):
         self.ResourceIds = params.get("ResourceIds")
         self.Status = params.get("Status")
         self.Region = params.get("Region")
         self.BeginTime = params.get("BeginTime")
         self.EndTime = params.get("EndTime")
         self.InquireNum = params.get("InquireNum")
         self.UsedNum = params.get("UsedNum")
         self.Type = params.get("Type")
+        self.RenewFlag = params.get("RenewFlag")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -920,28 +925,33 @@
         :type ValidTime: str
         :param Count: 资源数量
         :type Count: int
         :param Region: 资源所在地区
         :type Region: str
         :param MaxBotQPS: 使用qps的最大值
         :type MaxBotQPS: int
+        :param RenewFlag: 续费标志
+注意：此字段可能返回 null，表示取不到有效值。
+        :type RenewFlag: int
         """
         self.ResourceIds = None
         self.ValidTime = None
         self.Count = None
         self.Region = None
         self.MaxBotQPS = None
+        self.RenewFlag = None
 
 
     def _deserialize(self, params):
         self.ResourceIds = params.get("ResourceIds")
         self.ValidTime = params.get("ValidTime")
         self.Count = params.get("Count")
         self.Region = params.get("Region")
         self.MaxBotQPS = params.get("MaxBotQPS")
+        self.RenewFlag = params.get("RenewFlag")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -3508,32 +3518,37 @@
         :type EndTime: str
         :param InquireNum: 申请数量
 注意：此字段可能返回 null，表示取不到有效值。
         :type InquireNum: int
         :param UsedNum: 使用数量
 注意：此字段可能返回 null，表示取不到有效值。
         :type UsedNum: int
+        :param RenewFlag: 续费标志
+注意：此字段可能返回 null，表示取不到有效值。
+        :type RenewFlag: int
         """
         self.ResourceIds = None
         self.Status = None
         self.Region = None
         self.BeginTime = None
         self.EndTime = None
         self.InquireNum = None
         self.UsedNum = None
+        self.RenewFlag = None
 
 
     def _deserialize(self, params):
         self.ResourceIds = params.get("ResourceIds")
         self.Status = params.get("Status")
         self.Region = params.get("Region")
         self.BeginTime = params.get("BeginTime")
         self.EndTime = params.get("EndTime")
         self.InquireNum = params.get("InquireNum")
         self.UsedNum = params.get("UsedNum")
+        self.RenewFlag = params.get("RenewFlag")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -5367,36 +5382,36 @@
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class WafThreatenIntelligenceDetails(AbstractModel):
-    """Waf 威胁情报封禁模块配置详情
+    """当前WAF威胁情报封禁模块详情
 
     """
 
     def __init__(self):
         r"""
-        :param DefenseStatus: 封禁模组启用状态
-        :type DefenseStatus: int
         :param Tags: 封禁属性标签
 注意：此字段可能返回 null，表示取不到有效值。
         :type Tags: list of str
+        :param DefenseStatus: 封禁模组启用状态
+        :type DefenseStatus: int
         :param LastUpdateTime: 最后更新时间
         :type LastUpdateTime: str
         """
-        self.DefenseStatus = None
         self.Tags = None
+        self.DefenseStatus = None
         self.LastUpdateTime = None
 
 
     def _deserialize(self, params):
-        self.DefenseStatus = params.get("DefenseStatus")
         self.Tags = params.get("Tags")
+        self.DefenseStatus = params.get("DefenseStatus")
         self.LastUpdateTime = params.get("LastUpdateTime")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-waf-3.0.883/tencentcloud/__init__.py` & `tencentcloud-sdk-python-waf-3.0.884/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-waf-3.0.883/PKG-INFO` & `tencentcloud-sdk-python-waf-3.0.884/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-waf
-Version: 3.0.883
+Version: 3.0.884
 Summary: Tencent Cloud Waf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-waf-3.0.883/setup.py` & `tencentcloud-sdk-python-waf-3.0.884/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-waf-3.0.883/tencentcloud_sdk_python_waf.egg-info/PKG-INFO` & `tencentcloud-sdk-python-waf-3.0.884/tencentcloud_sdk_python_waf.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-waf
-Version: 3.0.883
+Version: 3.0.884
 Summary: Tencent Cloud Waf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

