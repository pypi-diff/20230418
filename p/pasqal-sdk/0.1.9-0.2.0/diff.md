# Comparing `tmp/pasqal-sdk-0.1.9.tar.gz` & `tmp/pasqal-sdk-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pasqal-sdk-0.1.9.tar", last modified: Tue Feb  7 17:21:18 2023, max compression
+gzip compressed data, was "pasqal-sdk-0.2.0.tar", last modified: Tue Apr 18 16:44:48 2023, max compression
```

## Comparing `pasqal-sdk-0.1.9.tar` & `pasqal-sdk-0.2.0.tar`

### file list

```diff
@@ -1,38 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 17:21:18.829423 pasqal-sdk-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-02-07 17:21:06.000000 pasqal-sdk-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 17:21:06.000000 pasqal-sdk-0.1.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-02-07 17:21:18.829423 pasqal-sdk-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-02-07 17:21:06.000000 pasqal-sdk-0.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 17:21:18.825422 pasqal-sdk-0.1.9/pasqal_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-02-07 17:21:18.000000 pasqal-sdk-0.1.9/pasqal_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-02-07 17:21:18.000000 pasqal-sdk-0.1.9/pasqal_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-07 17:21:18.000000 pasqal-sdk-0.1.9/pasqal_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-02-07 17:21:18.000000 pasqal-sdk-0.1.9/pasqal_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-07 17:21:18.000000 pasqal-sdk-0.1.9/pasqal_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-02-07 17:21:06.000000 pasqal-sdk-0.1.9/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 17:21:18.829423 pasqal-sdk-0.1.9/sdk/
--rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-02-07 17:21:06.000000 pasqal-sdk-0.1.9/sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-02-07 17:21:06.000000 pasqal-sdk-0.1.9/sdk/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5007 2023-02-07 17:21:06.000000 pasqal-sdk-0.1.9/sdk/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-02-07 17:21:06.000000 pasqal-sdk-0.1.9/sdk/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 17:21:18.829423 pasqal-sdk-0.1.9/sdk/device/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 17:21:06.000000 pasqal-sdk-0.1.9/sdk/device/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 17:21:18.829423 pasqal-sdk-0.1.9/sdk/device/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-02-07 17:21:06.000000 pasqal-sdk-0.1.9/sdk/device/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-02-07 17:21:06.000000 pasqal-sdk-0.1.9/sdk/device/configuration/base_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-02-07 17:21:06.000000 pasqal-sdk-0.1.9/sdk/device/configuration/emu_free.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-02-07 17:21:06.000000 pasqal-sdk-0.1.9/sdk/device/configuration/emu_sv.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-02-07 17:21:06.000000 pasqal-sdk-0.1.9/sdk/device/device_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-02-07 17:21:06.000000 pasqal-sdk-0.1.9/sdk/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-02-07 17:21:06.000000 pasqal-sdk-0.1.9/sdk/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-02-07 17:21:06.000000 pasqal-sdk-0.1.9/sdk/job.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 17:21:06.000000 pasqal-sdk-0.1.9/sdk/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 17:21:18.829423 pasqal-sdk-0.1.9/sdk/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 17:21:06.000000 pasqal-sdk-0.1.9/sdk/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-02-07 17:21:06.000000 pasqal-sdk-0.1.9/sdk/utils/jsend.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-02-07 17:21:06.000000 pasqal-sdk-0.1.9/sdk/utils/strenum.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-02-07 17:21:18.829423 pasqal-sdk-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-02-07 17:21:06.000000 pasqal-sdk-0.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 17:21:18.829423 pasqal-sdk-0.1.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-02-07 17:21:06.000000 pasqal-sdk-0.1.9/tests/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-02-07 17:21:06.000000 pasqal-sdk-0.1.9/tests/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:44:48.526936 pasqal-sdk-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-18 16:44:39.000000 pasqal-sdk-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 16:44:39.000000 pasqal-sdk-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-04-18 16:44:48.526936 pasqal-sdk-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-04-18 16:44:39.000000 pasqal-sdk-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:44:48.518936 pasqal-sdk-0.2.0/pasqal_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-04-18 16:44:48.000000 pasqal-sdk-0.2.0/pasqal_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-18 16:44:48.000000 pasqal-sdk-0.2.0/pasqal_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 16:44:48.000000 pasqal-sdk-0.2.0/pasqal_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-18 16:44:48.000000 pasqal-sdk-0.2.0/pasqal_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-18 16:44:48.000000 pasqal-sdk-0.2.0/pasqal_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-18 16:44:39.000000 pasqal-sdk-0.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:44:48.522936 pasqal-sdk-0.2.0/sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-04-18 16:44:39.000000 pasqal-sdk-0.2.0/sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-18 16:44:39.000000 pasqal-sdk-0.2.0/sdk/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-04-18 16:44:39.000000 pasqal-sdk-0.2.0/sdk/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-04-18 16:44:39.000000 pasqal-sdk-0.2.0/sdk/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5914 2023-04-18 16:44:39.000000 pasqal-sdk-0.2.0/sdk/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:44:48.522936 pasqal-sdk-0.2.0/sdk/device/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-18 16:44:39.000000 pasqal-sdk-0.2.0/sdk/device/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:44:48.522936 pasqal-sdk-0.2.0/sdk/device/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-18 16:44:39.000000 pasqal-sdk-0.2.0/sdk/device/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-04-18 16:44:39.000000 pasqal-sdk-0.2.0/sdk/device/configuration/base_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-18 16:44:39.000000 pasqal-sdk-0.2.0/sdk/device/configuration/emu_free.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-18 16:44:39.000000 pasqal-sdk-0.2.0/sdk/device/configuration/emu_tn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-18 16:44:39.000000 pasqal-sdk-0.2.0/sdk/device/emulator_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-18 16:44:39.000000 pasqal-sdk-0.2.0/sdk/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-18 16:44:39.000000 pasqal-sdk-0.2.0/sdk/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-18 16:44:39.000000 pasqal-sdk-0.2.0/sdk/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 16:44:39.000000 pasqal-sdk-0.2.0/sdk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:44:48.522936 pasqal-sdk-0.2.0/sdk/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 16:44:39.000000 pasqal-sdk-0.2.0/sdk/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-18 16:44:39.000000 pasqal-sdk-0.2.0/sdk/utils/jsend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-18 16:44:39.000000 pasqal-sdk-0.2.0/sdk/utils/strenum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-18 16:44:48.526936 pasqal-sdk-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-04-18 16:44:39.000000 pasqal-sdk-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:44:48.522936 pasqal-sdk-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 16:44:39.000000 pasqal-sdk-0.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-18 16:44:39.000000 pasqal-sdk-0.2.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6145 2023-04-18 16:44:39.000000 pasqal-sdk-0.2.0/tests/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-04-18 16:44:39.000000 pasqal-sdk-0.2.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-04-18 16:44:39.000000 pasqal-sdk-0.2.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-18 16:44:39.000000 pasqal-sdk-0.2.0/tests/test_device_specs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:44:48.526936 pasqal-sdk-0.2.0/tests/test_doubles/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 16:44:39.000000 pasqal-sdk-0.2.0/tests/test_doubles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-18 16:44:39.000000 pasqal-sdk-0.2.0/tests/test_doubles/authentication.py
```

### Comparing `pasqal-sdk-0.1.9/LICENSE` & `pasqal-sdk-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pasqal-sdk-0.1.9/pasqal_sdk.egg-info/SOURCES.txt` & `pasqal-sdk-0.2.0/pasqal_sdk.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -7,24 +7,31 @@
 pasqal_sdk.egg-info/PKG-INFO
 pasqal_sdk.egg-info/SOURCES.txt
 pasqal_sdk.egg-info/dependency_links.txt
 pasqal_sdk.egg-info/requires.txt
 pasqal_sdk.egg-info/top_level.txt
 sdk/__init__.py
 sdk/_version.py
+sdk/authentication.py
 sdk/batch.py
 sdk/client.py
 sdk/endpoints.py
 sdk/errors.py
 sdk/job.py
 sdk/py.typed
 sdk/device/__init__.py
-sdk/device/device_types.py
+sdk/device/emulator_types.py
 sdk/device/configuration/__init__.py
 sdk/device/configuration/base_config.py
 sdk/device/configuration/emu_free.py
-sdk/device/configuration/emu_sv.py
+sdk/device/configuration/emu_tn.py
 sdk/utils/__init__.py
 sdk/utils/jsend.py
 sdk/utils/strenum.py
+tests/__init__.py
+tests/conftest.py
 tests/test_batch.py
-tests/test_config.py
+tests/test_client.py
+tests/test_config.py
+tests/test_device_specs.py
+tests/test_doubles/__init__.py
+tests/test_doubles/authentication.py
```

### Comparing `pasqal-sdk-0.1.9/sdk/__init__.py` & `pasqal-sdk-0.2.0/sdk/batch.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,117 +1,132 @@
-# Copyright 2020 Pasqal Cloud Services development team
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#    http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
 import time
-from typing import Any, Dict, List, Optional
+from dataclasses import dataclass, field
+from typing import Any, Dict, Optional, Type, Union
 
-from sdk.batch import Batch, RESULT_POLLING_INTERVAL
 from sdk.client import Client
-from sdk.endpoints import Endpoints
 from sdk.job import Job
-from sdk.device.configuration import BaseConfig
-from sdk.device.device_types import DeviceType
+from sdk.device.configuration import BaseConfig, EmuTNConfig, EmuFreeConfig
+from sdk.device import EmulatorType
+
+RESULT_POLLING_INTERVAL = 2  # seconds
 
 
-class SDK:
+@dataclass
+class Batch:
+    """Class for batch data.
+
+    A batch groups up several jobs with the same sequence. When a batch is assigned to
+    a QPU, all its jobs are ran sequentially and no other batch can be assigned to the
+    device until all its jobs are done and it is declared complete.
+
+    Attributes:
+        - complete: Whether the batch has been declared as complete.
+        - created_at: Timestamp of the creation of the batch.
+        - updated_at: Timestamps of the last update of the batch.
+        - device_type: Type of device to run the batch on.
+        - group_id: Id of the owner group of the batch.
+        - id: Unique identifier for the batch.
+        - user_id: Unique identifier of the user that created the batch.
+        - priority: Level of priority of the batch.
+        - status: Status of the batch.
+        - webhook: Webhook where the job results are automatically sent to.
+        - sequence_builder: Pulser sequence of the batch.
+        - start_datetime: Timestamp of the time the batch was sent to the QPU.
+        - end_datetime: Timestamp of when the  batch process was finished.
+        - device_status: Status of the device where the batch is running.
+        - jobs: Dictionary of all the jobs added to the batch.
+        - jobs_count: number of jobs added to the batch.
+        - jobs_count_per_status: number of jobs per status.
+        - configuration: Further configuration for certain emulators.
+
+    """
+
+    complete: bool
+    created_at: str
+    updated_at: str
+    device_type: str
+    group_id: str
+    id: str
+    user_id: int
+    priority: int
+    status: str
+    webhook: str
     _client: Client
+    sequence_builder: str
+    start_datetime: Optional[str] = None
+    end_datetime: Optional[str] = None
+    device_status: Optional[str] = None
+    jobs: Dict[str, Job] = field(default_factory=dict)
+    jobs_count: int = 0
+    jobs_count_per_status: Dict[str, int] = field(default_factory=dict)
+    configuration: Optional[Union[BaseConfig, dict]] = None
+
+    def __post_init__(self) -> None:
+        """Post init method to convert the configuration to a BaseConfig object."""
+        if not isinstance(self.configuration, dict):
+            return
+        conf_class: Type[BaseConfig] = BaseConfig
+        if self.device_type == EmulatorType.EMU_TN.value:
+            conf_class = EmuTNConfig
+        elif self.device_type == EmulatorType.EMU_FREE.value:
+            conf_class = EmuFreeConfig
 
-    def __init__(
-        self,
-        client_id: str,
-        client_secret: str,
-        endpoints: Optional[Endpoints] = None,
-        webhook: Optional[str] = None,
-    ):
-        self._client = Client(client_id, client_secret, endpoints)
-        self.batches: Dict[str, Batch] = {}
-        self.webhook = webhook
+        self.configuration = conf_class.from_dict(self.configuration)
 
-    def create_batch(
+    def add_job(
         self,
-        serialized_sequence: str,
-        jobs: List[Dict[str, Any]],
-        device_type: DeviceType = DeviceType.QPU,
-        configuration: Optional[BaseConfig] = None,
+        runs: int = 100,
+        variables: Optional[Dict[str, Any]] = None,
         wait: bool = False,
-        fetch_results: bool = False,
-    ) -> Batch:
-        """Create a new batch and send it to the API.
-        For Iroise MVP, the batch must contain at least one job and will be declared as complete immediately.
+    ) -> Job:
+        """Add and send a new job for this batch.
 
         Args:
-            serialized_sequence: Serialized pulser sequence.
-            jobs: List of jobs to be added to the batch at creation. (#TODO: Make optional after Iroise MVP)
-            device_type: The type of device to use, either an emulator or a QPU
-              If set to QPU, the device_type will be set to the one
-              stored in the serialized sequence
-            configuration: A dictionary with extra configuration for the emulators that accept it.
-            wait: Whether to wait for the batch to be done
-            fetch_results: Whether to download the results. Implies waiting for the batch.
-
+            runs: number of times the job is ran on the QPU.
+            variables (optional): values for variables if sequence is parametrized.
+            wait: Whether to wait for the job to be done.
 
         Returns:
-            Batch: The new batch that has been created in the database.
+            - Job: the created job.
         """
+        job_data: Dict[str, Any] = {"runs": runs, "batch_id": self.id}
+        if variables:
+            job_data["variables"] = variables
+        job_rsp = self._client._send_job(job_data)
+        job = Job(**job_rsp)
+        self.jobs[job.id] = job
+        if wait:
+            while job.status in ["PENDING", "RUNNING"]:
+                time.sleep(RESULT_POLLING_INTERVAL)
+                job_rsp = self._client._get_job(job.id)
+                job = Job(**job_rsp)
+        return job
+
+    def declare_complete(
+        self, wait: bool = False, fetch_results: bool = False
+    ) -> Dict[str, Any]:
+        """Declare to PCS that the batch is complete.
 
-        req = {
-            "sequence_builder": serialized_sequence,
-            "webhook": self.webhook,
-            "jobs": jobs,
-        }
-
-        # the emulator field is only added in the case
-        # an emulator job is requested otherwise it's left empty
-        if device_type != DeviceType.QPU:
-            req.update({"emulator": device_type})
-
-        # The configuration field is only added in the case
-        # it's requested
-        if configuration:
-            req.update({"configuration": configuration.to_dict()})  # type: ignore
+        Args:
+            wait: Whether to wait for the batch to be done
+            fetch_results: Whether to download the results. Implies
+                waiting for the batch.
 
-        batch_rsp, jobs_rsp = self._client._send_batch(req)
-        batch_id = batch_rsp["id"]
+        A batch that is complete awaits no extra jobs. All jobs previously added
+        will be executed before the batch is terminated. When all its jobs are done,
+        the complete batch is unassigned to its running device.
+        """
+        self.complete = True
+        batch_rsp = self._client._complete_batch(self.id)
         if wait or fetch_results:
             while batch_rsp["status"] in ["PENDING", "RUNNING"]:
                 time.sleep(RESULT_POLLING_INTERVAL)
-                batch_rsp, jobs_rsp = self._client._get_batch(batch_id)
-
+                batch_rsp, jobs_rsp = self._client._get_batch(
+                    self.id,
+                )
             if fetch_results:
                 batch_rsp, jobs_rsp = self._client._get_batch(
-                    batch_id, fetch_results=True
+                    self.id, fetch_results=True
                 )
-        batch = Batch(**batch_rsp, _client=self._client)
-        for job_rsp in jobs_rsp:
-            batch.jobs[job_rsp["id"]] = Job(**job_rsp)
-
-        self.batches[batch.id] = batch
-        return batch
-
-    def get_batch(self, id: str, fetch_results: bool = False) -> Batch:
-        """Retrieve a batch's data and all its jobs.
-
-        Args:
-            id: Id of the batch.
-            fetch_results: whether to download job results
-
-        Returns:
-            Batch: the batch stored in the PCS database.
-        """
-
-        batch_rsp, jobs_rsp = self._client._get_batch(id, fetch_results=fetch_results)
-        batch = Batch(**batch_rsp, _client=self._client)
-        for job_rsp in jobs_rsp:
-            batch.jobs[job_rsp["id"]] = Job(**job_rsp)
-        self.batches[batch.id] = batch
-        return batch
+            for job_rsp in jobs_rsp:
+                self.jobs[job_rsp["id"]] = Job(**job_rsp)
+        return batch_rsp
```

### Comparing `pasqal-sdk-0.1.9/sdk/_version.py` & `pasqal-sdk-0.2.0/sdk/_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.1.9"
+__version__ = "0.2.0"
```

### Comparing `pasqal-sdk-0.1.9/sdk/client.py` & `pasqal-sdk-0.2.0/sdk/client.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,103 +7,116 @@
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from __future__ import annotations
 
+from getpass import getpass
 from typing import Any, Dict, List, Optional, Tuple
 
 import requests
+from requests.auth import AuthBase
 
-from sdk.endpoints import Endpoints
+from sdk.authentication import (
+    TokenProvider,
+    Auth0TokenProvider,
+    HTTPBearerAuthenticator,
+)
+from sdk.endpoints import Endpoints, Auth0Conf
 from sdk.errors import HTTPError
 from sdk.utils.jsend import JSendPayload
 
 TIMEOUT = 30  # client http requests timeout after 30s
 
 
 class Client:
-    client_id: str
-    client_secret: str
-
-    _token: str
+    authenticator: AuthBase
 
     def __init__(
         self,
-        client_id: str,
-        client_secret: str,
+        group_id: str,
+        username: Optional[str] = None,
+        password: Optional[str] = None,
+        token_provider: Optional[TokenProvider] = None,
         endpoints: Optional[Endpoints] = None,
+        auth0: Optional[Auth0Conf] = None,
     ):
-        self.client_id = client_id
-        self.client_secret = client_secret
-        self.endpoints = endpoints or Endpoints()
-        self.group_id = None
-        self._token = ""
-        self._fetch_group_id()
-
-    def _fetch_group_id(self) -> None:
-        url = f"{self.endpoints.account}/api/v1/auth/info"
-        data = self._request(
-            "GET",
-            url,
-        )
-        self.group_id = data["data"]["group_id"]
-
-    def _login(self) -> None:
-        url = f"{self.endpoints.account}/api/v1/auth/login"
-        payload = {
-            "type": "api_key",
-            "client_id": self.client_id,
-            "client_secret": self.client_secret,
-        }
-
-        rsp = requests.post(
-            url,
-            json=payload,
-            timeout=TIMEOUT,
-            headers={"content-type": "application/json"},
-        )
-        data = rsp.json()
+        if not username and not token_provider:
+            raise ValueError(
+                "At least a username or TokenProvider object should be provided."
+            )
+        if token_provider is not None:
+            self._check_token_provider(token_provider)
 
-        if rsp.status_code >= 400:
-            raise HTTPError(data)
+        self.endpoints = self._make_endpoints(endpoints)
 
-        self._token = data["token"]
+        if username:
+            auth0 = self._make_auth0(auth0)
+            token_provider = self._credential_login(username, password, auth0)
+
+        self.authenticator = HTTPBearerAuthenticator(token_provider)
+        self.group_id = group_id
+
+    @staticmethod
+    def _make_endpoints(endpoints: Optional[Endpoints]) -> Endpoints:
+        if endpoints is None:
+            return Endpoints()
+
+        if not isinstance(endpoints, Endpoints):
+            raise TypeError(f"endpoints must be a {Endpoints.__name__} instance")
+
+        return endpoints
+
+    @staticmethod
+    def _make_auth0(auth0: Optional[Auth0Conf]) -> Auth0Conf:
+        if auth0 is None:
+            return Auth0Conf()
+
+        if not isinstance(auth0, Auth0Conf):
+            raise TypeError(f"auth0 parameter must be a {Auth0Conf.__name__} instance")
+
+        return auth0
+
+    @staticmethod
+    def _check_token_provider(token_provider: TokenProvider) -> None:
+        try:
+            # The type ignore is because I wouldn't know how to fix the type problem
+            # but the code should be correct, and is tested
+            issubclass(token_provider, TokenProvider)  # type: ignore
+        except TypeError:
+            raise TypeError("token_provider must be a TokenProvider subclass")
+
+    def _credential_login(
+        self, username: str, password: Optional[str], auth0: Auth0Conf
+    ) -> TokenProvider:
+        if not password:
+            password = getpass("Enter your password:")
+            #   We want to allow an empty string at first, but then
+            #   it results in an error
+            if not password:
+                raise ValueError("The prompted password should not be empty")
 
-    def _headers(self) -> Dict[str, str]:
-        return {
-            "content-type": "application/json",
-            "authorization": f"Bearer {self._token}",
-        }
+        token_provider: TokenProvider = Auth0TokenProvider(username, password, auth0)
+        return token_provider
 
     def _request(
         self, method: str, url: str, payload: Optional[Dict[str, Any]] = None
     ) -> JSendPayload:
         rsp = requests.request(
             method,
             url,
             json=payload,
             timeout=TIMEOUT,
-            headers=self._headers(),
+            headers={"content-type": "application/json"},
+            auth=self.authenticator,
         )
         data: JSendPayload = rsp.json()
-        # If account returns unauthorized we attempt to login and retry request
-        if rsp.status_code == 401:
-            self._login()
-            rsp = requests.request(
-                method,
-                url,
-                json=payload,
-                headers=self._headers(),
-                timeout=TIMEOUT,
-            )
-            data = rsp.json()
-
         if rsp.status_code >= 400:
             raise HTTPError(data)
 
         return data
 
     def _send_batch(
         self, batch_data: Dict[str, Any]
@@ -145,7 +158,13 @@
         return batch_data, jobs_data
 
     def _get_job(self, job_id: str) -> Dict[str, Any]:
         job: Dict[str, Any] = self._request(
             "GET", f"{self.endpoints.core}/api/v1/jobs/{job_id}"
         )["data"]
         return job
+
+    def get_device_specs_dict(self) -> Dict[str, str]:
+        device_specs: Dict[str, str] = self._request(
+            "GET", f"{self.endpoints.core}/api/v1/devices/specs"
+        )["data"]
+        return device_specs
```

### Comparing `pasqal-sdk-0.1.9/sdk/device/configuration/base_config.py` & `pasqal-sdk-0.2.0/sdk/device/configuration/base_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 INVALID_KEY_ERROR_MSG = "Invalid key {} in Configuration.extra_config. Attempted to override a default field."
 
 
 @dataclass
 class BaseConfig:
     """Base class for all device configuration classes.
-    
+
     This class provides a common interface for all device configuration classes.
     It also provides a mechanism to add extra configuration parameters
     that are not part of the default configuration.
 
     The extra configuration parameters are stored in the `extra_config` field.
     This field is a dictionary that can be used to store any extra configuration
     parameters. The `extra_config` field is not part of the configuration
```

### Comparing `pasqal-sdk-0.1.9/sdk/device/configuration/emu_sv.py` & `pasqal-sdk-0.2.0/sdk/device/configuration/emu_tn.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,26 +2,32 @@
 
 from dataclasses import dataclass
 
 from sdk.device.configuration.base_config import BaseConfig, InvalidConfiguration
 
 DT_VALUE_NOT_VALID = "dt must be larger than 0. Not {}."
 PRECISION_NOT_VALID = "Precision {} not valid. Must be one of 'low', 'normal', 'high'"
+MAX_BOND_DIM_NOT_VALID = "Max bond dimension {} must be larger than 0. Not {}."
 
 
 @dataclass
-class EmuSVConfig(BaseConfig):
-    """Configuration for the EmuSV device type.
+class EmuTNConfig(BaseConfig):
+    """Configuration for the EmuTN device type.
 
     Args:
-        dt (float): The time step of the simulation. Defaults to 0.1.
+        dt (float): The time step in nanoseconds of the simulation. Defaults to 10.0.
         precision (str): The precision of the simulation. Defaults to "normal".
+        max_bond_dim (int): The maximum bond dimension of the Matrix Product State (MPS). Defaults to 500.
     """
-    dt: float = 0.1
+
+    dt: float = 10.0
     precision: str = "normal"
+    max_bond_dim: int = 500
 
     def _validate(self) -> None:
         if self.dt <= 0:
             raise InvalidConfiguration(DT_VALUE_NOT_VALID.format(self.dt))
         if self.precision not in ["low", "normal", "high"]:
             raise InvalidConfiguration(PRECISION_NOT_VALID.format(self.precision))
+        if self.max_bond_dim <= 0:
+            raise InvalidConfiguration(MAX_BOND_DIM_NOT_VALID.format(self.max_bond_dim))
         super()._validate()
```

### Comparing `pasqal-sdk-0.1.9/sdk/endpoints.py` & `pasqal-sdk-0.2.0/sdk/endpoints.py`

 * *Files 25% similar despite different names*

```diff
@@ -15,17 +15,30 @@
 from sys import version_info
 
 from dataclasses import dataclass
 
 if version_info[:2] >= (3, 8):
     from typing import Final
 else:
-    from typing_extensions import Final # type: ignore
+    from typing_extensions import Final  # type: ignore
 
-CORE_API_URL: Final[str] = "https://apis.pasqal.cloud/core"
-ACCOUNT_API_URL: Final[str] = "https://apis.pasqal.cloud/account"
+
+CORE_API_URL: Final[str] = "https://apis.pasqal.cloud/core-fast"
 
 
 @dataclass
 class Endpoints:
     core: str = CORE_API_URL
-    account: str = ACCOUNT_API_URL
+
+
+AUTH0_DOMAIN: Final[str] = "pasqal.eu.auth0.com"
+PUBLIC_CLIENT_ID: Final[str] = "PeZvo7Atx7IVv3iel59asJSb4Ig7vuSB"
+AUDIENCE: Final[str] = "https://apis.pasqal.cloud/account/api/v1"
+REALM: Final[str] = "pcs-users"
+
+
+@dataclass
+class Auth0Conf:
+    domain: str = AUTH0_DOMAIN
+    public_client_id: str = PUBLIC_CLIENT_ID
+    audience: str = AUDIENCE
+    realm: str = REALM
```

### Comparing `pasqal-sdk-0.1.9/sdk/errors.py` & `pasqal-sdk-0.2.0/sdk/errors.py`

 * *Files 13% similar despite different names*

```diff
@@ -35,7 +35,11 @@
         self.details = data
 
     def __str__(self) -> str:
         return (
             f"Error {self.code}: {self.description}\n"
             f"Details: {json.dumps(self.details, indent=2)}"
         )
+
+
+class LoginError(Exception):
+    pass
```

### Comparing `pasqal-sdk-0.1.9/sdk/job.py` & `pasqal-sdk-0.2.0/sdk/job.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,26 +8,28 @@
 
     Attributes:
         - runs: Number of time the job should be ran.
         - created_at: Timestamp of the creation of the batch.
         - updated_at: Timestamps of the last update of the batch.
         - start_timestamp(optional): The timestamp of when the job began processing.
         - end_timestamp(optional): The timestamp of when the job finished processing.
-        - batch_id: Id of the batch which the job belongs to.
+        - batch_id: ID of the batch which the job belongs to.
         - errors: Error messages that occured while processing job.
         - id: Unique identifier for the batch
+        - group_id: ID of the group which the users scheduling the job belong to.
         - status: Status of the job
         - result(optional): Result of the job.
         - variables (optional): dictionnary of variables of the job.
             None if the associated batch is non-parametrized
     """
 
     runs: int
     batch_id: str
     id: str
+    group_id: str
     status: str
     created_at: str
     updated_at: str
     errors: List[str]
     start_timestamp: Optional[str] = None
     end_timestamp: Optional[str] = None
     result: Optional[Dict[str, Any]] = None
```

### Comparing `pasqal-sdk-0.1.9/sdk/utils/jsend.py` & `pasqal-sdk-0.2.0/sdk/utils/jsend.py`

 * *Files identical despite different names*

### Comparing `pasqal-sdk-0.1.9/setup.py` & `pasqal-sdk-0.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,21 +32,28 @@
     license="Apache 2.0",
     # TODO:
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Programming Language :: Python :: 3",
     ],
     url="https://github.com/pasqal-io/cloud-sdk",
-    install_requires=["requests==2.25.1", "requests-mock==1.9.3"],
+    install_requires=[
+        "auth0-python==3.23.1",
+        "requests==2.25.1",
+        "requests-mock==1.9.3",
+        "pyjwt[crypto]==2.5.0",
+    ],
     extras_require={
         "dev": {
             "black==20.8b1",
             "flake8==3.9.0",
             "flake8-import-order==0.18.1",
             "mypy==0.982",
             "pytest==6.2.5",
             "pytest-cov==2.11.1",
-            "types-requests==2.25.1"
+            "types-requests==2.25.1",
         },
-        ":python_version == '3.7'": ["typing-extensions==4.4.0",]
+        ":python_version == '3.7'": [
+            "typing-extensions==4.4.0",
+        ],
     },
 )
```

### Comparing `pasqal-sdk-0.1.9/tests/test_batch.py` & `pasqal-sdk-0.2.0/tests/test_batch.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,59 +1,73 @@
+from unittest.mock import patch
+from uuid import uuid4
+
 import pytest
+from tests.test_doubles.authentication import FakeAuth0AuthenticationSuccess
 
-from sdk import SDK, DeviceType
-from sdk.device.configuration import BaseConfig, EmuFreeConfig, EmuSVConfig
+from sdk import SDK
+from sdk.device import BaseConfig, EmuFreeConfig, EmulatorType, EmuTNConfig
 
 
 class TestBatch:
     @pytest.fixture(autouse=True)
+    @patch("sdk.client.Auth0TokenProvider", FakeAuth0AuthenticationSuccess)
     def init_sdk(self, start_mock_request):
-        self.sdk = SDK(client_id="my_client_id", client_secret="my_client_secret")
+        self.sdk = SDK(
+            username="me@test.com", password="password", group_id=str(uuid4())
+        )
         self.pulser_sequence = "pulser_test_sequence"
-        self.batch_id = '00000000-0000-0000-0000-000000000001'
+        self.batch_id = "00000000-0000-0000-0000-000000000001"
         self.job_result = {"1001": 12, "0110": 35, "1111": 1}
         self.n_job_runs = 50
         self.job_id = "00000000-0000-0000-0000-000000022010"
         self.job_variables = {"Omega_max": 14.4, "last_target": "q1", "ts": [200, 500]}
 
-    @pytest.mark.parametrize("device_type", [d.value for d in DeviceType])
-    def test_create_batch(self, device_type):
+    @pytest.mark.parametrize("emulator", [None] + [e.value for e in EmulatorType])
+    def test_create_batch(self, emulator):
         job = {"runs": self.n_job_runs, "variables": self.job_variables}
         batch = self.sdk.create_batch(
             serialized_sequence=self.pulser_sequence,
             jobs=[job],
-            device_type=device_type,
+            emulator=emulator,
         )
         assert batch.id == self.batch_id
         assert batch.sequence_builder == self.pulser_sequence
         # TODO: Remove after IROISE MVP
         assert batch.complete
         assert batch.jobs[self.job_id].batch_id == batch.id
         assert batch.jobs[self.job_id].runs == self.n_job_runs
 
     def test_create_batch_and_wait(self, request_mock):
         job = {"runs": self.n_job_runs, "variables": self.job_variables}
         batch = self.sdk.create_batch(
             serialized_sequence=self.pulser_sequence, jobs=[job], wait=True
         )
-        assert batch.id == "00000000-0000-0000-0000-000000000001"  # the batch_id used in the mock data
+        assert (
+            batch.id == "00000000-0000-0000-0000-000000000001"
+        )  # the batch_id used in the mock data
         assert batch.sequence_builder == self.pulser_sequence
         assert batch.complete
         assert batch.jobs
         for job_id, job in batch.jobs.items():
             assert self.job_id == job_id
             assert job.result is None
         assert request_mock.last_request.method == "GET"
 
     def test_create_batch_and_fetch_results(self, request_mock):
         job = {"runs": self.n_job_runs, "variables": self.job_variables}
         batch = self.sdk.create_batch(
-            serialized_sequence=self.pulser_sequence, jobs=[job], wait=True, fetch_results=True
+            serialized_sequence=self.pulser_sequence,
+            jobs=[job],
+            wait=True,
+            fetch_results=True,
         )
-        assert batch.id == "00000000-0000-0000-0000-000000000001"  # the batch_id used in the mock data
+        assert (
+            batch.id == "00000000-0000-0000-0000-000000000001"
+        )  # the batch_id used in the mock data
         assert batch.sequence_builder == self.pulser_sequence
         assert batch.complete
         assert batch.jobs
         for job_id, job in batch.jobs.items():
             assert self.job_id == job_id
             assert job.result == self.job_result
         assert request_mock.last_request.method == "GET"
@@ -111,24 +125,32 @@
             request_mock.last_request.url
             == f"{self.sdk._client.endpoints.core}/api/v1/jobs/{self.job_id}"
         )
         assert batch.jobs[self.job_id].batch_id == batch.id
         assert batch.jobs[self.job_id].result == self.job_result
 
     @pytest.mark.parametrize(
-        "device_type, configuration, expected",
+        "emulator, configuration, expected",
         [
-            (DeviceType.EMU_SV, EmuSVConfig(), EmuSVConfig()),
-            (DeviceType.QPU, None, None),
-            (DeviceType.EMU_FREE, EmuFreeConfig(), EmuFreeConfig(extra_config={'dt': 0.1, 'precision': 'normal'})),
-            ('SomethingElse', BaseConfig(), BaseConfig(extra_config={'dt': 0.1, 'precision': 'normal'}))
+            (EmulatorType.EMU_TN, EmuTNConfig(), EmuTNConfig()),
+            (None, None, None),
+            (
+                EmulatorType.EMU_FREE,
+                EmuFreeConfig(),
+                EmuFreeConfig(extra_config={"dt": 10.0, "precision": "normal"}),
+            ),
+            (
+                "SomethingElse",
+                BaseConfig(),
+                BaseConfig(extra_config={"dt": 10.0, "precision": "normal"}),
+            ),
         ],
     )
-    def test_create_batch_configuration(self, device_type, configuration, expected):
+    def test_create_batch_configuration(self, emulator, configuration, expected):
         job = {"runs": self.n_job_runs, "variables": self.job_variables}
         batch = self.sdk.create_batch(
             serialized_sequence=self.pulser_sequence,
             jobs=[job],
-            device_type=device_type,
+            emulator=emulator,
             configuration=configuration,
         )
         assert batch.configuration == expected
```

### Comparing `pasqal-sdk-0.1.9/tests/test_config.py` & `pasqal-sdk-0.2.0/tests/test_config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,83 +1,91 @@
 from __future__ import annotations
 
 import pytest
 
+from sdk.device import EmuFreeConfig
 from sdk.device.configuration.base_config import (
     BaseConfig,
+    INVALID_KEY_ERROR_MSG,
     InvalidConfiguration,
-    INVALID_KEY_ERROR_MSG
 )
-from sdk.device.configuration import EmuFreeConfig
-from sdk.device.configuration.emu_sv import (
-    EmuSVConfig,
+from sdk.device.configuration.emu_tn import (
     DT_VALUE_NOT_VALID,
+    EmuTNConfig,
     PRECISION_NOT_VALID,
 )
 
 
 @pytest.mark.parametrize(
     "config, expected",
     [
         (
-            EmuSVConfig(
-                dt=0.5,
+            EmuTNConfig(
+                dt=10.0,
                 extra_config={"extra": "parameter", "extra_dict": {"key": "value"}},
             ),
             {
-                "dt": 0.5,
+                "dt": 10.0,
                 "precision": "normal",
+                "max_bond_dim": 500,
                 "extra": "parameter",
                 "extra_dict": {"key": "value"},
             },
         ),
-        (EmuSVConfig(), {"dt": 0.1, "precision": "normal"}),
+        (EmuTNConfig(), {"dt": 10.0, "precision": "normal", "max_bond_dim": 500}),
         (EmuFreeConfig(), {"with_noise": False}),
         (EmuFreeConfig(with_noise=True), {"with_noise": True}),
         (BaseConfig(), {}),
-        (BaseConfig(extra_config={"extra": "parameter"}), {"extra": "parameter"})
+        (BaseConfig(extra_config={"extra": "parameter"}), {"extra": "parameter"}),
     ],
 )
 def test_configuration_to_dict(config: BaseConfig, expected: dict):
     assert config.to_dict() == expected
 
 
 @pytest.mark.parametrize(
     "config_class, expected, config",
     [
-        (   EmuSVConfig,
-            EmuSVConfig(
+        (
+            EmuTNConfig,
+            EmuTNConfig(
                 dt=0.5,
                 extra_config={"extra": "parameter", "extra_dict": {"key": "value"}},
             ),
             {
                 "dt": 0.5,
                 "precision": "normal",
                 "extra": "parameter",
                 "extra_dict": {"key": "value"},
             },
         ),
-        (EmuSVConfig, EmuSVConfig(), {"dt": 0.1, "precision": "normal"}),
+        (EmuTNConfig, EmuTNConfig(), {"dt": 10.0, "precision": "normal"}),
         (EmuFreeConfig, EmuFreeConfig(), {"with_noise": False}),
         (EmuFreeConfig, EmuFreeConfig(with_noise=True), {"with_noise": True}),
         (BaseConfig, BaseConfig(), {}),
-        (BaseConfig, BaseConfig(extra_config={"extra": "parameter"}), {"extra": "parameter"})
+        (
+            BaseConfig,
+            BaseConfig(extra_config={"extra": "parameter"}),
+            {"extra": "parameter"},
+        ),
     ],
 )
-def test_configuration_from_dict(config_class: type, expected: BaseConfig, config: dict):
+def test_configuration_from_dict(
+    config_class: type, expected: BaseConfig, config: dict
+):
     assert config_class.from_dict(config) == expected
 
 
 @pytest.mark.parametrize(
     "config, extra_config, expected",
     [
-        (EmuSVConfig(), {"dt": 0.1}, INVALID_KEY_ERROR_MSG.format("dt")),
-        (EmuSVConfig(dt=-1), None, DT_VALUE_NOT_VALID.format(-1)),
+        (EmuTNConfig(), {"dt": 10.0}, INVALID_KEY_ERROR_MSG.format("dt")),
+        (EmuTNConfig(dt=-1), None, DT_VALUE_NOT_VALID.format(-1)),
         (
-            EmuSVConfig(precision="nonsense"),
+            EmuTNConfig(precision="nonsense"),
             None,
             PRECISION_NOT_VALID.format("nonsense"),
         ),
     ],
 )
 def test_wrong_configuration(config, extra_config, expected):
     config.extra_config = extra_config
```

