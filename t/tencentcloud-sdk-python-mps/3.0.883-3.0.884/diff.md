# Comparing `tmp/tencentcloud-sdk-python-mps-3.0.883.tar.gz` & `tmp/tencentcloud-sdk-python-mps-3.0.884.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-mps-3.0.883.tar", last modified: Thu Apr 27 00:41:05 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-mps-3.0.884.tar", last modified: Fri Apr 28 02:31:15 2023, max compression
```

## Comparing `tencentcloud-sdk-python-mps-3.0.883.tar` & `tencentcloud-sdk-python-mps-3.0.884.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:41:05.000000 tencentcloud-sdk-python-mps-3.0.883/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-27 00:41:05.000000 tencentcloud-sdk-python-mps-3.0.883/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:41:05.000000 tencentcloud-sdk-python-mps-3.0.883/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-27 00:41:05.000000 tencentcloud-sdk-python-mps-3.0.883/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:41:05.000000 tencentcloud-sdk-python-mps-3.0.883/tencentcloud/mps/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:41:05.000000 tencentcloud-sdk-python-mps-3.0.883/tencentcloud/mps/v20190612/
--rw-r--r--   0 root         (0) root         (0)    89755 2023-04-27 00:41:05.000000 tencentcloud-sdk-python-mps-3.0.883/tencentcloud/mps/v20190612/mps_client.py
--rw-r--r--   0 root         (0) root         (0)    13373 2023-04-27 00:41:05.000000 tencentcloud-sdk-python-mps-3.0.883/tencentcloud/mps/v20190612/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 00:41:05.000000 tencentcloud-sdk-python-mps-3.0.883/tencentcloud/mps/v20190612/__init__.py
--rw-r--r--   0 root         (0) root         (0)   798533 2023-04-27 00:41:05.000000 tencentcloud-sdk-python-mps-3.0.883/tencentcloud/mps/v20190612/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 00:41:05.000000 tencentcloud-sdk-python-mps-3.0.883/tencentcloud/mps/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:41:05.000000 tencentcloud-sdk-python-mps-3.0.883/tencentcloud_sdk_python_mps.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 00:41:05.000000 tencentcloud-sdk-python-mps-3.0.883/tencentcloud_sdk_python_mps.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-27 00:41:05.000000 tencentcloud-sdk-python-mps-3.0.883/tencentcloud_sdk_python_mps.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-27 00:41:05.000000 tencentcloud-sdk-python-mps-3.0.883/tencentcloud_sdk_python_mps.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-27 00:41:05.000000 tencentcloud-sdk-python-mps-3.0.883/tencentcloud_sdk_python_mps.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-27 00:41:05.000000 tencentcloud-sdk-python-mps-3.0.883/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-27 00:41:05.000000 tencentcloud-sdk-python-mps-3.0.883/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-27 00:41:05.000000 tencentcloud-sdk-python-mps-3.0.883/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:31:15.000000 tencentcloud-sdk-python-mps-3.0.884/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-28 02:31:15.000000 tencentcloud-sdk-python-mps-3.0.884/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:31:15.000000 tencentcloud-sdk-python-mps-3.0.884/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-28 02:31:15.000000 tencentcloud-sdk-python-mps-3.0.884/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:31:15.000000 tencentcloud-sdk-python-mps-3.0.884/tencentcloud/mps/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:31:15.000000 tencentcloud-sdk-python-mps-3.0.884/tencentcloud/mps/v20190612/
+-rw-r--r--   0 root         (0) root         (0)    89755 2023-04-28 02:31:15.000000 tencentcloud-sdk-python-mps-3.0.884/tencentcloud/mps/v20190612/mps_client.py
+-rw-r--r--   0 root         (0) root         (0)    13373 2023-04-28 02:31:15.000000 tencentcloud-sdk-python-mps-3.0.884/tencentcloud/mps/v20190612/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 02:31:15.000000 tencentcloud-sdk-python-mps-3.0.884/tencentcloud/mps/v20190612/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   798916 2023-04-28 02:31:15.000000 tencentcloud-sdk-python-mps-3.0.884/tencentcloud/mps/v20190612/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 02:31:15.000000 tencentcloud-sdk-python-mps-3.0.884/tencentcloud/mps/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:31:15.000000 tencentcloud-sdk-python-mps-3.0.884/tencentcloud_sdk_python_mps.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 02:31:15.000000 tencentcloud-sdk-python-mps-3.0.884/tencentcloud_sdk_python_mps.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-28 02:31:15.000000 tencentcloud-sdk-python-mps-3.0.884/tencentcloud_sdk_python_mps.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-28 02:31:15.000000 tencentcloud-sdk-python-mps-3.0.884/tencentcloud_sdk_python_mps.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-28 02:31:15.000000 tencentcloud-sdk-python-mps-3.0.884/tencentcloud_sdk_python_mps.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-28 02:31:15.000000 tencentcloud-sdk-python-mps-3.0.884/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-28 02:31:15.000000 tencentcloud-sdk-python-mps-3.0.884/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-28 02:31:15.000000 tencentcloud-sdk-python-mps-3.0.884/setup.cfg
```

### Comparing `tencentcloud-sdk-python-mps-3.0.883/README.rst` & `tencentcloud-sdk-python-mps-3.0.884/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mps-3.0.883/tencentcloud/__init__.py` & `tencentcloud-sdk-python-mps-3.0.884/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-mps-3.0.883/tencentcloud/mps/v20190612/mps_client.py` & `tencentcloud-sdk-python-mps-3.0.884/tencentcloud/mps/v20190612/mps_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mps-3.0.883/tencentcloud/mps/v20190612/errorcodes.py` & `tencentcloud-sdk-python-mps-3.0.884/tencentcloud/mps/v20190612/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mps-3.0.883/tencentcloud/mps/v20190612/models.py` & `tencentcloud-sdk-python-mps-3.0.884/tencentcloud/mps/v20190612/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -16597,25 +16597,28 @@
         :type OutputStorage: :class:`tencentcloud.mps.v20190612.models.TaskOutputStorage`
         :param OutputDir: 直播流处理生成的文件输出的目标目录，如`/movie/201909/`，如果不填为 `/` 目录。
         :type OutputDir: str
         :param AiContentReviewTask: 视频内容审核类型任务参数。
         :type AiContentReviewTask: :class:`tencentcloud.mps.v20190612.models.AiContentReviewTaskInput`
         :param AiRecognitionTask: 视频内容识别类型任务参数。
         :type AiRecognitionTask: :class:`tencentcloud.mps.v20190612.models.AiRecognitionTaskInput`
+        :param AiAnalysisTask: 视频内容分析类型任务参数。
+        :type AiAnalysisTask: :class:`tencentcloud.mps.v20190612.models.AiAnalysisTaskInput`
         :param SessionId: 用于去重的识别码，如果七天内曾有过相同的识别码的请求，则本次的请求会返回错误。最长 50 个字符，不带或者带空字符串表示不做去重。
         :type SessionId: str
         :param SessionContext: 来源上下文，用于透传用户请求信息，任务流状态变更回调将返回该字段值，最长 1000 个字符。
         :type SessionContext: str
         """
         self.Url = None
         self.TaskNotifyConfig = None
         self.OutputStorage = None
         self.OutputDir = None
         self.AiContentReviewTask = None
         self.AiRecognitionTask = None
+        self.AiAnalysisTask = None
         self.SessionId = None
         self.SessionContext = None
 
 
     def _deserialize(self, params):
         self.Url = params.get("Url")
         if params.get("TaskNotifyConfig") is not None:
@@ -16627,14 +16630,17 @@
         self.OutputDir = params.get("OutputDir")
         if params.get("AiContentReviewTask") is not None:
             self.AiContentReviewTask = AiContentReviewTaskInput()
             self.AiContentReviewTask._deserialize(params.get("AiContentReviewTask"))
         if params.get("AiRecognitionTask") is not None:
             self.AiRecognitionTask = AiRecognitionTaskInput()
             self.AiRecognitionTask._deserialize(params.get("AiRecognitionTask"))
+        if params.get("AiAnalysisTask") is not None:
+            self.AiAnalysisTask = AiAnalysisTaskInput()
+            self.AiAnalysisTask._deserialize(params.get("AiAnalysisTask"))
         self.SessionId = params.get("SessionId")
         self.SessionContext = params.get("SessionContext")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
```

### Comparing `tencentcloud-sdk-python-mps-3.0.883/tencentcloud_sdk_python_mps.egg-info/PKG-INFO` & `tencentcloud-sdk-python-mps-3.0.884/tencentcloud_sdk_python_mps.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-mps
-Version: 3.0.883
+Version: 3.0.884
 Summary: Tencent Cloud Mps SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-mps-3.0.883/PKG-INFO` & `tencentcloud-sdk-python-mps-3.0.884/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-mps
-Version: 3.0.883
+Version: 3.0.884
 Summary: Tencent Cloud Mps SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-mps-3.0.883/setup.py` & `tencentcloud-sdk-python-mps-3.0.884/setup.py`

 * *Files identical despite different names*

