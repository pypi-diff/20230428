# Comparing `tmp/tencentcloud-sdk-python-yinsuda-3.0.883.tar.gz` & `tmp/tencentcloud-sdk-python-yinsuda-3.0.884.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-yinsuda-3.0.883.tar", last modified: Thu Apr 27 01:04:02 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-yinsuda-3.0.884.tar", last modified: Fri Apr 28 02:48:11 2023, max compression
```

## Comparing `tencentcloud-sdk-python-yinsuda-3.0.883.tar` & `tencentcloud-sdk-python-yinsuda-3.0.884.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 01:04:02.000000 tencentcloud-sdk-python-yinsuda-3.0.883/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 01:04:02.000000 tencentcloud-sdk-python-yinsuda-3.0.883/tencentcloud_sdk_python_yinsuda.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 01:04:02.000000 tencentcloud-sdk-python-yinsuda-3.0.883/tencentcloud_sdk_python_yinsuda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      485 2023-04-27 01:04:02.000000 tencentcloud-sdk-python-yinsuda-3.0.883/tencentcloud_sdk_python_yinsuda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-04-27 01:04:02.000000 tencentcloud-sdk-python-yinsuda-3.0.883/tencentcloud_sdk_python_yinsuda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-27 01:04:02.000000 tencentcloud-sdk-python-yinsuda-3.0.883/tencentcloud_sdk_python_yinsuda.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      749 2023-04-27 01:04:02.000000 tencentcloud-sdk-python-yinsuda-3.0.883/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 01:04:02.000000 tencentcloud-sdk-python-yinsuda-3.0.883/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 01:04:02.000000 tencentcloud-sdk-python-yinsuda-3.0.883/tencentcloud/yinsuda/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 01:04:02.000000 tencentcloud-sdk-python-yinsuda-3.0.883/tencentcloud/yinsuda/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 01:04:02.000000 tencentcloud-sdk-python-yinsuda-3.0.883/tencentcloud/yinsuda/v20220527/
--rw-r--r--   0 root         (0) root         (0)     1440 2023-04-27 01:04:02.000000 tencentcloud-sdk-python-yinsuda-3.0.883/tencentcloud/yinsuda/v20220527/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 01:04:02.000000 tencentcloud-sdk-python-yinsuda-3.0.883/tencentcloud/yinsuda/v20220527/__init__.py
--rw-r--r--   0 root         (0) root         (0)    71463 2023-04-27 01:04:02.000000 tencentcloud-sdk-python-yinsuda-3.0.883/tencentcloud/yinsuda/v20220527/models.py
--rw-r--r--   0 root         (0) root         (0)    15889 2023-04-27 01:04:02.000000 tencentcloud-sdk-python-yinsuda-3.0.883/tencentcloud/yinsuda/v20220527/yinsuda_client.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-27 01:04:02.000000 tencentcloud-sdk-python-yinsuda-3.0.883/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1679 2023-04-27 01:04:02.000000 tencentcloud-sdk-python-yinsuda-3.0.883/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1014 2023-04-27 01:04:02.000000 tencentcloud-sdk-python-yinsuda-3.0.883/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-27 01:04:02.000000 tencentcloud-sdk-python-yinsuda-3.0.883/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:48:11.000000 tencentcloud-sdk-python-yinsuda-3.0.884/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:48:11.000000 tencentcloud-sdk-python-yinsuda-3.0.884/tencentcloud_sdk_python_yinsuda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 02:48:11.000000 tencentcloud-sdk-python-yinsuda-3.0.884/tencentcloud_sdk_python_yinsuda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      485 2023-04-28 02:48:11.000000 tencentcloud-sdk-python-yinsuda-3.0.884/tencentcloud_sdk_python_yinsuda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-04-28 02:48:11.000000 tencentcloud-sdk-python-yinsuda-3.0.884/tencentcloud_sdk_python_yinsuda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-28 02:48:11.000000 tencentcloud-sdk-python-yinsuda-3.0.884/tencentcloud_sdk_python_yinsuda.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      749 2023-04-28 02:48:10.000000 tencentcloud-sdk-python-yinsuda-3.0.884/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:48:11.000000 tencentcloud-sdk-python-yinsuda-3.0.884/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:48:11.000000 tencentcloud-sdk-python-yinsuda-3.0.884/tencentcloud/yinsuda/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 02:48:10.000000 tencentcloud-sdk-python-yinsuda-3.0.884/tencentcloud/yinsuda/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:48:11.000000 tencentcloud-sdk-python-yinsuda-3.0.884/tencentcloud/yinsuda/v20220527/
+-rw-r--r--   0 root         (0) root         (0)     1440 2023-04-28 02:48:10.000000 tencentcloud-sdk-python-yinsuda-3.0.884/tencentcloud/yinsuda/v20220527/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 02:48:10.000000 tencentcloud-sdk-python-yinsuda-3.0.884/tencentcloud/yinsuda/v20220527/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    72270 2023-04-28 02:48:10.000000 tencentcloud-sdk-python-yinsuda-3.0.884/tencentcloud/yinsuda/v20220527/models.py
+-rw-r--r--   0 root         (0) root         (0)    15889 2023-04-28 02:48:10.000000 tencentcloud-sdk-python-yinsuda-3.0.884/tencentcloud/yinsuda/v20220527/yinsuda_client.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-28 02:48:10.000000 tencentcloud-sdk-python-yinsuda-3.0.884/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-04-28 02:48:11.000000 tencentcloud-sdk-python-yinsuda-3.0.884/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-04-28 02:48:10.000000 tencentcloud-sdk-python-yinsuda-3.0.884/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-28 02:48:11.000000 tencentcloud-sdk-python-yinsuda-3.0.884/setup.cfg
```

### Comparing `tencentcloud-sdk-python-yinsuda-3.0.883/tencentcloud_sdk_python_yinsuda.egg-info/PKG-INFO` & `tencentcloud-sdk-python-yinsuda-3.0.884/tencentcloud_sdk_python_yinsuda.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-yinsuda
-Version: 3.0.883
+Version: 3.0.884
 Summary: Tencent Cloud Yinsuda SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-yinsuda-3.0.883/README.rst` & `tencentcloud-sdk-python-yinsuda-3.0.884/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-yinsuda-3.0.883/tencentcloud/yinsuda/v20220527/errorcodes.py` & `tencentcloud-sdk-python-yinsuda-3.0.884/tencentcloud/yinsuda/v20220527/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-yinsuda-3.0.883/tencentcloud/yinsuda/v20220527/models.py` & `tencentcloud-sdk-python-yinsuda-3.0.884/tencentcloud/yinsuda/v20220527/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -368,30 +368,36 @@
         :type ScrollToken: str
         :param Limit: 返回条数限制，默认 20，最大 50。
         :type Limit: int
         :param RightFilters: 权益过滤，取值有：
 <li>Play：可播；</li>
 <li>Sing：可唱。</li>
         :type RightFilters: list of str
+        :param MaterialFilters: 物料过滤，取值有：
+<li>Lyrics：含有歌词；</li>
+<li>Midi：含有音高线。</li>
+        :type MaterialFilters: list of str
         """
         self.AppName = None
         self.UserId = None
         self.TagId = None
         self.ScrollToken = None
         self.Limit = None
         self.RightFilters = None
+        self.MaterialFilters = None
 
 
     def _deserialize(self, params):
         self.AppName = params.get("AppName")
         self.UserId = params.get("UserId")
         self.TagId = params.get("TagId")
         self.ScrollToken = params.get("ScrollToken")
         self.Limit = params.get("Limit")
         self.RightFilters = params.get("RightFilters")
+        self.MaterialFilters = params.get("MaterialFilters")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -447,32 +453,38 @@
         :param RightFilters: 权益过滤，取值有：
 <li>Play：可播；</li>
 <li>Sing：可唱。</li>
         :type RightFilters: list of str
         :param PlayScene: 播放场景。默认为Chat
 <li>Live：直播</li><li>Chat：语聊</li>
         :type PlayScene: str
+        :param MaterialFilters: 物料过滤，取值有：
+<li>Lyrics：含有歌词；</li>
+<li>Midi：含有音高线。</li>
+        :type MaterialFilters: list of str
         """
         self.AppName = None
         self.UserId = None
         self.PlaylistId = None
         self.ScrollToken = None
         self.Limit = None
         self.RightFilters = None
         self.PlayScene = None
+        self.MaterialFilters = None
 
 
     def _deserialize(self, params):
         self.AppName = params.get("AppName")
         self.UserId = params.get("UserId")
         self.PlaylistId = params.get("PlaylistId")
         self.ScrollToken = params.get("ScrollToken")
         self.Limit = params.get("Limit")
         self.RightFilters = params.get("RightFilters")
         self.PlayScene = params.get("PlayScene")
+        self.MaterialFilters = params.get("MaterialFilters")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -1686,32 +1698,38 @@
         :param RightFilters: 权益过滤，取值有：
 <li>Play：可播；</li>
 <li>Sing：可唱。</li>
         :type RightFilters: list of str
         :param PlayScene: 播放场景。默认为Chat
 <li>Live：直播</li><li>Chat：语聊</li>
         :type PlayScene: str
+        :param MaterialFilters: 物料过滤，取值有：
+<li>Lyrics：含有歌词；</li>
+<li>Midi：含有音高线。</li>
+        :type MaterialFilters: list of str
         """
         self.AppName = None
         self.UserId = None
         self.KeyWord = None
         self.ScrollToken = None
         self.Limit = None
         self.RightFilters = None
         self.PlayScene = None
+        self.MaterialFilters = None
 
 
     def _deserialize(self, params):
         self.AppName = params.get("AppName")
         self.UserId = params.get("UserId")
         self.KeyWord = params.get("KeyWord")
         self.ScrollToken = params.get("ScrollToken")
         self.Limit = params.get("Limit")
         self.RightFilters = params.get("RightFilters")
         self.PlayScene = params.get("PlayScene")
+        self.MaterialFilters = params.get("MaterialFilters")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-yinsuda-3.0.883/tencentcloud/yinsuda/v20220527/yinsuda_client.py` & `tencentcloud-sdk-python-yinsuda-3.0.884/tencentcloud/yinsuda/v20220527/yinsuda_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-yinsuda-3.0.883/tencentcloud/__init__.py` & `tencentcloud-sdk-python-yinsuda-3.0.884/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-yinsuda-3.0.883/PKG-INFO` & `tencentcloud-sdk-python-yinsuda-3.0.884/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-yinsuda
-Version: 3.0.883
+Version: 3.0.884
 Summary: Tencent Cloud Yinsuda SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-yinsuda-3.0.883/setup.py` & `tencentcloud-sdk-python-yinsuda-3.0.884/setup.py`

 * *Files identical despite different names*

