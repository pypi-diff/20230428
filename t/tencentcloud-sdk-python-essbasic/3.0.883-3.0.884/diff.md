# Comparing `tmp/tencentcloud-sdk-python-essbasic-3.0.883.tar.gz` & `tmp/tencentcloud-sdk-python-essbasic-3.0.884.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.883.tar", last modified: Thu Apr 27 00:32:52 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.884.tar", last modified: Fri Apr 28 02:19:30 2023, max compression
```

## Comparing `tencentcloud-sdk-python-essbasic-3.0.883.tar` & `tencentcloud-sdk-python-essbasic-3.0.884.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:32:52.000000 tencentcloud-sdk-python-essbasic-3.0.883/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:32:52.000000 tencentcloud-sdk-python-essbasic-3.0.883/tencentcloud_sdk_python_essbasic.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 00:32:52.000000 tencentcloud-sdk-python-essbasic-3.0.883/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      678 2023-04-27 00:32:52.000000 tencentcloud-sdk-python-essbasic-3.0.883/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-04-27 00:32:52.000000 tencentcloud-sdk-python-essbasic-3.0.883/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-27 00:32:52.000000 tencentcloud-sdk-python-essbasic-3.0.883/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      752 2023-04-27 00:32:52.000000 tencentcloud-sdk-python-essbasic-3.0.883/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:32:52.000000 tencentcloud-sdk-python-essbasic-3.0.883/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-27 00:32:52.000000 tencentcloud-sdk-python-essbasic-3.0.883/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:32:52.000000 tencentcloud-sdk-python-essbasic-3.0.883/tencentcloud/essbasic/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:32:52.000000 tencentcloud-sdk-python-essbasic-3.0.883/tencentcloud/essbasic/v20210526/
--rw-r--r--   0 root         (0) root         (0)    15673 2023-04-27 00:32:52.000000 tencentcloud-sdk-python-essbasic-3.0.883/tencentcloud/essbasic/v20210526/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    50151 2023-04-27 00:32:52.000000 tencentcloud-sdk-python-essbasic-3.0.883/tencentcloud/essbasic/v20210526/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 00:32:52.000000 tencentcloud-sdk-python-essbasic-3.0.883/tencentcloud/essbasic/v20210526/__init__.py
--rw-r--r--   0 root         (0) root         (0)   229707 2023-04-27 00:32:52.000000 tencentcloud-sdk-python-essbasic-3.0.883/tencentcloud/essbasic/v20210526/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 00:32:52.000000 tencentcloud-sdk-python-essbasic-3.0.883/tencentcloud/essbasic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:32:52.000000 tencentcloud-sdk-python-essbasic-3.0.883/tencentcloud/essbasic/v20201222/
--rw-r--r--   0 root         (0) root         (0)     5392 2023-04-27 00:32:52.000000 tencentcloud-sdk-python-essbasic-3.0.883/tencentcloud/essbasic/v20201222/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    53845 2023-04-27 00:32:52.000000 tencentcloud-sdk-python-essbasic-3.0.883/tencentcloud/essbasic/v20201222/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 00:32:52.000000 tencentcloud-sdk-python-essbasic-3.0.883/tencentcloud/essbasic/v20201222/__init__.py
--rw-r--r--   0 root         (0) root         (0)   171664 2023-04-27 00:32:52.000000 tencentcloud-sdk-python-essbasic-3.0.883/tencentcloud/essbasic/v20201222/models.py
--rw-r--r--   0 root         (0) root         (0)     1684 2023-04-27 00:32:52.000000 tencentcloud-sdk-python-essbasic-3.0.883/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1016 2023-04-27 00:32:52.000000 tencentcloud-sdk-python-essbasic-3.0.883/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-27 00:32:52.000000 tencentcloud-sdk-python-essbasic-3.0.883/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:19:30.000000 tencentcloud-sdk-python-essbasic-3.0.884/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:19:30.000000 tencentcloud-sdk-python-essbasic-3.0.884/tencentcloud_sdk_python_essbasic.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 02:19:30.000000 tencentcloud-sdk-python-essbasic-3.0.884/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      678 2023-04-28 02:19:30.000000 tencentcloud-sdk-python-essbasic-3.0.884/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-04-28 02:19:30.000000 tencentcloud-sdk-python-essbasic-3.0.884/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-28 02:19:30.000000 tencentcloud-sdk-python-essbasic-3.0.884/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      752 2023-04-28 02:19:30.000000 tencentcloud-sdk-python-essbasic-3.0.884/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:19:30.000000 tencentcloud-sdk-python-essbasic-3.0.884/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-28 02:19:30.000000 tencentcloud-sdk-python-essbasic-3.0.884/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:19:30.000000 tencentcloud-sdk-python-essbasic-3.0.884/tencentcloud/essbasic/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:19:30.000000 tencentcloud-sdk-python-essbasic-3.0.884/tencentcloud/essbasic/v20210526/
+-rw-r--r--   0 root         (0) root         (0)    15673 2023-04-28 02:19:30.000000 tencentcloud-sdk-python-essbasic-3.0.884/tencentcloud/essbasic/v20210526/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    50524 2023-04-28 02:19:30.000000 tencentcloud-sdk-python-essbasic-3.0.884/tencentcloud/essbasic/v20210526/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 02:19:30.000000 tencentcloud-sdk-python-essbasic-3.0.884/tencentcloud/essbasic/v20210526/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   229707 2023-04-28 02:19:30.000000 tencentcloud-sdk-python-essbasic-3.0.884/tencentcloud/essbasic/v20210526/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 02:19:30.000000 tencentcloud-sdk-python-essbasic-3.0.884/tencentcloud/essbasic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:19:30.000000 tencentcloud-sdk-python-essbasic-3.0.884/tencentcloud/essbasic/v20201222/
+-rw-r--r--   0 root         (0) root         (0)     5392 2023-04-28 02:19:30.000000 tencentcloud-sdk-python-essbasic-3.0.884/tencentcloud/essbasic/v20201222/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    53845 2023-04-28 02:19:30.000000 tencentcloud-sdk-python-essbasic-3.0.884/tencentcloud/essbasic/v20201222/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 02:19:30.000000 tencentcloud-sdk-python-essbasic-3.0.884/tencentcloud/essbasic/v20201222/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   171664 2023-04-28 02:19:30.000000 tencentcloud-sdk-python-essbasic-3.0.884/tencentcloud/essbasic/v20201222/models.py
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-04-28 02:19:30.000000 tencentcloud-sdk-python-essbasic-3.0.884/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-04-28 02:19:30.000000 tencentcloud-sdk-python-essbasic-3.0.884/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-28 02:19:30.000000 tencentcloud-sdk-python-essbasic-3.0.884/setup.cfg
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.883/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-essbasic-3.0.884/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.883/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.884/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.883
+Version: 3.0.884
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.883/README.rst` & `tencentcloud-sdk-python-essbasic-3.0.884/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.883/tencentcloud/__init__.py` & `tencentcloud-sdk-python-essbasic-3.0.884/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-essbasic-3.0.883/tencentcloud/essbasic/v20210526/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.884/tencentcloud/essbasic/v20210526/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.883/tencentcloud/essbasic/v20210526/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.884/tencentcloud/essbasic/v20210526/essbasic_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -320,16 +320,23 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def ChannelCreateMultiFlowSignQRCode(self, request):
-        """此接口（ChannelCreateMultiFlowSignQRCode）用于创建一码多扫签署流程二维码。
-        适用的模版仅限于B2C（1、无序签署，2、顺序签署时B静默签署，3、顺序签署时B非首位签署）、单C的模版，且模版中发起方没有填写控件。
+        """此接口（ChannelCreateMultiFlowSignQRCode）用于创建一码多扫流程签署二维码。 适用场景：无需填写签署人信息，可通过模板id生成签署二维码，签署人可通过扫描二维码补充签署信息进行实名签署。常用于提前不知道签署人的身份信息场景，例如：劳务工招工、大批量员工入职等场景。
+
+        **本接口适用于发起方没有填写控件的 B2C或者单C模板**
+
+        **若是B2C模板,还要满足以下任意一个条件**
+
+        - 模板中配置的签署顺序是无序
+        - B端企业的签署方式是静默签署
+        - B端企业是非首位签署
 
         :param request: Request instance for ChannelCreateMultiFlowSignQRCode.
         :type request: :class:`tencentcloud.essbasic.v20210526.models.ChannelCreateMultiFlowSignQRCodeRequest`
         :rtype: :class:`tencentcloud.essbasic.v20210526.models.ChannelCreateMultiFlowSignQRCodeResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.883/tencentcloud/essbasic/v20210526/models.py` & `tencentcloud-sdk-python-essbasic-3.0.884/tencentcloud/essbasic/v20210526/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.883/tencentcloud/essbasic/v20201222/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.884/tencentcloud/essbasic/v20201222/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.883/tencentcloud/essbasic/v20201222/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.884/tencentcloud/essbasic/v20201222/essbasic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.883/tencentcloud/essbasic/v20201222/models.py` & `tencentcloud-sdk-python-essbasic-3.0.884/tencentcloud/essbasic/v20201222/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.883/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.884/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.883
+Version: 3.0.884
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.883/setup.py` & `tencentcloud-sdk-python-essbasic-3.0.884/setup.py`

 * *Files identical despite different names*

