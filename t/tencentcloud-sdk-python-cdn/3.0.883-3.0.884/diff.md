# Comparing `tmp/tencentcloud-sdk-python-cdn-3.0.883.tar.gz` & `tmp/tencentcloud-sdk-python-cdn-3.0.884.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cdn-3.0.883.tar", last modified: Thu Apr 27 00:20:22 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cdn-3.0.884.tar", last modified: Fri Apr 28 02:07:44 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cdn-3.0.883.tar` & `tencentcloud-sdk-python-cdn-3.0.884.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:20:22.000000 tencentcloud-sdk-python-cdn-3.0.883/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-27 00:20:21.000000 tencentcloud-sdk-python-cdn-3.0.883/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:20:22.000000 tencentcloud-sdk-python-cdn-3.0.883/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-27 00:20:21.000000 tencentcloud-sdk-python-cdn-3.0.883/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:20:22.000000 tencentcloud-sdk-python-cdn-3.0.883/tencentcloud/cdn/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 00:20:21.000000 tencentcloud-sdk-python-cdn-3.0.883/tencentcloud/cdn/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:20:22.000000 tencentcloud-sdk-python-cdn-3.0.883/tencentcloud/cdn/v20180606/
--rw-r--r--   0 root         (0) root         (0)    21844 2023-04-27 00:20:21.000000 tencentcloud-sdk-python-cdn-3.0.883/tencentcloud/cdn/v20180606/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    80657 2023-04-27 00:20:21.000000 tencentcloud-sdk-python-cdn-3.0.883/tencentcloud/cdn/v20180606/cdn_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 00:20:21.000000 tencentcloud-sdk-python-cdn-3.0.883/tencentcloud/cdn/v20180606/__init__.py
--rw-r--r--   0 root         (0) root         (0)   568258 2023-04-27 00:20:21.000000 tencentcloud-sdk-python-cdn-3.0.883/tencentcloud/cdn/v20180606/models.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-27 00:20:22.000000 tencentcloud-sdk-python-cdn-3.0.883/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:20:22.000000 tencentcloud-sdk-python-cdn-3.0.883/tencentcloud_sdk_python_cdn.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 00:20:22.000000 tencentcloud-sdk-python-cdn-3.0.883/tencentcloud_sdk_python_cdn.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-27 00:20:22.000000 tencentcloud-sdk-python-cdn-3.0.883/tencentcloud_sdk_python_cdn.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-27 00:20:22.000000 tencentcloud-sdk-python-cdn-3.0.883/tencentcloud_sdk_python_cdn.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-27 00:20:22.000000 tencentcloud-sdk-python-cdn-3.0.883/tencentcloud_sdk_python_cdn.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-27 00:20:21.000000 tencentcloud-sdk-python-cdn-3.0.883/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-27 00:20:22.000000 tencentcloud-sdk-python-cdn-3.0.883/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:07:44.000000 tencentcloud-sdk-python-cdn-3.0.884/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-28 02:07:44.000000 tencentcloud-sdk-python-cdn-3.0.884/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:07:44.000000 tencentcloud-sdk-python-cdn-3.0.884/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-28 02:07:44.000000 tencentcloud-sdk-python-cdn-3.0.884/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:07:44.000000 tencentcloud-sdk-python-cdn-3.0.884/tencentcloud/cdn/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 02:07:44.000000 tencentcloud-sdk-python-cdn-3.0.884/tencentcloud/cdn/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:07:44.000000 tencentcloud-sdk-python-cdn-3.0.884/tencentcloud/cdn/v20180606/
+-rw-r--r--   0 root         (0) root         (0)    21844 2023-04-28 02:07:44.000000 tencentcloud-sdk-python-cdn-3.0.884/tencentcloud/cdn/v20180606/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    80657 2023-04-28 02:07:44.000000 tencentcloud-sdk-python-cdn-3.0.884/tencentcloud/cdn/v20180606/cdn_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 02:07:44.000000 tencentcloud-sdk-python-cdn-3.0.884/tencentcloud/cdn/v20180606/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   568491 2023-04-28 02:07:44.000000 tencentcloud-sdk-python-cdn-3.0.884/tencentcloud/cdn/v20180606/models.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-28 02:07:44.000000 tencentcloud-sdk-python-cdn-3.0.884/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:07:44.000000 tencentcloud-sdk-python-cdn-3.0.884/tencentcloud_sdk_python_cdn.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 02:07:44.000000 tencentcloud-sdk-python-cdn-3.0.884/tencentcloud_sdk_python_cdn.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-28 02:07:44.000000 tencentcloud-sdk-python-cdn-3.0.884/tencentcloud_sdk_python_cdn.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-28 02:07:44.000000 tencentcloud-sdk-python-cdn-3.0.884/tencentcloud_sdk_python_cdn.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-28 02:07:44.000000 tencentcloud-sdk-python-cdn-3.0.884/tencentcloud_sdk_python_cdn.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-28 02:07:44.000000 tencentcloud-sdk-python-cdn-3.0.884/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-28 02:07:44.000000 tencentcloud-sdk-python-cdn-3.0.884/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cdn-3.0.883/README.rst` & `tencentcloud-sdk-python-cdn-3.0.884/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdn-3.0.883/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cdn-3.0.884/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cdn-3.0.883/tencentcloud/cdn/v20180606/errorcodes.py` & `tencentcloud-sdk-python-cdn-3.0.884/tencentcloud/cdn/v20180606/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdn-3.0.883/tencentcloud/cdn/v20180606/cdn_client.py` & `tencentcloud-sdk-python-cdn-3.0.884/tencentcloud/cdn/v20180606/cdn_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdn-3.0.883/tencentcloud/cdn/v20180606/models.py` & `tencentcloud-sdk-python-cdn-3.0.884/tencentcloud/cdn/v20180606/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -5573,26 +5573,34 @@
     """
 
     def __init__(self):
         r"""
         :param Area: 指定服务地域查询
 mainland：境内计费方式查询
 overseas：境外计费方式查询
-未填充时默认为 mainland
+global：全球计费方式查询
+未填充时，默认为 mainland
         :type Area: str
         :param Product: 指定查询的产品数据，可选为cdn或者ecdn，默认为cdn
         :type Product: str
+        :param Type: 指定资源包查询
+flux：流量包
+https：HTTPS请求包
+未填充时，默认为 flux
+        :type Type: str
         """
         self.Area = None
         self.Product = None
+        self.Type = None
 
 
     def _deserialize(self, params):
         self.Area = params.get("Area")
         self.Product = params.get("Product")
+        self.Type = params.get("Type")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -5601,38 +5609,39 @@
 class DescribePayTypeResponse(AbstractModel):
     """DescribePayType返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param PayType: 计费类型：
+        :param PayType: 计费类型
 flux：流量计费
 bandwidth：带宽计费
 request：请求数计费
 flux_sep：动静分离流量计费
 bandwidth_sep：动静分离带宽计费
 日结计费方式切换时，若当日产生消耗，则此字段表示第二天即将生效的计费方式，若未产生消耗，则表示已经生效的计费方式。
         :type PayType: str
-        :param BillingCycle: 计费周期：
+        :param BillingCycle: 计费周期
 day：日结计费
 month：月结计费
 hour：小时结计费
         :type BillingCycle: str
-        :param StatType: monthMax：日峰值月平均，月结模式
+        :param StatType: 统计类型
+monthMax：日峰值月平均，月结模式
 day95：日 95 带宽，月结模式
 month95：月95带宽，月结模式
 sum：总流量/总请求数，日结或月结模式
 max：峰值带宽，日结模式
         :type StatType: str
-        :param RegionType: 境外计费类型：
+        :param RegionType: 计费区域
 all：全地区统一计费
 multiple：分地区计费
         :type RegionType: str
-        :param CurrentPayType: 当前生效计费类型：
+        :param CurrentPayType: 当前生效计费类型
 flux：流量计费
 bandwidth：带宽计费
 request：请求数计费
 flux_sep：动静分离流量计费
 bandwidth_sep：动静分离带宽计费
         :type CurrentPayType: str
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
```

### Comparing `tencentcloud-sdk-python-cdn-3.0.883/PKG-INFO` & `tencentcloud-sdk-python-cdn-3.0.884/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdn
-Version: 3.0.883
+Version: 3.0.884
 Summary: Tencent Cloud Cdn SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdn-3.0.883/tencentcloud_sdk_python_cdn.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cdn-3.0.884/tencentcloud_sdk_python_cdn.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdn
-Version: 3.0.883
+Version: 3.0.884
 Summary: Tencent Cloud Cdn SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdn-3.0.883/setup.py` & `tencentcloud-sdk-python-cdn-3.0.884/setup.py`

 * *Files identical despite different names*

