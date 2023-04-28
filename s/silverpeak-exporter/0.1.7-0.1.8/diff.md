# Comparing `tmp/silverpeak_exporter-0.1.7.tar.gz` & `tmp/silverpeak_exporter-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "silverpeak_exporter-0.1.7.tar", max compression
+gzip compressed data, was "silverpeak_exporter-0.1.8.tar", max compression
```

## Comparing `silverpeak_exporter-0.1.7.tar` & `silverpeak_exporter-0.1.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1067 2023-02-17 20:15:02.783372 silverpeak_exporter-0.1.7/LICENSE
--rw-r--r--   0        0        0     1957 2023-02-17 20:15:02.783372 silverpeak_exporter-0.1.7/README.md
--rw-r--r--   0        0        0      841 2023-02-17 20:15:02.791372 silverpeak_exporter-0.1.7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-17 20:15:02.791372 silverpeak_exporter-0.1.7/silverpeak_exporter/__init__.py
--rw-r--r--   0        0        0     2448 2023-02-17 20:15:02.791372 silverpeak_exporter-0.1.7/silverpeak_exporter/args.py
--rw-r--r--   0        0        0    22851 2023-02-17 20:15:02.791372 silverpeak_exporter-0.1.7/silverpeak_exporter/collectors.py
--rw-r--r--   0        0        0     4761 2023-02-17 20:15:02.791372 silverpeak_exporter-0.1.7/silverpeak_exporter/file.py
--rw-r--r--   0        0        0     1254 2023-02-17 20:15:02.791372 silverpeak_exporter-0.1.7/silverpeak_exporter/logger.py
--rw-r--r--   0        0        0     3048 2023-02-17 20:15:02.791372 silverpeak_exporter-0.1.7/silverpeak_exporter/main.py
--rw-r--r--   0        0        0     8642 2023-02-17 20:15:02.791372 silverpeak_exporter-0.1.7/silverpeak_exporter/metrics.py
--rw-r--r--   0        0        0     3092 2023-02-17 20:15:02.791372 silverpeak_exporter-0.1.7/silverpeak_exporter/utls.py
--rw-r--r--   0        0        0     2885 1970-01-01 00:00:00.000000 silverpeak_exporter-0.1.7/setup.py
--rw-r--r--   0        0        0     2672 1970-01-01 00:00:00.000000 silverpeak_exporter-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-28 19:32:57.750019 silverpeak_exporter-0.1.8/LICENSE
+-rw-r--r--   0        0        0     2039 2023-04-28 19:32:57.750019 silverpeak_exporter-0.1.8/README.md
+-rw-r--r--   0        0        0      841 2023-04-28 19:32:57.766019 silverpeak_exporter-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-28 19:32:57.766019 silverpeak_exporter-0.1.8/silverpeak_exporter/__init__.py
+-rw-r--r--   0        0        0     2448 2023-04-28 19:32:57.766019 silverpeak_exporter-0.1.8/silverpeak_exporter/args.py
+-rw-r--r--   0        0        0    23637 2023-04-28 19:32:57.766019 silverpeak_exporter-0.1.8/silverpeak_exporter/collectors.py
+-rw-r--r--   0        0        0     4761 2023-04-28 19:32:57.766019 silverpeak_exporter-0.1.8/silverpeak_exporter/file.py
+-rw-r--r--   0        0        0     1254 2023-04-28 19:32:57.766019 silverpeak_exporter-0.1.8/silverpeak_exporter/logger.py
+-rw-r--r--   0        0        0     3048 2023-04-28 19:32:57.766019 silverpeak_exporter-0.1.8/silverpeak_exporter/main.py
+-rw-r--r--   0        0        0     9156 2023-04-28 19:32:57.766019 silverpeak_exporter-0.1.8/silverpeak_exporter/metrics.py
+-rw-r--r--   0        0        0     3092 2023-04-28 19:32:57.766019 silverpeak_exporter-0.1.8/silverpeak_exporter/utls.py
+-rw-r--r--   0        0        0     2971 1970-01-01 00:00:00.000000 silverpeak_exporter-0.1.8/setup.py
+-rw-r--r--   0        0        0     2754 1970-01-01 00:00:00.000000 silverpeak_exporter-0.1.8/PKG-INFO
```

### Comparing `silverpeak_exporter-0.1.7/LICENSE` & `silverpeak_exporter-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `silverpeak_exporter-0.1.7/README.md` & `silverpeak_exporter-0.1.8/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,19 @@
 ![Open Issues](https://img.shields.io/github/issues/ipHeaders/silverpeak-prometheus)
 ![](https://img.shields.io/github/languages/top/ipHeaders/silverpeak-prometheus)
 ![](https://img.shields.io/pypi/pyversions/silverpeak-exporter)
 ![Docker Pulls](https://img.shields.io/docker/pulls/ipheaders/silverpeak-prometheus)
 [![Downloads](https://static.pepy.tech/personalized-badge/silverpeak-exporter?period=total&units=none&left_color=grey&right_color=orange&left_text=PyPI%20Downloads)](https://pepy.tech/project/silverpeak-exporter)
 
 # silverpeak-prometheus-exporter
-Silverpeak/Aruba SD-WAN Prometheus Exporter, this tool is to query the Silverpeak/Aruba SD-WAN orchestrator export the metrics to a prometheus database.
+Silverpeak/Aruba SD-WAN Prometheus Exporter, this tool is to query the Silverpeak/Aruba SD-WAN orchestrator export the metrics to a prometheus database. 
+
+```diff
+! For better security practices make sure the API key is read only.
+```
 
 ## Requierements
 
 - Orchestraor API Key
 - Python3.9>=
 
 ## Installation Methods
```

### Comparing `silverpeak_exporter-0.1.7/pyproject.toml` & `silverpeak_exporter-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "silverpeak_exporter"
-version = "0.1.7"
+version = "0.1.8"
 description = "Prometheus exporter for Silverpeak SD-WAN Appliances."
 authors = ["IP Headers <ipHeaders@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "silverpeak_exporter"}]
 
 [tool.poetry.scripts]
```

### Comparing `silverpeak_exporter-0.1.7/silverpeak_exporter/args.py` & `silverpeak_exporter-0.1.8/silverpeak_exporter/args.py`

 * *Files identical despite different names*

### Comparing `silverpeak_exporter-0.1.7/silverpeak_exporter/collectors.py` & `silverpeak_exporter-0.1.8/silverpeak_exporter/collectors.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,14 +71,20 @@
     @errorHandler
     def _getOrchServerBrief(self):
        orch_return = self.orch.get_orchestrator_server_info()   
        uptime.labels(orchName=self.hostname).info({'uptime' : orch_return['uptime']}) #Setting Metric
        release.labels(orchName=self.hostname).info({'release' : orch_return['release']}) #Setting Metric
        platform.labels(orchName=self.hostname).info({'platform' : orch_return['platform']}) #Setting Metric
        numActiveUsers.labels(orchName=self.hostname).set(orch_return['numActiveUsers']) #Setting Metric
+
+       if orch_return['platform'] != "DOCKER":
+           totalCPUs.labels(orchName=self.hostname).set(orch_return['numCpus']) #Setting Metric
+           loadAverage.labels(orchName=self.hostname).set(orch_return['loadAverage']) #Setting Metric
+           totalMemSize.labels(orchName=self.hostname).set(orch_return['memSize']) #Setting Metric
+       
        return orch_return
 
     @errorHandler
     def _getAlarmCountOrchestratoAndAppliances(self):
         orch_return = self.orch.get_alarm_count_orchestrator_and_appliances() 
         for key,value in orch_return.items():
             activeAlarms.labels(orchName=self.hostname,severity=key).set(value) #Setting Metric
@@ -169,14 +175,24 @@
 
     @errorHandler
     def _getTotalTunnelCount(self):
         orch_return = self.orch.get_total_tunnel_count()
         totalTunnelCount.labels(orchName=self.hostname).set(orch_return['totalTunnelCount'])
         return orch_return
 
+    @errorHandler
+    def _getAppliancesInMaintenance(self):
+        orch_return = self.orch.get_maintenance_mode_appliances()
+        supressAlarm = orch_return['suppressAlarm']
+        supressOrch = orch_return['pauseOrchestration']
+        
+        unique = supressAlarm + list(set(supressOrch) - set(supressAlarm))
+        maintenaceModeAppliances.labels(orchName=self.hostname).set(len(unique))
+        return orch_return
+    
 #--------------------------------------------------#
 # Metrics Collections for the Appliances
 #--------------------------------------------------#
 
 def applianceCollector(**kwargs):
     applianceName = kwargs['applianceName']
     ne_pk = kwargs['ne_pk']
@@ -441,15 +457,15 @@
             if self.Break == False:
                 wait(self.interval)
             else:
                 break
 
     @errorHandler
     def _getApplianceFlows(self):
-        orch_return = self.orch.get_appliance_flows(self.ne_pk,uptime="term5m")
+        orch_return = self.orch.get_appliance_flows(self.ne_pk, uptime="term5m")
 
         activeTotalFlows.labels(applianceName=self.applianceName).set(orch_return['active']['total_flows']) #Setting Metric
         activeStaleFlows.labels(applianceName=self.applianceName).set(orch_return['active']['stale_flows']) #Setting Metric
         activeInconsistentFlows.labels(applianceName=self.applianceName).set(orch_return['active']['inconsistent_flows']) #Setting Metric
         activeFlowsWithIssues.labels(applianceName=self.applianceName).set(orch_return['active']['flows_with_issues']) #Setting Metric
         activeFlowsOptimized.labels(applianceName=self.applianceName).set(orch_return['active']['flows_optimized']) #Setting Metric
         activeFlowsWithIgnores.labels(applianceName=self.applianceName).set(orch_return['active']['flows_with_ignores']) #Setting Metric
```

### Comparing `silverpeak_exporter-0.1.7/silverpeak_exporter/file.py` & `silverpeak_exporter-0.1.8/silverpeak_exporter/file.py`

 * *Files identical despite different names*

### Comparing `silverpeak_exporter-0.1.7/silverpeak_exporter/logger.py` & `silverpeak_exporter-0.1.8/silverpeak_exporter/logger.py`

 * *Files identical despite different names*

### Comparing `silverpeak_exporter-0.1.7/silverpeak_exporter/main.py` & `silverpeak_exporter-0.1.8/silverpeak_exporter/main.py`

 * *Files identical despite different names*

### Comparing `silverpeak_exporter-0.1.7/silverpeak_exporter/metrics.py` & `silverpeak_exporter-0.1.8/silverpeak_exporter/metrics.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,15 +32,18 @@
 totalRegions = Gauge('totalRegions', 'number of regions configured',['orchName'])
 totalSaasApps = Gauge('totalSaasApps', 'list of unique SaaS applications in the internet services database',['orchName'])
 totalAppDefinition = Gauge('totalAppDefinition', 'count for application definition data for Address Map from Cloud Portal',['orchName'])
 totalOrchSaasApps = Gauge('totalOrchSaasApps', 'count of internet services defined on Orchestrator',['orchName'])
 orchPortalStatus = Enum('orchPortalStatus', 'current connectivity status between Orchestrator and Cloud Portal',['orchName'], states=['unable to connect', 'connected', 'connecting'])
 cloudPortalServices = Gauge('cloudPortalServices', 'silverpeak cloud portal service and status',['orchName','portalService','status'])
 totalTunnelCount = Gauge('totalTunnelCount', 'get total tunnel count across all appliances',['orchName'])
-
+totalCPUs = Gauge('totalCPUs', 'the total amount of CPU on the orchestrator, works only when orch is not running in container',['orchName'])
+loadAverage = Gauge('loadAverage', 'orchestrator load average, works only when orch is not running in container',['orchName'])
+totalMemSize = Gauge('totalMemSize', 'total memory of the server, works only when orch is not running in container',['orchName'])
+maintenaceModeAppliances = Gauge('maintenacModeAppliances', 'appliances currently in maintenance mode',['orchName'])
 #---------#---------#---------#---------#---------#
 # Appliance Metrics
 #---------#---------#---------#---------#---------#
 applianceHostname = Info('applianceHostname', 'name of the silverpeak edge connect',['applianceName'])
 applianceModel = Info('applianceModel', 'mode of the silverpeak appliance',['applianceName'])
 appliancePlatform = Info('appliancePlatform', 'platform of the silverpeak appliance',['applianceName'])
 applianceUptime = Gauge('applianceUptime', 'uptime in milliseconds for the silverpeak appliance',['applianceName'])
```

### Comparing `silverpeak_exporter-0.1.7/silverpeak_exporter/utls.py` & `silverpeak_exporter-0.1.8/silverpeak_exporter/utls.py`

 * *Files identical despite different names*

### Comparing `silverpeak_exporter-0.1.7/setup.py` & `silverpeak_exporter-0.1.8/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,17 +15,17 @@
  'tomli==2.0.1']
 
 entry_points = \
 {'console_scripts': ['spexporter = silverpeak_exporter.main:main']}
 
 setup_kwargs = {
     'name': 'silverpeak-exporter',
-    'version': '0.1.7',
+    'version': '0.1.8',
     'description': 'Prometheus exporter for Silverpeak SD-WAN Appliances.',
-    'long_description': '![Release](https://img.shields.io/github/v/tag/ipHeaders/silverpeak-prometheus)\n![License](https://img.shields.io/github/license/ipHeaders/silverpeak-prometheus)\n![Open Issues](https://img.shields.io/github/issues/ipHeaders/silverpeak-prometheus)\n![](https://img.shields.io/github/languages/top/ipHeaders/silverpeak-prometheus)\n![](https://img.shields.io/pypi/pyversions/silverpeak-exporter)\n![Docker Pulls](https://img.shields.io/docker/pulls/ipheaders/silverpeak-prometheus)\n[![Downloads](https://static.pepy.tech/personalized-badge/silverpeak-exporter?period=total&units=none&left_color=grey&right_color=orange&left_text=PyPI%20Downloads)](https://pepy.tech/project/silverpeak-exporter)\n\n# silverpeak-prometheus-exporter\nSilverpeak/Aruba SD-WAN Prometheus Exporter, this tool is to query the Silverpeak/Aruba SD-WAN orchestrator export the metrics to a prometheus database.\n\n## Requierements\n\n- Orchestraor API Key\n- Python3.9>=\n\n## Installation Methods\n- Installing using [Pypi](https://github.com/ipHeaders/silverpeak-prometheus/tree/main/docs/installing_using_pypi.md)\n- Installing directly from [Github](https://github.com/ipHeaders/silverpeak-prometheus/tree/main/docs/installing_from_github.md)\n- Running on [Container](https://github.com/ipHeaders/silverpeak-prometheus/tree/main/docs/running_on_container.md)\n\n## References\n- Avaiable Exposed Metrics [Metrics](https://github.com/ipHeaders/silverpeak-prometheus/tree/main/docs/metrics.md)\n- DockerHub Project [Docker](https://hub.docker.com/r/ipheaders/silverpeak-prometheus)\n- Grafana Dashboard [Grafana](https://grafana.com/grafana/dashboards/17745-spexporter/)\n- Application Flow [Flow](https://github.com/ipHeaders/silverpeak-prometheus/tree/main/docs/appflow.png)\n\n## Grafana Example\n### Orchestrator\n![alt text](docs/grafana_orch.png)\n\n### Appliances\n![alt text](docs/grafana_appliace.png)\n\n### BGP\n![alt text](docs/grafana_bgp.png)\n\n## Maintainer\n[IPheaders](https://github.com/ipHeaders)\n',
+    'long_description': '![Release](https://img.shields.io/github/v/tag/ipHeaders/silverpeak-prometheus)\n![License](https://img.shields.io/github/license/ipHeaders/silverpeak-prometheus)\n![Open Issues](https://img.shields.io/github/issues/ipHeaders/silverpeak-prometheus)\n![](https://img.shields.io/github/languages/top/ipHeaders/silverpeak-prometheus)\n![](https://img.shields.io/pypi/pyversions/silverpeak-exporter)\n![Docker Pulls](https://img.shields.io/docker/pulls/ipheaders/silverpeak-prometheus)\n[![Downloads](https://static.pepy.tech/personalized-badge/silverpeak-exporter?period=total&units=none&left_color=grey&right_color=orange&left_text=PyPI%20Downloads)](https://pepy.tech/project/silverpeak-exporter)\n\n# silverpeak-prometheus-exporter\nSilverpeak/Aruba SD-WAN Prometheus Exporter, this tool is to query the Silverpeak/Aruba SD-WAN orchestrator export the metrics to a prometheus database. \n\n```diff\n! For better security practices make sure the API key is read only.\n```\n\n## Requierements\n\n- Orchestraor API Key\n- Python3.9>=\n\n## Installation Methods\n- Installing using [Pypi](https://github.com/ipHeaders/silverpeak-prometheus/tree/main/docs/installing_using_pypi.md)\n- Installing directly from [Github](https://github.com/ipHeaders/silverpeak-prometheus/tree/main/docs/installing_from_github.md)\n- Running on [Container](https://github.com/ipHeaders/silverpeak-prometheus/tree/main/docs/running_on_container.md)\n\n## References\n- Avaiable Exposed Metrics [Metrics](https://github.com/ipHeaders/silverpeak-prometheus/tree/main/docs/metrics.md)\n- DockerHub Project [Docker](https://hub.docker.com/r/ipheaders/silverpeak-prometheus)\n- Grafana Dashboard [Grafana](https://grafana.com/grafana/dashboards/17745-spexporter/)\n- Application Flow [Flow](https://github.com/ipHeaders/silverpeak-prometheus/tree/main/docs/appflow.png)\n\n## Grafana Example\n### Orchestrator\n![alt text](docs/grafana_orch.png)\n\n### Appliances\n![alt text](docs/grafana_appliace.png)\n\n### BGP\n![alt text](docs/grafana_bgp.png)\n\n## Maintainer\n[IPheaders](https://github.com/ipHeaders)\n',
     'author': 'IP Headers',
     'author_email': 'ipHeaders@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `silverpeak_exporter-0.1.7/PKG-INFO` & `silverpeak_exporter-0.1.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: silverpeak-exporter
-Version: 0.1.7
+Version: 0.1.8
 Summary: Prometheus exporter for Silverpeak SD-WAN Appliances.
 License: MIT
 Author: IP Headers
 Author-email: ipHeaders@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -23,15 +23,19 @@
 ![Open Issues](https://img.shields.io/github/issues/ipHeaders/silverpeak-prometheus)
 ![](https://img.shields.io/github/languages/top/ipHeaders/silverpeak-prometheus)
 ![](https://img.shields.io/pypi/pyversions/silverpeak-exporter)
 ![Docker Pulls](https://img.shields.io/docker/pulls/ipheaders/silverpeak-prometheus)
 [![Downloads](https://static.pepy.tech/personalized-badge/silverpeak-exporter?period=total&units=none&left_color=grey&right_color=orange&left_text=PyPI%20Downloads)](https://pepy.tech/project/silverpeak-exporter)
 
 # silverpeak-prometheus-exporter
-Silverpeak/Aruba SD-WAN Prometheus Exporter, this tool is to query the Silverpeak/Aruba SD-WAN orchestrator export the metrics to a prometheus database.
+Silverpeak/Aruba SD-WAN Prometheus Exporter, this tool is to query the Silverpeak/Aruba SD-WAN orchestrator export the metrics to a prometheus database. 
+
+```diff
+! For better security practices make sure the API key is read only.
+```
 
 ## Requierements
 
 - Orchestraor API Key
 - Python3.9>=
 
 ## Installation Methods
```

