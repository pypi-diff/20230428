# Comparing `tmp/prefect-kubernetes-0.2.5.tar.gz` & `tmp/prefect-kubernetes-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/prefect-kubernetes/prefect-kubernetes/dist/.tmp-r8p0z9xb/prefect-kubernetes-0.2.5.tar", last modified: Fri Apr 21 00:03:22 2023, max compression
+gzip compressed data, was "/home/runner/work/prefect-kubernetes/prefect-kubernetes/dist/.tmp-6rqdzdp5/prefect-kubernetes-0.2.6.tar", last modified: Fri Apr 28 14:47:52 2023, max compression
```

## Comparing `prefect-kubernetes-0.2.5.tar` & `prefect-kubernetes-0.2.6.tar`

### file list

```diff
@@ -1,41 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:03:22.000000 prefect-kubernetes-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-04-21 00:02:01.000000 prefect-kubernetes-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-21 00:02:01.000000 prefect-kubernetes-0.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-04-21 00:03:22.000000 prefect-kubernetes-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-04-21 00:02:01.000000 prefect-kubernetes-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:03:22.000000 prefect-kubernetes-0.2.5/prefect_kubernetes/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-21 00:02:01.000000 prefect-kubernetes-0.2.5/prefect_kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-21 00:03:22.000000 prefect-kubernetes-0.2.5/prefect_kubernetes/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-04-21 00:02:01.000000 prefect-kubernetes-0.2.5/prefect_kubernetes/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)    15378 2023-04-21 00:02:01.000000 prefect-kubernetes-0.2.5/prefect_kubernetes/custom_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-04-21 00:02:01.000000 prefect-kubernetes-0.2.5/prefect_kubernetes/deployments.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-21 00:02:01.000000 prefect-kubernetes-0.2.5/prefect_kubernetes/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-21 00:02:01.000000 prefect-kubernetes-0.2.5/prefect_kubernetes/flows.py
--rw-r--r--   0 runner    (1001) docker     (123)    19500 2023-04-21 00:02:01.000000 prefect-kubernetes-0.2.5/prefect_kubernetes/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12076 2023-04-21 00:02:01.000000 prefect-kubernetes-0.2.5/prefect_kubernetes/pods.py
--rw-r--r--   0 runner    (1001) docker     (123)     9722 2023-04-21 00:02:01.000000 prefect-kubernetes-0.2.5/prefect_kubernetes/services.py
--rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-04-21 00:02:01.000000 prefect-kubernetes-0.2.5/prefect_kubernetes/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    31472 2023-04-21 00:02:01.000000 prefect-kubernetes-0.2.5/prefect_kubernetes/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:03:22.000000 prefect-kubernetes-0.2.5/prefect_kubernetes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-04-21 00:03:22.000000 prefect-kubernetes-0.2.5/prefect_kubernetes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-21 00:03:22.000000 prefect-kubernetes-0.2.5/prefect_kubernetes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 00:03:22.000000 prefect-kubernetes-0.2.5/prefect_kubernetes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-21 00:03:22.000000 prefect-kubernetes-0.2.5/prefect_kubernetes.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-21 00:03:22.000000 prefect-kubernetes-0.2.5/prefect_kubernetes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-21 00:03:22.000000 prefect-kubernetes-0.2.5/prefect_kubernetes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-21 00:02:01.000000 prefect-kubernetes-0.2.5/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-21 00:02:01.000000 prefect-kubernetes-0.2.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-21 00:03:22.000000 prefect-kubernetes-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-04-21 00:02:01.000000 prefect-kubernetes-0.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 00:03:22.000000 prefect-kubernetes-0.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-21 00:02:01.000000 prefect-kubernetes-0.2.5/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-21 00:02:01.000000 prefect-kubernetes-0.2.5/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     9652 2023-04-21 00:02:01.000000 prefect-kubernetes-0.2.5/tests/test_custom_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-04-21 00:02:01.000000 prefect-kubernetes-0.2.5/tests/test_deployments.py
--rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-04-21 00:02:01.000000 prefect-kubernetes-0.2.5/tests/test_flows.py
--rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-04-21 00:02:01.000000 prefect-kubernetes-0.2.5/tests/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6775 2023-04-21 00:02:01.000000 prefect-kubernetes-0.2.5/tests/test_pods.py
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-04-21 00:02:01.000000 prefect-kubernetes-0.2.5/tests/test_services.py
--rw-r--r--   0 runner    (1001) docker     (123)     6751 2023-04-21 00:02:01.000000 prefect-kubernetes-0.2.5/tests/test_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    77561 2023-04-21 00:02:01.000000 prefect-kubernetes-0.2.5/tests/test_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-04-21 00:02:01.000000 prefect-kubernetes-0.2.5/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:47:52.000000 prefect-kubernetes-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-04-28 14:46:03.000000 prefect-kubernetes-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-28 14:46:03.000000 prefect-kubernetes-0.2.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-04-28 14:47:52.000000 prefect-kubernetes-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-04-28 14:46:03.000000 prefect-kubernetes-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:47:52.000000 prefect-kubernetes-0.2.6/prefect_kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-28 14:46:03.000000 prefect-kubernetes-0.2.6/prefect_kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 14:47:52.000000 prefect-kubernetes-0.2.6/prefect_kubernetes/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-04-28 14:46:03.000000 prefect-kubernetes-0.2.6/prefect_kubernetes/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15378 2023-04-28 14:46:03.000000 prefect-kubernetes-0.2.6/prefect_kubernetes/custom_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-04-28 14:46:03.000000 prefect-kubernetes-0.2.6/prefect_kubernetes/deployments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-28 14:46:03.000000 prefect-kubernetes-0.2.6/prefect_kubernetes/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-28 14:46:03.000000 prefect-kubernetes-0.2.6/prefect_kubernetes/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-28 14:46:03.000000 prefect-kubernetes-0.2.6/prefect_kubernetes/flows.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19500 2023-04-28 14:46:03.000000 prefect-kubernetes-0.2.6/prefect_kubernetes/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12076 2023-04-28 14:46:03.000000 prefect-kubernetes-0.2.6/prefect_kubernetes/pods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9722 2023-04-28 14:46:03.000000 prefect-kubernetes-0.2.6/prefect_kubernetes/services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-04-28 14:46:03.000000 prefect-kubernetes-0.2.6/prefect_kubernetes/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32697 2023-04-28 14:46:03.000000 prefect-kubernetes-0.2.6/prefect_kubernetes/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:47:52.000000 prefect-kubernetes-0.2.6/prefect_kubernetes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-04-28 14:47:52.000000 prefect-kubernetes-0.2.6/prefect_kubernetes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-28 14:47:52.000000 prefect-kubernetes-0.2.6/prefect_kubernetes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 14:47:52.000000 prefect-kubernetes-0.2.6/prefect_kubernetes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-28 14:47:52.000000 prefect-kubernetes-0.2.6/prefect_kubernetes.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-28 14:47:52.000000 prefect-kubernetes-0.2.6/prefect_kubernetes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-28 14:47:52.000000 prefect-kubernetes-0.2.6/prefect_kubernetes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-28 14:46:03.000000 prefect-kubernetes-0.2.6/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-28 14:46:03.000000 prefect-kubernetes-0.2.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-28 14:47:52.000000 prefect-kubernetes-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-04-28 14:46:03.000000 prefect-kubernetes-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 14:47:52.000000 prefect-kubernetes-0.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-28 14:46:03.000000 prefect-kubernetes-0.2.6/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-28 14:46:03.000000 prefect-kubernetes-0.2.6/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9652 2023-04-28 14:46:03.000000 prefect-kubernetes-0.2.6/tests/test_custom_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-04-28 14:46:03.000000 prefect-kubernetes-0.2.6/tests/test_deployments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14069 2023-04-28 14:46:03.000000 prefect-kubernetes-0.2.6/tests/test_events_replicator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-04-28 14:46:03.000000 prefect-kubernetes-0.2.6/tests/test_flows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-04-28 14:46:03.000000 prefect-kubernetes-0.2.6/tests/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6775 2023-04-28 14:46:03.000000 prefect-kubernetes-0.2.6/tests/test_pods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-04-28 14:46:03.000000 prefect-kubernetes-0.2.6/tests/test_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6751 2023-04-28 14:46:03.000000 prefect-kubernetes-0.2.6/tests/test_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77624 2023-04-28 14:46:03.000000 prefect-kubernetes-0.2.6/tests/test_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-04-28 14:46:03.000000 prefect-kubernetes-0.2.6/versioneer.py
```

### Comparing `prefect-kubernetes-0.2.5/LICENSE` & `prefect-kubernetes-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.5/PKG-INFO` & `prefect-kubernetes-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-kubernetes
-Version: 0.2.5
+Version: 0.2.6
 Summary: Prefect integrations for interacting with Kubernetes.
 Home-page: https://github.com/PrefectHQ/prefect-kubernetes
 Author: Prefect Technologies, Inc.
 Author-email: help@prefect.io
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
```

### Comparing `prefect-kubernetes-0.2.5/README.md` & `prefect-kubernetes-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.5/prefect_kubernetes/credentials.py` & `prefect-kubernetes-0.2.6/prefect_kubernetes/credentials.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.5/prefect_kubernetes/custom_objects.py` & `prefect-kubernetes-0.2.6/prefect_kubernetes/custom_objects.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.5/prefect_kubernetes/deployments.py` & `prefect-kubernetes-0.2.6/prefect_kubernetes/deployments.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.5/prefect_kubernetes/exceptions.py` & `prefect-kubernetes-0.2.6/prefect_kubernetes/exceptions.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.5/prefect_kubernetes/flows.py` & `prefect-kubernetes-0.2.6/prefect_kubernetes/flows.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.5/prefect_kubernetes/jobs.py` & `prefect-kubernetes-0.2.6/prefect_kubernetes/jobs.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.5/prefect_kubernetes/pods.py` & `prefect-kubernetes-0.2.6/prefect_kubernetes/pods.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.5/prefect_kubernetes/services.py` & `prefect-kubernetes-0.2.6/prefect_kubernetes/services.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.5/prefect_kubernetes/utilities.py` & `prefect-kubernetes-0.2.6/prefect_kubernetes/utilities.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.5/prefect_kubernetes/worker.py` & `prefect-kubernetes-0.2.6/prefect_kubernetes/worker.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,19 +88,21 @@
 checkout out the [Prefect docs](https://docs.prefect.io/concepts/work-pools/).
 """
 import enum
 import math
 import os
 import time
 from contextlib import contextmanager
-from typing import TYPE_CHECKING, Any, Dict, Generator, Optional, Tuple
+from typing import TYPE_CHECKING, Any, Dict, Generator, List, Optional, Tuple
 
 import anyio.abc
 from prefect.blocks.kubernetes import KubernetesClusterConfig
 from prefect.docker import get_prefect_image_name
+from prefect.events import RelatedResource
+from prefect.events.related import object_as_related_resource, tags_as_related_resources
 from prefect.exceptions import InfrastructureNotAvailable, InfrastructureNotFound
 from prefect.server.schemas.core import Flow
 from prefect.server.schemas.responses import DeploymentResponse
 from prefect.utilities.asyncutils import run_sync_in_worker_thread
 from prefect.utilities.importtools import lazy_import
 from prefect.utilities.pydantic import JsonPatch
 from prefect.utilities.templating import find_placeholders
@@ -109,28 +111,29 @@
     BaseVariables,
     BaseWorker,
     BaseWorkerResult,
 )
 from pydantic import Field, validator
 from typing_extensions import Literal
 
+from prefect_kubernetes.events import KubernetesEventsReplicator
 from prefect_kubernetes.utilities import (
     _slugify_label_key,
     _slugify_label_value,
     _slugify_name,
 )
 
 if TYPE_CHECKING:
     import kubernetes
     import kubernetes.client
     import kubernetes.client.exceptions
     import kubernetes.config
+    import kubernetes.watch
     from kubernetes.client import ApiClient, BatchV1Api, CoreV1Api, V1Job, V1Pod
     from prefect.client.schemas import FlowRun
-
 else:
     kubernetes = lazy_import("kubernetes")
 
 
 def _get_default_job_manifest_template() -> Dict[str, Any]:
     """Returns the default job manifest template used by the Kubernetes worker."""
     return {
@@ -388,14 +391,29 @@
             if self.name:
                 generate_name = _slugify_name(self.name)
             # _slugify_name will return None if the slugified name in an exception
             if not generate_name:
                 generate_name = "prefect-job"
             self.job_manifest["metadata"]["generateName"] = f"{generate_name}-"
 
+    def _related_resources(self) -> List[RelatedResource]:
+        tags = set()
+        related = []
+
+        for kind, obj in self._related_objects.items():
+            # TODO: Remove this method once we've updated the Prefect core side
+            # to ignore objects that are None.
+            if not obj:
+                continue
+            if hasattr(obj, "tags"):
+                tags.update(obj.tags)
+            related.append(object_as_related_resource(kind=kind, role=kind, object=obj))
+
+        return related + tags_as_related_resources(tags)
+
 
 class KubernetesWorkerVariables(BaseVariables):
     """
     Default variables for the Kubernetes worker.
 
     The schema for this class is used to populate the `variables` section of the default
     base job template.
@@ -487,17 +505,29 @@
                 self._get_infrastructure_pid, job, client
             )
             # Indicate that the job has started
             if task_status is not None:
                 task_status.started(pid)
 
             # Monitor the job until completion
-            status_code = await run_sync_in_worker_thread(
-                self._watch_job, job.metadata.name, configuration, client
+
+            events_replicator = KubernetesEventsReplicator(
+                client=client,
+                job_name=job.metadata.name,
+                namespace=configuration.namespace,
+                worker_resource=self._event_resource(),
+                related_resources=self._event_related_resources(
+                    configuration=configuration
+                ),
             )
+
+            with events_replicator:
+                status_code = await run_sync_in_worker_thread(
+                    self._watch_job, job.metadata.name, configuration, client
+                )
             return KubernetesWorkerResult(identifier=pid, status_code=status_code)
 
     async def kill_infrastructure(
         self,
         infrastructure_pid: str,
         configuration: KubernetesWorkerJobConfiguration,
         grace_seconds: int = 30,
```

### Comparing `prefect-kubernetes-0.2.5/prefect_kubernetes.egg-info/PKG-INFO` & `prefect-kubernetes-0.2.6/prefect_kubernetes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-kubernetes
-Version: 0.2.5
+Version: 0.2.6
 Summary: Prefect integrations for interacting with Kubernetes.
 Home-page: https://github.com/PrefectHQ/prefect-kubernetes
 Author: Prefect Technologies, Inc.
 Author-email: help@prefect.io
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
```

### Comparing `prefect-kubernetes-0.2.5/prefect_kubernetes.egg-info/SOURCES.txt` & `prefect-kubernetes-0.2.6/prefect_kubernetes.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 setup.py
 versioneer.py
 prefect_kubernetes/__init__.py
 prefect_kubernetes/_version.py
 prefect_kubernetes/credentials.py
 prefect_kubernetes/custom_objects.py
 prefect_kubernetes/deployments.py
+prefect_kubernetes/events.py
 prefect_kubernetes/exceptions.py
 prefect_kubernetes/flows.py
 prefect_kubernetes/jobs.py
 prefect_kubernetes/pods.py
 prefect_kubernetes/services.py
 prefect_kubernetes/utilities.py
 prefect_kubernetes/worker.py
@@ -24,13 +25,14 @@
 prefect_kubernetes.egg-info/entry_points.txt
 prefect_kubernetes.egg-info/requires.txt
 prefect_kubernetes.egg-info/top_level.txt
 tests/test_block_standards.py
 tests/test_credentials.py
 tests/test_custom_objects.py
 tests/test_deployments.py
+tests/test_events_replicator.py
 tests/test_flows.py
 tests/test_jobs.py
 tests/test_pods.py
 tests/test_services.py
 tests/test_utilities.py
 tests/test_worker.py
```

### Comparing `prefect-kubernetes-0.2.5/setup.cfg` & `prefect-kubernetes-0.2.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.5/setup.py` & `prefect-kubernetes-0.2.6/setup.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.5/tests/test_block_standards.py` & `prefect-kubernetes-0.2.6/tests/test_block_standards.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.5/tests/test_credentials.py` & `prefect-kubernetes-0.2.6/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.5/tests/test_custom_objects.py` & `prefect-kubernetes-0.2.6/tests/test_custom_objects.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.5/tests/test_deployments.py` & `prefect-kubernetes-0.2.6/tests/test_deployments.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.5/tests/test_flows.py` & `prefect-kubernetes-0.2.6/tests/test_flows.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.5/tests/test_jobs.py` & `prefect-kubernetes-0.2.6/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.5/tests/test_pods.py` & `prefect-kubernetes-0.2.6/tests/test_pods.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.5/tests/test_services.py` & `prefect-kubernetes-0.2.6/tests/test_services.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.5/tests/test_utilities.py` & `prefect-kubernetes-0.2.6/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `prefect-kubernetes-0.2.5/tests/test_worker.py` & `prefect-kubernetes-0.2.6/tests/test_worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,15 +123,18 @@
 def _mock_pods_stream_that_returns_running_pod(*args, **kwargs):
     job_pod = MagicMock(spec=kubernetes.client.V1Pod)
     job_pod.status.phase = "Running"
 
     job = MagicMock(spec=kubernetes.client.V1Job)
     job.status.completion_time = pendulum.now("utc").timestamp()
 
-    return [{"object": job_pod}, {"object": job}]
+    return [
+        {"object": job_pod, "type": "MODIFIED"},
+        {"object": job, "type": "MODIFIED"},
+    ]
 
 
 from_template_and_values_cases = [
     (
         # default base template with no values
         KubernetesWorker.get_default_base_job_template(),
         {},
```

### Comparing `prefect-kubernetes-0.2.5/versioneer.py` & `prefect-kubernetes-0.2.6/versioneer.py`

 * *Files identical despite different names*

