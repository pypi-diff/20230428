# Comparing `tmp/tencentcloud-sdk-python-bma-3.0.883.tar.gz` & `tmp/tencentcloud-sdk-python-bma-3.0.884.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-bma-3.0.883.tar", last modified: Thu Apr 27 00:18:13 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-bma-3.0.884.tar", last modified: Fri Apr 28 02:05:51 2023, max compression
```

## Comparing `tencentcloud-sdk-python-bma-3.0.883.tar` & `tencentcloud-sdk-python-bma-3.0.884.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:18:13.000000 tencentcloud-sdk-python-bma-3.0.883/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-27 00:18:13.000000 tencentcloud-sdk-python-bma-3.0.883/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:18:13.000000 tencentcloud-sdk-python-bma-3.0.883/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:18:13.000000 tencentcloud-sdk-python-bma-3.0.883/tencentcloud/bma/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:18:13.000000 tencentcloud-sdk-python-bma-3.0.883/tencentcloud/bma/v20210624/
--rw-r--r--   0 root         (0) root         (0)     1829 2023-04-27 00:18:13.000000 tencentcloud-sdk-python-bma-3.0.883/tencentcloud/bma/v20210624/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    25791 2023-04-27 00:18:13.000000 tencentcloud-sdk-python-bma-3.0.883/tencentcloud/bma/v20210624/bma_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 00:18:13.000000 tencentcloud-sdk-python-bma-3.0.883/tencentcloud/bma/v20210624/__init__.py
--rw-r--r--   0 root         (0) root         (0)    82603 2023-04-27 00:18:13.000000 tencentcloud-sdk-python-bma-3.0.883/tencentcloud/bma/v20210624/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:18:13.000000 tencentcloud-sdk-python-bma-3.0.883/tencentcloud/bma/v20221115/
--rw-r--r--   0 root         (0) root         (0)     3348 2023-04-27 00:18:13.000000 tencentcloud-sdk-python-bma-3.0.883/tencentcloud/bma/v20221115/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    10527 2023-04-27 00:18:13.000000 tencentcloud-sdk-python-bma-3.0.883/tencentcloud/bma/v20221115/bma_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 00:18:13.000000 tencentcloud-sdk-python-bma-3.0.883/tencentcloud/bma/v20221115/__init__.py
--rw-r--r--   0 root         (0) root         (0)    38587 2023-04-27 00:18:13.000000 tencentcloud-sdk-python-bma-3.0.883/tencentcloud/bma/v20221115/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 00:18:13.000000 tencentcloud-sdk-python-bma-3.0.883/tencentcloud/bma/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-27 00:18:13.000000 tencentcloud-sdk-python-bma-3.0.883/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-27 00:18:13.000000 tencentcloud-sdk-python-bma-3.0.883/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:18:13.000000 tencentcloud-sdk-python-bma-3.0.883/tencentcloud_sdk_python_bma.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 00:18:13.000000 tencentcloud-sdk-python-bma-3.0.883/tencentcloud_sdk_python_bma.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      603 2023-04-27 00:18:13.000000 tencentcloud-sdk-python-bma-3.0.883/tencentcloud_sdk_python_bma.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-27 00:18:13.000000 tencentcloud-sdk-python-bma-3.0.883/tencentcloud_sdk_python_bma.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-27 00:18:13.000000 tencentcloud-sdk-python-bma-3.0.883/tencentcloud_sdk_python_bma.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-27 00:18:13.000000 tencentcloud-sdk-python-bma-3.0.883/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-27 00:18:13.000000 tencentcloud-sdk-python-bma-3.0.883/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:05:51.000000 tencentcloud-sdk-python-bma-3.0.884/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-28 02:05:51.000000 tencentcloud-sdk-python-bma-3.0.884/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:05:51.000000 tencentcloud-sdk-python-bma-3.0.884/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:05:51.000000 tencentcloud-sdk-python-bma-3.0.884/tencentcloud/bma/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:05:51.000000 tencentcloud-sdk-python-bma-3.0.884/tencentcloud/bma/v20210624/
+-rw-r--r--   0 root         (0) root         (0)     1829 2023-04-28 02:05:51.000000 tencentcloud-sdk-python-bma-3.0.884/tencentcloud/bma/v20210624/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    25791 2023-04-28 02:05:51.000000 tencentcloud-sdk-python-bma-3.0.884/tencentcloud/bma/v20210624/bma_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 02:05:51.000000 tencentcloud-sdk-python-bma-3.0.884/tencentcloud/bma/v20210624/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    82603 2023-04-28 02:05:51.000000 tencentcloud-sdk-python-bma-3.0.884/tencentcloud/bma/v20210624/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:05:51.000000 tencentcloud-sdk-python-bma-3.0.884/tencentcloud/bma/v20221115/
+-rw-r--r--   0 root         (0) root         (0)     3348 2023-04-28 02:05:51.000000 tencentcloud-sdk-python-bma-3.0.884/tencentcloud/bma/v20221115/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    10527 2023-04-28 02:05:51.000000 tencentcloud-sdk-python-bma-3.0.884/tencentcloud/bma/v20221115/bma_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 02:05:51.000000 tencentcloud-sdk-python-bma-3.0.884/tencentcloud/bma/v20221115/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    38994 2023-04-28 02:05:51.000000 tencentcloud-sdk-python-bma-3.0.884/tencentcloud/bma/v20221115/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 02:05:51.000000 tencentcloud-sdk-python-bma-3.0.884/tencentcloud/bma/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-28 02:05:51.000000 tencentcloud-sdk-python-bma-3.0.884/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-28 02:05:51.000000 tencentcloud-sdk-python-bma-3.0.884/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:05:51.000000 tencentcloud-sdk-python-bma-3.0.884/tencentcloud_sdk_python_bma.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 02:05:51.000000 tencentcloud-sdk-python-bma-3.0.884/tencentcloud_sdk_python_bma.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      603 2023-04-28 02:05:51.000000 tencentcloud-sdk-python-bma-3.0.884/tencentcloud_sdk_python_bma.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-28 02:05:51.000000 tencentcloud-sdk-python-bma-3.0.884/tencentcloud_sdk_python_bma.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-28 02:05:51.000000 tencentcloud-sdk-python-bma-3.0.884/tencentcloud_sdk_python_bma.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-28 02:05:51.000000 tencentcloud-sdk-python-bma-3.0.884/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-28 02:05:51.000000 tencentcloud-sdk-python-bma-3.0.884/setup.cfg
```

### Comparing `tencentcloud-sdk-python-bma-3.0.883/README.rst` & `tencentcloud-sdk-python-bma-3.0.884/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bma-3.0.883/tencentcloud/bma/v20210624/errorcodes.py` & `tencentcloud-sdk-python-bma-3.0.884/tencentcloud/bma/v20210624/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bma-3.0.883/tencentcloud/bma/v20210624/bma_client.py` & `tencentcloud-sdk-python-bma-3.0.884/tencentcloud/bma/v20210624/bma_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bma-3.0.883/tencentcloud/bma/v20210624/models.py` & `tencentcloud-sdk-python-bma-3.0.884/tencentcloud/bma/v20210624/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bma-3.0.883/tencentcloud/bma/v20221115/errorcodes.py` & `tencentcloud-sdk-python-bma-3.0.884/tencentcloud/bma/v20221115/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bma-3.0.883/tencentcloud/bma/v20221115/bma_client.py` & `tencentcloud-sdk-python-bma-3.0.884/tencentcloud/bma/v20221115/bma_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bma-3.0.883/tencentcloud/bma/v20221115/models.py` & `tencentcloud-sdk-python-bma-3.0.884/tencentcloud/bma/v20221115/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,14 +108,16 @@
 
     def __init__(self):
         r"""
         :param BrandName: 品牌名称
         :type BrandName: str
         :param CompanyName: 企业名称
         :type CompanyName: str
+        :param BrandLogo: 品牌logo
+        :type BrandLogo: str
         :param Phone: 联系电话
         :type Phone: str
         :param License: 营业执照
         :type License: str
         :param Authorization: 授权书
         :type Authorization: str
         :param TrademarkNames: 商标名称
@@ -133,14 +135,15 @@
         :param ProtectOfficialAccounts: 保护公众号
         :type ProtectOfficialAccounts: list of str
         :param ProtectMiniPrograms: 保护小程序
         :type ProtectMiniPrograms: list of str
         """
         self.BrandName = None
         self.CompanyName = None
+        self.BrandLogo = None
         self.Phone = None
         self.License = None
         self.Authorization = None
         self.TrademarkNames = None
         self.Trademarks = None
         self.IsTransfers = None
         self.Transfers = None
@@ -149,14 +152,15 @@
         self.ProtectOfficialAccounts = None
         self.ProtectMiniPrograms = None
 
 
     def _deserialize(self, params):
         self.BrandName = params.get("BrandName")
         self.CompanyName = params.get("CompanyName")
+        self.BrandLogo = params.get("BrandLogo")
         self.Phone = params.get("Phone")
         self.License = params.get("License")
         self.Authorization = params.get("Authorization")
         self.TrademarkNames = params.get("TrademarkNames")
         self.Trademarks = params.get("Trademarks")
         self.IsTransfers = params.get("IsTransfers")
         self.Transfers = params.get("Transfers")
@@ -891,14 +895,17 @@
         :type InsertTime: str
         :param CertificationStatus: 资质证明状态：0-不可用 1-可用
 注意：此字段可能返回 null，表示取不到有效值。
         :type CertificationStatus: int
         :param Snapshot: 网址截图
 注意：此字段可能返回 null，表示取不到有效值。
         :type Snapshot: str
+        :param AccountStatus: 账户资源状态：0-不可用 1-可用
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AccountStatus: int
         """
         self.FakeURLId = None
         self.BrandName = None
         self.Origin = None
         self.FakeURL = None
         self.FakeDomain = None
         self.Heat = None
@@ -913,14 +920,15 @@
         self.WebName = None
         self.WebICP = None
         self.WebCreateTime = None
         self.WebExpireTime = None
         self.InsertTime = None
         self.CertificationStatus = None
         self.Snapshot = None
+        self.AccountStatus = None
 
 
     def _deserialize(self, params):
         self.FakeURLId = params.get("FakeURLId")
         self.BrandName = params.get("BrandName")
         self.Origin = params.get("Origin")
         self.FakeURL = params.get("FakeURL")
@@ -937,14 +945,15 @@
         self.WebName = params.get("WebName")
         self.WebICP = params.get("WebICP")
         self.WebCreateTime = params.get("WebCreateTime")
         self.WebExpireTime = params.get("WebExpireTime")
         self.InsertTime = params.get("InsertTime")
         self.CertificationStatus = params.get("CertificationStatus")
         self.Snapshot = params.get("Snapshot")
+        self.AccountStatus = params.get("AccountStatus")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-bma-3.0.883/tencentcloud/__init__.py` & `tencentcloud-sdk-python-bma-3.0.884/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-bma-3.0.883/PKG-INFO` & `tencentcloud-sdk-python-bma-3.0.884/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-bma
-Version: 3.0.883
+Version: 3.0.884
 Summary: Tencent Cloud Bma SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-bma-3.0.883/tencentcloud_sdk_python_bma.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-bma-3.0.884/tencentcloud_sdk_python_bma.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-bma-3.0.883/tencentcloud_sdk_python_bma.egg-info/PKG-INFO` & `tencentcloud-sdk-python-bma-3.0.884/tencentcloud_sdk_python_bma.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-bma
-Version: 3.0.883
+Version: 3.0.884
 Summary: Tencent Cloud Bma SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-bma-3.0.883/setup.py` & `tencentcloud-sdk-python-bma-3.0.884/setup.py`

 * *Files identical despite different names*

