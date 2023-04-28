# Comparing `tmp/tencentcloud-sdk-python-tcaplusdb-3.0.883.tar.gz` & `tmp/tencentcloud-sdk-python-tcaplusdb-3.0.884.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tcaplusdb-3.0.883.tar", last modified: Thu Apr 27 00:52:42 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tcaplusdb-3.0.884.tar", last modified: Fri Apr 28 02:39:35 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tcaplusdb-3.0.883.tar` & `tencentcloud-sdk-python-tcaplusdb-3.0.884.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:52:42.000000 tencentcloud-sdk-python-tcaplusdb-3.0.883/
--rw-r--r--   0 root         (0) root         (0)      755 2023-04-27 00:52:42.000000 tencentcloud-sdk-python-tcaplusdb-3.0.883/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:52:42.000000 tencentcloud-sdk-python-tcaplusdb-3.0.883/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-27 00:52:42.000000 tencentcloud-sdk-python-tcaplusdb-3.0.883/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:52:42.000000 tencentcloud-sdk-python-tcaplusdb-3.0.883/tencentcloud/tcaplusdb/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 00:52:42.000000 tencentcloud-sdk-python-tcaplusdb-3.0.883/tencentcloud/tcaplusdb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:52:42.000000 tencentcloud-sdk-python-tcaplusdb-3.0.883/tencentcloud/tcaplusdb/v20190823/
--rw-r--r--   0 root         (0) root         (0)    48988 2023-04-27 00:52:42.000000 tencentcloud-sdk-python-tcaplusdb-3.0.883/tencentcloud/tcaplusdb/v20190823/tcaplusdb_client.py
--rw-r--r--   0 root         (0) root         (0)     3614 2023-04-27 00:52:42.000000 tencentcloud-sdk-python-tcaplusdb-3.0.883/tencentcloud/tcaplusdb/v20190823/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 00:52:42.000000 tencentcloud-sdk-python-tcaplusdb-3.0.883/tencentcloud/tcaplusdb/v20190823/__init__.py
--rw-r--r--   0 root         (0) root         (0)   195509 2023-04-27 00:52:42.000000 tencentcloud-sdk-python-tcaplusdb-3.0.883/tencentcloud/tcaplusdb/v20190823/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:52:42.000000 tencentcloud-sdk-python-tcaplusdb-3.0.883/tencentcloud_sdk_python_tcaplusdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 00:52:42.000000 tencentcloud-sdk-python-tcaplusdb-3.0.883/tencentcloud_sdk_python_tcaplusdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      505 2023-04-27 00:52:42.000000 tencentcloud-sdk-python-tcaplusdb-3.0.883/tencentcloud_sdk_python_tcaplusdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1689 2023-04-27 00:52:42.000000 tencentcloud-sdk-python-tcaplusdb-3.0.883/tencentcloud_sdk_python_tcaplusdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-27 00:52:42.000000 tencentcloud-sdk-python-tcaplusdb-3.0.883/tencentcloud_sdk_python_tcaplusdb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1689 2023-04-27 00:52:42.000000 tencentcloud-sdk-python-tcaplusdb-3.0.883/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1018 2023-04-27 00:52:42.000000 tencentcloud-sdk-python-tcaplusdb-3.0.883/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-27 00:52:42.000000 tencentcloud-sdk-python-tcaplusdb-3.0.883/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:39:35.000000 tencentcloud-sdk-python-tcaplusdb-3.0.884/
+-rw-r--r--   0 root         (0) root         (0)      755 2023-04-28 02:39:35.000000 tencentcloud-sdk-python-tcaplusdb-3.0.884/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:39:35.000000 tencentcloud-sdk-python-tcaplusdb-3.0.884/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-28 02:39:35.000000 tencentcloud-sdk-python-tcaplusdb-3.0.884/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:39:35.000000 tencentcloud-sdk-python-tcaplusdb-3.0.884/tencentcloud/tcaplusdb/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 02:39:35.000000 tencentcloud-sdk-python-tcaplusdb-3.0.884/tencentcloud/tcaplusdb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:39:35.000000 tencentcloud-sdk-python-tcaplusdb-3.0.884/tencentcloud/tcaplusdb/v20190823/
+-rw-r--r--   0 root         (0) root         (0)    48988 2023-04-28 02:39:35.000000 tencentcloud-sdk-python-tcaplusdb-3.0.884/tencentcloud/tcaplusdb/v20190823/tcaplusdb_client.py
+-rw-r--r--   0 root         (0) root         (0)     3614 2023-04-28 02:39:35.000000 tencentcloud-sdk-python-tcaplusdb-3.0.884/tencentcloud/tcaplusdb/v20190823/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 02:39:35.000000 tencentcloud-sdk-python-tcaplusdb-3.0.884/tencentcloud/tcaplusdb/v20190823/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   195509 2023-04-28 02:39:35.000000 tencentcloud-sdk-python-tcaplusdb-3.0.884/tencentcloud/tcaplusdb/v20190823/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:39:35.000000 tencentcloud-sdk-python-tcaplusdb-3.0.884/tencentcloud_sdk_python_tcaplusdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 02:39:35.000000 tencentcloud-sdk-python-tcaplusdb-3.0.884/tencentcloud_sdk_python_tcaplusdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      505 2023-04-28 02:39:35.000000 tencentcloud-sdk-python-tcaplusdb-3.0.884/tencentcloud_sdk_python_tcaplusdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1689 2023-04-28 02:39:35.000000 tencentcloud-sdk-python-tcaplusdb-3.0.884/tencentcloud_sdk_python_tcaplusdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-28 02:39:35.000000 tencentcloud-sdk-python-tcaplusdb-3.0.884/tencentcloud_sdk_python_tcaplusdb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1689 2023-04-28 02:39:35.000000 tencentcloud-sdk-python-tcaplusdb-3.0.884/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1018 2023-04-28 02:39:35.000000 tencentcloud-sdk-python-tcaplusdb-3.0.884/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-28 02:39:35.000000 tencentcloud-sdk-python-tcaplusdb-3.0.884/setup.cfg
```

### Comparing `tencentcloud-sdk-python-tcaplusdb-3.0.883/README.rst` & `tencentcloud-sdk-python-tcaplusdb-3.0.884/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcaplusdb-3.0.883/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tcaplusdb-3.0.884/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tcaplusdb-3.0.883/tencentcloud/tcaplusdb/v20190823/tcaplusdb_client.py` & `tencentcloud-sdk-python-tcaplusdb-3.0.884/tencentcloud/tcaplusdb/v20190823/tcaplusdb_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcaplusdb-3.0.883/tencentcloud/tcaplusdb/v20190823/errorcodes.py` & `tencentcloud-sdk-python-tcaplusdb-3.0.884/tencentcloud/tcaplusdb/v20190823/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcaplusdb-3.0.883/tencentcloud/tcaplusdb/v20190823/models.py` & `tencentcloud-sdk-python-tcaplusdb-3.0.884/tencentcloud/tcaplusdb/v20190823/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tcaplusdb-3.0.883/tencentcloud_sdk_python_tcaplusdb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tcaplusdb-3.0.884/tencentcloud_sdk_python_tcaplusdb.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tcaplusdb
-Version: 3.0.883
+Version: 3.0.884
 Summary: Tencent Cloud Tcaplusdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tcaplusdb-3.0.883/PKG-INFO` & `tencentcloud-sdk-python-tcaplusdb-3.0.884/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tcaplusdb
-Version: 3.0.883
+Version: 3.0.884
 Summary: Tencent Cloud Tcaplusdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tcaplusdb-3.0.883/setup.py` & `tencentcloud-sdk-python-tcaplusdb-3.0.884/setup.py`

 * *Files identical despite different names*

