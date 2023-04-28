# Comparing `tmp/microservicebus-py-0.9.0.tar.gz` & `tmp/microservicebus-py-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microservicebus-py-0.9.0.tar", last modified: Tue Mar  7 08:19:32 2023, max compression
+gzip compressed data, was "microservicebus-py-0.9.1.tar", last modified: Fri Apr 28 14:19:27 2023, max compression
```

## Comparing `microservicebus-py-0.9.0.tar` & `microservicebus-py-0.9.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0 mikael    (1000) mikael    (1000)        0 2023-03-07 08:19:32.118764 microservicebus-py-0.9.0/
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     4745 2023-03-07 08:19:32.114577 microservicebus-py-0.9.0/PKG-INFO
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     3680 2022-12-12 08:25:32.000000 microservicebus-py-0.9.0/README.md
-drwxrwxrwx   0 mikael    (1000) mikael    (1000)        0 2023-03-07 08:19:31.737670 microservicebus-py-0.9.0/microservicebus_py.egg-info/
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     4745 2023-03-07 08:19:31.000000 microservicebus-py-0.9.0/microservicebus_py.egg-info/PKG-INFO
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)      455 2023-03-07 08:19:31.000000 microservicebus-py-0.9.0/microservicebus_py.egg-info/SOURCES.txt
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)        1 2023-03-07 08:19:31.000000 microservicebus-py-0.9.0/microservicebus_py.egg-info/dependency_links.txt
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)       55 2023-03-07 08:19:31.000000 microservicebus-py-0.9.0/microservicebus_py.egg-info/entry_points.txt
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)        4 2023-03-07 08:19:31.000000 microservicebus-py-0.9.0/microservicebus_py.egg-info/top_level.txt
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)       38 2023-03-07 08:19:32.119775 microservicebus-py-0.9.0/setup.cfg
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     1711 2023-03-07 08:09:06.000000 microservicebus-py-0.9.0/setup.py
-drwxrwxrwx   0 mikael    (1000) mikael    (1000)        0 2023-03-07 08:19:32.085179 microservicebus-py-0.9.0/src/
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)      807 2022-12-19 11:22:24.000000 microservicebus-py-0.9.0/src/axians.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     5687 2023-03-06 08:28:59.000000 microservicebus-py-0.9.0/src/base_service.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     1324 2023-01-05 09:33:48.000000 microservicebus-py-0.9.0/src/logger_service.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)    29298 2023-03-07 08:17:54.000000 microservicebus-py-0.9.0/src/msb_handler.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     6536 2023-03-06 08:30:37.000000 microservicebus-py-0.9.0/src/orchestrator_service.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)      340 2022-03-14 19:13:32.000000 microservicebus-py-0.9.0/src/queue_message.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     4414 2022-12-02 13:59:45.000000 microservicebus-py-0.9.0/src/rauc_handler.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)      807 2023-01-24 11:06:53.000000 microservicebus-py-0.9.0/src/start.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     3311 2023-01-09 21:54:56.000000 microservicebus-py-0.9.0/src/terminal_service.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)      672 2022-03-23 09:36:17.000000 microservicebus-py-0.9.0/src/test.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)      472 2022-04-27 07:36:56.000000 microservicebus-py-0.9.0/src/utils.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     3136 2022-12-12 08:35:01.000000 microservicebus-py-0.9.0/src/vpn_helper.py
+drwxrwxrwx   0 mikael    (1000) mikael    (1000)        0 2023-04-28 14:19:27.627327 microservicebus-py-0.9.1/
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     4745 2023-04-28 14:19:27.623328 microservicebus-py-0.9.1/PKG-INFO
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     3680 2022-12-12 08:25:32.000000 microservicebus-py-0.9.1/README.md
+drwxrwxrwx   0 mikael    (1000) mikael    (1000)        0 2023-04-28 14:19:27.155788 microservicebus-py-0.9.1/microservicebus_py.egg-info/
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     4745 2023-04-28 14:19:26.000000 microservicebus-py-0.9.1/microservicebus_py.egg-info/PKG-INFO
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)      455 2023-04-28 14:19:26.000000 microservicebus-py-0.9.1/microservicebus_py.egg-info/SOURCES.txt
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)        1 2023-04-28 14:19:26.000000 microservicebus-py-0.9.1/microservicebus_py.egg-info/dependency_links.txt
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)       55 2023-04-28 14:19:26.000000 microservicebus-py-0.9.1/microservicebus_py.egg-info/entry_points.txt
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)        4 2023-04-28 14:19:26.000000 microservicebus-py-0.9.1/microservicebus_py.egg-info/top_level.txt
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)       38 2023-04-28 14:19:27.629352 microservicebus-py-0.9.1/setup.cfg
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     1711 2023-04-28 14:15:01.000000 microservicebus-py-0.9.1/setup.py
+drwxrwxrwx   0 mikael    (1000) mikael    (1000)        0 2023-04-28 14:19:27.591430 microservicebus-py-0.9.1/src/
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)      807 2022-12-19 11:22:24.000000 microservicebus-py-0.9.1/src/axians.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     5687 2023-03-06 08:28:59.000000 microservicebus-py-0.9.1/src/base_service.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     1324 2023-01-05 09:33:48.000000 microservicebus-py-0.9.1/src/logger_service.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)    29588 2023-04-26 22:27:47.000000 microservicebus-py-0.9.1/src/msb_handler.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     6536 2023-03-06 08:30:37.000000 microservicebus-py-0.9.1/src/orchestrator_service.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)      340 2022-03-14 19:13:32.000000 microservicebus-py-0.9.1/src/queue_message.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     4414 2022-12-02 13:59:45.000000 microservicebus-py-0.9.1/src/rauc_handler.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)      807 2023-01-24 11:06:53.000000 microservicebus-py-0.9.1/src/start.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     3311 2023-01-09 21:54:56.000000 microservicebus-py-0.9.1/src/terminal_service.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)      672 2022-03-23 09:36:17.000000 microservicebus-py-0.9.1/src/test.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)      472 2022-04-27 07:36:56.000000 microservicebus-py-0.9.1/src/utils.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     3136 2022-12-12 08:35:01.000000 microservicebus-py-0.9.1/src/vpn_helper.py
```

### Comparing `microservicebus-py-0.9.0/PKG-INFO` & `microservicebus-py-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microservicebus-py
-Version: 0.9.0
+Version: 0.9.1
 Summary: Python agent for microServiceBus.com. Please visit https://microservicebus.com for more information.
 Home-page: https://github.com/axians/microservicebus-py
 Author: AXIANS IoT Operations
 Author-email: microservicebus@axians.com
 License: MIT
 Description: # microservicebus-py
```

### Comparing `microservicebus-py-0.9.0/README.md` & `microservicebus-py-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `microservicebus-py-0.9.0/microservicebus_py.egg-info/PKG-INFO` & `microservicebus-py-0.9.1/microservicebus_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microservicebus-py
-Version: 0.9.0
+Version: 0.9.1
 Summary: Python agent for microServiceBus.com. Please visit https://microservicebus.com for more information.
 Home-page: https://github.com/axians/microservicebus-py
 Author: AXIANS IoT Operations
 Author-email: microservicebus@axians.com
 License: MIT
 Description: # microservicebus-py
```

### Comparing `microservicebus-py-0.9.0/setup.py` & `microservicebus-py-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `microservicebus-py-0.9.0/src/axians.py` & `microservicebus-py-0.9.1/src/axians.py`

 * *Files identical despite different names*

### Comparing `microservicebus-py-0.9.0/src/base_service.py` & `microservicebus-py-0.9.1/src/base_service.py`

 * *Files identical despite different names*

### Comparing `microservicebus-py-0.9.0/src/logger_service.py` & `microservicebus-py-0.9.1/src/logger_service.py`

 * *Files identical despite different names*

### Comparing `microservicebus-py-0.9.0/src/msb_handler.py` & `microservicebus-py-0.9.1/src/msb_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,23 +129,29 @@
 
         packageInfo = self.get_package_info()
         await self.Debug("Package version: \033[95m" + packageInfo["version"] + "\033[0m")
         await self.Debug("Node id: \033[95m" + settings["nodeName"] + "\033[0m")
         await self.Debug("Organization id:\033[95m " + settings["organizationId"] + "\033[0m")
         await self.Debug("Mac addresses:\033[95m " + ':'.join(re.findall('..', '%012x' % uuid.getnode())) + "\033[0m")
 
+        ipAddresses = []
+        for interface, snics in psutil.net_if_addrs().items():
+            for snic in snics:
+                if snic.family == socket.AF_INET:
+                    ipAddresses.append(snic.address)
 
         hostData = {
             "id": "",
             "connectionId": "",
             "Name": settings["nodeName"],
             "machineName": socket.gethostname(),
             "OrganizationID": settings["organizationId"],
             "npmVersion": packageInfo["version"] ,
             "sas": settings["sas"],
+            "ipAddresses": ipAddresses,
             "recoveredSignIn": "False",
             "macAddresses": [':'.join(re.findall('..', '%012x' % uuid.getnode()))]
         }
 
         # Use for debugging
         #self.connection.send("signIn", [hostData])
         self.connection.send("signInAsync", [hostData])
@@ -352,15 +358,15 @@
         if os.path.isdir(self.service_path) == False:
             os.mkdir(self.service_path)
 
         state = self.settings["state"]
         asyncio.run(self.Debug(f"Node state {state}"))
         asyncio.run(self.SubmitAction("orchestrator", "_set_state", {"state": state}))
 
-        if sign_in_response['itineraries'] is not None:
+        if sign_in_response['itineraries'] is not None and state == "Active":
             for itinerary in sign_in_response['itineraries']:
                 pythonActivities = [srv for srv in itinerary["activities"]
                                     if "baseType" in srv["userData"] and srv["userData"]["baseType"] == 'pythonfile']
                 for pythonActivity in pythonActivities:
                     try:
                         host_config = [srv for srv in pythonActivity["userData"]
                                     ["config"]["generalConfig"] if srv["id"] == 'host']
```

### Comparing `microservicebus-py-0.9.0/src/orchestrator_service.py` & `microservicebus-py-0.9.1/src/orchestrator_service.py`

 * *Files identical despite different names*

### Comparing `microservicebus-py-0.9.0/src/rauc_handler.py` & `microservicebus-py-0.9.1/src/rauc_handler.py`

 * *Files identical despite different names*

### Comparing `microservicebus-py-0.9.0/src/start.py` & `microservicebus-py-0.9.1/src/start.py`

 * *Files identical despite different names*

### Comparing `microservicebus-py-0.9.0/src/terminal_service.py` & `microservicebus-py-0.9.1/src/terminal_service.py`

 * *Files identical despite different names*

### Comparing `microservicebus-py-0.9.0/src/test.py` & `microservicebus-py-0.9.1/src/test.py`

 * *Files identical despite different names*

### Comparing `microservicebus-py-0.9.0/src/vpn_helper.py` & `microservicebus-py-0.9.1/src/vpn_helper.py`

 * *Files identical despite different names*

