# Comparing `tmp/tencentcloud-sdk-python-tsf-3.0.883.tar.gz` & `tmp/tencentcloud-sdk-python-tsf-3.0.884.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tsf-3.0.883.tar", last modified: Thu Apr 27 00:59:31 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tsf-3.0.884.tar", last modified: Fri Apr 28 02:46:38 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tsf-3.0.883.tar` & `tencentcloud-sdk-python-tsf-3.0.884.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:59:31.000000 tencentcloud-sdk-python-tsf-3.0.883/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-27 00:59:31.000000 tencentcloud-sdk-python-tsf-3.0.883/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:59:31.000000 tencentcloud-sdk-python-tsf-3.0.883/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:59:31.000000 tencentcloud-sdk-python-tsf-3.0.883/tencentcloud/tsf/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:59:31.000000 tencentcloud-sdk-python-tsf-3.0.883/tencentcloud/tsf/v20180326/
--rw-r--r--   0 root         (0) root         (0)    49509 2023-04-27 00:59:31.000000 tencentcloud-sdk-python-tsf-3.0.883/tencentcloud/tsf/v20180326/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   193599 2023-04-27 00:59:31.000000 tencentcloud-sdk-python-tsf-3.0.883/tencentcloud/tsf/v20180326/tsf_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 00:59:31.000000 tencentcloud-sdk-python-tsf-3.0.883/tencentcloud/tsf/v20180326/__init__.py
--rw-r--r--   0 root         (0) root         (0)   798817 2023-04-27 00:59:31.000000 tencentcloud-sdk-python-tsf-3.0.883/tencentcloud/tsf/v20180326/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 00:59:31.000000 tencentcloud-sdk-python-tsf-3.0.883/tencentcloud/tsf/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-27 00:59:31.000000 tencentcloud-sdk-python-tsf-3.0.883/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:59:31.000000 tencentcloud-sdk-python-tsf-3.0.883/tencentcloud_sdk_python_tsf.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 00:59:31.000000 tencentcloud-sdk-python-tsf-3.0.883/tencentcloud_sdk_python_tsf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-27 00:59:31.000000 tencentcloud-sdk-python-tsf-3.0.883/tencentcloud_sdk_python_tsf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-27 00:59:31.000000 tencentcloud-sdk-python-tsf-3.0.883/tencentcloud_sdk_python_tsf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-27 00:59:31.000000 tencentcloud-sdk-python-tsf-3.0.883/tencentcloud_sdk_python_tsf.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-27 00:59:31.000000 tencentcloud-sdk-python-tsf-3.0.883/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-27 00:59:31.000000 tencentcloud-sdk-python-tsf-3.0.883/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-27 00:59:31.000000 tencentcloud-sdk-python-tsf-3.0.883/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:46:38.000000 tencentcloud-sdk-python-tsf-3.0.884/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-28 02:46:38.000000 tencentcloud-sdk-python-tsf-3.0.884/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:46:38.000000 tencentcloud-sdk-python-tsf-3.0.884/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:46:38.000000 tencentcloud-sdk-python-tsf-3.0.884/tencentcloud/tsf/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:46:38.000000 tencentcloud-sdk-python-tsf-3.0.884/tencentcloud/tsf/v20180326/
+-rw-r--r--   0 root         (0) root         (0)    49509 2023-04-28 02:46:38.000000 tencentcloud-sdk-python-tsf-3.0.884/tencentcloud/tsf/v20180326/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   193599 2023-04-28 02:46:38.000000 tencentcloud-sdk-python-tsf-3.0.884/tencentcloud/tsf/v20180326/tsf_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 02:46:38.000000 tencentcloud-sdk-python-tsf-3.0.884/tencentcloud/tsf/v20180326/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   798817 2023-04-28 02:46:38.000000 tencentcloud-sdk-python-tsf-3.0.884/tencentcloud/tsf/v20180326/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 02:46:38.000000 tencentcloud-sdk-python-tsf-3.0.884/tencentcloud/tsf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-28 02:46:38.000000 tencentcloud-sdk-python-tsf-3.0.884/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:46:38.000000 tencentcloud-sdk-python-tsf-3.0.884/tencentcloud_sdk_python_tsf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 02:46:38.000000 tencentcloud-sdk-python-tsf-3.0.884/tencentcloud_sdk_python_tsf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-28 02:46:38.000000 tencentcloud-sdk-python-tsf-3.0.884/tencentcloud_sdk_python_tsf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-28 02:46:38.000000 tencentcloud-sdk-python-tsf-3.0.884/tencentcloud_sdk_python_tsf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-28 02:46:38.000000 tencentcloud-sdk-python-tsf-3.0.884/tencentcloud_sdk_python_tsf.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-28 02:46:38.000000 tencentcloud-sdk-python-tsf-3.0.884/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-28 02:46:38.000000 tencentcloud-sdk-python-tsf-3.0.884/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-28 02:46:38.000000 tencentcloud-sdk-python-tsf-3.0.884/setup.cfg
```

### Comparing `tencentcloud-sdk-python-tsf-3.0.883/README.rst` & `tencentcloud-sdk-python-tsf-3.0.884/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tsf-3.0.883/tencentcloud/tsf/v20180326/errorcodes.py` & `tencentcloud-sdk-python-tsf-3.0.884/tencentcloud/tsf/v20180326/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tsf-3.0.883/tencentcloud/tsf/v20180326/tsf_client.py` & `tencentcloud-sdk-python-tsf-3.0.884/tencentcloud/tsf/v20180326/tsf_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tsf-3.0.883/tencentcloud/tsf/v20180326/models.py` & `tencentcloud-sdk-python-tsf-3.0.884/tencentcloud/tsf/v20180326/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tsf-3.0.883/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tsf-3.0.884/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tsf-3.0.883/tencentcloud_sdk_python_tsf.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tsf-3.0.884/tencentcloud_sdk_python_tsf.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tsf
-Version: 3.0.883
+Version: 3.0.884
 Summary: Tencent Cloud Tsf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tsf-3.0.883/PKG-INFO` & `tencentcloud-sdk-python-tsf-3.0.884/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tsf
-Version: 3.0.883
+Version: 3.0.884
 Summary: Tencent Cloud Tsf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tsf-3.0.883/setup.py` & `tencentcloud-sdk-python-tsf-3.0.884/setup.py`

 * *Files identical despite different names*

