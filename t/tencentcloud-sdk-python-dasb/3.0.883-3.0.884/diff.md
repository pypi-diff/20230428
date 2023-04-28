# Comparing `tmp/tencentcloud-sdk-python-dasb-3.0.883.tar.gz` & `tmp/tencentcloud-sdk-python-dasb-3.0.884.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-dasb-3.0.883.tar", last modified: Thu Apr 27 00:27:04 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-dasb-3.0.884.tar", last modified: Fri Apr 28 02:13:48 2023, max compression
```

## Comparing `tencentcloud-sdk-python-dasb-3.0.883.tar` & `tencentcloud-sdk-python-dasb-3.0.884.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:27:04.000000 tencentcloud-sdk-python-dasb-3.0.883/
--rw-r--r--   0 root         (0) root         (0)      740 2023-04-27 00:27:04.000000 tencentcloud-sdk-python-dasb-3.0.883/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:27:04.000000 tencentcloud-sdk-python-dasb-3.0.883/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:27:04.000000 tencentcloud-sdk-python-dasb-3.0.883/tencentcloud/dasb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:27:04.000000 tencentcloud-sdk-python-dasb-3.0.883/tencentcloud/dasb/v20191018/
--rw-r--r--   0 root         (0) root         (0)     2500 2023-04-27 00:27:04.000000 tencentcloud-sdk-python-dasb-3.0.883/tencentcloud/dasb/v20191018/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 00:27:04.000000 tencentcloud-sdk-python-dasb-3.0.883/tencentcloud/dasb/v20191018/__init__.py
--rw-r--r--   0 root         (0) root         (0)   152157 2023-04-27 00:27:04.000000 tencentcloud-sdk-python-dasb-3.0.883/tencentcloud/dasb/v20191018/models.py
--rw-r--r--   0 root         (0) root         (0)    45577 2023-04-27 00:27:04.000000 tencentcloud-sdk-python-dasb-3.0.883/tencentcloud/dasb/v20191018/dasb_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 00:27:04.000000 tencentcloud-sdk-python-dasb-3.0.883/tencentcloud/dasb/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-27 00:27:04.000000 tencentcloud-sdk-python-dasb-3.0.883/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:27:04.000000 tencentcloud-sdk-python-dasb-3.0.883/tencentcloud_sdk_python_dasb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 00:27:04.000000 tencentcloud-sdk-python-dasb-3.0.883/tencentcloud_sdk_python_dasb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-04-27 00:27:04.000000 tencentcloud-sdk-python-dasb-3.0.883/tencentcloud_sdk_python_dasb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-04-27 00:27:04.000000 tencentcloud-sdk-python-dasb-3.0.883/tencentcloud_sdk_python_dasb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-27 00:27:04.000000 tencentcloud-sdk-python-dasb-3.0.883/tencentcloud_sdk_python_dasb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-04-27 00:27:04.000000 tencentcloud-sdk-python-dasb-3.0.883/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-04-27 00:27:04.000000 tencentcloud-sdk-python-dasb-3.0.883/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-27 00:27:04.000000 tencentcloud-sdk-python-dasb-3.0.883/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:13:48.000000 tencentcloud-sdk-python-dasb-3.0.884/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-04-28 02:13:48.000000 tencentcloud-sdk-python-dasb-3.0.884/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:13:48.000000 tencentcloud-sdk-python-dasb-3.0.884/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:13:48.000000 tencentcloud-sdk-python-dasb-3.0.884/tencentcloud/dasb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:13:48.000000 tencentcloud-sdk-python-dasb-3.0.884/tencentcloud/dasb/v20191018/
+-rw-r--r--   0 root         (0) root         (0)     2500 2023-04-28 02:13:48.000000 tencentcloud-sdk-python-dasb-3.0.884/tencentcloud/dasb/v20191018/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 02:13:48.000000 tencentcloud-sdk-python-dasb-3.0.884/tencentcloud/dasb/v20191018/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   157347 2023-04-28 02:13:48.000000 tencentcloud-sdk-python-dasb-3.0.884/tencentcloud/dasb/v20191018/models.py
+-rw-r--r--   0 root         (0) root         (0)    45577 2023-04-28 02:13:48.000000 tencentcloud-sdk-python-dasb-3.0.884/tencentcloud/dasb/v20191018/dasb_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 02:13:48.000000 tencentcloud-sdk-python-dasb-3.0.884/tencentcloud/dasb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-28 02:13:48.000000 tencentcloud-sdk-python-dasb-3.0.884/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:13:48.000000 tencentcloud-sdk-python-dasb-3.0.884/tencentcloud_sdk_python_dasb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 02:13:48.000000 tencentcloud-sdk-python-dasb-3.0.884/tencentcloud_sdk_python_dasb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-04-28 02:13:48.000000 tencentcloud-sdk-python-dasb-3.0.884/tencentcloud_sdk_python_dasb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-04-28 02:13:48.000000 tencentcloud-sdk-python-dasb-3.0.884/tencentcloud_sdk_python_dasb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-28 02:13:48.000000 tencentcloud-sdk-python-dasb-3.0.884/tencentcloud_sdk_python_dasb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-04-28 02:13:48.000000 tencentcloud-sdk-python-dasb-3.0.884/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-04-28 02:13:48.000000 tencentcloud-sdk-python-dasb-3.0.884/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-28 02:13:48.000000 tencentcloud-sdk-python-dasb-3.0.884/setup.cfg
```

### Comparing `tencentcloud-sdk-python-dasb-3.0.883/README.rst` & `tencentcloud-sdk-python-dasb-3.0.884/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dasb-3.0.883/tencentcloud/dasb/v20191018/errorcodes.py` & `tencentcloud-sdk-python-dasb-3.0.884/tencentcloud/dasb/v20191018/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dasb-3.0.883/tencentcloud/dasb/v20191018/models.py` & `tencentcloud-sdk-python-dasb-3.0.884/tencentcloud/dasb/v20191018/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -544,26 +544,81 @@
         :type Cmd: str
         :param Time: 命令输入的时间
         :type Time: str
         :param TimeOffset: 命令执行时间相对于所属会话开始时间的偏移量，单位ms
         :type TimeOffset: int
         :param Action: 命令执行情况，1--允许，2--拒绝，3--确认
         :type Action: int
+        :param Sid: 会话id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Sid: str
+        :param UserName: 用户名
+注意：此字段可能返回 null，表示取不到有效值。
+        :type UserName: str
+        :param Account: 设备account
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Account: str
+        :param InstanceId: 设备ip
+注意：此字段可能返回 null，表示取不到有效值。
+        :type InstanceId: str
+        :param FromIp: source ip
+注意：此字段可能返回 null，表示取不到有效值。
+        :type FromIp: str
+        :param SessTime: 该命令所属会话的会话开始时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SessTime: str
+        :param ConfirmTime: 复核时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ConfirmTime: str
+        :param UserDepartmentId: 用户部门id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type UserDepartmentId: str
+        :param UserDepartmentName: 用户部门name
+注意：此字段可能返回 null，表示取不到有效值。
+        :type UserDepartmentName: str
+        :param DeviceDepartmentId: 设备部门id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DeviceDepartmentId: str
+        :param DeviceDepartmentName: 设备部门name
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DeviceDepartmentName: str
         """
         self.Cmd = None
         self.Time = None
         self.TimeOffset = None
         self.Action = None
+        self.Sid = None
+        self.UserName = None
+        self.Account = None
+        self.InstanceId = None
+        self.FromIp = None
+        self.SessTime = None
+        self.ConfirmTime = None
+        self.UserDepartmentId = None
+        self.UserDepartmentName = None
+        self.DeviceDepartmentId = None
+        self.DeviceDepartmentName = None
 
 
     def _deserialize(self, params):
         self.Cmd = params.get("Cmd")
         self.Time = params.get("Time")
         self.TimeOffset = params.get("TimeOffset")
         self.Action = params.get("Action")
+        self.Sid = params.get("Sid")
+        self.UserName = params.get("UserName")
+        self.Account = params.get("Account")
+        self.InstanceId = params.get("InstanceId")
+        self.FromIp = params.get("FromIp")
+        self.SessTime = params.get("SessTime")
+        self.ConfirmTime = params.get("ConfirmTime")
+        self.UserDepartmentId = params.get("UserDepartmentId")
+        self.UserDepartmentName = params.get("UserDepartmentName")
+        self.DeviceDepartmentId = params.get("DeviceDepartmentId")
+        self.DeviceDepartmentName = params.get("DeviceDepartmentName")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -760,22 +815,28 @@
 
     def __init__(self):
         r"""
         :param Name: 模板名，最大长度32字符，不能包含空白字符
         :type Name: str
         :param CmdList: 命令列表，\n分隔，最大长度32768字节
         :type CmdList: str
+        :param Encoding: 标识cmdlist字段前端是否为base64加密传值.
+0:表示非base64加密
+1:表示是base64加密
+        :type Encoding: int
         """
         self.Name = None
         self.CmdList = None
+        self.Encoding = None
 
 
     def _deserialize(self, params):
         self.Name = params.get("Name")
         self.CmdList = params.get("CmdList")
+        self.Encoding = params.get("Encoding")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -3582,31 +3643,36 @@
 
     def __init__(self):
         r"""
         :param Sid: 会话Id
         :type Sid: str
         :param Cmd: 命令，可模糊搜索
         :type Cmd: str
+        :param Encoding: Cmd字段是前端传值是否进行base64.
+0:否，1：是
+        :type Encoding: int
         :param Offset: 偏移量
         :type Offset: int
         :param Limit: 每页容量，默认20，最大200
         :type Limit: int
         :param AuditAction: 根据拦截状态进行过滤
         :type AuditAction: list of int non-negative
         """
         self.Sid = None
         self.Cmd = None
+        self.Encoding = None
         self.Offset = None
         self.Limit = None
         self.AuditAction = None
 
 
     def _deserialize(self, params):
         self.Sid = params.get("Sid")
         self.Cmd = params.get("Cmd")
+        self.Encoding = params.get("Encoding")
         self.Offset = params.get("Offset")
         self.Limit = params.get("Limit")
         self.AuditAction = params.get("AuditAction")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
@@ -3666,14 +3732,17 @@
         :type DeviceName: str
         :param PublicIp: 资产的公网IP
         :type PublicIp: str
         :param PrivateIp: 资产的内网IP
         :type PrivateIp: str
         :param Cmd: 执行的命令
         :type Cmd: str
+        :param Encoding: Cmd字段是前端传值是否进行base64.
+0:否，1：是
+        :type Encoding: int
         :param AuditAction: 根据拦截状态进行过滤：1 - 已执行，2 - 被阻断
         :type AuditAction: list of int non-negative
         :param Limit: 每页容量，默认20，最大200
         :type Limit: int
         :param Offset: 分页偏移位置，默认值为0
         :type Offset: int
         """
@@ -3682,14 +3751,15 @@
         self.UserName = None
         self.RealName = None
         self.InstanceId = None
         self.DeviceName = None
         self.PublicIp = None
         self.PrivateIp = None
         self.Cmd = None
+        self.Encoding = None
         self.AuditAction = None
         self.Limit = None
         self.Offset = None
 
 
     def _deserialize(self, params):
         self.StartTime = params.get("StartTime")
@@ -3697,14 +3767,15 @@
         self.UserName = params.get("UserName")
         self.RealName = params.get("RealName")
         self.InstanceId = params.get("InstanceId")
         self.DeviceName = params.get("DeviceName")
         self.PublicIp = params.get("PublicIp")
         self.PrivateIp = params.get("PrivateIp")
         self.Cmd = params.get("Cmd")
+        self.Encoding = params.get("Encoding")
         self.AuditAction = params.get("AuditAction")
         self.Limit = params.get("Limit")
         self.Offset = params.get("Offset")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
@@ -3768,40 +3839,80 @@
         :type Cmd: str
         :param Action: 命令执行情况，1--允许，2--拒绝
         :type Action: int
         :param Sid: 命令所属的会话ID
         :type Sid: str
         :param TimeOffset: 命令执行时间相对于所属会话开始时间的偏移量，单位ms
         :type TimeOffset: int
+        :param Account: 账号
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Account: str
+        :param FromIp: source ip
+注意：此字段可能返回 null，表示取不到有效值。
+        :type FromIp: str
+        :param SessTime: 该命令所属会话的会话开始时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SessTime: str
+        :param ConfirmTime: 复核时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ConfirmTime: str
+        :param UserDepartmentId: 部门id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type UserDepartmentId: str
+        :param UserDepartmentName: 用户部门名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type UserDepartmentName: str
+        :param DeviceDepartmentId: 设备部门id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DeviceDepartmentId: str
+        :param DeviceDepartmentName: 设备部门名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DeviceDepartmentName: str
         """
         self.Time = None
         self.UserName = None
         self.RealName = None
         self.InstanceId = None
         self.DeviceName = None
         self.PublicIp = None
         self.PrivateIp = None
         self.Cmd = None
         self.Action = None
         self.Sid = None
         self.TimeOffset = None
+        self.Account = None
+        self.FromIp = None
+        self.SessTime = None
+        self.ConfirmTime = None
+        self.UserDepartmentId = None
+        self.UserDepartmentName = None
+        self.DeviceDepartmentId = None
+        self.DeviceDepartmentName = None
 
 
     def _deserialize(self, params):
         self.Time = params.get("Time")
         self.UserName = params.get("UserName")
         self.RealName = params.get("RealName")
         self.InstanceId = params.get("InstanceId")
         self.DeviceName = params.get("DeviceName")
         self.PublicIp = params.get("PublicIp")
         self.PrivateIp = params.get("PrivateIp")
         self.Cmd = params.get("Cmd")
         self.Action = params.get("Action")
         self.Sid = params.get("Sid")
         self.TimeOffset = params.get("TimeOffset")
+        self.Account = params.get("Account")
+        self.FromIp = params.get("FromIp")
+        self.SessTime = params.get("SessTime")
+        self.ConfirmTime = params.get("ConfirmTime")
+        self.UserDepartmentId = params.get("UserDepartmentId")
+        self.UserDepartmentName = params.get("UserDepartmentName")
+        self.DeviceDepartmentId = params.get("DeviceDepartmentId")
+        self.DeviceDepartmentName = params.get("DeviceDepartmentName")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -4147,29 +4258,34 @@
         :type Cmd: str
         :param StartTime: 开始时间，不得早于当前时间的180天前
         :type StartTime: str
         :param Offset: 分页偏移位置，默认值为0
         :type Offset: int
         :param Limit: 默认值为20，最大200
         :type Limit: int
+        :param Encoding: Cmd字段前端是否做base64加密
+0：否，1：是
+        :type Encoding: int
         :param EndTime: 结束时间
         :type EndTime: str
         """
         self.Cmd = None
         self.StartTime = None
         self.Offset = None
         self.Limit = None
+        self.Encoding = None
         self.EndTime = None
 
 
     def _deserialize(self, params):
         self.Cmd = params.get("Cmd")
         self.StartTime = params.get("StartTime")
         self.Offset = params.get("Offset")
         self.Limit = params.get("Limit")
+        self.Encoding = params.get("Encoding")
         self.EndTime = params.get("EndTime")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-dasb-3.0.883/tencentcloud/dasb/v20191018/dasb_client.py` & `tencentcloud-sdk-python-dasb-3.0.884/tencentcloud/dasb/v20191018/dasb_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dasb-3.0.883/tencentcloud/__init__.py` & `tencentcloud-sdk-python-dasb-3.0.884/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-dasb-3.0.883/tencentcloud_sdk_python_dasb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-dasb-3.0.884/tencentcloud_sdk_python_dasb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dasb
-Version: 3.0.883
+Version: 3.0.884
 Summary: Tencent Cloud Dasb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dasb-3.0.883/PKG-INFO` & `tencentcloud-sdk-python-dasb-3.0.884/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dasb
-Version: 3.0.883
+Version: 3.0.884
 Summary: Tencent Cloud Dasb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dasb-3.0.883/setup.py` & `tencentcloud-sdk-python-dasb-3.0.884/setup.py`

 * *Files identical despite different names*

