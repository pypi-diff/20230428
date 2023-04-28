# Comparing `tmp/gxabm-2.3.0.tar.gz` & `tmp/gxabm-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gxabm-2.3.0.tar", last modified: Thu Apr 27 20:19:21 2023, max compression
+gzip compressed data, was "gxabm-2.3.1.tar", last modified: Fri Apr 28 19:36:39 2023, max compression
```

## Comparing `gxabm-2.3.0.tar` & `gxabm-2.3.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-04-27 20:19:21.140571 gxabm-2.3.0/
--rw-r--r--   0 suderman   (502) staff       (20)       42 2022-03-07 12:56:12.000000 gxabm-2.3.0/MANIFEST.in
--rw-r--r--   0 suderman   (502) staff       (20)    19487 2023-04-27 20:19:21.140352 gxabm-2.3.0/PKG-INFO
--rw-r--r--   0 suderman   (502) staff       (20)    16395 2022-03-22 19:06:33.000000 gxabm-2.3.0/README.md
-drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-04-27 20:19:21.132981 gxabm-2.3.0/abm/
--rw-r--r--   0 suderman   (502) staff       (20)        5 2023-04-27 20:18:52.000000 gxabm-2.3.0/abm/VERSION
--rw-r--r--   0 suderman   (502) staff       (20)      290 2022-03-07 12:56:12.000000 gxabm-2.3.0/abm/__init__.py
--rw-r--r--   0 suderman   (502) staff       (20)     8362 2023-04-24 20:24:38.000000 gxabm-2.3.0/abm/__main__.py
-drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-04-27 20:19:21.137822 gxabm-2.3.0/abm/lib/
--rw-r--r--   0 suderman   (502) staff       (20)      447 2022-03-07 12:56:12.000000 gxabm-2.3.0/abm/lib/__init__.py
--rw-r--r--   0 suderman   (502) staff       (20)    18434 2023-04-27 20:18:52.000000 gxabm-2.3.0/abm/lib/benchmark.py
--rw-r--r--   0 suderman   (502) staff       (20)     7812 2022-10-19 17:36:24.000000 gxabm-2.3.0/abm/lib/cloudlaunch.py
--rw-r--r--   0 suderman   (502) staff       (20)     5458 2023-04-27 20:18:52.000000 gxabm-2.3.0/abm/lib/common.py
--rw-r--r--   0 suderman   (502) staff       (20)     5433 2022-10-19 17:36:24.000000 gxabm-2.3.0/abm/lib/config.py
--rw-r--r--   0 suderman   (502) staff       (20)     6483 2023-04-27 20:18:52.000000 gxabm-2.3.0/abm/lib/dataset.py
--rw-r--r--   0 suderman   (502) staff       (20)     7727 2023-04-27 20:18:52.000000 gxabm-2.3.0/abm/lib/experiment.py
--rw-r--r--   0 suderman   (502) staff       (20)      883 2022-03-07 12:56:12.000000 gxabm-2.3.0/abm/lib/folder.py
--rw-r--r--   0 suderman   (502) staff       (20)     4185 2022-10-27 02:48:01.000000 gxabm-2.3.0/abm/lib/helm.py
--rw-r--r--   0 suderman   (502) staff       (20)      282 2022-03-07 12:56:12.000000 gxabm-2.3.0/abm/lib/histories.yml
--rw-r--r--   0 suderman   (502) staff       (20)     9582 2023-04-27 20:14:45.000000 gxabm-2.3.0/abm/lib/history.py
--rw-r--r--   0 suderman   (502) staff       (20)     3382 2023-04-27 20:18:52.000000 gxabm-2.3.0/abm/lib/job.py
--rw-r--r--   0 suderman   (502) staff       (20)     1264 2022-03-07 12:56:12.000000 gxabm-2.3.0/abm/lib/kubectl.py
--rw-r--r--   0 suderman   (502) staff       (20)     2518 2023-04-24 20:08:21.000000 gxabm-2.3.0/abm/lib/library.py
--rw-r--r--   0 suderman   (502) staff       (20)    11186 2023-04-27 20:18:52.000000 gxabm-2.3.0/abm/lib/menu.yml
--rw-r--r--   0 suderman   (502) staff       (20)     3480 2022-10-19 17:36:24.000000 gxabm-2.3.0/abm/lib/users.py
--rw-r--r--   0 suderman   (502) staff       (20)     6930 2023-04-27 20:18:52.000000 gxabm-2.3.0/abm/lib/workflow.py
-drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-04-27 20:19:21.138692 gxabm-2.3.0/gxabm.egg-info/
--rw-r--r--   0 suderman   (502) staff       (20)    19487 2023-04-27 20:19:21.000000 gxabm-2.3.0/gxabm.egg-info/PKG-INFO
--rw-r--r--   0 suderman   (502) staff       (20)      669 2023-04-27 20:19:21.000000 gxabm-2.3.0/gxabm.egg-info/SOURCES.txt
--rw-r--r--   0 suderman   (502) staff       (20)        1 2023-04-27 20:19:21.000000 gxabm-2.3.0/gxabm.egg-info/dependency_links.txt
--rw-r--r--   0 suderman   (502) staff       (20)       49 2023-04-27 20:19:21.000000 gxabm-2.3.0/gxabm.egg-info/entry_points.txt
--rw-r--r--   0 suderman   (502) staff       (20)       48 2023-04-27 20:19:21.000000 gxabm-2.3.0/gxabm.egg-info/requires.txt
--rw-r--r--   0 suderman   (502) staff       (20)        9 2023-04-27 20:19:21.000000 gxabm-2.3.0/gxabm.egg-info/top_level.txt
--rw-r--r--   0 suderman   (502) staff       (20)       38 2023-04-27 20:19:21.140628 gxabm-2.3.0/setup.cfg
--rw-r--r--   0 suderman   (502) staff       (20)     1036 2022-10-19 17:36:24.000000 gxabm-2.3.0/setup.py
-drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-04-27 20:19:21.139894 gxabm-2.3.0/test/
--rw-r--r--   0 suderman   (502) staff       (20)      147 2022-03-07 12:56:12.000000 gxabm-2.3.0/test/__init__.py
--rwxr-xr-x   0 suderman   (502) staff       (20)     8684 2022-12-23 17:29:52.000000 gxabm-2.3.0/test/check_tools.py
--rw-r--r--   0 suderman   (502) staff       (20)     2160 2022-10-27 04:03:53.000000 gxabm-2.3.0/test/metrics.py
--rw-r--r--   0 suderman   (502) staff       (20)      298 2022-03-07 12:56:12.000000 gxabm-2.3.0/test/test_environments.py
--rw-r--r--   0 suderman   (502) staff       (20)      272 2023-03-14 21:04:32.000000 gxabm-2.3.0/test/workflow.py
+drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-04-28 19:36:39.724062 gxabm-2.3.1/
+-rw-r--r--   0 suderman   (502) staff       (20)       42 2022-03-07 12:56:12.000000 gxabm-2.3.1/MANIFEST.in
+-rw-r--r--   0 suderman   (502) staff       (20)    19487 2023-04-28 19:36:39.723883 gxabm-2.3.1/PKG-INFO
+-rw-r--r--   0 suderman   (502) staff       (20)    16395 2022-03-22 19:06:33.000000 gxabm-2.3.1/README.md
+drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-04-28 19:36:39.715787 gxabm-2.3.1/abm/
+-rw-r--r--   0 suderman   (502) staff       (20)        6 2023-04-28 19:36:16.000000 gxabm-2.3.1/abm/VERSION
+-rw-r--r--   0 suderman   (502) staff       (20)      290 2022-03-07 12:56:12.000000 gxabm-2.3.1/abm/__init__.py
+-rw-r--r--   0 suderman   (502) staff       (20)     8362 2023-04-24 20:24:38.000000 gxabm-2.3.1/abm/__main__.py
+drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-04-28 19:36:39.720768 gxabm-2.3.1/abm/lib/
+-rw-r--r--   0 suderman   (502) staff       (20)      447 2022-03-07 12:56:12.000000 gxabm-2.3.1/abm/lib/__init__.py
+-rw-r--r--   0 suderman   (502) staff       (20)    18434 2023-04-27 20:18:52.000000 gxabm-2.3.1/abm/lib/benchmark.py
+-rw-r--r--   0 suderman   (502) staff       (20)     7812 2022-10-19 17:36:24.000000 gxabm-2.3.1/abm/lib/cloudlaunch.py
+-rw-r--r--   0 suderman   (502) staff       (20)     5458 2023-04-27 20:18:52.000000 gxabm-2.3.1/abm/lib/common.py
+-rw-r--r--   0 suderman   (502) staff       (20)     5433 2022-10-19 17:36:24.000000 gxabm-2.3.1/abm/lib/config.py
+-rw-r--r--   0 suderman   (502) staff       (20)     6483 2023-04-27 20:18:52.000000 gxabm-2.3.1/abm/lib/dataset.py
+-rw-r--r--   0 suderman   (502) staff       (20)     7661 2023-04-28 19:35:54.000000 gxabm-2.3.1/abm/lib/experiment.py
+-rw-r--r--   0 suderman   (502) staff       (20)      883 2022-03-07 12:56:12.000000 gxabm-2.3.1/abm/lib/folder.py
+-rw-r--r--   0 suderman   (502) staff       (20)     4185 2022-10-27 02:48:01.000000 gxabm-2.3.1/abm/lib/helm.py
+-rw-r--r--   0 suderman   (502) staff       (20)      282 2022-03-07 12:56:12.000000 gxabm-2.3.1/abm/lib/histories.yml
+-rw-r--r--   0 suderman   (502) staff       (20)     9582 2023-04-27 20:14:45.000000 gxabm-2.3.1/abm/lib/history.py
+-rw-r--r--   0 suderman   (502) staff       (20)     3382 2023-04-27 20:18:52.000000 gxabm-2.3.1/abm/lib/job.py
+-rw-r--r--   0 suderman   (502) staff       (20)     1264 2022-03-07 12:56:12.000000 gxabm-2.3.1/abm/lib/kubectl.py
+-rw-r--r--   0 suderman   (502) staff       (20)     2518 2023-04-24 20:08:21.000000 gxabm-2.3.1/abm/lib/library.py
+-rw-r--r--   0 suderman   (502) staff       (20)    11186 2023-04-27 20:18:52.000000 gxabm-2.3.1/abm/lib/menu.yml
+-rw-r--r--   0 suderman   (502) staff       (20)     3480 2022-10-19 17:36:24.000000 gxabm-2.3.1/abm/lib/users.py
+-rw-r--r--   0 suderman   (502) staff       (20)     6930 2023-04-27 20:18:52.000000 gxabm-2.3.1/abm/lib/workflow.py
+drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-04-28 19:36:39.721573 gxabm-2.3.1/gxabm.egg-info/
+-rw-r--r--   0 suderman   (502) staff       (20)    19487 2023-04-28 19:36:39.000000 gxabm-2.3.1/gxabm.egg-info/PKG-INFO
+-rw-r--r--   0 suderman   (502) staff       (20)      669 2023-04-28 19:36:39.000000 gxabm-2.3.1/gxabm.egg-info/SOURCES.txt
+-rw-r--r--   0 suderman   (502) staff       (20)        1 2023-04-28 19:36:39.000000 gxabm-2.3.1/gxabm.egg-info/dependency_links.txt
+-rw-r--r--   0 suderman   (502) staff       (20)       49 2023-04-28 19:36:39.000000 gxabm-2.3.1/gxabm.egg-info/entry_points.txt
+-rw-r--r--   0 suderman   (502) staff       (20)       48 2023-04-28 19:36:39.000000 gxabm-2.3.1/gxabm.egg-info/requires.txt
+-rw-r--r--   0 suderman   (502) staff       (20)        9 2023-04-28 19:36:39.000000 gxabm-2.3.1/gxabm.egg-info/top_level.txt
+-rw-r--r--   0 suderman   (502) staff       (20)       38 2023-04-28 19:36:39.724110 gxabm-2.3.1/setup.cfg
+-rw-r--r--   0 suderman   (502) staff       (20)     1036 2022-10-19 17:36:24.000000 gxabm-2.3.1/setup.py
+drwxr-xr-x   0 suderman   (502) staff       (20)        0 2023-04-28 19:36:39.723139 gxabm-2.3.1/test/
+-rw-r--r--   0 suderman   (502) staff       (20)      147 2022-03-07 12:56:12.000000 gxabm-2.3.1/test/__init__.py
+-rwxr-xr-x   0 suderman   (502) staff       (20)     8684 2022-12-23 17:29:52.000000 gxabm-2.3.1/test/check_tools.py
+-rw-r--r--   0 suderman   (502) staff       (20)     2160 2022-10-27 04:03:53.000000 gxabm-2.3.1/test/metrics.py
+-rw-r--r--   0 suderman   (502) staff       (20)      298 2022-03-07 12:56:12.000000 gxabm-2.3.1/test/test_environments.py
+-rw-r--r--   0 suderman   (502) staff       (20)      272 2023-03-14 21:04:32.000000 gxabm-2.3.1/test/workflow.py
```

### Comparing `gxabm-2.3.0/PKG-INFO` & `gxabm-2.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gxabm
-Version: 2.3.0
+Version: 2.3.1
 Summary: Opinionated Benchmarking Automatation in Galaxy
 Home-page: https://github.com/galaxyproject/gxabm
 Author: Keith Suderman
 Author-email: suderman@jhu.edu
 License: MIT
 Description: # Automated Benchmarking in Galaxy
         An opinionated Python Bioblend script for automating benchmarking tasks in Galaxy.
```

### Comparing `gxabm-2.3.0/README.md` & `gxabm-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `gxabm-2.3.0/abm/__main__.py` & `gxabm-2.3.1/abm/__main__.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.3.0/abm/lib/benchmark.py` & `gxabm-2.3.1/abm/lib/benchmark.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.3.0/abm/lib/cloudlaunch.py` & `gxabm-2.3.1/abm/lib/cloudlaunch.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.3.0/abm/lib/common.py` & `gxabm-2.3.1/abm/lib/common.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.3.0/abm/lib/config.py` & `gxabm-2.3.1/abm/lib/config.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.3.0/abm/lib/dataset.py` & `gxabm-2.3.1/abm/lib/dataset.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.3.0/abm/lib/experiment.py` & `gxabm-2.3.1/abm/lib/experiment.py`

 * *Files 3% similar despite different names*

```diff
@@ -143,19 +143,18 @@
     print(header_row)
     for input_dir in input_dirs:
         for file in os.listdir(input_dir):
             input_path = os.path.join(input_dir, file)
             if not os.path.isfile(input_path) or not input_path.endswith('.json'):
                 continue
             try:
-                print(f"Loading {input_path}")
                 with open(input_path, 'r') as f:
                     data = json.load(f)
-                if data['job_metrics']['tool_id'] == 'upload1':
-                    print('Ignoring upload tool')
+                if data['metrics']['tool_id'] == 'upload1':
+                    #print('Ignoring upload tool')
                     continue
                 row = make_row(data)
                 print(separator.join([ str(x) for x in row]))
             except Exception as e:
                 # Silently fail to allow the remainder of the table to be generated.
                 print(f"Unable to process {input_path}")
                 print(e)
@@ -163,23 +162,23 @@
                 #pass
 
 
 accept_metrics = ['galaxy_slots', 'galaxy_memory_mb', 'runtime_seconds', 'cpuacct.usage','memory.limit_in_bytes', 'memory.max_usage_in_bytes']  #,'memory.soft_limit_in_bytes']
 
 def make_table_row(data: dict):
     row = [ str(data[key]) for key in ['run', 'cloud', 'job_conf', 'workflow_id', 'history_id', 'inputs']]
-    row.append(parse_toolid(data['job_metrics']['tool_id']))
-    row.append(data['job_metrics']['state'])
-    for e in _get_metrics(data['job_metrics']['job_metrics']):
+    row.append(parse_toolid(data['metrics']['tool_id']))
+    row.append(data['metrics']['state'])
+    for e in _get_metrics(data['metrics']['job_metrics']):
         row.append(e)
     return row
 
 
 def make_model_row(data: dict):
-    metrics = data['job_metrics']
+    metrics = data['metrics']
     row = []
     row.append(metrics['id'])
     tool_id = metrics['tool_id']
     row.append(tool_id)
     row.append(tool_id.split('/')[-1])
     row.append(metrics['state'])
     job_metrics = parse_job_metrics(metrics['job_metrics'])
```

### Comparing `gxabm-2.3.0/abm/lib/folder.py` & `gxabm-2.3.1/abm/lib/folder.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.3.0/abm/lib/helm.py` & `gxabm-2.3.1/abm/lib/helm.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.3.0/abm/lib/history.py` & `gxabm-2.3.1/abm/lib/history.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.3.0/abm/lib/job.py` & `gxabm-2.3.1/abm/lib/job.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.3.0/abm/lib/kubectl.py` & `gxabm-2.3.1/abm/lib/kubectl.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.3.0/abm/lib/library.py` & `gxabm-2.3.1/abm/lib/library.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.3.0/abm/lib/menu.yml` & `gxabm-2.3.1/abm/lib/menu.yml`

 * *Files identical despite different names*

### Comparing `gxabm-2.3.0/abm/lib/users.py` & `gxabm-2.3.1/abm/lib/users.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.3.0/abm/lib/workflow.py` & `gxabm-2.3.1/abm/lib/workflow.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.3.0/gxabm.egg-info/PKG-INFO` & `gxabm-2.3.1/gxabm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gxabm
-Version: 2.3.0
+Version: 2.3.1
 Summary: Opinionated Benchmarking Automatation in Galaxy
 Home-page: https://github.com/galaxyproject/gxabm
 Author: Keith Suderman
 Author-email: suderman@jhu.edu
 License: MIT
 Description: # Automated Benchmarking in Galaxy
         An opinionated Python Bioblend script for automating benchmarking tasks in Galaxy.
```

### Comparing `gxabm-2.3.0/gxabm.egg-info/SOURCES.txt` & `gxabm-2.3.1/gxabm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gxabm-2.3.0/setup.py` & `gxabm-2.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.3.0/test/check_tools.py` & `gxabm-2.3.1/test/check_tools.py`

 * *Files identical despite different names*

### Comparing `gxabm-2.3.0/test/metrics.py` & `gxabm-2.3.1/test/metrics.py`

 * *Files identical despite different names*

