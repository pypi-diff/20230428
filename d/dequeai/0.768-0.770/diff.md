# Comparing `tmp/dequeai-0.768.tar.gz` & `tmp/dequeai-0.770.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dequeai-0.768.tar", last modified: Wed Apr 26 15:27:57 2023, max compression
+gzip compressed data, was "dequeai-0.770.tar", last modified: Thu Apr 27 16:00:20 2023, max compression
```

## Comparing `dequeai-0.768.tar` & `dequeai-0.770.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 15:27:57.535545 dequeai-0.768/
--rw-r--r--   0 root         (0) root         (0)      319 2023-04-26 15:27:57.535545 dequeai-0.768/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 15:27:57.531545 dequeai-0.768/dequeai/
--rw-r--r--   0 root         (0) root         (0)      370 2023-04-21 15:01:14.000000 dequeai-0.768/dequeai/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15384 2023-04-11 16:25:26.000000 dequeai-0.768/dequeai/datatypes.py
--rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.768/dequeai/deque_config.py
--rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.768/dequeai/deque_environment.py
--rw-r--r--   0 root         (0) root         (0)      955 2023-04-26 15:26:45.000000 dequeai-0.768/dequeai/dequeai.py
--rw-r--r--   0 root         (0) root         (0)    29846 2023-04-26 14:48:28.000000 dequeai-0.768/dequeai/dequeai_run.py
--rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.768/dequeai/parsing_service.py
--rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.768/dequeai/redis_services.py
--rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.768/dequeai/rest_connect.py
--rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.768/dequeai/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 15:27:57.531545 dequeai-0.768/dequeai.egg-info/
--rw-r--r--   0 root         (0) root         (0)      319 2023-04-26 15:27:57.000000 dequeai-0.768/dequeai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      391 2023-04-26 15:27:57.000000 dequeai-0.768/dequeai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 15:27:57.000000 dequeai-0.768/dequeai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-04-26 15:27:57.000000 dequeai-0.768/dequeai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-26 15:27:57.000000 dequeai-0.768/dequeai.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 15:27:57.535545 dequeai-0.768/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      494 2023-04-26 15:27:42.000000 dequeai-0.768/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:00:20.696032 dequeai-0.770/
+-rw-r--r--   0 root         (0) root         (0)      319 2023-04-27 16:00:20.696032 dequeai-0.770/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:00:20.692032 dequeai-0.770/dequeai/
+-rw-r--r--   0 root         (0) root         (0)      370 2023-04-21 15:01:14.000000 dequeai-0.770/dequeai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15384 2023-04-11 16:25:26.000000 dequeai-0.770/dequeai/datatypes.py
+-rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.770/dequeai/deque_config.py
+-rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.770/dequeai/deque_environment.py
+-rw-r--r--   0 root         (0) root         (0)      955 2023-04-26 15:26:45.000000 dequeai-0.770/dequeai/dequeai.py
+-rw-r--r--   0 root         (0) root         (0)    29561 2023-04-27 15:59:27.000000 dequeai-0.770/dequeai/dequeai_run.py
+-rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.770/dequeai/parsing_service.py
+-rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.770/dequeai/redis_services.py
+-rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.770/dequeai/rest_connect.py
+-rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.770/dequeai/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 16:00:20.696032 dequeai-0.770/dequeai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      319 2023-04-27 16:00:20.000000 dequeai-0.770/dequeai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      391 2023-04-27 16:00:20.000000 dequeai-0.770/dequeai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 16:00:20.000000 dequeai-0.770/dequeai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-04-27 16:00:20.000000 dequeai-0.770/dequeai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-27 16:00:20.000000 dequeai-0.770/dequeai.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-27 16:00:20.696032 dequeai-0.770/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      494 2023-04-26 19:29:39.000000 dequeai-0.770/setup.py
```

### Comparing `dequeai-0.768/dequeai/datatypes.py` & `dequeai-0.770/dequeai/datatypes.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.768/dequeai/dequeai.py` & `dequeai-0.770/dequeai/dequeai.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.768/dequeai/dequeai_run.py` & `dequeai-0.770/dequeai/dequeai_run.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,17 +46,15 @@
         self._running = False
         self._environment_logged = False
         self._resources_logged = False
         self._res_monitor = None
         self._run_start_time = None
 
     def init(self, user_name, api_key, project_name=None):
-        print("My project name is " + project_name)
-        print("My user name is " + user_name)
-        print("My api key is " + api_key)
+
         os.environ["running"] = "yes"
         is_authenticated = self._authenticate(user_name=user_name, api_key=api_key)
         if is_authenticated:
             self.user_name = user_name
             self._api_key = api_key
         else:
             self.user_name = None
@@ -70,17 +68,16 @@
                # "Deque AI package is only supported wihtin the Creator's App. Download the app from https://deque.ai")
 
         self._submission_id = os.getenv("submission_id")
         self._agent_id = os.getenv("agent_id")
         if project_name is None:
             raise ValueError("Project name cannot be empty")
         else:
-            print("Project name is " + project_name)
             self._project_name = project_name
-            print("Project name is " + self._project_name)
+
         self._run_id = str(coolname.generate_slug(2))
         self._step = 1
         # p2 = multiprocessing.Process(target=self._start_parser)
         # p2.start()
         self._run_meta_data = {"submission_id": self._submission_id, "run_id": self._run_id,
                                "workload_type": self._workload_type, "workload_id": self._workload_id,
                                "project_name": self._project_name, "user_name": user_name}
@@ -227,24 +224,24 @@
         # let's add some System metadata to the data
         metadata = {}
         gpu_count = len(GPUtil.getGPUs())
         for i in range(gpu_count):
             gpu_free_memory = GPUtil.getGPUs()[i].memoryFree
             current_gpu_load = 100 * GPUtil.getGPUs()[i].load
             total_gpu_memory = GPUtil.getGPUs()[i].memoryTotal
-            metadata.update({"GPU": {str(i): {"total_memory": total_gpu_memory, "free_memory": gpu_free_memory,
+            metadata.update({"GPU": {str(i): {"memory": {"total":total_gpu_memory, "free": gpu_free_memory},
                                               "utilization": current_gpu_load}}})
 
         metadata.update({"CPU": {"utilization": float(psutil.cpu_percent(interval=1))}})
 
         metadata.update({"CPU": {"count": int(psutil.cpu_count())},"cores": int(psutil.cpu_count(logical=True))})
-        metadata.update({"Memory": {"available_memory": psutil.virtual_memory()[1]}})
-        metadata.update({"Memory": {"total_memory": psutil.virtual_memory()[0]}})
-        metadata.update({"Memory": {"memory_utilization": psutil.virtual_memory()[2]}})
-        metadata.update({"Disk": {"free_disk_space": psutil.disk_usage(os.path.sep)[1]}})
+        metadata.update({"memory": {"available": psutil.virtual_memory()[1]}})
+        metadata.update({"memory": {"total": psutil.virtual_memory()[0]}})
+        metadata.update({"memory": {"utilization": psutil.virtual_memory()[2]}})
+        metadata.update({"disk": {"free": psutil.disk_usage(os.path.sep)[1]}})
         data["experiment_data"].update({"System": metadata})
 
         pickled_data = pickle.dumps(data)
         self._rest.post_binary(url=TRACKING_ENDPOINT, data=pickled_data)
 
     def log_artifact(self, artifact_type, path):
         if self._run_meta_data is None:
```

### Comparing `dequeai-0.768/dequeai/parsing_service.py` & `dequeai-0.770/dequeai/parsing_service.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.768/dequeai/rest_connect.py` & `dequeai-0.770/dequeai/rest_connect.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.768/dequeai/util.py` & `dequeai-0.770/dequeai/util.py`

 * *Files identical despite different names*

