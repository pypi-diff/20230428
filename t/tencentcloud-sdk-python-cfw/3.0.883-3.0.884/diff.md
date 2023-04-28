# Comparing `tmp/tencentcloud-sdk-python-cfw-3.0.883.tar.gz` & `tmp/tencentcloud-sdk-python-cfw-3.0.884.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cfw-3.0.883.tar", last modified: Thu Apr 27 00:21:05 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cfw-3.0.884.tar", last modified: Fri Apr 28 02:08:16 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cfw-3.0.883.tar` & `tencentcloud-sdk-python-cfw-3.0.884.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:21:05.000000 tencentcloud-sdk-python-cfw-3.0.883/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-27 00:21:05.000000 tencentcloud-sdk-python-cfw-3.0.883/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:21:05.000000 tencentcloud-sdk-python-cfw-3.0.883/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:21:05.000000 tencentcloud-sdk-python-cfw-3.0.883/tencentcloud/cfw/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:21:05.000000 tencentcloud-sdk-python-cfw-3.0.883/tencentcloud/cfw/v20190904/
--rw-r--r--   0 root         (0) root         (0)     1836 2023-04-27 00:21:05.000000 tencentcloud-sdk-python-cfw-3.0.883/tencentcloud/cfw/v20190904/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    65621 2023-04-27 00:21:05.000000 tencentcloud-sdk-python-cfw-3.0.883/tencentcloud/cfw/v20190904/cfw_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 00:21:05.000000 tencentcloud-sdk-python-cfw-3.0.883/tencentcloud/cfw/v20190904/__init__.py
--rw-r--r--   0 root         (0) root         (0)   215547 2023-04-27 00:21:05.000000 tencentcloud-sdk-python-cfw-3.0.883/tencentcloud/cfw/v20190904/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 00:21:05.000000 tencentcloud-sdk-python-cfw-3.0.883/tencentcloud/cfw/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-27 00:21:05.000000 tencentcloud-sdk-python-cfw-3.0.883/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:21:05.000000 tencentcloud-sdk-python-cfw-3.0.883/tencentcloud_sdk_python_cfw.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 00:21:05.000000 tencentcloud-sdk-python-cfw-3.0.883/tencentcloud_sdk_python_cfw.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-27 00:21:05.000000 tencentcloud-sdk-python-cfw-3.0.883/tencentcloud_sdk_python_cfw.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-27 00:21:05.000000 tencentcloud-sdk-python-cfw-3.0.883/tencentcloud_sdk_python_cfw.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-27 00:21:05.000000 tencentcloud-sdk-python-cfw-3.0.883/tencentcloud_sdk_python_cfw.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-27 00:21:05.000000 tencentcloud-sdk-python-cfw-3.0.883/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-27 00:21:05.000000 tencentcloud-sdk-python-cfw-3.0.883/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-27 00:21:05.000000 tencentcloud-sdk-python-cfw-3.0.883/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:08:16.000000 tencentcloud-sdk-python-cfw-3.0.884/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-28 02:08:16.000000 tencentcloud-sdk-python-cfw-3.0.884/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:08:16.000000 tencentcloud-sdk-python-cfw-3.0.884/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:08:16.000000 tencentcloud-sdk-python-cfw-3.0.884/tencentcloud/cfw/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:08:16.000000 tencentcloud-sdk-python-cfw-3.0.884/tencentcloud/cfw/v20190904/
+-rw-r--r--   0 root         (0) root         (0)     1836 2023-04-28 02:08:16.000000 tencentcloud-sdk-python-cfw-3.0.884/tencentcloud/cfw/v20190904/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    65621 2023-04-28 02:08:16.000000 tencentcloud-sdk-python-cfw-3.0.884/tencentcloud/cfw/v20190904/cfw_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 02:08:16.000000 tencentcloud-sdk-python-cfw-3.0.884/tencentcloud/cfw/v20190904/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   215744 2023-04-28 02:08:16.000000 tencentcloud-sdk-python-cfw-3.0.884/tencentcloud/cfw/v20190904/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 02:08:16.000000 tencentcloud-sdk-python-cfw-3.0.884/tencentcloud/cfw/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-28 02:08:16.000000 tencentcloud-sdk-python-cfw-3.0.884/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:08:16.000000 tencentcloud-sdk-python-cfw-3.0.884/tencentcloud_sdk_python_cfw.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 02:08:16.000000 tencentcloud-sdk-python-cfw-3.0.884/tencentcloud_sdk_python_cfw.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-28 02:08:16.000000 tencentcloud-sdk-python-cfw-3.0.884/tencentcloud_sdk_python_cfw.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-28 02:08:16.000000 tencentcloud-sdk-python-cfw-3.0.884/tencentcloud_sdk_python_cfw.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-28 02:08:16.000000 tencentcloud-sdk-python-cfw-3.0.884/tencentcloud_sdk_python_cfw.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-28 02:08:16.000000 tencentcloud-sdk-python-cfw-3.0.884/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-28 02:08:16.000000 tencentcloud-sdk-python-cfw-3.0.884/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-28 02:08:16.000000 tencentcloud-sdk-python-cfw-3.0.884/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cfw-3.0.883/README.rst` & `tencentcloud-sdk-python-cfw-3.0.884/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cfw-3.0.883/tencentcloud/cfw/v20190904/errorcodes.py` & `tencentcloud-sdk-python-cfw-3.0.884/tencentcloud/cfw/v20190904/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cfw-3.0.883/tencentcloud/cfw/v20190904/cfw_client.py` & `tencentcloud-sdk-python-cfw-3.0.884/tencentcloud/cfw/v20190904/cfw_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cfw-3.0.883/tencentcloud/cfw/v20190904/models.py` & `tencentcloud-sdk-python-cfw-3.0.884/tencentcloud/cfw/v20190904/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -519,14 +519,17 @@
         :type UniqueId: str
         :param MatchTimes: 规则命中次数
 注意：此字段可能返回 null，表示取不到有效值。
         :type MatchTimes: int
         :param Country: 国家
 注意：此字段可能返回 null，表示取不到有效值。
         :type Country: str
+        :param Comment: 备注
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Comment: str
         """
         self.Domain = None
         self.Ioc = None
         self.Level = None
         self.EventName = None
         self.Direction = None
         self.Protocol = None
@@ -535,14 +538,15 @@
         self.StartTime = None
         self.EndTime = None
         self.IgnoreReason = None
         self.Source = None
         self.UniqueId = None
         self.MatchTimes = None
         self.Country = None
+        self.Comment = None
 
 
     def _deserialize(self, params):
         self.Domain = params.get("Domain")
         self.Ioc = params.get("Ioc")
         self.Level = params.get("Level")
         self.EventName = params.get("EventName")
@@ -553,14 +557,15 @@
         self.StartTime = params.get("StartTime")
         self.EndTime = params.get("EndTime")
         self.IgnoreReason = params.get("IgnoreReason")
         self.Source = params.get("Source")
         self.UniqueId = params.get("UniqueId")
         self.MatchTimes = params.get("MatchTimes")
         self.Country = params.get("Country")
+        self.Comment = params.get("Comment")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -1933,17 +1938,17 @@
         :type Limit: int
         :param Offset: 页偏移量
         :type Offset: int
         :param Direction: 方向：1互联网入站，0互联网出站，3内网，空 全部方向
         :type Direction: str
         :param RuleType: 规则类型：1封禁，2放通
         :type RuleType: int
-        :param Order: 排序列：EndTime结束时间，StartTime开始时间，MatchTimes命中次数
+        :param Order: 排序类型：desc降序，asc正序
         :type Order: str
-        :param By: 排序类型：desc降序，asc正序
+        :param By: 排序列：EndTime结束时间，StartTime开始时间，MatchTimes命中次数
         :type By: str
         :param SearchValue: 搜索参数，json格式字符串，空则传"{}"，域名：domain，危险等级：level，放通原因：ignore_reason，安全事件来源：rule_source，地理位置：address，模糊搜索：common
         :type SearchValue: str
         """
         self.Limit = None
         self.Offset = None
         self.Direction = None
```

### Comparing `tencentcloud-sdk-python-cfw-3.0.883/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cfw-3.0.884/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cfw-3.0.883/tencentcloud_sdk_python_cfw.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cfw-3.0.884/tencentcloud_sdk_python_cfw.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cfw
-Version: 3.0.883
+Version: 3.0.884
 Summary: Tencent Cloud Cfw SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cfw-3.0.883/PKG-INFO` & `tencentcloud-sdk-python-cfw-3.0.884/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cfw
-Version: 3.0.883
+Version: 3.0.884
 Summary: Tencent Cloud Cfw SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cfw-3.0.883/setup.py` & `tencentcloud-sdk-python-cfw-3.0.884/setup.py`

 * *Files identical despite different names*

