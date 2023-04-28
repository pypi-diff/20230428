# Comparing `tmp/tencentcloud-sdk-python-vod-3.0.883.tar.gz` & `tmp/tencentcloud-sdk-python-vod-3.0.884.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-vod-3.0.883.tar", last modified: Thu Apr 27 01:00:13 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-vod-3.0.884.tar", last modified: Fri Apr 28 02:47:21 2023, max compression
```

## Comparing `tencentcloud-sdk-python-vod-3.0.883.tar` & `tencentcloud-sdk-python-vod-3.0.884.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 01:00:13.000000 tencentcloud-sdk-python-vod-3.0.883/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-27 01:00:13.000000 tencentcloud-sdk-python-vod-3.0.883/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 01:00:13.000000 tencentcloud-sdk-python-vod-3.0.883/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 01:00:13.000000 tencentcloud-sdk-python-vod-3.0.883/tencentcloud/vod/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 01:00:13.000000 tencentcloud-sdk-python-vod-3.0.883/tencentcloud/vod/v20180717/
--rw-r--r--   0 root         (0) root         (0)   172410 2023-04-27 01:00:13.000000 tencentcloud-sdk-python-vod-3.0.883/tencentcloud/vod/v20180717/vod_client.py
--rw-r--r--   0 root         (0) root         (0)    25111 2023-04-27 01:00:13.000000 tencentcloud-sdk-python-vod-3.0.883/tencentcloud/vod/v20180717/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 01:00:13.000000 tencentcloud-sdk-python-vod-3.0.883/tencentcloud/vod/v20180717/__init__.py
--rw-r--r--   0 root         (0) root         (0)  1171666 2023-04-27 01:00:13.000000 tencentcloud-sdk-python-vod-3.0.883/tencentcloud/vod/v20180717/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 01:00:13.000000 tencentcloud-sdk-python-vod-3.0.883/tencentcloud/vod/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-27 01:00:13.000000 tencentcloud-sdk-python-vod-3.0.883/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 01:00:13.000000 tencentcloud-sdk-python-vod-3.0.883/tencentcloud_sdk_python_vod.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 01:00:13.000000 tencentcloud-sdk-python-vod-3.0.883/tencentcloud_sdk_python_vod.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-27 01:00:13.000000 tencentcloud-sdk-python-vod-3.0.883/tencentcloud_sdk_python_vod.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-27 01:00:13.000000 tencentcloud-sdk-python-vod-3.0.883/tencentcloud_sdk_python_vod.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-27 01:00:13.000000 tencentcloud-sdk-python-vod-3.0.883/tencentcloud_sdk_python_vod.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-27 01:00:13.000000 tencentcloud-sdk-python-vod-3.0.883/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-27 01:00:13.000000 tencentcloud-sdk-python-vod-3.0.883/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-27 01:00:13.000000 tencentcloud-sdk-python-vod-3.0.883/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:47:21.000000 tencentcloud-sdk-python-vod-3.0.884/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-28 02:47:21.000000 tencentcloud-sdk-python-vod-3.0.884/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:47:21.000000 tencentcloud-sdk-python-vod-3.0.884/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:47:21.000000 tencentcloud-sdk-python-vod-3.0.884/tencentcloud/vod/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:47:21.000000 tencentcloud-sdk-python-vod-3.0.884/tencentcloud/vod/v20180717/
+-rw-r--r--   0 root         (0) root         (0)   172410 2023-04-28 02:47:21.000000 tencentcloud-sdk-python-vod-3.0.884/tencentcloud/vod/v20180717/vod_client.py
+-rw-r--r--   0 root         (0) root         (0)    25111 2023-04-28 02:47:21.000000 tencentcloud-sdk-python-vod-3.0.884/tencentcloud/vod/v20180717/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 02:47:21.000000 tencentcloud-sdk-python-vod-3.0.884/tencentcloud/vod/v20180717/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  1171841 2023-04-28 02:47:21.000000 tencentcloud-sdk-python-vod-3.0.884/tencentcloud/vod/v20180717/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 02:47:21.000000 tencentcloud-sdk-python-vod-3.0.884/tencentcloud/vod/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-28 02:47:21.000000 tencentcloud-sdk-python-vod-3.0.884/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:47:21.000000 tencentcloud-sdk-python-vod-3.0.884/tencentcloud_sdk_python_vod.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 02:47:21.000000 tencentcloud-sdk-python-vod-3.0.884/tencentcloud_sdk_python_vod.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-28 02:47:21.000000 tencentcloud-sdk-python-vod-3.0.884/tencentcloud_sdk_python_vod.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-28 02:47:21.000000 tencentcloud-sdk-python-vod-3.0.884/tencentcloud_sdk_python_vod.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-28 02:47:21.000000 tencentcloud-sdk-python-vod-3.0.884/tencentcloud_sdk_python_vod.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-28 02:47:21.000000 tencentcloud-sdk-python-vod-3.0.884/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-28 02:47:21.000000 tencentcloud-sdk-python-vod-3.0.884/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-28 02:47:21.000000 tencentcloud-sdk-python-vod-3.0.884/setup.cfg
```

### Comparing `tencentcloud-sdk-python-vod-3.0.883/README.rst` & `tencentcloud-sdk-python-vod-3.0.884/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vod-3.0.883/tencentcloud/vod/v20180717/vod_client.py` & `tencentcloud-sdk-python-vod-3.0.884/tencentcloud/vod/v20180717/vod_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vod-3.0.883/tencentcloud/vod/v20180717/errorcodes.py` & `tencentcloud-sdk-python-vod-3.0.884/tencentcloud/vod/v20180717/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vod-3.0.883/tencentcloud/vod/v20180717/models.py` & `tencentcloud-sdk-python-vod-3.0.884/tencentcloud/vod/v20180717/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -10388,20 +10388,24 @@
 
     """
 
     def __init__(self):
         r"""
         :param Md5: 媒体文件的 Md5 值。
         :type Md5: str
+        :param Sha1: 媒体文件的 Sha1 值。
+        :type Sha1: str
         """
         self.Md5 = None
+        self.Sha1 = None
 
 
     def _deserialize(self, params):
         self.Md5 = params.get("Md5")
+        self.Sha1 = params.get("Sha1")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -14410,16 +14414,17 @@
     """单个图片处理操作。
 
     """
 
     def __init__(self):
         r"""
         :param Type: 图片处理类型。可选类型有：
-<li>Scale : 图片缩略处理。</li>
-<li>CenterCut : 图片裁剪处理。</li>
+<li>Scale : 图片缩略处理；</li>
+<li>CenterCut : 图片裁剪处理；</li>
+<li>Blur : 图片模糊处理。</li>
         :type Type: str
         :param Scale: 图片缩略处理，仅当 Type 为 Scale 时有效。
         :type Scale: :class:`tencentcloud.vod.v20180717.models.ImageScale`
         :param CenterCut: 图片裁剪处理，仅当 Type 为 CenterCut 时有效。
         :type CenterCut: :class:`tencentcloud.vod.v20180717.models.ImageCenterCut`
         :param Blur: 图片模糊处理，仅当 Type 为 Blur 时有效。
         :type Blur: :class:`tencentcloud.vod.v20180717.models.ImageBlur`
```

### Comparing `tencentcloud-sdk-python-vod-3.0.883/tencentcloud/__init__.py` & `tencentcloud-sdk-python-vod-3.0.884/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-vod-3.0.883/tencentcloud_sdk_python_vod.egg-info/PKG-INFO` & `tencentcloud-sdk-python-vod-3.0.884/tencentcloud_sdk_python_vod.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vod
-Version: 3.0.883
+Version: 3.0.884
 Summary: Tencent Cloud Vod SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vod-3.0.883/PKG-INFO` & `tencentcloud-sdk-python-vod-3.0.884/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vod
-Version: 3.0.883
+Version: 3.0.884
 Summary: Tencent Cloud Vod SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vod-3.0.883/setup.py` & `tencentcloud-sdk-python-vod-3.0.884/setup.py`

 * *Files identical despite different names*

