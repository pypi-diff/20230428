# Comparing `tmp/tencentcloud-sdk-python-wedata-3.0.883.tar.gz` & `tmp/tencentcloud-sdk-python-wedata-3.0.884.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-wedata-3.0.883.tar", last modified: Thu Apr 27 01:03:48 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-wedata-3.0.884.tar", last modified: Fri Apr 28 02:47:56 2023, max compression
```

## Comparing `tencentcloud-sdk-python-wedata-3.0.883.tar` & `tencentcloud-sdk-python-wedata-3.0.884.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 01:03:48.000000 tencentcloud-sdk-python-wedata-3.0.883/
--rw-r--r--   0 root         (0) root         (0)      746 2023-04-27 01:03:48.000000 tencentcloud-sdk-python-wedata-3.0.883/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 01:03:48.000000 tencentcloud-sdk-python-wedata-3.0.883/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 01:03:48.000000 tencentcloud-sdk-python-wedata-3.0.883/tencentcloud/wedata/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 01:03:48.000000 tencentcloud-sdk-python-wedata-3.0.883/tencentcloud/wedata/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 01:03:48.000000 tencentcloud-sdk-python-wedata-3.0.883/tencentcloud/wedata/v20210820/
--rw-r--r--   0 root         (0) root         (0)     3323 2023-04-27 01:03:48.000000 tencentcloud-sdk-python-wedata-3.0.883/tencentcloud/wedata/v20210820/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 01:03:48.000000 tencentcloud-sdk-python-wedata-3.0.883/tencentcloud/wedata/v20210820/__init__.py
--rw-r--r--   0 root         (0) root         (0)   183418 2023-04-27 01:03:48.000000 tencentcloud-sdk-python-wedata-3.0.883/tencentcloud/wedata/v20210820/wedata_client.py
--rw-r--r--   0 root         (0) root         (0)   689715 2023-04-27 01:03:48.000000 tencentcloud-sdk-python-wedata-3.0.883/tencentcloud/wedata/v20210820/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-27 01:03:48.000000 tencentcloud-sdk-python-wedata-3.0.883/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 01:03:48.000000 tencentcloud-sdk-python-wedata-3.0.883/tencentcloud_sdk_python_wedata.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 01:03:48.000000 tencentcloud-sdk-python-wedata-3.0.883/tencentcloud_sdk_python_wedata.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      475 2023-04-27 01:03:48.000000 tencentcloud-sdk-python-wedata-3.0.883/tencentcloud_sdk_python_wedata.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-04-27 01:03:48.000000 tencentcloud-sdk-python-wedata-3.0.883/tencentcloud_sdk_python_wedata.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-27 01:03:48.000000 tencentcloud-sdk-python-wedata-3.0.883/tencentcloud_sdk_python_wedata.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-04-27 01:03:48.000000 tencentcloud-sdk-python-wedata-3.0.883/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1012 2023-04-27 01:03:48.000000 tencentcloud-sdk-python-wedata-3.0.883/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-27 01:03:48.000000 tencentcloud-sdk-python-wedata-3.0.883/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:47:56.000000 tencentcloud-sdk-python-wedata-3.0.884/
+-rw-r--r--   0 root         (0) root         (0)      746 2023-04-28 02:47:56.000000 tencentcloud-sdk-python-wedata-3.0.884/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:47:56.000000 tencentcloud-sdk-python-wedata-3.0.884/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:47:56.000000 tencentcloud-sdk-python-wedata-3.0.884/tencentcloud/wedata/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 02:47:56.000000 tencentcloud-sdk-python-wedata-3.0.884/tencentcloud/wedata/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:47:56.000000 tencentcloud-sdk-python-wedata-3.0.884/tencentcloud/wedata/v20210820/
+-rw-r--r--   0 root         (0) root         (0)     3323 2023-04-28 02:47:56.000000 tencentcloud-sdk-python-wedata-3.0.884/tencentcloud/wedata/v20210820/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 02:47:56.000000 tencentcloud-sdk-python-wedata-3.0.884/tencentcloud/wedata/v20210820/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   184325 2023-04-28 02:47:56.000000 tencentcloud-sdk-python-wedata-3.0.884/tencentcloud/wedata/v20210820/wedata_client.py
+-rw-r--r--   0 root         (0) root         (0)   696535 2023-04-28 02:47:56.000000 tencentcloud-sdk-python-wedata-3.0.884/tencentcloud/wedata/v20210820/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-28 02:47:56.000000 tencentcloud-sdk-python-wedata-3.0.884/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:47:56.000000 tencentcloud-sdk-python-wedata-3.0.884/tencentcloud_sdk_python_wedata.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 02:47:56.000000 tencentcloud-sdk-python-wedata-3.0.884/tencentcloud_sdk_python_wedata.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      475 2023-04-28 02:47:56.000000 tencentcloud-sdk-python-wedata-3.0.884/tencentcloud_sdk_python_wedata.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-04-28 02:47:56.000000 tencentcloud-sdk-python-wedata-3.0.884/tencentcloud_sdk_python_wedata.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-28 02:47:56.000000 tencentcloud-sdk-python-wedata-3.0.884/tencentcloud_sdk_python_wedata.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-04-28 02:47:56.000000 tencentcloud-sdk-python-wedata-3.0.884/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-04-28 02:47:56.000000 tencentcloud-sdk-python-wedata-3.0.884/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-28 02:47:56.000000 tencentcloud-sdk-python-wedata-3.0.884/setup.cfg
```

### Comparing `tencentcloud-sdk-python-wedata-3.0.883/README.rst` & `tencentcloud-sdk-python-wedata-3.0.884/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-wedata-3.0.883/tencentcloud/wedata/v20210820/errorcodes.py` & `tencentcloud-sdk-python-wedata-3.0.884/tencentcloud/wedata/v20210820/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-wedata-3.0.883/tencentcloud/wedata/v20210820/wedata_client.py` & `tencentcloud-sdk-python-wedata-3.0.884/tencentcloud/wedata/v20210820/wedata_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -2201,14 +2201,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DescribeOperateTasks(self, request):
+        """任务运维列表组合条件查询
+
+        :param request: Request instance for DescribeOperateTasks.
+        :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeOperateTasksRequest`
+        :rtype: :class:`tencentcloud.wedata.v20210820.models.DescribeOperateTasksResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeOperateTasks", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeOperateTasksResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DescribeOrganizationalFunctions(self, request):
         """查询全量函数
 
         :param request: Request instance for DescribeOrganizationalFunctions.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeOrganizationalFunctionsRequest`
         :rtype: :class:`tencentcloud.wedata.v20210820.models.DescribeOrganizationalFunctionsResponse`
```

### Comparing `tencentcloud-sdk-python-wedata-3.0.883/tencentcloud/wedata/v20210820/models.py` & `tencentcloud-sdk-python-wedata-3.0.884/tencentcloud/wedata/v20210820/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,30 +135,35 @@
         :type TriggerType: int
         :param EstimatedTime: 预计的超时时间，分钟级别
 注意：此字段可能返回 null，表示取不到有效值。
         :type EstimatedTime: int
         :param Operator: 实时任务告警需要的参数
 注意：此字段可能返回 null，表示取不到有效值。
         :type Operator: int
+        :param AlarmIndicatorUnit: 告警指标阈值单位：ms(毫秒)、s(秒)、min(分钟)
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AlarmIndicatorUnit: str
         """
         self.Id = None
         self.AlarmIndicator = None
         self.AlarmIndicatorDesc = None
         self.TriggerType = None
         self.EstimatedTime = None
         self.Operator = None
+        self.AlarmIndicatorUnit = None
 
 
     def _deserialize(self, params):
         self.Id = params.get("Id")
         self.AlarmIndicator = params.get("AlarmIndicator")
         self.AlarmIndicatorDesc = params.get("AlarmIndicatorDesc")
         self.TriggerType = params.get("TriggerType")
         self.EstimatedTime = params.get("EstimatedTime")
         self.Operator = params.get("Operator")
+        self.AlarmIndicatorUnit = params.get("AlarmIndicatorUnit")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -3499,14 +3504,17 @@
         :type CreateTime: int
         :param ParamsString: Params json字符串
 注意：此字段可能返回 null，表示取不到有效值。
         :type ParamsString: str
         :param BizParamsString: BizParams json字符串
 注意：此字段可能返回 null，表示取不到有效值。
         :type BizParamsString: str
+        :param ModifiedTime: 修改时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ModifiedTime: int
         """
         self.DatabaseName = None
         self.Description = None
         self.ID = None
         self.Instance = None
         self.Name = None
         self.Region = None
@@ -3529,14 +3537,15 @@
         self.Edit = None
         self.Author = None
         self.Deliver = None
         self.DataSourceStatus = None
         self.CreateTime = None
         self.ParamsString = None
         self.BizParamsString = None
+        self.ModifiedTime = None
 
 
     def _deserialize(self, params):
         self.DatabaseName = params.get("DatabaseName")
         self.Description = params.get("Description")
         self.ID = params.get("ID")
         self.Instance = params.get("Instance")
@@ -3561,14 +3570,15 @@
         self.Edit = params.get("Edit")
         self.Author = params.get("Author")
         self.Deliver = params.get("Deliver")
         self.DataSourceStatus = params.get("DataSourceStatus")
         self.CreateTime = params.get("CreateTime")
         self.ParamsString = params.get("ParamsString")
         self.BizParamsString = params.get("BizParamsString")
+        self.ModifiedTime = params.get("ModifiedTime")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -5098,21 +5108,30 @@
 class DescribeDatabaseInfoListRequest(AbstractModel):
     """DescribeDatabaseInfoList请求参数结构体
 
     """
 
     def __init__(self):
         r"""
+        :param Filters: 过滤参数
+        :type Filters: list of Filter
         :param ConnectionType: 如果是hive这里写rpc，如果是其他类型不传
         :type ConnectionType: str
         """
+        self.Filters = None
         self.ConnectionType = None
 
 
     def _deserialize(self, params):
+        if params.get("Filters") is not None:
+            self.Filters = []
+            for item in params.get("Filters"):
+                obj = Filter()
+                obj._deserialize(item)
+                self.Filters.append(obj)
         self.ConnectionType = params.get("ConnectionType")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -7141,14 +7160,117 @@
 
     def _deserialize(self, params):
         self.Token = params.get("Token")
         self.Data = params.get("Data")
         self.RequestId = params.get("RequestId")
 
 
+class DescribeOperateTasksRequest(AbstractModel):
+    """DescribeOperateTasks请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ProjectId: 项目id
+        :type ProjectId: str
+        :param FolderIdList: 文件夹id，多个文件夹以逗号分隔
+        :type FolderIdList: str
+        :param WorkFlowIdList: 工作流id，多个工作流id之间以英文字符逗号分隔
+        :type WorkFlowIdList: str
+        :param WorkFlowNameList: 工作流名称，多个工作流名称之间以英文字符逗号分隔
+        :type WorkFlowNameList: str
+        :param TaskNameList: 任务名称，多个任务名称之间以英文字符逗号分隔
+        :type TaskNameList: str
+        :param TaskIdList: 任务id，多个任务id之间以英文字符逗号分隔
+        :type TaskIdList: str
+        :param PageNumber: 页号
+        :type PageNumber: str
+        :param PageSize: 分页大小
+        :type PageSize: str
+        :param SortItem: 排序字段，支持字段为FirstSubmitTime和FirstRunTime，标识最近提交和首次执行事件
+        :type SortItem: str
+        :param SortType: 排序类型。两种取值 DESC、ASC
+        :type SortType: str
+        :param InChargeList: 责任人，多个责任人之间以英文字符逗号分隔
+        :type InChargeList: str
+        :param TaskTypeIdList: 任务类型Id字符串，多个任务类型id之间以英文字符逗号分隔
+        :type TaskTypeIdList: str
+        :param StatusList: 任务状态字符串，多个任务状态之间以英文字符逗号分隔
+        :type StatusList: str
+        :param TaskCycleUnitList: 任务周期类型字符串，多个任务周期之间以英文字符逗号分隔
+        :type TaskCycleUnitList: str
+        :param ProductNameList: 任务所属产品类型
+        :type ProductNameList: str
+        """
+        self.ProjectId = None
+        self.FolderIdList = None
+        self.WorkFlowIdList = None
+        self.WorkFlowNameList = None
+        self.TaskNameList = None
+        self.TaskIdList = None
+        self.PageNumber = None
+        self.PageSize = None
+        self.SortItem = None
+        self.SortType = None
+        self.InChargeList = None
+        self.TaskTypeIdList = None
+        self.StatusList = None
+        self.TaskCycleUnitList = None
+        self.ProductNameList = None
+
+
+    def _deserialize(self, params):
+        self.ProjectId = params.get("ProjectId")
+        self.FolderIdList = params.get("FolderIdList")
+        self.WorkFlowIdList = params.get("WorkFlowIdList")
+        self.WorkFlowNameList = params.get("WorkFlowNameList")
+        self.TaskNameList = params.get("TaskNameList")
+        self.TaskIdList = params.get("TaskIdList")
+        self.PageNumber = params.get("PageNumber")
+        self.PageSize = params.get("PageSize")
+        self.SortItem = params.get("SortItem")
+        self.SortType = params.get("SortType")
+        self.InChargeList = params.get("InChargeList")
+        self.TaskTypeIdList = params.get("TaskTypeIdList")
+        self.StatusList = params.get("StatusList")
+        self.TaskCycleUnitList = params.get("TaskCycleUnitList")
+        self.ProductNameList = params.get("ProductNameList")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeOperateTasksResponse(AbstractModel):
+    """DescribeOperateTasks返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Data: 任务列表信息
+        :type Data: :class:`tencentcloud.wedata.v20210820.models.TaskInfoPage`
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Data = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("Data") is not None:
+            self.Data = TaskInfoPage()
+            self.Data._deserialize(params.get("Data"))
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeOrganizationalFunctionsRequest(AbstractModel):
     """DescribeOrganizationalFunctions请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -7517,26 +7639,34 @@
 class DescribeRealTimeTaskMetricOverviewRequest(AbstractModel):
     """DescribeRealTimeTaskMetricOverview请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param TaskId: 无
+        :param TaskId: 要查看的实时任务的任务Id
         :type TaskId: str
         :param ProjectId: 无
         :type ProjectId: str
+        :param StartTime: 开始时间
+        :type StartTime: int
+        :param EndTime: 结束时间
+        :type EndTime: int
         """
         self.TaskId = None
         self.ProjectId = None
+        self.StartTime = None
+        self.EndTime = None
 
 
     def _deserialize(self, params):
         self.TaskId = params.get("TaskId")
         self.ProjectId = params.get("ProjectId")
+        self.StartTime = params.get("StartTime")
+        self.EndTime = params.get("EndTime")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -11296,14 +11426,16 @@
         :type AddDataFiles: int
         :param AddEqualityDeletes: 增加的Equality delete数量阈值, 超过值将触发小文件合并
         :type AddEqualityDeletes: int
         :param AddPositionDeletes: 增加的Position delete数量阈值, 超过值将触发小文件合并
         :type AddPositionDeletes: int
         :param AddDeleteFiles: 增加的delete file数量阈值
         :type AddDeleteFiles: int
+        :param TargetDatasourceId: 下游节点数据源ID
+        :type TargetDatasourceId: str
         """
         self.ProjectId = None
         self.SinkDatabase = None
         self.Id = None
         self.MsType = None
         self.DatasourceId = None
         self.SourceDatabase = None
@@ -11317,14 +11449,15 @@
         self.TableVersion = None
         self.UpsertFlag = None
         self.TableComment = None
         self.AddDataFiles = None
         self.AddEqualityDeletes = None
         self.AddPositionDeletes = None
         self.AddDeleteFiles = None
+        self.TargetDatasourceId = None
 
 
     def _deserialize(self, params):
         self.ProjectId = params.get("ProjectId")
         self.SinkDatabase = params.get("SinkDatabase")
         self.Id = params.get("Id")
         self.MsType = params.get("MsType")
@@ -11355,14 +11488,15 @@
         self.TableVersion = params.get("TableVersion")
         self.UpsertFlag = params.get("UpsertFlag")
         self.TableComment = params.get("TableComment")
         self.AddDataFiles = params.get("AddDataFiles")
         self.AddEqualityDeletes = params.get("AddEqualityDeletes")
         self.AddPositionDeletes = params.get("AddPositionDeletes")
         self.AddDeleteFiles = params.get("AddDeleteFiles")
+        self.TargetDatasourceId = params.get("TargetDatasourceId")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -19362,14 +19496,55 @@
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
+
+
+class TaskInfoPage(AbstractModel):
+    """任务分页查询
+
+    """
+
+    def __init__(self):
+        r"""
+        :param PageNumber: 页号
+        :type PageNumber: int
+        :param PageSize: 页大小
+        :type PageSize: int
+        :param Items: 工作流列表信息
+        :type Items: list of TaskCanvasInfo
+        :param TotalPage: 总页数
+        :type TotalPage: int
+        """
+        self.PageNumber = None
+        self.PageSize = None
+        self.Items = None
+        self.TotalPage = None
+
+
+    def _deserialize(self, params):
+        self.PageNumber = params.get("PageNumber")
+        self.PageSize = params.get("PageSize")
+        if params.get("Items") is not None:
+            self.Items = []
+            for item in params.get("Items"):
+                obj = TaskCanvasInfo()
+                obj._deserialize(item)
+                self.Items.append(obj)
+        self.TotalPage = params.get("TotalPage")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
 
 
 class TaskInnerInfo(AbstractModel):
     """任务属性
 
     """
```

### Comparing `tencentcloud-sdk-python-wedata-3.0.883/tencentcloud/__init__.py` & `tencentcloud-sdk-python-wedata-3.0.884/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-wedata-3.0.883/tencentcloud_sdk_python_wedata.egg-info/PKG-INFO` & `tencentcloud-sdk-python-wedata-3.0.884/tencentcloud_sdk_python_wedata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-wedata
-Version: 3.0.883
+Version: 3.0.884
 Summary: Tencent Cloud Wedata SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-wedata-3.0.883/PKG-INFO` & `tencentcloud-sdk-python-wedata-3.0.884/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-wedata
-Version: 3.0.883
+Version: 3.0.884
 Summary: Tencent Cloud Wedata SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-wedata-3.0.883/setup.py` & `tencentcloud-sdk-python-wedata-3.0.884/setup.py`

 * *Files identical despite different names*

