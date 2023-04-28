# Comparing `tmp/tencentcloud-sdk-python-teo-3.0.883.tar.gz` & `tmp/tencentcloud-sdk-python-teo-3.0.884.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-teo-3.0.883.tar", last modified: Thu Apr 27 00:54:15 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-teo-3.0.884.tar", last modified: Fri Apr 28 02:41:14 2023, max compression
```

## Comparing `tencentcloud-sdk-python-teo-3.0.883.tar` & `tencentcloud-sdk-python-teo-3.0.884.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:54:15.000000 tencentcloud-sdk-python-teo-3.0.883/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-27 00:54:15.000000 tencentcloud-sdk-python-teo-3.0.883/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:54:15.000000 tencentcloud-sdk-python-teo-3.0.883/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:54:15.000000 tencentcloud-sdk-python-teo-3.0.883/tencentcloud/teo/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:54:15.000000 tencentcloud-sdk-python-teo-3.0.883/tencentcloud/teo/v20220106/
--rw-r--r--   0 root         (0) root         (0)     2192 2023-04-27 00:54:15.000000 tencentcloud-sdk-python-teo-3.0.883/tencentcloud/teo/v20220106/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 00:54:15.000000 tencentcloud-sdk-python-teo-3.0.883/tencentcloud/teo/v20220106/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24724 2023-04-27 00:54:15.000000 tencentcloud-sdk-python-teo-3.0.883/tencentcloud/teo/v20220106/models.py
--rw-r--r--   0 root         (0) root         (0)     5379 2023-04-27 00:54:15.000000 tencentcloud-sdk-python-teo-3.0.883/tencentcloud/teo/v20220106/teo_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 00:54:15.000000 tencentcloud-sdk-python-teo-3.0.883/tencentcloud/teo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:54:15.000000 tencentcloud-sdk-python-teo-3.0.883/tencentcloud/teo/v20220901/
--rw-r--r--   0 root         (0) root         (0)    21826 2023-04-27 00:54:15.000000 tencentcloud-sdk-python-teo-3.0.883/tencentcloud/teo/v20220901/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 00:54:15.000000 tencentcloud-sdk-python-teo-3.0.883/tencentcloud/teo/v20220901/__init__.py
--rw-r--r--   0 root         (0) root         (0)   512047 2023-04-27 00:54:15.000000 tencentcloud-sdk-python-teo-3.0.883/tencentcloud/teo/v20220901/models.py
--rw-r--r--   0 root         (0) root         (0)    84601 2023-04-27 00:54:15.000000 tencentcloud-sdk-python-teo-3.0.883/tencentcloud/teo/v20220901/teo_client.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-27 00:54:15.000000 tencentcloud-sdk-python-teo-3.0.883/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-27 00:54:15.000000 tencentcloud-sdk-python-teo-3.0.883/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:54:15.000000 tencentcloud-sdk-python-teo-3.0.883/tencentcloud_sdk_python_teo.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 00:54:15.000000 tencentcloud-sdk-python-teo-3.0.883/tencentcloud_sdk_python_teo.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      603 2023-04-27 00:54:15.000000 tencentcloud-sdk-python-teo-3.0.883/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-27 00:54:15.000000 tencentcloud-sdk-python-teo-3.0.883/tencentcloud_sdk_python_teo.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-27 00:54:15.000000 tencentcloud-sdk-python-teo-3.0.883/tencentcloud_sdk_python_teo.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-27 00:54:15.000000 tencentcloud-sdk-python-teo-3.0.883/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-27 00:54:15.000000 tencentcloud-sdk-python-teo-3.0.883/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:41:14.000000 tencentcloud-sdk-python-teo-3.0.884/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-28 02:41:14.000000 tencentcloud-sdk-python-teo-3.0.884/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:41:14.000000 tencentcloud-sdk-python-teo-3.0.884/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:41:14.000000 tencentcloud-sdk-python-teo-3.0.884/tencentcloud/teo/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:41:14.000000 tencentcloud-sdk-python-teo-3.0.884/tencentcloud/teo/v20220106/
+-rw-r--r--   0 root         (0) root         (0)     2192 2023-04-28 02:41:14.000000 tencentcloud-sdk-python-teo-3.0.884/tencentcloud/teo/v20220106/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 02:41:14.000000 tencentcloud-sdk-python-teo-3.0.884/tencentcloud/teo/v20220106/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24724 2023-04-28 02:41:14.000000 tencentcloud-sdk-python-teo-3.0.884/tencentcloud/teo/v20220106/models.py
+-rw-r--r--   0 root         (0) root         (0)     5379 2023-04-28 02:41:14.000000 tencentcloud-sdk-python-teo-3.0.884/tencentcloud/teo/v20220106/teo_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 02:41:14.000000 tencentcloud-sdk-python-teo-3.0.884/tencentcloud/teo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:41:14.000000 tencentcloud-sdk-python-teo-3.0.884/tencentcloud/teo/v20220901/
+-rw-r--r--   0 root         (0) root         (0)    21826 2023-04-28 02:41:14.000000 tencentcloud-sdk-python-teo-3.0.884/tencentcloud/teo/v20220901/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 02:41:14.000000 tencentcloud-sdk-python-teo-3.0.884/tencentcloud/teo/v20220901/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   512265 2023-04-28 02:41:14.000000 tencentcloud-sdk-python-teo-3.0.884/tencentcloud/teo/v20220901/models.py
+-rw-r--r--   0 root         (0) root         (0)    84601 2023-04-28 02:41:14.000000 tencentcloud-sdk-python-teo-3.0.884/tencentcloud/teo/v20220901/teo_client.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-28 02:41:14.000000 tencentcloud-sdk-python-teo-3.0.884/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-28 02:41:14.000000 tencentcloud-sdk-python-teo-3.0.884/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:41:14.000000 tencentcloud-sdk-python-teo-3.0.884/tencentcloud_sdk_python_teo.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 02:41:14.000000 tencentcloud-sdk-python-teo-3.0.884/tencentcloud_sdk_python_teo.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      603 2023-04-28 02:41:14.000000 tencentcloud-sdk-python-teo-3.0.884/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-28 02:41:14.000000 tencentcloud-sdk-python-teo-3.0.884/tencentcloud_sdk_python_teo.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-28 02:41:14.000000 tencentcloud-sdk-python-teo-3.0.884/tencentcloud_sdk_python_teo.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-28 02:41:14.000000 tencentcloud-sdk-python-teo-3.0.884/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-28 02:41:14.000000 tencentcloud-sdk-python-teo-3.0.884/setup.cfg
```

### Comparing `tencentcloud-sdk-python-teo-3.0.883/README.rst` & `tencentcloud-sdk-python-teo-3.0.884/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.883/tencentcloud/teo/v20220106/errorcodes.py` & `tencentcloud-sdk-python-teo-3.0.884/tencentcloud/teo/v20220106/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.883/tencentcloud/teo/v20220106/models.py` & `tencentcloud-sdk-python-teo-3.0.884/tencentcloud/teo/v20220106/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.883/tencentcloud/teo/v20220106/teo_client.py` & `tencentcloud-sdk-python-teo-3.0.884/tencentcloud/teo/v20220106/teo_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.883/tencentcloud/teo/v20220901/errorcodes.py` & `tencentcloud-sdk-python-teo-3.0.884/tencentcloud/teo/v20220901/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.883/tencentcloud/teo/v20220901/models.py` & `tencentcloud-sdk-python-teo-3.0.884/tencentcloud/teo/v20220901/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -13386,16 +13386,17 @@
         :type ActiveStatus: str
         :param AliasZoneName: 站点别名。数字、英文、-和_组合，限制20个字符。
 注意：此字段可能返回 null，表示取不到有效值。
         :type AliasZoneName: str
         :param IsFake: 是否伪站点，取值有：
 <li> 0：非伪站点；</li>
 <li> 1：伪站点。</li>
-注意：此字段可能返回 null，表示取不到有效值。
         :type IsFake: int
+        :param LockStatus: 锁定状态，取值有：<li> enable：正常，允许进行修改操作；</li><li> disable：锁定中，不允许进行修改操作。</li>
+        :type LockStatus: str
         """
         self.ZoneId = None
         self.ZoneName = None
         self.OriginalNameServers = None
         self.NameServers = None
         self.Status = None
         self.Type = None
@@ -13408,14 +13409,15 @@
         self.ModifiedOn = None
         self.Area = None
         self.VanityNameServers = None
         self.VanityNameServersIps = None
         self.ActiveStatus = None
         self.AliasZoneName = None
         self.IsFake = None
+        self.LockStatus = None
 
 
     def _deserialize(self, params):
         self.ZoneId = params.get("ZoneId")
         self.ZoneName = params.get("ZoneName")
         self.OriginalNameServers = params.get("OriginalNameServers")
         self.NameServers = params.get("NameServers")
@@ -13447,14 +13449,15 @@
             for item in params.get("VanityNameServersIps"):
                 obj = VanityNameServersIps()
                 obj._deserialize(item)
                 self.VanityNameServersIps.append(obj)
         self.ActiveStatus = params.get("ActiveStatus")
         self.AliasZoneName = params.get("AliasZoneName")
         self.IsFake = params.get("IsFake")
+        self.LockStatus = params.get("LockStatus")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-teo-3.0.883/tencentcloud/teo/v20220901/teo_client.py` & `tencentcloud-sdk-python-teo-3.0.884/tencentcloud/teo/v20220901/teo_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.883/tencentcloud/__init__.py` & `tencentcloud-sdk-python-teo-3.0.884/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-teo-3.0.883/PKG-INFO` & `tencentcloud-sdk-python-teo-3.0.884/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-teo
-Version: 3.0.883
+Version: 3.0.884
 Summary: Tencent Cloud Teo SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-teo-3.0.883/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-teo-3.0.884/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.883/tencentcloud_sdk_python_teo.egg-info/PKG-INFO` & `tencentcloud-sdk-python-teo-3.0.884/tencentcloud_sdk_python_teo.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-teo
-Version: 3.0.883
+Version: 3.0.884
 Summary: Tencent Cloud Teo SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-teo-3.0.883/setup.py` & `tencentcloud-sdk-python-teo-3.0.884/setup.py`

 * *Files identical despite different names*

