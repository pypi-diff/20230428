# Comparing `tmp/tencentcloud-sdk-python-oceanus-3.0.883.tar.gz` & `tmp/tencentcloud-sdk-python-oceanus-3.0.884.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-oceanus-3.0.883.tar", last modified: Thu Apr 27 00:41:57 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-oceanus-3.0.884.tar", last modified: Fri Apr 28 02:35:05 2023, max compression
```

## Comparing `tencentcloud-sdk-python-oceanus-3.0.883.tar` & `tencentcloud-sdk-python-oceanus-3.0.884.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:41:57.000000 tencentcloud-sdk-python-oceanus-3.0.883/
--rw-r--r--   0 root         (0) root         (0)      749 2023-04-27 00:41:56.000000 tencentcloud-sdk-python-oceanus-3.0.883/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:41:57.000000 tencentcloud-sdk-python-oceanus-3.0.883/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-27 00:41:56.000000 tencentcloud-sdk-python-oceanus-3.0.883/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:41:57.000000 tencentcloud-sdk-python-oceanus-3.0.883/tencentcloud/oceanus/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 00:41:56.000000 tencentcloud-sdk-python-oceanus-3.0.883/tencentcloud/oceanus/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:41:57.000000 tencentcloud-sdk-python-oceanus-3.0.883/tencentcloud/oceanus/v20190422/
--rw-r--r--   0 root         (0) root         (0)     9176 2023-04-27 00:41:56.000000 tencentcloud-sdk-python-oceanus-3.0.883/tencentcloud/oceanus/v20190422/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 00:41:56.000000 tencentcloud-sdk-python-oceanus-3.0.883/tencentcloud/oceanus/v20190422/__init__.py
--rw-r--r--   0 root         (0) root         (0)   108322 2023-04-27 00:41:56.000000 tencentcloud-sdk-python-oceanus-3.0.883/tencentcloud/oceanus/v20190422/models.py
--rw-r--r--   0 root         (0) root         (0)    23497 2023-04-27 00:41:56.000000 tencentcloud-sdk-python-oceanus-3.0.883/tencentcloud/oceanus/v20190422/oceanus_client.py
--rw-r--r--   0 root         (0) root         (0)     1679 2023-04-27 00:41:57.000000 tencentcloud-sdk-python-oceanus-3.0.883/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1014 2023-04-27 00:41:56.000000 tencentcloud-sdk-python-oceanus-3.0.883/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-27 00:41:57.000000 tencentcloud-sdk-python-oceanus-3.0.883/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:41:57.000000 tencentcloud-sdk-python-oceanus-3.0.883/tencentcloud_sdk_python_oceanus.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 00:41:57.000000 tencentcloud-sdk-python-oceanus-3.0.883/tencentcloud_sdk_python_oceanus.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      485 2023-04-27 00:41:57.000000 tencentcloud-sdk-python-oceanus-3.0.883/tencentcloud_sdk_python_oceanus.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-04-27 00:41:57.000000 tencentcloud-sdk-python-oceanus-3.0.883/tencentcloud_sdk_python_oceanus.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-27 00:41:57.000000 tencentcloud-sdk-python-oceanus-3.0.883/tencentcloud_sdk_python_oceanus.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:35:05.000000 tencentcloud-sdk-python-oceanus-3.0.884/
+-rw-r--r--   0 root         (0) root         (0)      749 2023-04-28 02:35:05.000000 tencentcloud-sdk-python-oceanus-3.0.884/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:35:05.000000 tencentcloud-sdk-python-oceanus-3.0.884/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-28 02:35:05.000000 tencentcloud-sdk-python-oceanus-3.0.884/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:35:05.000000 tencentcloud-sdk-python-oceanus-3.0.884/tencentcloud/oceanus/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 02:35:05.000000 tencentcloud-sdk-python-oceanus-3.0.884/tencentcloud/oceanus/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:35:05.000000 tencentcloud-sdk-python-oceanus-3.0.884/tencentcloud/oceanus/v20190422/
+-rw-r--r--   0 root         (0) root         (0)     9176 2023-04-28 02:35:05.000000 tencentcloud-sdk-python-oceanus-3.0.884/tencentcloud/oceanus/v20190422/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 02:35:05.000000 tencentcloud-sdk-python-oceanus-3.0.884/tencentcloud/oceanus/v20190422/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   108322 2023-04-28 02:35:05.000000 tencentcloud-sdk-python-oceanus-3.0.884/tencentcloud/oceanus/v20190422/models.py
+-rw-r--r--   0 root         (0) root         (0)    23497 2023-04-28 02:35:05.000000 tencentcloud-sdk-python-oceanus-3.0.884/tencentcloud/oceanus/v20190422/oceanus_client.py
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-04-28 02:35:05.000000 tencentcloud-sdk-python-oceanus-3.0.884/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-04-28 02:35:05.000000 tencentcloud-sdk-python-oceanus-3.0.884/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-28 02:35:05.000000 tencentcloud-sdk-python-oceanus-3.0.884/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:35:05.000000 tencentcloud-sdk-python-oceanus-3.0.884/tencentcloud_sdk_python_oceanus.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 02:35:05.000000 tencentcloud-sdk-python-oceanus-3.0.884/tencentcloud_sdk_python_oceanus.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      485 2023-04-28 02:35:05.000000 tencentcloud-sdk-python-oceanus-3.0.884/tencentcloud_sdk_python_oceanus.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-04-28 02:35:05.000000 tencentcloud-sdk-python-oceanus-3.0.884/tencentcloud_sdk_python_oceanus.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-28 02:35:05.000000 tencentcloud-sdk-python-oceanus-3.0.884/tencentcloud_sdk_python_oceanus.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-oceanus-3.0.883/README.rst` & `tencentcloud-sdk-python-oceanus-3.0.884/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-oceanus-3.0.883/tencentcloud/__init__.py` & `tencentcloud-sdk-python-oceanus-3.0.884/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-oceanus-3.0.883/tencentcloud/oceanus/v20190422/errorcodes.py` & `tencentcloud-sdk-python-oceanus-3.0.884/tencentcloud/oceanus/v20190422/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-oceanus-3.0.883/tencentcloud/oceanus/v20190422/models.py` & `tencentcloud-sdk-python-oceanus-3.0.884/tencentcloud/oceanus/v20190422/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-oceanus-3.0.883/tencentcloud/oceanus/v20190422/oceanus_client.py` & `tencentcloud-sdk-python-oceanus-3.0.884/tencentcloud/oceanus/v20190422/oceanus_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-oceanus-3.0.883/PKG-INFO` & `tencentcloud-sdk-python-oceanus-3.0.884/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-oceanus
-Version: 3.0.883
+Version: 3.0.884
 Summary: Tencent Cloud Oceanus SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-oceanus-3.0.883/setup.py` & `tencentcloud-sdk-python-oceanus-3.0.884/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-oceanus-3.0.883/tencentcloud_sdk_python_oceanus.egg-info/PKG-INFO` & `tencentcloud-sdk-python-oceanus-3.0.884/tencentcloud_sdk_python_oceanus.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-oceanus
-Version: 3.0.883
+Version: 3.0.884
 Summary: Tencent Cloud Oceanus SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

