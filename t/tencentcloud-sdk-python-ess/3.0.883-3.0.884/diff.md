# Comparing `tmp/tencentcloud-sdk-python-ess-3.0.883.tar.gz` & `tmp/tencentcloud-sdk-python-ess-3.0.884.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.883.tar", last modified: Thu Apr 27 00:32:45 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.884.tar", last modified: Fri Apr 28 02:19:24 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ess-3.0.883.tar` & `tencentcloud-sdk-python-ess-3.0.884.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:32:45.000000 tencentcloud-sdk-python-ess-3.0.883/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-27 00:32:45.000000 tencentcloud-sdk-python-ess-3.0.883/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:32:45.000000 tencentcloud-sdk-python-ess-3.0.883/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-27 00:32:45.000000 tencentcloud-sdk-python-ess-3.0.883/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:32:45.000000 tencentcloud-sdk-python-ess-3.0.883/tencentcloud/ess/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 00:32:45.000000 tencentcloud-sdk-python-ess-3.0.883/tencentcloud/ess/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:32:45.000000 tencentcloud-sdk-python-ess-3.0.883/tencentcloud/ess/v20201111/
--rw-r--r--   0 root         (0) root         (0)    49192 2023-04-27 00:32:45.000000 tencentcloud-sdk-python-ess-3.0.883/tencentcloud/ess/v20201111/ess_client.py
--rw-r--r--   0 root         (0) root         (0)    23727 2023-04-27 00:32:45.000000 tencentcloud-sdk-python-ess-3.0.883/tencentcloud/ess/v20201111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 00:32:45.000000 tencentcloud-sdk-python-ess-3.0.883/tencentcloud/ess/v20201111/__init__.py
--rw-r--r--   0 root         (0) root         (0)   219487 2023-04-27 00:32:45.000000 tencentcloud-sdk-python-ess-3.0.883/tencentcloud/ess/v20201111/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:32:45.000000 tencentcloud-sdk-python-ess-3.0.883/tencentcloud_sdk_python_ess.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 00:32:45.000000 tencentcloud-sdk-python-ess-3.0.883/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-27 00:32:45.000000 tencentcloud-sdk-python-ess-3.0.883/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-27 00:32:45.000000 tencentcloud-sdk-python-ess-3.0.883/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-27 00:32:45.000000 tencentcloud-sdk-python-ess-3.0.883/tencentcloud_sdk_python_ess.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-27 00:32:45.000000 tencentcloud-sdk-python-ess-3.0.883/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-27 00:32:45.000000 tencentcloud-sdk-python-ess-3.0.883/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-27 00:32:45.000000 tencentcloud-sdk-python-ess-3.0.883/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:19:24.000000 tencentcloud-sdk-python-ess-3.0.884/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-28 02:19:24.000000 tencentcloud-sdk-python-ess-3.0.884/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:19:24.000000 tencentcloud-sdk-python-ess-3.0.884/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-28 02:19:24.000000 tencentcloud-sdk-python-ess-3.0.884/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:19:24.000000 tencentcloud-sdk-python-ess-3.0.884/tencentcloud/ess/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 02:19:24.000000 tencentcloud-sdk-python-ess-3.0.884/tencentcloud/ess/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:19:24.000000 tencentcloud-sdk-python-ess-3.0.884/tencentcloud/ess/v20201111/
+-rw-r--r--   0 root         (0) root         (0)    49606 2023-04-28 02:19:24.000000 tencentcloud-sdk-python-ess-3.0.884/tencentcloud/ess/v20201111/ess_client.py
+-rw-r--r--   0 root         (0) root         (0)    23727 2023-04-28 02:19:24.000000 tencentcloud-sdk-python-ess-3.0.884/tencentcloud/ess/v20201111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 02:19:24.000000 tencentcloud-sdk-python-ess-3.0.884/tencentcloud/ess/v20201111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   219543 2023-04-28 02:19:24.000000 tencentcloud-sdk-python-ess-3.0.884/tencentcloud/ess/v20201111/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:19:24.000000 tencentcloud-sdk-python-ess-3.0.884/tencentcloud_sdk_python_ess.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 02:19:24.000000 tencentcloud-sdk-python-ess-3.0.884/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-28 02:19:24.000000 tencentcloud-sdk-python-ess-3.0.884/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-28 02:19:24.000000 tencentcloud-sdk-python-ess-3.0.884/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-28 02:19:24.000000 tencentcloud-sdk-python-ess-3.0.884/tencentcloud_sdk_python_ess.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-28 02:19:24.000000 tencentcloud-sdk-python-ess-3.0.884/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-28 02:19:24.000000 tencentcloud-sdk-python-ess-3.0.884/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-28 02:19:24.000000 tencentcloud-sdk-python-ess-3.0.884/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ess-3.0.883/README.rst` & `tencentcloud-sdk-python-ess-3.0.884/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.883/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ess-3.0.884/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ess-3.0.883/tencentcloud/ess/v20201111/ess_client.py` & `tencentcloud-sdk-python-ess-3.0.884/tencentcloud/ess/v20201111/ess_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -393,15 +393,21 @@
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreateMultiFlowSignQRCode(self, request):
         """此接口（CreateMultiFlowSignQRCode）用于创建一码多扫流程签署二维码。
         适用场景：无需填写签署人信息，可通过模板id生成签署二维码，签署人可通过扫描二维码补充签署信息进行实名签署。常用于提前不知道签署人的身份信息场景，例如：劳务工招工、大批量员工入职等场景。
-        适用的模板仅限于B2C（1、无序签署，2、顺序签署时B静默签署，3、顺序签署时B非首位签署）、单C的模板，且模板中发起方没有填写控件。
+
+        **本接口适用于发起方没有填写控件的 B2C或者单C模板**
+
+        **若是B2C模板,还要满足以下任意一个条件**
+        - 模板中配置的签署顺序是无序
+        - B端企业的签署方式是静默签署
+        - B端企业是非首位签署
 
         :param request: Request instance for CreateMultiFlowSignQRCode.
         :type request: :class:`tencentcloud.ess.v20201111.models.CreateMultiFlowSignQRCodeRequest`
         :rtype: :class:`tencentcloud.ess.v20201111.models.CreateMultiFlowSignQRCodeResponse`
 
         """
         try:
@@ -441,15 +447,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreatePreparedPersonalEsign(self, request):
-        """本接口（CreatePreparedPersonalEsign）用于创建导入个人印章。
+        """本接口（CreatePreparedPersonalEsign）用于创建导入个人印章（处方单场景专用，在开通个人自动签之后调用，使用此接口请与客户经理确认）。
 
         :param request: Request instance for CreatePreparedPersonalEsign.
         :type request: :class:`tencentcloud.ess.v20201111.models.CreatePreparedPersonalEsignRequest`
         :rtype: :class:`tencentcloud.ess.v20201111.models.CreatePreparedPersonalEsignResponse`
 
         """
         try:
@@ -543,15 +549,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreateUserAutoSignEnableUrl(self, request):
-        """企业方可以通过此接口获取个人用户开启自动签的跳转链接
+        """企业方可以通过此接口获取个人用户开启自动签的跳转链接（处方单场景专用，使用此接口请与客户经理确认）
 
         :param request: Request instance for CreateUserAutoSignEnableUrl.
         :type request: :class:`tencentcloud.ess.v20201111.models.CreateUserAutoSignEnableUrlRequest`
         :rtype: :class:`tencentcloud.ess.v20201111.models.CreateUserAutoSignEnableUrlResponse`
 
         """
         try:
@@ -893,15 +899,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeUserAutoSignStatus(self, request):
-        """企业方可以通过此接口查询个人用户自动签开启状态
+        """企业方可以通过此接口查询个人用户自动签开启状态。（处方单场景专用，使用此接口请与客户经理确认）
 
         :param request: Request instance for DescribeUserAutoSignStatus.
         :type request: :class:`tencentcloud.ess.v20201111.models.DescribeUserAutoSignStatusRequest`
         :rtype: :class:`tencentcloud.ess.v20201111.models.DescribeUserAutoSignStatusResponse`
 
         """
         try:
@@ -916,15 +922,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DisableUserAutoSign(self, request):
-        """企业方可以通过此接口关闭个人的自动签功能
+        """企业方可以通过此接口关闭个人的自动签功能（处方单场景专用，使用此接口请与客户经理确认）
 
         :param request: Request instance for DisableUserAutoSign.
         :type request: :class:`tencentcloud.ess.v20201111.models.DisableUserAutoSignRequest`
         :rtype: :class:`tencentcloud.ess.v20201111.models.DisableUserAutoSignResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-ess-3.0.883/tencentcloud/ess/v20201111/errorcodes.py` & `tencentcloud-sdk-python-ess-3.0.884/tencentcloud/ess/v20201111/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.883/tencentcloud/ess/v20201111/models.py` & `tencentcloud-sdk-python-ess-3.0.884/tencentcloud/ess/v20201111/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2330,15 +2330,15 @@
         :param SceneKey: 自动签场景:
 E_PRESCRIPTION_AUTO_SIGN 电子处方
         :type SceneKey: str
         :param AutoSignConfig: 自动签开通，签署相关配置
         :type AutoSignConfig: :class:`tencentcloud.ess.v20201111.models.AutoSignConfig`
         :param UrlType: 链接类型，空-默认小程序端链接，H5SIGN-h5端链接
         :type UrlType: str
-        :param NotifyType: 通知类型，默认不填为不通知开通方，填写 SMS 为短息通知。
+        :param NotifyType: 通知类型，默认不填为不通知开通方，填写 SMS 为短信通知。
         :type NotifyType: str
         :param NotifyAddress: 若上方填写为 SMS，则此处为手机号
         :type NotifyAddress: str
         """
         self.Operator = None
         self.SceneKey = None
         self.AutoSignConfig = None
@@ -2743,15 +2743,16 @@
 class DescribeFileUrlsResponse(AbstractModel):
     """DescribeFileUrls返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param FileUrls: URL信息
+        :param FileUrls: 文件URL信息；
+链接不是永久链接，有效期5分钟后链接失效。
         :type FileUrls: list of FileUrl
         :param TotalCount: URL数量
         :type TotalCount: int
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.FileUrls = None
@@ -4110,17 +4111,17 @@
         :type ApproverIdCardNumber: str
         :param RecipientId: 签署方经办人在模板中的角色ID
         :type RecipientId: str
         :param VerifyChannel: 签署意愿确认渠道,WEIXINAPP:人脸识别
         :type VerifyChannel: list of str
         :param NotifyType: 是否发送短信，sms--短信通知，none--不通知，默认为sms；发起方=签署方时不发送短信
         :type NotifyType: str
-        :param IsFullText: 签署前置条件：是否需要阅读全文，默认为不需要
+        :param IsFullText: 合同强制需要阅读全文，无需传此参数
         :type IsFullText: bool
-        :param PreReadTime: 签署前置条件：阅读时长限制，单位秒，默认为不需要
+        :param PreReadTime: 合同的强制预览时间：3~300s，未指定则按合同页数计算
         :type PreReadTime: int
         :param UserId: 签署方经办人的用户ID,和签署方经办人姓名+手机号+证件必须有一个。
         :type UserId: str
         :param Required: 当前只支持true，默认为true
         :type Required: bool
         :param ApproverSource: 签署人用户来源,企微侧用户请传入：WEWORKAPP
         :type ApproverSource: str
```

### Comparing `tencentcloud-sdk-python-ess-3.0.883/tencentcloud_sdk_python_ess.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.884/tencentcloud_sdk_python_ess.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.883
+Version: 3.0.884
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.883/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.884/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.883
+Version: 3.0.884
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.883/setup.py` & `tencentcloud-sdk-python-ess-3.0.884/setup.py`

 * *Files identical despite different names*

