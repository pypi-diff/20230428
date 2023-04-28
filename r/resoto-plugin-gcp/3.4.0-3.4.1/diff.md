# Comparing `tmp/resoto-plugin-gcp-3.4.0.tar.gz` & `tmp/resoto-plugin-gcp-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-gcp-3.4.0.tar", last modified: Thu Apr 27 11:24:33 2023, max compression
+gzip compressed data, was "resoto-plugin-gcp-3.4.1.tar", last modified: Fri Apr 28 15:15:58 2023, max compression
```

## Comparing `resoto-plugin-gcp-3.4.0.tar` & `resoto-plugin-gcp-3.4.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:24:33.852740 resoto-plugin-gcp-3.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-27 11:19:59.000000 resoto-plugin-gcp-3.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-27 11:24:33.852740 resoto-plugin-gcp-3.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-27 11:19:59.000000 resoto-plugin-gcp-3.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-27 11:19:59.000000 resoto-plugin-gcp-3.4.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:24:33.844740 resoto-plugin-gcp-3.4.0/resoto_plugin_gcp/
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-04-27 11:19:59.000000 resoto-plugin-gcp-3.4.0/resoto_plugin_gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    64093 2023-04-27 11:19:59.000000 resoto-plugin-gcp-3.4.0/resoto_plugin_gcp/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-27 11:19:59.000000 resoto-plugin-gcp-3.4.0/resoto_plugin_gcp/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-04-27 11:19:59.000000 resoto-plugin-gcp-3.4.0/resoto_plugin_gcp/gcp_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    29516 2023-04-27 11:19:59.000000 resoto-plugin-gcp-3.4.0/resoto_plugin_gcp/gcp_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-04-27 11:19:59.000000 resoto-plugin-gcp-3.4.0/resoto_plugin_gcp/project_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:24:33.852740 resoto-plugin-gcp-3.4.0/resoto_plugin_gcp/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 11:19:59.000000 resoto-plugin-gcp-3.4.0/resoto_plugin_gcp/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18813 2023-04-27 11:19:59.000000 resoto-plugin-gcp-3.4.0/resoto_plugin_gcp/resources/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11818 2023-04-27 11:19:59.000000 resoto-plugin-gcp-3.4.0/resoto_plugin_gcp/resources/billing.py
--rw-r--r--   0 runner    (1001) docker     (123)   278397 2023-04-27 11:19:59.000000 resoto-plugin-gcp-3.4.0/resoto_plugin_gcp/resources/compute.py
--rw-r--r--   0 runner    (1001) docker     (123)    49330 2023-04-27 11:19:59.000000 resoto-plugin-gcp-3.4.0/resoto_plugin_gcp/resources/container.py
--rw-r--r--   0 runner    (1001) docker     (123)    41166 2023-04-27 11:19:59.000000 resoto-plugin-gcp-3.4.0/resoto_plugin_gcp/resources/sqladmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     9109 2023-04-27 11:19:59.000000 resoto-plugin-gcp-3.4.0/resoto_plugin_gcp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:24:33.848739 resoto-plugin-gcp-3.4.0/resoto_plugin_gcp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-27 11:24:33.000000 resoto-plugin-gcp-3.4.0/resoto_plugin_gcp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-27 11:24:33.000000 resoto-plugin-gcp-3.4.0/resoto_plugin_gcp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 11:24:33.000000 resoto-plugin-gcp-3.4.0/resoto_plugin_gcp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-27 11:24:33.000000 resoto-plugin-gcp-3.4.0/resoto_plugin_gcp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 11:24:33.000000 resoto-plugin-gcp-3.4.0/resoto_plugin_gcp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-27 11:24:33.000000 resoto-plugin-gcp-3.4.0/resoto_plugin_gcp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-27 11:24:33.000000 resoto-plugin-gcp-3.4.0/resoto_plugin_gcp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-27 11:24:33.856740 resoto-plugin-gcp-3.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-27 11:19:59.000000 resoto-plugin-gcp-3.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 11:24:33.852740 resoto-plugin-gcp-3.4.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 11:19:59.000000 resoto-plugin-gcp-3.4.0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-04-27 11:19:59.000000 resoto-plugin-gcp-3.4.0/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    11881 2023-04-27 11:19:59.000000 resoto-plugin-gcp-3.4.0/test/random_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-04-27 11:19:59.000000 resoto-plugin-gcp-3.4.0/test/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-27 11:19:59.000000 resoto-plugin-gcp-3.4.0/test/test_billing.py
--rw-r--r--   0 runner    (1001) docker     (123)    12633 2023-04-27 11:19:59.000000 resoto-plugin-gcp-3.4.0/test/test_compute.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-27 11:19:59.000000 resoto-plugin-gcp-3.4.0/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-27 11:19:59.000000 resoto-plugin-gcp-3.4.0/test/test_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-04-27 11:19:59.000000 resoto-plugin-gcp-3.4.0/test/test_project_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-27 11:19:59.000000 resoto-plugin-gcp-3.4.0/test/test_sqladmin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:15:58.023901 resoto-plugin-gcp-3.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-28 15:12:40.000000 resoto-plugin-gcp-3.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-28 15:15:58.023901 resoto-plugin-gcp-3.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-28 15:12:40.000000 resoto-plugin-gcp-3.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-28 15:12:40.000000 resoto-plugin-gcp-3.4.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:15:58.019901 resoto-plugin-gcp-3.4.1/resoto_plugin_gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-04-28 15:12:40.000000 resoto-plugin-gcp-3.4.1/resoto_plugin_gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64109 2023-04-28 15:12:40.000000 resoto-plugin-gcp-3.4.1/resoto_plugin_gcp/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-28 15:12:40.000000 resoto-plugin-gcp-3.4.1/resoto_plugin_gcp/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-04-28 15:12:40.000000 resoto-plugin-gcp-3.4.1/resoto_plugin_gcp/gcp_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29516 2023-04-28 15:12:40.000000 resoto-plugin-gcp-3.4.1/resoto_plugin_gcp/gcp_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-04-28 15:12:40.000000 resoto-plugin-gcp-3.4.1/resoto_plugin_gcp/project_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:15:58.023901 resoto-plugin-gcp-3.4.1/resoto_plugin_gcp/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 15:12:40.000000 resoto-plugin-gcp-3.4.1/resoto_plugin_gcp/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18813 2023-04-28 15:12:40.000000 resoto-plugin-gcp-3.4.1/resoto_plugin_gcp/resources/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11818 2023-04-28 15:12:40.000000 resoto-plugin-gcp-3.4.1/resoto_plugin_gcp/resources/billing.py
+-rw-r--r--   0 runner    (1001) docker     (123)   278367 2023-04-28 15:12:40.000000 resoto-plugin-gcp-3.4.1/resoto_plugin_gcp/resources/compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49330 2023-04-28 15:12:40.000000 resoto-plugin-gcp-3.4.1/resoto_plugin_gcp/resources/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41161 2023-04-28 15:12:40.000000 resoto-plugin-gcp-3.4.1/resoto_plugin_gcp/resources/sqladmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9109 2023-04-28 15:12:40.000000 resoto-plugin-gcp-3.4.1/resoto_plugin_gcp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:15:58.019901 resoto-plugin-gcp-3.4.1/resoto_plugin_gcp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-28 15:15:58.000000 resoto-plugin-gcp-3.4.1/resoto_plugin_gcp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-28 15:15:58.000000 resoto-plugin-gcp-3.4.1/resoto_plugin_gcp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 15:15:58.000000 resoto-plugin-gcp-3.4.1/resoto_plugin_gcp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-28 15:15:58.000000 resoto-plugin-gcp-3.4.1/resoto_plugin_gcp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 15:15:58.000000 resoto-plugin-gcp-3.4.1/resoto_plugin_gcp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-28 15:15:58.000000 resoto-plugin-gcp-3.4.1/resoto_plugin_gcp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-28 15:15:58.000000 resoto-plugin-gcp-3.4.1/resoto_plugin_gcp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-28 15:15:58.023901 resoto-plugin-gcp-3.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-28 15:12:40.000000 resoto-plugin-gcp-3.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:15:58.023901 resoto-plugin-gcp-3.4.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 15:12:40.000000 resoto-plugin-gcp-3.4.1/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-04-28 15:12:40.000000 resoto-plugin-gcp-3.4.1/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11881 2023-04-28 15:12:40.000000 resoto-plugin-gcp-3.4.1/test/random_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-04-28 15:12:40.000000 resoto-plugin-gcp-3.4.1/test/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-28 15:12:40.000000 resoto-plugin-gcp-3.4.1/test/test_billing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12633 2023-04-28 15:12:40.000000 resoto-plugin-gcp-3.4.1/test/test_compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-28 15:12:40.000000 resoto-plugin-gcp-3.4.1/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-28 15:12:40.000000 resoto-plugin-gcp-3.4.1/test/test_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-04-28 15:12:40.000000 resoto-plugin-gcp-3.4.1/test/test_project_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-28 15:12:40.000000 resoto-plugin-gcp-3.4.1/test/test_sqladmin.py
```

### Comparing `resoto-plugin-gcp-3.4.0/PKG-INFO` & `resoto-plugin-gcp-3.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-gcp
-Version: 3.4.0
+Version: 3.4.1
 Summary: Resoto GCP Collector Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/gcp
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-gcp-3.4.0/resoto_plugin_gcp/__init__.py` & `resoto-plugin-gcp-3.4.1/resoto_plugin_gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.4.0/resoto_plugin_gcp/collector.py` & `resoto-plugin-gcp-3.4.1/resoto_plugin_gcp/collector.py`

 * *Files 1% similar despite different names*

```diff
@@ -830,15 +830,15 @@
     def collect_disk_types(self):
         def post_process(resource: GCPDiskType, graph: Graph):
             if resource.region(graph).name == "undefined" and resource.zone(graph).name == "undefined":
                 log.debug(f"Resource {resource.rtdname} has no region or zone" " - removing from graph")
                 graph.remove_node(resource)
                 return
 
-            log.debug((f"Looking up pricing for {resource.rtdname}" f" in {resource.location(graph).rtdname}"))
+            log.debug((f"Looking up pricing for {resource.rtdname}" f" in {resource.resource_location(graph).rtdname}"))
             resource_group_map = {
                 "local-ssd": "LocalSSD",
                 "pd-balanced": "SSD",
                 "pd-ssd": "SSD",
                 "pd-standard": "PDStandard",
             }
             resource_group = resource_group_map.get(resource.name)
@@ -1020,15 +1020,15 @@
         TODO: Implement GPU types
         """
         if resource.region(graph).name == "undefined" and resource.zone(graph).name == "undefined":
             log.debug(f"Resource {resource.rtdname} has no region or zone" " - removing from graph")
             graph.remove_node(resource)
             return
 
-        log.debug((f"Looking up pricing for {resource.rtdname}" f" in {resource.location(graph).rtdname}"))
+        log.debug(f"Looking up pricing for {resource.rtdname}" f" in {resource.resource_location(graph).rtdname}")
         skus = []
         for sku in graph.searchall(
             {
                 "kind": "gcp_service_sku",
                 "resource_family": "Compute",
                 "usage_type": "OnDemand",
             }
```

### Comparing `resoto-plugin-gcp-3.4.0/resoto_plugin_gcp/config.py` & `resoto-plugin-gcp-3.4.1/resoto_plugin_gcp/config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.4.0/resoto_plugin_gcp/gcp_client.py` & `resoto-plugin-gcp-3.4.1/resoto_plugin_gcp/gcp_client.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.4.0/resoto_plugin_gcp/gcp_resources.py` & `resoto-plugin-gcp-3.4.1/resoto_plugin_gcp/gcp_resources.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.4.0/resoto_plugin_gcp/project_collector.py` & `resoto-plugin-gcp-3.4.1/resoto_plugin_gcp/project_collector.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.4.0/resoto_plugin_gcp/resources/base.py` & `resoto-plugin-gcp-3.4.1/resoto_plugin_gcp/resources/base.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.4.0/resoto_plugin_gcp/resources/billing.py` & `resoto-plugin-gcp-3.4.1/resoto_plugin_gcp/resources/billing.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.4.0/resoto_plugin_gcp/resources/compute.py` & `resoto-plugin-gcp-3.4.1/resoto_plugin_gcp/resources/compute.py`

 * *Files 0% similar despite different names*

```diff
@@ -3001,19 +3001,19 @@
         "name": S("name"),
         "source": S("source"),
         "start_time": S("startTime"),
         "state": S("state"),
     }
     affected_circuits: Optional[List[str]] = field(default=None)
     description: Optional[str] = field(default=None)
-    end_time: Optional[datetime] = field(default=None)
+    end_time: Optional[str] = field(default=None)
     issue_type: Optional[str] = field(default=None)
     name: Optional[str] = field(default=None)
     source: Optional[str] = field(default=None)
-    start_time: Optional[datetime] = field(default=None)
+    start_time: Optional[str] = field(default=None)
     state: Optional[str] = field(default=None)
 
 
 @define(eq=False, slots=False)
 class GcpInterconnect(GcpResource):
     kind: ClassVar[str] = "gcp_interconnect"
     api_spec: ClassVar[GcpApiSpec] = GcpApiSpec(
@@ -3569,15 +3569,15 @@
 class GcpNodeGroupMaintenanceWindow:
     kind: ClassVar[str] = "gcp_node_group_maintenance_window"
     mapping: ClassVar[Dict[str, Bender]] = {
         "maintenance_duration": S("maintenanceDuration", default={}) >> Bend(GcpDuration.mapping),
         "start_time": S("startTime"),
     }
     maintenance_duration: Optional[GcpDuration] = field(default=None)
-    start_time: Optional[datetime] = field(default=None)
+    start_time: Optional[str] = field(default=None)
 
 
 @define(eq=False, slots=False)
 class GcpShareSettingsProjectConfig:
     kind: ClassVar[str] = "gcp_share_settings_project_config"
     mapping: ClassVar[Dict[str, Bender]] = {"project_id": S("projectId")}
     project_id: Optional[str] = field(default=None)
@@ -5023,37 +5023,37 @@
     mapping: ClassVar[Dict[str, Bender]] = {
         "days_in_cycle": S("daysInCycle"),
         "duration": S("duration"),
         "start_time": S("startTime"),
     }
     days_in_cycle: Optional[int] = field(default=None)
     duration: Optional[str] = field(default=None)
-    start_time: Optional[datetime] = field(default=None)
+    start_time: Optional[str] = field(default=None)
 
 
 @define(eq=False, slots=False)
 class GcpResourcePolicyHourlyCycle:
     kind: ClassVar[str] = "gcp_resource_policy_hourly_cycle"
     mapping: ClassVar[Dict[str, Bender]] = {
         "duration": S("duration"),
         "hours_in_cycle": S("hoursInCycle"),
         "start_time": S("startTime"),
     }
     duration: Optional[str] = field(default=None)
     hours_in_cycle: Optional[int] = field(default=None)
-    start_time: Optional[datetime] = field(default=None)
+    start_time: Optional[str] = field(default=None)
 
 
 @define(eq=False, slots=False)
 class GcpResourcePolicyWeeklyCycleDayOfWeek:
     kind: ClassVar[str] = "gcp_resource_policy_weekly_cycle_day_of_week"
     mapping: ClassVar[Dict[str, Bender]] = {"day": S("day"), "duration": S("duration"), "start_time": S("startTime")}
     day: Optional[str] = field(default=None)
     duration: Optional[str] = field(default=None)
-    start_time: Optional[datetime] = field(default=None)
+    start_time: Optional[str] = field(default=None)
 
 
 @define(eq=False, slots=False)
 class GcpResourcePolicyWeeklyCycle:
     kind: ClassVar[str] = "gcp_resource_policy_weekly_cycle"
     mapping: ClassVar[Dict[str, Bender]] = {
         "day_of_weeks": S("dayOfWeeks", default=[]) >> ForallBend(GcpResourcePolicyWeeklyCycleDayOfWeek.mapping)
```

### Comparing `resoto-plugin-gcp-3.4.0/resoto_plugin_gcp/resources/container.py` & `resoto-plugin-gcp-3.4.1/resoto_plugin_gcp/resources/container.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.4.0/resoto_plugin_gcp/resources/sqladmin.py` & `resoto-plugin-gcp-3.4.1/resoto_plugin_gcp/resources/sqladmin.py`

 * *Files 0% similar despite different names*

```diff
@@ -342,15 +342,15 @@
     }
     backup_retention_settings: Optional[GcpSqlBackupRetentionSettings] = field(default=None)
     binary_log_enabled: Optional[bool] = field(default=None)
     enabled: Optional[bool] = field(default=None)
     location: Optional[str] = field(default=None)
     point_in_time_recovery_enabled: Optional[bool] = field(default=None)
     replication_log_archiving_enabled: Optional[bool] = field(default=None)
-    start_time: Optional[datetime] = field(default=None)
+    start_time: Optional[str] = field(default=None)
     transaction_log_retention_days: Optional[int] = field(default=None)
 
 
 @define(eq=False, slots=False)
 class GcpSqlDatabaseFlags:
     kind: ClassVar[str] = "gcp_sql_database_flags"
     mapping: ClassVar[Dict[str, Bender]] = {"name": S("name"), "value": S("value")}
```

### Comparing `resoto-plugin-gcp-3.4.0/resoto_plugin_gcp/utils.py` & `resoto-plugin-gcp-3.4.1/resoto_plugin_gcp/utils.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.4.0/resoto_plugin_gcp.egg-info/PKG-INFO` & `resoto-plugin-gcp-3.4.1/resoto_plugin_gcp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-gcp
-Version: 3.4.0
+Version: 3.4.1
 Summary: Resoto GCP Collector Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/gcp
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-gcp-3.4.0/resoto_plugin_gcp.egg-info/SOURCES.txt` & `resoto-plugin-gcp-3.4.1/resoto_plugin_gcp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.4.0/setup.py` & `resoto-plugin-gcp-3.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def read(file_name: str) -> str:
     with open(os.path.join(os.path.dirname(__file__), file_name)) as of:
         return of.read()
 
 
 setup(
     name="resoto-plugin-gcp",
-    version="3.4.0",
+    version="3.4.1",
     description="Resoto GCP Collector Plugin",
     license="Apache 2.0",
     packages=find_packages(),
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     entry_points={"resoto.plugins": ["gcp = resoto_plugin_gcp:GCPCollectorPlugin"]},
     include_package_data=True,
```

### Comparing `resoto-plugin-gcp-3.4.0/test/conftest.py` & `resoto-plugin-gcp-3.4.1/test/conftest.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.4.0/test/random_client.py` & `resoto-plugin-gcp-3.4.1/test/random_client.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.4.0/test/test_base.py` & `resoto-plugin-gcp-3.4.1/test/test_base.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.4.0/test/test_billing.py` & `resoto-plugin-gcp-3.4.1/test/test_billing.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.4.0/test/test_compute.py` & `resoto-plugin-gcp-3.4.1/test/test_compute.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.4.0/test/test_config.py` & `resoto-plugin-gcp-3.4.1/test/test_config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.4.0/test/test_container.py` & `resoto-plugin-gcp-3.4.1/test/test_container.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.4.0/test/test_project_collector.py` & `resoto-plugin-gcp-3.4.1/test/test_project_collector.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.4.0/test/test_sqladmin.py` & `resoto-plugin-gcp-3.4.1/test/test_sqladmin.py`

 * *Files identical despite different names*

