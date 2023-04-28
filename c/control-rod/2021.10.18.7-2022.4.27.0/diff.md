# Comparing `tmp/control_rod-2021.10.18.7.tar.gz` & `tmp/control_rod-2022.4.27.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "control_rod-2021.10.18.7.tar", last modified: Mon Oct 18 21:13:26 2021, max compression
+gzip compressed data, was "control_rod-2022.4.27.0.tar", last modified: Fri Apr 28 17:27:21 2023, max compression
```

## Comparing `control_rod-2021.10.18.7.tar` & `control_rod-2022.4.27.0.tar`

### file list

```diff
@@ -1,32 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-18 21:13:26.708196 control_rod-2021.10.18.7/
--rw-r--r--   0 runner    (1001) docker     (121)      509 2021-10-18 21:13:26.708196 control_rod-2021.10.18.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       91 2021-10-18 21:13:10.000000 control_rod-2021.10.18.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-18 21:13:26.704196 control_rod-2021.10.18.7/abobjs/
--rw-r--r--   0 runner    (1001) docker     (121)     1504 2021-10-18 21:13:10.000000 control_rod-2021.10.18.7/abobjs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1470 2021-10-18 21:13:10.000000 control_rod-2021.10.18.7/abobjs/assertion.py
--rw-r--r--   0 runner    (1001) docker     (121)    24345 2021-10-18 21:13:10.000000 control_rod-2021.10.18.7/abobjs/base.py
--rw-r--r--   0 runner    (1001) docker     (121)      958 2021-10-18 21:13:10.000000 control_rod-2021.10.18.7/abobjs/continuous_monitoring_monitor_results.py
--rw-r--r--   0 runner    (1001) docker     (121)      790 2021-10-18 21:13:10.000000 control_rod-2021.10.18.7/abobjs/continuous_monitoring_monitors.py
--rw-r--r--   0 runner    (1001) docker     (121)      786 2021-10-18 21:13:10.000000 control_rod-2021.10.18.7/abobjs/continuous_monitoring_systems.py
--rw-r--r--   0 runner    (1001) docker     (121)      679 2021-10-18 21:13:10.000000 control_rod-2021.10.18.7/abobjs/control.py
--rw-r--r--   0 runner    (1001) docker     (121)     4802 2021-10-18 21:13:10.000000 control_rod-2021.10.18.7/abobjs/controlrod.py
--rw-r--r--   0 runner    (1001) docker     (121)     1460 2021-10-18 21:13:10.000000 control_rod-2021.10.18.7/abobjs/controls_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     1113 2021-10-18 21:13:10.000000 control_rod-2021.10.18.7/abobjs/effectiveness_option.py
--rw-r--r--   0 runner    (1001) docker     (121)     2758 2021-10-18 21:13:10.000000 control_rod-2021.10.18.7/abobjs/entity.py
--rw-r--r--   0 runner    (1001) docker     (121)     1503 2021-10-18 21:13:10.000000 control_rod-2021.10.18.7/abobjs/file.py
--rw-r--r--   0 runner    (1001) docker     (121)     1240 2021-10-18 21:13:10.000000 control_rod-2021.10.18.7/abobjs/process.py
--rw-r--r--   0 runner    (1001) docker     (121)     1355 2021-10-18 21:13:10.000000 control_rod-2021.10.18.7/abobjs/region.py
--rw-r--r--   0 runner    (1001) docker     (121)     1310 2021-10-18 21:13:10.000000 control_rod-2021.10.18.7/abobjs/risk.py
--rw-r--r--   0 runner    (1001) docker     (121)     1261 2021-10-18 21:13:10.000000 control_rod-2021.10.18.7/abobjs/status_option.py
--rw-r--r--   0 runner    (1001) docker     (121)     1252 2021-10-18 21:13:10.000000 control_rod-2021.10.18.7/abobjs/subprocess.py
--rw-r--r--   0 runner    (1001) docker     (121)     3141 2021-10-18 21:13:10.000000 control_rod-2021.10.18.7/abobjs/test.py
--rw-r--r--   0 runner    (1001) docker     (121)     1257 2021-10-18 21:13:10.000000 control_rod-2021.10.18.7/abobjs/test_section.py
--rw-r--r--   0 runner    (1001) docker     (121)     1308 2021-10-18 21:13:10.000000 control_rod-2021.10.18.7/abobjs/test_type.py
--rw-r--r--   0 runner    (1001) docker     (121)     1055 2021-10-18 21:13:10.000000 control_rod-2021.10.18.7/abobjs/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-18 21:13:26.708196 control_rod-2021.10.18.7/control_rod.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      509 2021-10-18 21:13:26.000000 control_rod-2021.10.18.7/control_rod.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      656 2021-10-18 21:13:26.000000 control_rod-2021.10.18.7/control_rod.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-18 21:13:26.000000 control_rod-2021.10.18.7/control_rod.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-10-18 21:13:26.000000 control_rod-2021.10.18.7/control_rod.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-10-18 21:13:10.000000 control_rod-2021.10.18.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      491 2021-10-18 21:13:26.708196 control_rod-2021.10.18.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:27:21.736346 control_rod-2022.4.27.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-28 17:27:21.736346 control_rod-2022.4.27.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:27:21.732346 control_rod-2022.4.27.0/abobjs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/abobjs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/abobjs/assertion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/abobjs/auditable_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/abobjs/auditable_entity_regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/abobjs/auditable_entity_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24740 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/abobjs/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/abobjs/buisness_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/abobjs/continuous_monitoring_monitor_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/abobjs/continuous_monitoring_monitors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/abobjs/continuous_monitoring_systems.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/abobjs/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/abobjs/controlrod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/abobjs/controls_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/abobjs/departments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/abobjs/effectiveness_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/abobjs/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/abobjs/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/abobjs/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/abobjs/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/abobjs/region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/abobjs/risk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/abobjs/status_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/abobjs/subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/abobjs/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/abobjs/test_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/abobjs/test_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/abobjs/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:27:21.736346 control_rod-2022.4.27.0/control_rod.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-28 17:27:21.000000 control_rod-2022.4.27.0/control_rod.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-04-28 17:27:21.000000 control_rod-2022.4.27.0/control_rod.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 17:27:21.000000 control_rod-2022.4.27.0/control_rod.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-28 17:27:21.000000 control_rod-2022.4.27.0/control_rod.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-28 17:27:21.740346 control_rod-2022.4.27.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:27:21.736346 control_rod-2022.4.27.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/tests/test_assertion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/tests/test_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/tests/test_controlrod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/tests/test_controlsdatum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/tests/test_effectivenessoption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/tests/test_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/tests/test_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/tests/test_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/tests/test_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/tests/test_risk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/tests/test_status_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/tests/test_subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/tests/test_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/tests/test_testsection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/tests/test_testtypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/tests/test_workspace.py
```

### Comparing `control_rod-2021.10.18.7/abobjs/__init__.py` & `control_rod-2022.4.27.0/abobjs/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,24 +16,35 @@
 from .test import AB_Test
 from .file import AB_File
 
 from .continuous_monitoring_systems import AB_Continous_Monitoring_Systems
 from .continuous_monitoring_monitors import AB_Continous_Monitoring_Monitors
 from .continuous_monitoring_monitor_results import AB_Continous_Monitoring_Monitor_Results
 
+from .auditable_entity import AB_Auditable_Entities
+from .auditable_entity_regions import AB_Auditable_Entity_Regions
+from .auditable_entity_types import AB_Auditable_Entity_Types
+
+from .buisness_units import AB_Business_Unit
+from .departments import AB_Departments
+
+from .multi import AB_Multi
+
 SUBOBJ_LK = {"region_id": {"obj": AB_Region},
              "process_id": {"obj": AB_Process},
              "subprocess_id": {"obj": AB_SubProcess},
              "risk_id": {"obj": AB_Risk},
              "control_id": {"obj": AB_Control},
              "entity_id": {"obj": AB_Entity},
              "controls_datum_ids": {"obj": AB_Controls_Data},
              "test_ids": {"obj": AB_Test},
              "file_ids": {"obj": AB_File},
              "continuous_monitoring_system_id": {"obj": AB_Continous_Monitoring_Systems},
-             "continuous_monitoring_monitor_id": {"obj": AB_Continous_Monitoring_Monitors}
+             "continuous_monitoring_monitor_id": {"obj": AB_Continous_Monitoring_Monitors},
+             "auditable_entity_id": {"obj": AB_Auditable_Entities},
+             "auditable_entity_region_id": {"obj": AB_Auditable_Entity_Regions}
             }
 
 
 from .controlrod import AB_ControlRod
 
 USER_AGENT = "control_rod/0.0.0"
```

### Comparing `control_rod-2021.10.18.7/abobjs/assertion.py` & `control_rod-2022.4.27.0/abobjs/assertion.py`

 * *Files identical despite different names*

### Comparing `control_rod-2021.10.18.7/abobjs/base.py` & `control_rod-2022.4.27.0/abobjs/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,19 @@
 import pyjq
 import xmltodict
 
 import abobjs
 
 
 class AB_Base:
+
+    '''
+    Base Object for API Calls
+    '''
+
     # People need to set these three
     _endpoint = None
     _single = None
     _name = "base"
     _file_modal = None
     _fileable_type = None
 
@@ -82,15 +87,16 @@
         ignore_read = False
         self.init_action_taken = "none"
 
         if self.kwargs.get("init_action", "read") in ("read", "readorcreate") and self.id is None:
             # I didn't get an ID
             if self.kwargs.get("uid", None) is not None or \
                     self.kwargs.get("search_name", None) is not None or \
-                    self.kwargs.get("search_complex", None) is not None:
+                    self.kwargs.get("search_complex", None) is not None or \
+                    self.kwargs.get("multi", False) is True:
 
                 # I searched for and found (or not) a result
                 try:
                     self.id = self.search()
                 except Exception as error_in_search:
                     self.logger.debug(error_in_search)
                     raise error_in_search
@@ -238,14 +244,20 @@
                             break
 
                 if all_passed is True:
                     self.logger.debug("Found object via complex match {}".format(self.kwargs["search_complex"]))
                     found_item = potential
                     break
 
+            elif self.kwargs.get("multi", False) is True:
+                # This is a multi request, we're going to use the results from kwargs["all_data"] So we just want
+                # to leave as soon as possible.
+                found_item = potential
+                break
+
             else:
                 # Continue to the Next Item to search for it.
                 pass
 
         found_id = None
 
         if found_item is None:
```

### Comparing `control_rod-2021.10.18.7/abobjs/continuous_monitoring_monitor_results.py` & `control_rod-2022.4.27.0/abobjs/continuous_monitoring_monitor_results.py`

 * *Files identical despite different names*

### Comparing `control_rod-2021.10.18.7/abobjs/continuous_monitoring_monitors.py` & `control_rod-2022.4.27.0/abobjs/continuous_monitoring_monitors.py`

 * *Files identical despite different names*

### Comparing `control_rod-2021.10.18.7/abobjs/continuous_monitoring_systems.py` & `control_rod-2022.4.27.0/abobjs/continuous_monitoring_systems.py`

 * *Files identical despite different names*

### Comparing `control_rod-2021.10.18.7/abobjs/control.py` & `control_rod-2022.4.27.0/abobjs/control.py`

 * *Files identical despite different names*

### Comparing `control_rod-2021.10.18.7/abobjs/controlrod.py` & `control_rod-2022.4.27.0/abobjs/controlrod.py`

 * *Files identical despite different names*

### Comparing `control_rod-2021.10.18.7/abobjs/controls_data.py` & `control_rod-2022.4.27.0/abobjs/controls_data.py`

 * *Files identical despite different names*

### Comparing `control_rod-2021.10.18.7/abobjs/effectiveness_option.py` & `control_rod-2022.4.27.0/abobjs/effectiveness_option.py`

 * *Files identical despite different names*

### Comparing `control_rod-2021.10.18.7/abobjs/entity.py` & `control_rod-2022.4.27.0/abobjs/entity.py`

 * *Files identical despite different names*

### Comparing `control_rod-2021.10.18.7/abobjs/file.py` & `control_rod-2022.4.27.0/abobjs/file.py`

 * *Files identical despite different names*

### Comparing `control_rod-2021.10.18.7/abobjs/process.py` & `control_rod-2022.4.27.0/abobjs/process.py`

 * *Files identical despite different names*

### Comparing `control_rod-2021.10.18.7/abobjs/region.py` & `control_rod-2022.4.27.0/abobjs/region.py`

 * *Files identical despite different names*

### Comparing `control_rod-2021.10.18.7/abobjs/risk.py` & `control_rod-2022.4.27.0/abobjs/risk.py`

 * *Files identical despite different names*

### Comparing `control_rod-2021.10.18.7/abobjs/status_option.py` & `control_rod-2022.4.27.0/abobjs/status_option.py`

 * *Files identical despite different names*

### Comparing `control_rod-2021.10.18.7/abobjs/subprocess.py` & `control_rod-2022.4.27.0/abobjs/subprocess.py`

 * *Files identical despite different names*

### Comparing `control_rod-2021.10.18.7/abobjs/test.py` & `control_rod-2022.4.27.0/abobjs/test.py`

 * *Files identical despite different names*

### Comparing `control_rod-2021.10.18.7/abobjs/test_section.py` & `control_rod-2022.4.27.0/abobjs/test_section.py`

 * *Files identical despite different names*

### Comparing `control_rod-2021.10.18.7/abobjs/test_type.py` & `control_rod-2022.4.27.0/abobjs/test_type.py`

 * *Files identical despite different names*

### Comparing `control_rod-2021.10.18.7/abobjs/workspace.py` & `control_rod-2022.4.27.0/abobjs/workspace.py`

 * *Files identical despite different names*

### Comparing `control_rod-2021.10.18.7/control_rod.egg-info/SOURCES.txt` & `control_rod-2022.4.27.0/control_rod.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,28 +1,50 @@
 README.md
 pyproject.toml
 setup.cfg
 abobjs/__init__.py
 abobjs/assertion.py
+abobjs/auditable_entity.py
+abobjs/auditable_entity_regions.py
+abobjs/auditable_entity_types.py
 abobjs/base.py
+abobjs/buisness_units.py
 abobjs/continuous_monitoring_monitor_results.py
 abobjs/continuous_monitoring_monitors.py
 abobjs/continuous_monitoring_systems.py
 abobjs/control.py
 abobjs/controlrod.py
 abobjs/controls_data.py
+abobjs/departments.py
 abobjs/effectiveness_option.py
 abobjs/entity.py
 abobjs/file.py
+abobjs/multi.py
 abobjs/process.py
 abobjs/region.py
 abobjs/risk.py
 abobjs/status_option.py
 abobjs/subprocess.py
 abobjs/test.py
 abobjs/test_section.py
 abobjs/test_type.py
 abobjs/workspace.py
 control_rod.egg-info/PKG-INFO
 control_rod.egg-info/SOURCES.txt
 control_rod.egg-info/dependency_links.txt
-control_rod.egg-info/top_level.txt
+control_rod.egg-info/top_level.txt
+tests/test_assertion.py
+tests/test_control.py
+tests/test_controlrod.py
+tests/test_controlsdatum.py
+tests/test_effectivenessoption.py
+tests/test_entity.py
+tests/test_files.py
+tests/test_process.py
+tests/test_region.py
+tests/test_risk.py
+tests/test_status_option.py
+tests/test_subprocess.py
+tests/test_test.py
+tests/test_testsection.py
+tests/test_testtypes.py
+tests/test_workspace.py
```

