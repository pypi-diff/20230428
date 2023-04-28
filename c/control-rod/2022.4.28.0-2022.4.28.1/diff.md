# Comparing `tmp/control_rod-2022.4.28.0.tar.gz` & `tmp/control_rod-2022.4.28.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "control_rod-2022.4.28.0.tar", last modified: Fri Apr 28 17:49:36 2023, max compression
+gzip compressed data, was "control_rod-2022.4.28.1.tar", last modified: Fri Apr 28 18:40:54 2023, max compression
```

## Comparing `control_rod-2022.4.28.0.tar` & `control_rod-2022.4.28.1.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:49:36.848988 control_rod-2022.4.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-28 17:49:36.848988 control_rod-2022.4.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:49:36.844988 control_rod-2022.4.28.0/abobjs/
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/abobjs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/abobjs/assertion.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/abobjs/auditable_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/abobjs/auditable_entity_regions.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/abobjs/auditable_entity_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    25231 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/abobjs/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/abobjs/buisness_units.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/abobjs/continuous_monitoring_monitor_results.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/abobjs/continuous_monitoring_monitors.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/abobjs/continuous_monitoring_systems.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/abobjs/control.py
--rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/abobjs/controlrod.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/abobjs/controls_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/abobjs/departments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/abobjs/effectiveness_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/abobjs/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/abobjs/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/abobjs/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/abobjs/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/abobjs/region.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/abobjs/risk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/abobjs/status_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/abobjs/subprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/abobjs/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/abobjs/test_section.py
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/abobjs/test_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/abobjs/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:49:36.844988 control_rod-2022.4.28.0/control_rod.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-28 17:49:36.000000 control_rod-2022.4.28.0/control_rod.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-04-28 17:49:36.000000 control_rod-2022.4.28.0/control_rod.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 17:49:36.000000 control_rod-2022.4.28.0/control_rod.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-28 17:49:36.000000 control_rod-2022.4.28.0/control_rod.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-28 17:49:36.848988 control_rod-2022.4.28.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:49:36.848988 control_rod-2022.4.28.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/tests/test_assertion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/tests/test_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/tests/test_controlrod.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/tests/test_controlsdatum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/tests/test_effectivenessoption.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/tests/test_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/tests/test_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/tests/test_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/tests/test_region.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/tests/test_risk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/tests/test_status_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/tests/test_subprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/tests/test_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/tests/test_testsection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/tests/test_testtypes.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/tests/test_workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:40:54.842665 control_rod-2022.4.28.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-28 18:40:54.842665 control_rod-2022.4.28.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-28 18:40:38.000000 control_rod-2022.4.28.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:40:54.838665 control_rod-2022.4.28.1/abobjs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-04-28 18:40:38.000000 control_rod-2022.4.28.1/abobjs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-04-28 18:40:38.000000 control_rod-2022.4.28.1/abobjs/assertion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-28 18:40:38.000000 control_rod-2022.4.28.1/abobjs/auditable_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-28 18:40:38.000000 control_rod-2022.4.28.1/abobjs/auditable_entity_regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-28 18:40:38.000000 control_rod-2022.4.28.1/abobjs/auditable_entity_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25231 2023-04-28 18:40:38.000000 control_rod-2022.4.28.1/abobjs/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-28 18:40:38.000000 control_rod-2022.4.28.1/abobjs/buisness_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-28 18:40:38.000000 control_rod-2022.4.28.1/abobjs/continuous_monitoring_monitor_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-28 18:40:38.000000 control_rod-2022.4.28.1/abobjs/continuous_monitoring_monitors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-28 18:40:38.000000 control_rod-2022.4.28.1/abobjs/continuous_monitoring_systems.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-04-28 18:40:38.000000 control_rod-2022.4.28.1/abobjs/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-04-28 18:40:38.000000 control_rod-2022.4.28.1/abobjs/controlrod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-04-28 18:40:38.000000 control_rod-2022.4.28.1/abobjs/controls_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-28 18:40:38.000000 control_rod-2022.4.28.1/abobjs/departments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-28 18:40:38.000000 control_rod-2022.4.28.1/abobjs/effectiveness_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-04-28 18:40:38.000000 control_rod-2022.4.28.1/abobjs/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-28 18:40:38.000000 control_rod-2022.4.28.1/abobjs/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-28 18:40:38.000000 control_rod-2022.4.28.1/abobjs/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-28 18:40:38.000000 control_rod-2022.4.28.1/abobjs/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-28 18:40:38.000000 control_rod-2022.4.28.1/abobjs/region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-28 18:40:38.000000 control_rod-2022.4.28.1/abobjs/risk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-28 18:40:38.000000 control_rod-2022.4.28.1/abobjs/status_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-04-28 18:40:38.000000 control_rod-2022.4.28.1/abobjs/subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-28 18:40:38.000000 control_rod-2022.4.28.1/abobjs/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-04-28 18:40:38.000000 control_rod-2022.4.28.1/abobjs/test_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-28 18:40:38.000000 control_rod-2022.4.28.1/abobjs/test_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-28 18:40:38.000000 control_rod-2022.4.28.1/abobjs/vendor_criticalities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-28 18:40:38.000000 control_rod-2022.4.28.1/abobjs/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:40:54.838665 control_rod-2022.4.28.1/control_rod.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-28 18:40:54.000000 control_rod-2022.4.28.1/control_rod.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-28 18:40:54.000000 control_rod-2022.4.28.1/control_rod.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 18:40:54.000000 control_rod-2022.4.28.1/control_rod.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-28 18:40:54.000000 control_rod-2022.4.28.1/control_rod.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-28 18:40:38.000000 control_rod-2022.4.28.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-28 18:40:54.842665 control_rod-2022.4.28.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:40:54.842665 control_rod-2022.4.28.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-04-28 18:40:38.000000 control_rod-2022.4.28.1/tests/test_assertion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-04-28 18:40:38.000000 control_rod-2022.4.28.1/tests/test_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-04-28 18:40:38.000000 control_rod-2022.4.28.1/tests/test_controlrod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-28 18:40:38.000000 control_rod-2022.4.28.1/tests/test_controlsdatum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-04-28 18:40:38.000000 control_rod-2022.4.28.1/tests/test_effectivenessoption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-28 18:40:38.000000 control_rod-2022.4.28.1/tests/test_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-28 18:40:38.000000 control_rod-2022.4.28.1/tests/test_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-28 18:40:38.000000 control_rod-2022.4.28.1/tests/test_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-04-28 18:40:38.000000 control_rod-2022.4.28.1/tests/test_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-04-28 18:40:38.000000 control_rod-2022.4.28.1/tests/test_risk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-04-28 18:40:38.000000 control_rod-2022.4.28.1/tests/test_status_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-04-28 18:40:38.000000 control_rod-2022.4.28.1/tests/test_subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-28 18:40:38.000000 control_rod-2022.4.28.1/tests/test_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-04-28 18:40:38.000000 control_rod-2022.4.28.1/tests/test_testsection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-28 18:40:38.000000 control_rod-2022.4.28.1/tests/test_testtypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-28 18:40:38.000000 control_rod-2022.4.28.1/tests/test_workspace.py
```

### Comparing `control_rod-2022.4.28.0/abobjs/__init__.py` & `control_rod-2022.4.28.1/abobjs/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from .continuous_monitoring_systems import AB_Continous_Monitoring_Systems
 from .continuous_monitoring_monitors import AB_Continous_Monitoring_Monitors
 from .continuous_monitoring_monitor_results import AB_Continous_Monitoring_Monitor_Results
 
 from .auditable_entity import AB_Auditable_Entities
 from .auditable_entity_regions import AB_Auditable_Entity_Regions
 from .auditable_entity_types import AB_Auditable_Entity_Types
+from .vendor_criticalities import AB_Vendor_Criticality
 
 from .buisness_units import AB_Business_Unit
 from .departments import AB_Departments
 
 from .multi import AB_Multi
 
 SUBOBJ_LK = {"region_id": {"obj": AB_Region},
@@ -37,14 +38,15 @@
              "entity_id": {"obj": AB_Entity},
              "controls_datum_ids": {"obj": AB_Controls_Data},
              "test_ids": {"obj": AB_Test},
              "file_ids": {"obj": AB_File},
              "continuous_monitoring_system_id": {"obj": AB_Continous_Monitoring_Systems},
              "continuous_monitoring_monitor_id": {"obj": AB_Continous_Monitoring_Monitors},
              "auditable_entity_id": {"obj": AB_Auditable_Entities},
-             "auditable_entity_region_id": {"obj": AB_Auditable_Entity_Regions}
+             "auditable_entity_region_id": {"obj": AB_Auditable_Entity_Regions},
+             "vendor_criticalities_id": {"obj": AB_Vendor_Criticality}
             }
 
 
 from .controlrod import AB_ControlRod
 
 USER_AGENT = "control_rod/0.0.0"
```

### Comparing `control_rod-2022.4.28.0/abobjs/assertion.py` & `control_rod-2022.4.28.1/abobjs/assertion.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.28.0/abobjs/auditable_entity.py` & `control_rod-2022.4.28.1/abobjs/auditable_entity.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.28.0/abobjs/auditable_entity_regions.py` & `control_rod-2022.4.28.1/abobjs/auditable_entity_regions.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.28.0/abobjs/auditable_entity_types.py` & `control_rod-2022.4.28.1/abobjs/auditable_entity_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import abobjs
 
 class AB_Auditable_Entity_Types(abobjs.AB_Base):
 
     _endpoint = "/api/v1/auditable_entity_types"
     _single = ".auditable_entity_types[0]"
     _name = "auditable_entity_type"
+    _uid_field = "key"
 
     def __init__(self, id=None, api_info=None, **kwargs):
 
         # Dunder Handling
         endpoint = kwargs.get("endpoint", self._endpoint)
         single = kwargs.get("single", self._single)
         name = kwargs.get("name", self._name)
```

### Comparing `control_rod-2022.4.28.0/abobjs/base.py` & `control_rod-2022.4.28.1/abobjs/base.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.28.0/abobjs/buisness_units.py` & `control_rod-2022.4.28.1/abobjs/buisness_units.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.28.0/abobjs/continuous_monitoring_monitor_results.py` & `control_rod-2022.4.28.1/abobjs/continuous_monitoring_monitor_results.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.28.0/abobjs/continuous_monitoring_monitors.py` & `control_rod-2022.4.28.1/abobjs/continuous_monitoring_monitors.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.28.0/abobjs/continuous_monitoring_systems.py` & `control_rod-2022.4.28.1/abobjs/continuous_monitoring_systems.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.28.0/abobjs/control.py` & `control_rod-2022.4.28.1/abobjs/control.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.28.0/abobjs/controlrod.py` & `control_rod-2022.4.28.1/abobjs/controlrod.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.28.0/abobjs/controls_data.py` & `control_rod-2022.4.28.1/abobjs/controls_data.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.28.0/abobjs/departments.py` & `control_rod-2022.4.28.1/abobjs/departments.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.28.0/abobjs/effectiveness_option.py` & `control_rod-2022.4.28.1/abobjs/effectiveness_option.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.28.0/abobjs/entity.py` & `control_rod-2022.4.28.1/abobjs/entity.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.28.0/abobjs/file.py` & `control_rod-2022.4.28.1/abobjs/file.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.28.0/abobjs/multi.py` & `control_rod-2022.4.28.1/abobjs/multi.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.28.0/abobjs/process.py` & `control_rod-2022.4.28.1/abobjs/process.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.28.0/abobjs/region.py` & `control_rod-2022.4.28.1/abobjs/region.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.28.0/abobjs/risk.py` & `control_rod-2022.4.28.1/abobjs/risk.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.28.0/abobjs/status_option.py` & `control_rod-2022.4.28.1/abobjs/status_option.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.28.0/abobjs/subprocess.py` & `control_rod-2022.4.28.1/abobjs/subprocess.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.28.0/abobjs/test.py` & `control_rod-2022.4.28.1/abobjs/test.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.28.0/abobjs/test_section.py` & `control_rod-2022.4.28.1/abobjs/test_section.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.28.0/abobjs/test_type.py` & `control_rod-2022.4.28.1/abobjs/test_type.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.28.0/abobjs/workspace.py` & `control_rod-2022.4.28.1/abobjs/workspace.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.28.0/control_rod.egg-info/SOURCES.txt` & `control_rod-2022.4.28.1/control_rod.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 abobjs/region.py
 abobjs/risk.py
 abobjs/status_option.py
 abobjs/subprocess.py
 abobjs/test.py
 abobjs/test_section.py
 abobjs/test_type.py
+abobjs/vendor_criticalities.py
 abobjs/workspace.py
 control_rod.egg-info/PKG-INFO
 control_rod.egg-info/SOURCES.txt
 control_rod.egg-info/dependency_links.txt
 control_rod.egg-info/top_level.txt
 tests/test_assertion.py
 tests/test_control.py
```

### Comparing `control_rod-2022.4.28.0/tests/test_assertion.py` & `control_rod-2022.4.28.1/tests/test_assertion.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.28.0/tests/test_control.py` & `control_rod-2022.4.28.1/tests/test_control.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.28.0/tests/test_controlrod.py` & `control_rod-2022.4.28.1/tests/test_controlrod.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.28.0/tests/test_controlsdatum.py` & `control_rod-2022.4.28.1/tests/test_controlsdatum.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.28.0/tests/test_effectivenessoption.py` & `control_rod-2022.4.28.1/tests/test_effectivenessoption.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.28.0/tests/test_entity.py` & `control_rod-2022.4.28.1/tests/test_entity.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.28.0/tests/test_files.py` & `control_rod-2022.4.28.1/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.28.0/tests/test_process.py` & `control_rod-2022.4.28.1/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.28.0/tests/test_region.py` & `control_rod-2022.4.28.1/tests/test_region.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.28.0/tests/test_risk.py` & `control_rod-2022.4.28.1/tests/test_risk.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.28.0/tests/test_status_option.py` & `control_rod-2022.4.28.1/tests/test_status_option.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.28.0/tests/test_subprocess.py` & `control_rod-2022.4.28.1/tests/test_subprocess.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.28.0/tests/test_test.py` & `control_rod-2022.4.28.1/tests/test_test.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.28.0/tests/test_testsection.py` & `control_rod-2022.4.28.1/tests/test_testsection.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.28.0/tests/test_testtypes.py` & `control_rod-2022.4.28.1/tests/test_testtypes.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.28.0/tests/test_workspace.py` & `control_rod-2022.4.28.1/tests/test_workspace.py`

 * *Files identical despite different names*

