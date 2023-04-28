# Comparing `tmp/control_rod-2022.4.27.0.tar.gz` & `tmp/control_rod-2022.4.28.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "control_rod-2022.4.27.0.tar", last modified: Fri Apr 28 17:27:21 2023, max compression
+gzip compressed data, was "control_rod-2022.4.28.0.tar", last modified: Fri Apr 28 17:49:36 2023, max compression
```

## Comparing `control_rod-2022.4.27.0.tar` & `control_rod-2022.4.28.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:27:21.736346 control_rod-2022.4.27.0/
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-28 17:27:21.736346 control_rod-2022.4.27.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:27:21.732346 control_rod-2022.4.27.0/abobjs/
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/abobjs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/abobjs/assertion.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/abobjs/auditable_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/abobjs/auditable_entity_regions.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/abobjs/auditable_entity_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    24740 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/abobjs/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/abobjs/buisness_units.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/abobjs/continuous_monitoring_monitor_results.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/abobjs/continuous_monitoring_monitors.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/abobjs/continuous_monitoring_systems.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/abobjs/control.py
--rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/abobjs/controlrod.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/abobjs/controls_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/abobjs/departments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/abobjs/effectiveness_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/abobjs/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/abobjs/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/abobjs/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/abobjs/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/abobjs/region.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/abobjs/risk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/abobjs/status_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/abobjs/subprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/abobjs/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/abobjs/test_section.py
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/abobjs/test_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/abobjs/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:27:21.736346 control_rod-2022.4.27.0/control_rod.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-28 17:27:21.000000 control_rod-2022.4.27.0/control_rod.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-04-28 17:27:21.000000 control_rod-2022.4.27.0/control_rod.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 17:27:21.000000 control_rod-2022.4.27.0/control_rod.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-28 17:27:21.000000 control_rod-2022.4.27.0/control_rod.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-28 17:27:21.740346 control_rod-2022.4.27.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:27:21.736346 control_rod-2022.4.27.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/tests/test_assertion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/tests/test_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/tests/test_controlrod.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/tests/test_controlsdatum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/tests/test_effectivenessoption.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/tests/test_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/tests/test_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/tests/test_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/tests/test_region.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/tests/test_risk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/tests/test_status_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/tests/test_subprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/tests/test_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/tests/test_testsection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/tests/test_testtypes.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-28 17:27:01.000000 control_rod-2022.4.27.0/tests/test_workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:49:36.848988 control_rod-2022.4.28.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-28 17:49:36.848988 control_rod-2022.4.28.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:49:36.844988 control_rod-2022.4.28.0/abobjs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/abobjs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/abobjs/assertion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/abobjs/auditable_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/abobjs/auditable_entity_regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/abobjs/auditable_entity_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25231 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/abobjs/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/abobjs/buisness_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/abobjs/continuous_monitoring_monitor_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/abobjs/continuous_monitoring_monitors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/abobjs/continuous_monitoring_systems.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/abobjs/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/abobjs/controlrod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/abobjs/controls_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/abobjs/departments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/abobjs/effectiveness_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/abobjs/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/abobjs/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/abobjs/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/abobjs/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/abobjs/region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/abobjs/risk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/abobjs/status_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/abobjs/subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/abobjs/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/abobjs/test_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/abobjs/test_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/abobjs/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:49:36.844988 control_rod-2022.4.28.0/control_rod.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-28 17:49:36.000000 control_rod-2022.4.28.0/control_rod.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-04-28 17:49:36.000000 control_rod-2022.4.28.0/control_rod.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 17:49:36.000000 control_rod-2022.4.28.0/control_rod.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-28 17:49:36.000000 control_rod-2022.4.28.0/control_rod.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-28 17:49:36.848988 control_rod-2022.4.28.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 17:49:36.848988 control_rod-2022.4.28.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/tests/test_assertion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/tests/test_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/tests/test_controlrod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/tests/test_controlsdatum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/tests/test_effectivenessoption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/tests/test_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/tests/test_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/tests/test_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/tests/test_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/tests/test_risk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/tests/test_status_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/tests/test_subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/tests/test_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/tests/test_testsection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/tests/test_testtypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-28 17:49:20.000000 control_rod-2022.4.28.0/tests/test_workspace.py
```

### Comparing `control_rod-2022.4.27.0/abobjs/__init__.py` & `control_rod-2022.4.28.0/abobjs/__init__.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.27.0/abobjs/assertion.py` & `control_rod-2022.4.28.0/abobjs/assertion.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.27.0/abobjs/auditable_entity.py` & `control_rod-2022.4.28.0/abobjs/auditable_entity.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.27.0/abobjs/auditable_entity_regions.py` & `control_rod-2022.4.28.0/abobjs/auditable_entity_regions.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.27.0/abobjs/auditable_entity_types.py` & `control_rod-2022.4.28.0/abobjs/auditable_entity_types.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.27.0/abobjs/base.py` & `control_rod-2022.4.28.0/abobjs/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -419,20 +419,31 @@
         """
         Reads AB Datestring with miliseconds and converts it to datetime object
 
         :param datestring:
         :return:
         """
 
-        front, back = datestring.split(".")
+        this_date = None
 
-        this_ms = int("{}000".format(back.strip("Z")))
-        this_date = datetime.datetime.strptime(front, self.datefront)
+        try:
+            front, back = datestring.split(".")
+        except ValueError as abnormal_date:
+            self.logger.warning("Abnormal Date String: {}".format(datestring))
+
+            try:
+                this_date = datetime.datetime.strptime("%Y-%m-%d", datestring)
+            except Exception as not_secondary_date:
+                self.logger.warning("Abnormal Date String not day, returning as string: {}".format(datestring))
+                this_date = datestring
+        else:
+            this_ms = int("{}000".format(back.strip("Z")))
+            this_date = datetime.datetime.strptime(front, self.datefront)
 
-        this_date.replace(microsecond=this_ms)
+            this_date.replace(microsecond=this_ms)
 
         return this_date
 
     def datewrite(self, dateobj):
 
         """
         Reads a Datetime and returns it in the format that Datestring Needs
```

### Comparing `control_rod-2022.4.27.0/abobjs/buisness_units.py` & `control_rod-2022.4.28.0/abobjs/buisness_units.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.27.0/abobjs/continuous_monitoring_monitor_results.py` & `control_rod-2022.4.28.0/abobjs/continuous_monitoring_monitor_results.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.27.0/abobjs/continuous_monitoring_monitors.py` & `control_rod-2022.4.28.0/abobjs/continuous_monitoring_monitors.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.27.0/abobjs/continuous_monitoring_systems.py` & `control_rod-2022.4.28.0/abobjs/continuous_monitoring_systems.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.27.0/abobjs/control.py` & `control_rod-2022.4.28.0/abobjs/control.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.27.0/abobjs/controlrod.py` & `control_rod-2022.4.28.0/abobjs/controlrod.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.27.0/abobjs/controls_data.py` & `control_rod-2022.4.28.0/abobjs/controls_data.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.27.0/abobjs/departments.py` & `control_rod-2022.4.28.0/abobjs/departments.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.27.0/abobjs/effectiveness_option.py` & `control_rod-2022.4.28.0/abobjs/effectiveness_option.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.27.0/abobjs/entity.py` & `control_rod-2022.4.28.0/abobjs/entity.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.27.0/abobjs/file.py` & `control_rod-2022.4.28.0/abobjs/file.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.27.0/abobjs/multi.py` & `control_rod-2022.4.28.0/abobjs/multi.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.27.0/abobjs/process.py` & `control_rod-2022.4.28.0/abobjs/process.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.27.0/abobjs/region.py` & `control_rod-2022.4.28.0/abobjs/region.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.27.0/abobjs/risk.py` & `control_rod-2022.4.28.0/abobjs/risk.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.27.0/abobjs/status_option.py` & `control_rod-2022.4.28.0/abobjs/status_option.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.27.0/abobjs/subprocess.py` & `control_rod-2022.4.28.0/abobjs/subprocess.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.27.0/abobjs/test.py` & `control_rod-2022.4.28.0/abobjs/test.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.27.0/abobjs/test_section.py` & `control_rod-2022.4.28.0/abobjs/test_section.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.27.0/abobjs/test_type.py` & `control_rod-2022.4.28.0/abobjs/test_type.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.27.0/abobjs/workspace.py` & `control_rod-2022.4.28.0/abobjs/workspace.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.27.0/control_rod.egg-info/SOURCES.txt` & `control_rod-2022.4.28.0/control_rod.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.27.0/tests/test_assertion.py` & `control_rod-2022.4.28.0/tests/test_assertion.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.27.0/tests/test_control.py` & `control_rod-2022.4.28.0/tests/test_control.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.27.0/tests/test_controlrod.py` & `control_rod-2022.4.28.0/tests/test_controlrod.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.27.0/tests/test_controlsdatum.py` & `control_rod-2022.4.28.0/tests/test_controlsdatum.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.27.0/tests/test_effectivenessoption.py` & `control_rod-2022.4.28.0/tests/test_effectivenessoption.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.27.0/tests/test_entity.py` & `control_rod-2022.4.28.0/tests/test_entity.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.27.0/tests/test_files.py` & `control_rod-2022.4.28.0/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.27.0/tests/test_process.py` & `control_rod-2022.4.28.0/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.27.0/tests/test_region.py` & `control_rod-2022.4.28.0/tests/test_region.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.27.0/tests/test_risk.py` & `control_rod-2022.4.28.0/tests/test_risk.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.27.0/tests/test_status_option.py` & `control_rod-2022.4.28.0/tests/test_status_option.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.27.0/tests/test_subprocess.py` & `control_rod-2022.4.28.0/tests/test_subprocess.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.27.0/tests/test_test.py` & `control_rod-2022.4.28.0/tests/test_test.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.27.0/tests/test_testsection.py` & `control_rod-2022.4.28.0/tests/test_testsection.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.27.0/tests/test_testtypes.py` & `control_rod-2022.4.28.0/tests/test_testtypes.py`

 * *Files identical despite different names*

### Comparing `control_rod-2022.4.27.0/tests/test_workspace.py` & `control_rod-2022.4.28.0/tests/test_workspace.py`

 * *Files identical despite different names*

