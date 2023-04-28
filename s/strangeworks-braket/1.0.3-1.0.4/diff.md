# Comparing `tmp/strangeworks_braket-1.0.3.tar.gz` & `tmp/strangeworks_braket-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strangeworks_braket-1.0.3.tar", max compression
+gzip compressed data, was "strangeworks_braket-1.0.4.tar", max compression
```

## Comparing `strangeworks_braket-1.0.3.tar` & `strangeworks_braket-1.0.4.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0      457 2023-04-25 15:47:32.936948 strangeworks_braket-1.0.3/DESCRIPTION.md
--rw-r--r--   0        0        0    11357 2023-04-25 15:47:32.936948 strangeworks_braket-1.0.3/LICENSE
--rw-r--r--   0        0        0     1317 2023-04-25 15:47:50.529147 strangeworks_braket-1.0.3/pyproject.toml
--rw-r--r--   0        0        0      232 2023-04-25 15:47:32.936948 strangeworks_braket-1.0.3/strangeworks_braket/__init__.py
--rw-r--r--   0        0        0     6022 2023-04-25 15:47:32.936948 strangeworks_braket-1.0.3/strangeworks_braket/device.py
--rw-r--r--   0        0        0    10889 2023-04-25 15:47:32.936948 strangeworks_braket-1.0.3/strangeworks_braket/task.py
--rw-r--r--   0        0        0      691 2023-04-25 15:47:32.936948 strangeworks_braket-1.0.3/strangeworks_braket/utils/serializer.py
--rw-r--r--   0        0        0     1207 1970-01-01 00:00:00.000000 strangeworks_braket-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0      457 2023-04-28 10:10:35.110807 strangeworks_braket-1.0.4/DESCRIPTION.md
+-rw-r--r--   0        0        0    11357 2023-04-28 10:10:35.110807 strangeworks_braket-1.0.4/LICENSE
+-rw-r--r--   0        0        0     1319 2023-04-28 10:10:52.122973 strangeworks_braket-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0      286 2023-04-28 10:10:35.114807 strangeworks_braket-1.0.4/strangeworks_braket/__init__.py
+-rw-r--r--   0        0        0     6794 2023-04-28 10:10:35.114807 strangeworks_braket-1.0.4/strangeworks_braket/device.py
+-rw-r--r--   0        0        0     8503 2023-04-28 10:10:35.114807 strangeworks_braket-1.0.4/strangeworks_braket/job.py
+-rw-r--r--   0        0        0    10889 2023-04-28 10:10:35.114807 strangeworks_braket-1.0.4/strangeworks_braket/task.py
+-rw-r--r--   0        0        0      691 2023-04-28 10:10:35.114807 strangeworks_braket-1.0.4/strangeworks_braket/utils/serializer.py
+-rw-r--r--   0        0        0     1260 1970-01-01 00:00:00.000000 strangeworks_braket-1.0.4/PKG-INFO
```

### Comparing `strangeworks_braket-1.0.3/LICENSE` & `strangeworks_braket-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `strangeworks_braket-1.0.3/pyproject.toml` & `strangeworks_braket-1.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "strangeworks-braket"
-version = "1.0.3"
+version = "1.0.4"
 description = "Strangeworks Braket SDK extension"
 readme = "DESCRIPTION.md"
 authors = ["Strange Devs <hello@strangeworks.com>"]
 license = "Apache-2.0"
 packages = [
     {include = "strangeworks_braket"},
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.9,<3.11"
+python = ">=3.9,<3.11.4"
 amazon-braket-sdk = "^1.31.1"
 strangeworks-python-core = "^0.1.6"
 python-jose = "^3.3.0"
 strangeworks = "^0.4.1"
 llvmlite = "0.39.1"
 strawberryfields = "^0.23.0"
```

### Comparing `strangeworks_braket-1.0.3/strangeworks_braket/device.py` & `strangeworks_braket-1.0.4/strangeworks_braket/device.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from __future__ import annotations
 
 import json
-from typing import Optional, Union
+from typing import Any, Dict, Optional, Union
 
 import strangeworks as sw
 from braket.annealing.problem import Problem
 from braket.aws.aws_device import Device
 from braket.circuits import Circuit
 from braket.device_schema import DeviceCapabilities
 from braket.ir.openqasm import Program as OpenQasmProgram
 from braket.tasks.quantum_task import QuantumTask
 
+from strangeworks_braket.job import StrangeworksQuantumJob
 from strangeworks_braket.task import StrangeworksQuantumTask
 from strangeworks_braket.utils.serializer import pickle_deserializer
 
 
 class StrangeworksDevice(Device):
     def __init__(
         self,
@@ -52,14 +53,38 @@
         task: QuantumTask (StrangeworksQuantumTask)
             The task that was run.
         """
         return StrangeworksQuantumTask.create(
             self.arn, task_specification, shots or 1000, *args, **kwargs
         )
 
+    def run_hybrid(
+        self,
+        filepath: str,
+        hyperparameters: Dict[str, Any],
+        *args,
+        **kwargs,
+    ) -> QuantumTask:
+        """Run a task on the device.
+        Parameters
+        ----------
+        filepath: str
+            Path to the python file that will be run.
+        hyperparameters: Dict[str, Any]
+            Dictionary of hyperparameters to pass to the task.
+            Must be json serializable.
+        Returns
+        -------
+        Job: QuantumJob (StrangeworksQuantumJob)
+            The job that was run.
+        """
+        return StrangeworksQuantumJob.create_hybrid(
+            self.arn, filepath, hyperparameters, *args, **kwargs
+        )
+
     @staticmethod
     def get_devices(
         arns: Optional[list[str]] = None,
         names: Optional[list[str]] = None,
         statuses: Optional[list[str]] = None,
     ) -> list[StrangeworksDevice]:
         """Get a list of devices.
```

### Comparing `strangeworks_braket-1.0.3/strangeworks_braket/task.py` & `strangeworks_braket-1.0.4/strangeworks_braket/task.py`

 * *Files identical despite different names*

### Comparing `strangeworks_braket-1.0.3/strangeworks_braket/utils/serializer.py` & `strangeworks_braket-1.0.4/strangeworks_braket/utils/serializer.py`

 * *Files identical despite different names*

### Comparing `strangeworks_braket-1.0.3/PKG-INFO` & `strangeworks_braket-1.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: strangeworks-braket
-Version: 1.0.3
+Version: 1.0.4
 Summary: Strangeworks Braket SDK extension
 License: Apache-2.0
 Author: Strange Devs
 Author-email: hello@strangeworks.com
-Requires-Python: >=3.9,<3.11
+Requires-Python: >=3.9,<3.11.4
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: amazon-braket-sdk (>=1.31.1,<2.0.0)
 Requires-Dist: llvmlite (==0.39.1)
 Requires-Dist: python-jose (>=3.3.0,<4.0.0)
 Requires-Dist: strangeworks (>=0.4.1,<0.5.0)
 Requires-Dist: strangeworks-python-core (>=0.1.6,<0.2.0)
 Requires-Dist: strawberryfields (>=0.23.0,<0.24.0)
 Description-Content-Type: text/markdown
```

