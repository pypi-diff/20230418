# Comparing `tmp/strangeworks_braket-1.0.0.tar.gz` & `tmp/strangeworks_braket-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strangeworks_braket-1.0.0.tar", max compression
+gzip compressed data, was "strangeworks_braket-1.0.1.tar", max compression
```

## Comparing `strangeworks_braket-1.0.0.tar` & `strangeworks_braket-1.0.1.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0      457 2023-03-15 14:39:14.438242 strangeworks_braket-1.0.0/DESCRIPTION.md
--rw-r--r--   0        0        0    11357 2023-03-15 14:39:14.438242 strangeworks_braket-1.0.0/LICENSE
--rw-r--r--   0        0        0     1216 2023-03-15 14:39:30.326238 strangeworks_braket-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      233 2023-03-15 14:39:14.438242 strangeworks_braket-1.0.0/strangeworks_braket/__init__.py
--rw-r--r--   0        0        0     2789 2023-03-15 14:39:14.438242 strangeworks_braket-1.0.0/strangeworks_braket/device.py
--rw-r--r--   0        0        0     9745 2023-03-15 14:39:14.438242 strangeworks_braket-1.0.0/strangeworks_braket/task.py
--rw-r--r--   0        0        0     1127 1970-01-01 00:00:00.000000 strangeworks_braket-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      457 2023-04-18 14:26:23.303558 strangeworks_braket-1.0.1/DESCRIPTION.md
+-rw-r--r--   0        0        0    11357 2023-04-18 14:26:23.303558 strangeworks_braket-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1261 2023-04-18 14:26:36.599722 strangeworks_braket-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      232 2023-04-18 14:26:23.307558 strangeworks_braket-1.0.1/strangeworks_braket/__init__.py
+-rw-r--r--   0        0        0     3228 2023-04-18 14:26:23.307558 strangeworks_braket-1.0.1/strangeworks_braket/device.py
+-rw-r--r--   0        0        0    10213 2023-04-18 14:26:23.307558 strangeworks_braket-1.0.1/strangeworks_braket/task.py
+-rw-r--r--   0        0        0      691 2023-04-18 14:26:23.307558 strangeworks_braket-1.0.1/strangeworks_braket/utils/serializer.py
+-rw-r--r--   0        0        0     1171 1970-01-01 00:00:00.000000 strangeworks_braket-1.0.1/PKG-INFO
```

### Comparing `strangeworks_braket-1.0.0/LICENSE` & `strangeworks_braket-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `strangeworks_braket-1.0.0/pyproject.toml` & `strangeworks_braket-1.0.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 [tool.poetry]
 name = "strangeworks-braket"
-version = "1.0.0"
+version = "1.0.1"
 description = "Strangeworks Braket SDK extension"
 readme = "DESCRIPTION.md"
 authors = ["Strange Devs <hello@strangeworks.com>"]
 license = "Apache-2.0"
 packages = [
     {include = "strangeworks_braket"},
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-strangeworks = "^0.4.0"
 amazon-braket-sdk = "^1.31.1"
 strangeworks-python-core = "^0.1.6"
+python-jose = "^3.3.0"
+strangeworks = "^0.4.1"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.1.0"
 pytest = "^7.0.1"
 Flake8-pyproject = "^1.1.0"
 mdformat = "^0.7.14"
 mdformat-black = "^0.1.1"
 pre-commit = "^2.20.0"
 isort = "^5.11.4"
 python-dotenv = "^0.21.0"
+ipykernel = "^6.22.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "setuptools", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
```

### Comparing `strangeworks_braket-1.0.0/strangeworks_braket/device.py` & `strangeworks_braket-1.0.1/strangeworks_braket/device.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 from __future__ import annotations
 
+import json
 from typing import Optional, Union
 
 import strangeworks as sw
 from braket.annealing.problem import Problem
 from braket.aws.aws_device import Device
 from braket.circuits import Circuit
+from braket.device_schema import DeviceCapabilities
 from braket.ir.openqasm import Program as OpenQasmProgram
 from braket.tasks.quantum_task import QuantumTask
 
 from strangeworks_braket.task import StrangeworksQuantumTask
+from strangeworks_braket.utils.serializer import pickle_deserializer
 
 
 class StrangeworksDevice(Device):
     def __init__(
         self,
         arn: str,
         name: Optional[str] = None,
@@ -29,22 +32,20 @@
         self,
         task_specification: Union[Circuit, Problem, OpenQasmProgram],
         shots: Optional[int],
         *args,
         **kwargs,
     ) -> QuantumTask:
         """Run a task on the device.
-
         Parameters
         ----------
         task_specification: Union[Circuit, Problem, OpenQasmProgram]
             The task specification.
         shots: Optional[int]
             The number of shots to run the task for. Defaults to 1000.
-
         Returns
         -------
         task: QuantumTask (StrangeworksQuantumTask)
             The task that was run.
         """
         return StrangeworksQuantumTask.create(
             self.arn, task_specification, shots or 1000, *args, **kwargs
@@ -53,24 +54,22 @@
     @staticmethod
     def get_devices(
         arns: Optional[list[str]] = None,
         names: Optional[list[str]] = None,
         statuses: Optional[list[str]] = None,
     ) -> list[StrangeworksDevice]:
         """Get a list of devices.
-
         Parameters
         ----------
         arns: Optional[list[str]
             Filter by list of device ARNs. Defaults to None.
         names: Optional[list[str]]
             Filter by list of device names. Defaults to None.
         statuses: Optional[list[str]]
             Filter by list of device statuses. Defaults to None.
-
         Returns
         -------
         devices: list[SwDevice]
             List of devices that match the provided filters.
         """
         backends = sw.backends(product_slugs=["amazon-braket"])
         devices = []
@@ -88,7 +87,18 @@
                     backend.name,
                     backend.remote_status,
                     backend.slug,
                 )
             )
 
         return devices
+
+    def get_properties(self) -> DeviceCapabilities:
+
+        payload = {
+            "aws_device_arn": self.arn,
+        }
+
+        res = sw.execute_post(
+            StrangeworksQuantumTask._product_slug, payload, "properties"
+        )
+        self.properties = pickle_deserializer(json.loads(res), "json")
```

### Comparing `strangeworks_braket-1.0.0/strangeworks_braket/task.py` & `strangeworks_braket-1.0.1/strangeworks_braket/task.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,25 +3,28 @@
 import asyncio
 import json
 import time
 from functools import singledispatch
 from typing import Any, Dict, Optional, Tuple, Union
 
 import strangeworks as sw
+from braket.ahs.analog_hamiltonian_simulation import AnalogHamiltonianSimulation
 from braket.annealing.problem import Problem
 from braket.circuits import Circuit
 from braket.circuits.serialization import IRType
 from braket.ir.openqasm import Program as OpenQasmProgram
 from braket.schema_common import BraketSchemaBase
 from braket.tasks.annealing_quantum_task_result import AnnealingQuantumTaskResult
 from braket.tasks.gate_model_quantum_task_result import GateModelQuantumTaskResult
 from braket.tasks.quantum_task import QuantumTask
 from strangeworks_core.errors.error import StrangeworksError
 from strangeworks_core.types.job import Job, Status
 
+from strangeworks_braket.utils.serializer import pickle_serializer
+
 
 class StrangeworksQuantumTask(QuantumTask):
     _product_slug = "amazon-braket"
 
     def __init__(self, job: Job, *args, **kwargs):
         self.job: Job = job
 
@@ -251,15 +254,17 @@
 
         remix = {to_camel_case(key): value for key, value in d.items()}
         return Job.from_dict(remix)
 
 
 @singledispatch
 def _sw_task_specification(
-    task_specification: Union[Circuit, Problem, OpenQasmProgram]
+    task_specification: Union[
+        Circuit, Problem, OpenQasmProgram, AnalogHamiltonianSimulation
+    ]
 ) -> Tuple[str, str]:
     raise NotImplementedError
 
 
 # register a function for each type
 @_sw_task_specification.register
 def _sw_task_specification_circuit(task_specification: Circuit) -> Tuple[str, str]:
@@ -272,7 +277,15 @@
 
 
 @_sw_task_specification.register
 def _sw_task_specification_openqasm(
     task_specification: OpenQasmProgram,
 ) -> Tuple[str, str]:
     return "qasm", task_specification.json()
+
+
+@_sw_task_specification.register
+def _sw_task_specification_aquila(
+    task_specification: AnalogHamiltonianSimulation,
+) -> Tuple[str, str]:
+    task_new_specification = json.dumps(pickle_serializer(task_specification, "json"))
+    return "aquila", task_new_specification
```

### Comparing `strangeworks_braket-1.0.0/PKG-INFO` & `strangeworks_braket-1.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: strangeworks-braket
-Version: 1.0.0
+Version: 1.0.1
 Summary: Strangeworks Braket SDK extension
 License: Apache-2.0
 Author: Strange Devs
 Author-email: hello@strangeworks.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: amazon-braket-sdk (>=1.31.1,<2.0.0)
-Requires-Dist: strangeworks (>=0.4.0,<0.5.0)
+Requires-Dist: python-jose (>=3.3.0,<4.0.0)
+Requires-Dist: strangeworks (>=0.4.1,<0.5.0)
 Requires-Dist: strangeworks-python-core (>=0.1.6,<0.2.0)
 Description-Content-Type: text/markdown
 
 | ⚠️ | This SDK is currently in pre-release alpha state and subject to change. To get
 more info or access to test features check out the
 [Strangeworks Backstage Pass Program](https://strangeworks.com/backstage). |
 |---------------|:------------------------|
```

