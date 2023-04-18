# Comparing `tmp/qiskit-ionq-0.3.9.tar.gz` & `tmp/qiskit-ionq-0.4.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit-ionq-0.3.9.tar", last modified: Wed Nov  2 18:26:12 2022, max compression
+gzip compressed data, was "qiskit-ionq-0.4.0.dev0.tar", last modified: Tue Apr 18 19:43:54 2023, max compression
```

## Comparing `qiskit-ionq-0.3.9.tar` & `qiskit-ionq-0.4.0.dev0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 18:26:12.051128 qiskit-ionq-0.3.9/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 18:26:12.043128 qiskit-ionq-0.3.9/.eggs/
--rw-r--r--   0 runner    (1001) docker     (121)      211 2022-11-02 18:26:11.000000 qiskit-ionq-0.3.9/.eggs/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 18:26:12.039127 qiskit-ionq-0.3.9/.eggs/pytest_runner-6.0.0-py3.9.egg/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 18:26:12.043128 qiskit-ionq-0.3.9/.eggs/pytest_runner-6.0.0-py3.9.egg/EGG-INFO/
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-11-02 18:26:11.000000 qiskit-ionq-0.3.9/.eggs/pytest_runner-6.0.0-py3.9.egg/EGG-INFO/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      236 2022-11-02 18:26:11.000000 qiskit-ionq-0.3.9/.eggs/pytest_runner-6.0.0-py3.9.egg/EGG-INFO/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-11-02 18:26:11.000000 qiskit-ionq-0.3.9/.eggs/pytest_runner-6.0.0-py3.9.egg/EGG-INFO/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    11416 2022-11-02 18:26:01.000000 qiskit-ionq-0.3.9/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-11-02 18:26:01.000000 qiskit-ionq-0.3.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6494 2022-11-02 18:26:12.051128 qiskit-ionq-0.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5455 2022-11-02 18:26:01.000000 qiskit-ionq-0.3.9/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-11-02 18:26:01.000000 qiskit-ionq-0.3.9/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 18:26:12.047128 qiskit-ionq-0.3.9/qiskit_ionq/
--rw-r--r--   0 runner    (1001) docker     (121)     1229 2022-11-02 18:26:01.000000 qiskit-ionq-0.3.9/qiskit_ionq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2074 2022-11-02 18:26:01.000000 qiskit-ionq-0.3.9/qiskit_ionq/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     8792 2022-11-02 18:26:01.000000 qiskit-ionq-0.3.9/qiskit_ionq/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)    14779 2022-11-02 18:26:01.000000 qiskit-ionq-0.3.9/qiskit_ionq/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)    12899 2022-11-02 18:26:01.000000 qiskit-ionq-0.3.9/qiskit_ionq/ionq_backend.py
--rw-r--r--   0 runner    (1001) docker     (121)     7331 2022-11-02 18:26:01.000000 qiskit-ionq-0.3.9/qiskit_ionq/ionq_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     4832 2022-11-02 18:26:01.000000 qiskit-ionq-0.3.9/qiskit_ionq/ionq_gates.py
--rw-r--r--   0 runner    (1001) docker     (121)    15647 2022-11-02 18:26:01.000000 qiskit-ionq-0.3.9/qiskit_ionq/ionq_job.py
--rw-r--r--   0 runner    (1001) docker     (121)     5036 2022-11-02 18:26:01.000000 qiskit-ionq-0.3.9/qiskit_ionq/ionq_provider.py
--rw-r--r--   0 runner    (1001) docker     (121)     3336 2022-11-02 18:26:01.000000 qiskit-ionq-0.3.9/qiskit_ionq/ionq_result.py
--rw-r--r--   0 runner    (1001) docker     (121)     2915 2022-11-02 18:26:01.000000 qiskit-ionq-0.3.9/qiskit_ionq/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 18:26:12.047128 qiskit-ionq-0.3.9/qiskit_ionq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6494 2022-11-02 18:26:11.000000 qiskit-ionq-0.3.9/qiskit_ionq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1036 2022-11-02 18:26:11.000000 qiskit-ionq-0.3.9/qiskit_ionq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-02 18:26:11.000000 qiskit-ionq-0.3.9/qiskit_ionq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-02 18:26:11.000000 qiskit-ionq-0.3.9/qiskit_ionq.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       95 2022-11-02 18:26:11.000000 qiskit-ionq-0.3.9/qiskit_ionq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-11-02 18:26:11.000000 qiskit-ionq-0.3.9/qiskit_ionq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      152 2022-11-02 18:26:01.000000 qiskit-ionq-0.3.9/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-11-02 18:26:01.000000 qiskit-ionq-0.3.9/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (121)       95 2022-11-02 18:26:01.000000 qiskit-ionq-0.3.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      142 2022-11-02 18:26:12.051128 qiskit-ionq-0.3.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3304 2022-11-02 18:26:01.000000 qiskit-ionq-0.3.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 18:26:12.051128 qiskit-ionq-0.3.9/test/
--rw-r--r--   0 runner    (1001) docker     (121)     7096 2022-11-02 18:26:01.000000 qiskit-ionq-0.3.9/test/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     3889 2022-11-02 18:26:01.000000 qiskit-ionq-0.3.9/test/test_mock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:43:54.583224 qiskit-ionq-0.4.0.dev0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:43:54.579224 qiskit-ionq-0.4.0.dev0/.eggs/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-18 19:43:53.000000 qiskit-ionq-0.4.0.dev0/.eggs/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:43:54.575224 qiskit-ionq-0.4.0.dev0/.eggs/pytest_runner-6.0.0-py3.9.egg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:43:54.579224 qiskit-ionq-0.4.0.dev0/.eggs/pytest_runner-6.0.0-py3.9.egg/EGG-INFO/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-18 19:43:54.000000 qiskit-ionq-0.4.0.dev0/.eggs/pytest_runner-6.0.0-py3.9.egg/EGG-INFO/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-18 19:43:54.000000 qiskit-ionq-0.4.0.dev0/.eggs/pytest_runner-6.0.0-py3.9.egg/EGG-INFO/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-18 19:43:54.000000 qiskit-ionq-0.4.0.dev0/.eggs/pytest_runner-6.0.0-py3.9.egg/EGG-INFO/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-04-18 19:43:45.000000 qiskit-ionq-0.4.0.dev0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-18 19:43:45.000000 qiskit-ionq-0.4.0.dev0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6739 2023-04-18 19:43:54.583224 qiskit-ionq-0.4.0.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-04-18 19:43:45.000000 qiskit-ionq-0.4.0.dev0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-18 19:43:45.000000 qiskit-ionq-0.4.0.dev0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:43:54.579224 qiskit-ionq-0.4.0.dev0/qiskit_ionq/
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-18 19:43:45.000000 qiskit-ionq-0.4.0.dev0/qiskit_ionq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-04-18 19:43:45.000000 qiskit-ionq-0.4.0.dev0/qiskit_ionq/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9123 2023-04-18 19:43:45.000000 qiskit-ionq-0.4.0.dev0/qiskit_ionq/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15179 2023-04-18 19:43:45.000000 qiskit-ionq-0.4.0.dev0/qiskit_ionq/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14014 2023-04-18 19:43:45.000000 qiskit-ionq-0.4.0.dev0/qiskit_ionq/ionq_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7688 2023-04-18 19:43:45.000000 qiskit-ionq-0.4.0.dev0/qiskit_ionq/ionq_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-04-18 19:43:45.000000 qiskit-ionq-0.4.0.dev0/qiskit_ionq/ionq_gates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16098 2023-04-18 19:43:45.000000 qiskit-ionq-0.4.0.dev0/qiskit_ionq/ionq_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-04-18 19:43:45.000000 qiskit-ionq-0.4.0.dev0/qiskit_ionq/ionq_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-04-18 19:43:45.000000 qiskit-ionq-0.4.0.dev0/qiskit_ionq/ionq_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-04-18 19:43:45.000000 qiskit-ionq-0.4.0.dev0/qiskit_ionq/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:43:54.583224 qiskit-ionq-0.4.0.dev0/qiskit_ionq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6739 2023-04-18 19:43:54.000000 qiskit-ionq-0.4.0.dev0/qiskit_ionq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-18 19:43:54.000000 qiskit-ionq-0.4.0.dev0/qiskit_ionq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 19:43:54.000000 qiskit-ionq-0.4.0.dev0/qiskit_ionq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 19:43:54.000000 qiskit-ionq-0.4.0.dev0/qiskit_ionq.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-18 19:43:54.000000 qiskit-ionq-0.4.0.dev0/qiskit_ionq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-18 19:43:54.000000 qiskit-ionq-0.4.0.dev0/qiskit_ionq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-18 19:43:45.000000 qiskit-ionq-0.4.0.dev0/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-18 19:43:45.000000 qiskit-ionq-0.4.0.dev0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-18 19:43:45.000000 qiskit-ionq-0.4.0.dev0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-18 19:43:54.583224 qiskit-ionq-0.4.0.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-04-18 19:43:45.000000 qiskit-ionq-0.4.0.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 19:43:54.583224 qiskit-ionq-0.4.0.dev0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    10551 2023-04-18 19:43:45.000000 qiskit-ionq-0.4.0.dev0/test/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-04-18 19:43:45.000000 qiskit-ionq-0.4.0.dev0/test/test_mock.py
```

### Comparing `qiskit-ionq-0.3.9/LICENSE.txt` & `qiskit-ionq-0.4.0.dev0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qiskit-ionq-0.3.9/PKG-INFO` & `qiskit-ionq-0.4.0.dev0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-ionq
-Version: 0.3.9
+Version: 0.4.0.dev0
 Summary: Qiskit provider for IonQ backends
 Home-page: https://github.com/qiskit-partners/qiskit-ionq
 Author: IonQ
 Author-email: info@ionq.com
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/qiskit-partners/qiskit-ionq/issues
 Project-URL: Source Code, https://github.com/qiskit-partners/qiskit-ionq
@@ -97,30 +97,35 @@
 ### Submitting a Circuit
 
 Once a backend has been specified, it may be used to submit circuits.
 For example, running a Bell State:
 
 ```python
 from qiskit import QuantumCircuit
+from qiskit_ionq.constants import AggregationType
 
 # Create a basic Bell State circuit:
 qc = QuantumCircuit(2, 2)
 qc.h(0)
 qc.cx(0, 1)
 qc.measure([0, 1], [0, 1])
 
 # Run the circuit on IonQ's platform:
 job = simulator_backend.run(qc)
 
 # Print the results.
-print(job.get_counts())
+print(job.result().get_counts())
+
+# Get results with a different aggregation method when symmetrization
+# is applied as an error mitigation strategy
+print(job.result(AggregationType.AVERAGE).get_counts())
 
 # The simulator specifically provides the the ideal probabilities and creates
 # counts by sampling from these probabilities. The raw probabilities are also accessible:
-print(job.get_probabilities())
+print(job.result().get_probabilities())
 ```
 
 ### Basis gates and transpilation
 
 The IonQ provider provides access to the full IonQ Cloud backend, which includes its own transpilation and compilation pipeline. As such, IonQ provider backends have a broad set of "basis gates" that they will accept — effectively anything the IonQ API will accept. They are `ccx, ch, cnot, cp, crx, cry, crz, csx, cx, cy, cz, h, i, id, mcp, mct, mcx, measure, p, rx, rxx, ry, ryy, rz, rzz, s, sdg, swap, sx, sxdg, t, tdg, toffoli, x, y` and `z`.
 
 If you have circuits that you'd like to run on IonQ backends that use other gates than this (`u` or `iswap` for example), you will either need to manually rewrite the circuit to only use the above list, or use the Qiskit transpiler, per the example below. Please note that not all circuits can be automatically transpiled.
```

### Comparing `qiskit-ionq-0.3.9/README.md` & `qiskit-ionq-0.4.0.dev0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -70,30 +70,35 @@
 ### Submitting a Circuit
 
 Once a backend has been specified, it may be used to submit circuits.
 For example, running a Bell State:
 
 ```python
 from qiskit import QuantumCircuit
+from qiskit_ionq.constants import AggregationType
 
 # Create a basic Bell State circuit:
 qc = QuantumCircuit(2, 2)
 qc.h(0)
 qc.cx(0, 1)
 qc.measure([0, 1], [0, 1])
 
 # Run the circuit on IonQ's platform:
 job = simulator_backend.run(qc)
 
 # Print the results.
-print(job.get_counts())
+print(job.result().get_counts())
+
+# Get results with a different aggregation method when symmetrization
+# is applied as an error mitigation strategy
+print(job.result(AggregationType.AVERAGE).get_counts())
 
 # The simulator specifically provides the the ideal probabilities and creates
 # counts by sampling from these probabilities. The raw probabilities are also accessible:
-print(job.get_probabilities())
+print(job.result().get_probabilities())
 ```
 
 ### Basis gates and transpilation
 
 The IonQ provider provides access to the full IonQ Cloud backend, which includes its own transpilation and compilation pipeline. As such, IonQ provider backends have a broad set of "basis gates" that they will accept — effectively anything the IonQ API will accept. They are `ccx, ch, cnot, cp, crx, cry, crz, csx, cx, cy, cz, h, i, id, mcp, mct, mcx, measure, p, rx, rxx, ry, ryy, rz, rzz, s, sdg, swap, sx, sxdg, t, tdg, toffoli, x, y` and `z`.
 
 If you have circuits that you'd like to run on IonQ backends that use other gates than this (`u` or `iswap` for example), you will either need to manually rewrite the circuit to only use the above list, or use the Qiskit transpiler, per the example below. Please note that not all circuits can be automatically transpiled.
```

### Comparing `qiskit-ionq-0.3.9/qiskit_ionq/__init__.py` & `qiskit-ionq-0.4.0.dev0/qiskit_ionq/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -25,7 +25,8 @@
 # limitations under the License.
 
 """Provider for IonQ backends"""
 
 from .ionq_provider import IonQProvider
 from .version import __version__
 from .ionq_gates import GPIGate, GPI2Gate, MSGate
+from .constants import AggregationType, ErrorMitigation
```

### Comparing `qiskit-ionq-0.3.9/qiskit_ionq/constants.py` & `qiskit-ionq-0.4.0.dev0/qiskit_ionq/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -59,8 +59,22 @@
     READY = jobstatus.JobStatus.QUEUED.name
     RUNNING = jobstatus.JobStatus.RUNNING.name
     CANCELED = jobstatus.JobStatus.CANCELLED.name
     COMPLETED = jobstatus.JobStatus.DONE.name
     FAILED = jobstatus.JobStatus.ERROR.name
 
 
+class AggregationType(enum.Enum):
+    """Class for job results aggregation enumerated type."""
+
+    AVERAGE = "average"
+    PLURALITY = "plurality"
+
+
+class ErrorMitigation(enum.Enum):
+    """Class for error mitigation settings enumerated type."""
+
+    SYMMETRIZATION = {"symmetrization": True}
+    NO_SYMMETRIZATION = {"symmetrization": False}
+
+
 __all__ = ["APIJobStatus", "JobStatusMap"]
```

### Comparing `qiskit-ionq-0.3.9/qiskit_ionq/exceptions.py` & `qiskit-ionq-0.4.0.dev0/qiskit_ionq/exceptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,40 +48,46 @@
 class IonQCredentialsError(IonQError):
     """Errors generated from bad credentials or config"""
 
 
 class IonQClientError(IonQError):
     """Errors that arise from unexpected behavior while using IonQClient."""
 
+
 class IonQRetriableError(IonQError):
     """Errors that do not indicate a failure related to the request, and can be retried."""
 
     def __init__(self, cause):
         self._cause = cause
         super().__init__(cause.message)
 
 # pylint: disable=no-member
 
+
 # https://support.cloudflare.com/hc/en-us/articles/115003014512-4xx-Client-Error
 # "Cloudflare will generate and serve a 409 response for a Error 1001: DNS Resolution Error."
 # We may want to condition on the body as well, to allow for some GET requests to return 409 in
 # the future.
 _RETRIABLE_FOR_GETS = {requests.codes.conflict}
 # Retriable regardless of the source
 # Handle 52x responses from cloudflare.
 # See https://support.cloudflare.com/hc/en-us/articles/115003011431/
 _RETRIABLE_STATUS_CODES = {
     requests.codes.internal_server_error,
+    requests.codes.bad_gateway,
     requests.codes.service_unavailable,
     *list(range(520, 530)),
 }
 # pylint: enable=no-member
+
+
 def _is_retriable(method, code):
     return code in _RETRIABLE_STATUS_CODES or (method == "GET" and code in _RETRIABLE_FOR_GETS)
 
+
 class IonQAPIError(IonQError):
     """Base exception for fatal API errors.
 
     Attributes:
         status_code(int): An HTTP response status code.
         error_type(str): An error type string from the IonQ REST API.
     """
@@ -89,41 +95,43 @@
     @classmethod
     def raise_for_status(cls, response):
         """Raise an instance of the exception class from an API response object if needed.
         Args:
             response (:class:`Response <requests.Response>`): An IonQ REST API response.
 
         Raises:
-            IonQAPIError: instance of `cls` with error detail from `response`."""
+            IonQAPIError: instance of `cls` with error detail from `response`.
+            IonQRetriableError:  instance of `cls` with error detail from `response`."""
         status_code = response.status_code
         if status_code == 200:
             return None
         res = cls.from_response(response)
-        raise (IonQRetriableError(res)
-                if _is_retriable(response.request.method, status_code)
-                else res)
-
+        if _is_retriable(response.request.method, status_code):
+            raise IonQRetriableError(res)
+        raise res
 
     @classmethod
     def from_response(cls, response):
         """Raise an instance of the exception class from an API response object.
 
         Args:
             response (:class:`Response <requests.Response>`): An IonQ REST API response.
 
         Returns:
             IonQAPIError: instance of `cls` with error detail from `response`.
 
         """
         # TODO: Pending API changes will cleanup this error logic:
         status_code = response.status_code
+        headers = response.headers
+        body = response.text
         try:
             response_json = response.json()
         except jd.JSONDecodeError:
-            response_json = { 'invalid_json': response.text }
+            response_json = {'invalid_json': response.text}
         # Defaults, if items cannot be extracted from the response.
         error_type = "internal_error"
         message = "No error details provided."
         if "code" in response_json:
             # { "code": <int>, "message": <str> }
             message = response_json.get("message") or message
         elif "statusCode" in response_json:
@@ -131,26 +139,30 @@
             message = response_json.get("message") or message
             error_type = response_json.get("error") or error_type
         elif "error" in response_json:
             # { "error": { "type": <str>, "message: <str> } }
             error_data = response_json.get("error")
             message = error_data.get("message") or message
             error_type = error_data.get("type") or error_type
-        return cls(message, status_code, error_type)
+        return cls(message, status_code, headers, body, error_type)
 
-    def __init__(self, message, status_code, error_type):
+    def __init__(self, message, status_code, headers, body, error_type):
+        super().__init__(message)
         self.status_code = status_code
+        self.headers = headers
+        self.body = body
         self.error_type = error_type
-        super().__init__(message)
 
     def __str__(self):
         return (
             f"{self.__class__.__name__}("
             f"message={self.message!r},"
-            f"status_code={self.status_code},"
+            f"status_code={self.status_code!r},"
+            f"headers={self.headers},"
+            f"body={self.body},"
             f"error_type={self.error_type!r})"
         )
 
 
 class IonQBackendError(IonQError):
     """Errors generated from improper usage of IonQBackend objects."""
 
@@ -175,17 +187,17 @@
     """
 
     def __init__(self, gate_name, gateset):
         self.gate_name = gate_name
         self.gateset = gateset
         super().__init__(
             (f"gate '{gate_name}' is not supported on the '{gateset}' IonQ backends. "
-              "Please use the qiskit.transpile method, manually rewrite to remove the gate, "
-              "or change the gateset selection as appropriate."
-            )
+             "Please use the qiskit.transpile method, manually rewrite to remove the gate, "
+             "or change the gateset selection as appropriate."
+             )
         )
 
     def __repr__(self):
         return f"{self.__class__.__name__}(gate_name={self.gate_name!r}, gateset={self.gateset!r})"
 
 
 class IonQMidCircuitMeasurementError(IonQError, JobError):
```

### Comparing `qiskit-ionq-0.3.9/qiskit_ionq/helpers.py` & `qiskit-ionq-0.4.0.dev0/qiskit_ionq/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,16 +36,18 @@
 
 from qiskit import __version__ as qiskit_terra_version
 from qiskit.circuit import controlledgate as q_cgates
 from qiskit.circuit.library import standard_gates as q_gates
 
 # Use this to get version instead of __version__ to avoid circular dependency.
 from importlib_metadata import version
+from qiskit_ionq.constants import ErrorMitigation
 from . import exceptions
 
+
 # the qiskit gates that the IonQ backend can serialize to our IR
 # not the actual hardware basis gates for the system — we do our own transpilation pass.
 # also not an exact/complete list of the gates IonQ's backend takes
 #   by name — please refer to IonQ docs for that.
 ionq_basis_gates = [
     "ccx",
     "ch",
@@ -225,15 +227,16 @@
             # If this is a multi-control, use more than one qubit.
             if instruction.num_ctrl_qubits > 1:
                 controls = [
                     input_circuit.qubits.index(qargs[i])
                     for i in range(instruction.num_ctrl_qubits)
                 ]
                 targets = [
-                    input_circuit.qubits.index(qargs[instruction.num_ctrl_qubits])
+                    input_circuit.qubits.index(
+                        qargs[instruction.num_ctrl_qubits])
                 ]
             if gate == "swap":
                 # If this is a cswap, we have two targets:
                 targets = [
                     input_circuit.qubits.index(qargs[-2]),
                     input_circuit.qubits.index(qargs[-1]),
                 ]
@@ -349,56 +352,65 @@
         backend (:class:`qiskit_ionq.IonQBackend`): The IonQ backend.
         passed_args (dict): Dictionary containing additional passed arguments, eg. shots.
 
     Returns:
         str: A string / JSON-serialized dictionary with IonQ API compatible values.
     """
     passed_args = passed_args or {}
-    ionq_circ, _, meas_map = qiskit_circ_to_ionq_circ(circuit, backend.gateset())
+    ionq_circ, _, meas_map = qiskit_circ_to_ionq_circ(
+        circuit, backend.gateset())
     creg_sizes, clbit_labels = get_register_sizes_and_labels(circuit.cregs)
     qreg_sizes, qubit_labels = get_register_sizes_and_labels(circuit.qregs)
     qiskit_header = compress_dict_to_metadata_string(
         {
             "memory_slots": circuit.num_clbits,  # int
             "global_phase": circuit.global_phase,  # float
             "n_qubits": circuit.num_qubits,  # int
             "name": circuit.name,  # str
-            "creg_sizes": creg_sizes,  # list of [str, int] tuples cardinality memory_slots
-            "clbit_labels": clbit_labels,  # list of [str, int] tuples cardinality memory_slots
-            "qreg_sizes": qreg_sizes,  # list of [str, int] tuples cardinality num_qubits
-            "qubit_labels": qubit_labels,  # list of [str, int] tuples cardinality num_qubits
+            # list of [str, int] tuples cardinality memory_slots
+            "creg_sizes": creg_sizes,
+            # list of [str, int] tuples cardinality memory_slots
+            "clbit_labels": clbit_labels,
+            # list of [str, int] tuples cardinality num_qubits
+            "qreg_sizes": qreg_sizes,
+            # list of [str, int] tuples cardinality num_qubits
+            "qubit_labels": qubit_labels,
         }
     )
 
     target = backend.name()[5:]
     ionq_json = {
-        "lang": "json",
         "target": target,
         "shots": passed_args.get("shots"),
-        "body": {
+        "name": circuit.name,
+        "input": {
+            "format": "ionq.circuit.v0",
             "gateset": backend.gateset(),
             "qubits": circuit.num_qubits,
             "circuit": ionq_circ,
         },
         "registers": {"meas_mapped": meas_map} if meas_map else {},
         # store a couple of things we'll need later for result formatting
         "metadata": {
             "shots": str(passed_args.get("shots")),
             "sampler_seed": str(passed_args.get("sampler_seed")),
             "qiskit_header": qiskit_header,
         },
     }
     if target == "simulator":
         ionq_json["noise"] = {
-                "model": backend.options.noise_model,
-                "seed": backend.options.sampler_seed,
+            "model": passed_args.get("noise_model") or backend.options.noise_model,
+            "seed": backend.options.sampler_seed,
         }
     settings = passed_args.get("job_settings") or None
     if settings is not None:
         ionq_json["settings"] = settings
+    error_mitigation = passed_args.get("error_mitigation")
+    if error_mitigation and isinstance(error_mitigation, ErrorMitigation):
+        ionq_json["error_mitigation"] = error_mitigation.value
     return json.dumps(ionq_json)
 
 
 def get_user_agent():
     """Generates the user agent string which is helpful in identifying
     different tools in the internet. Valid user-agent ionq_client header that
     indicates the request is from qiskit_ionq along with the system, os,
```

### Comparing `qiskit-ionq-0.3.9/qiskit_ionq/ionq_backend.py` & `qiskit-ionq-0.4.0.dev0/qiskit_ionq/ionq_backend.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,17 +23,17 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """IonQ provider backends."""
 
 import abc
+from datetime import datetime
 import warnings
 
-import dateutil.parser
 from qiskit.providers import BackendV1 as Backend
 from qiskit.providers.models import BackendConfiguration
 from qiskit.providers.models.backendstatus import BackendStatus
 from qiskit.providers import Options
 
 from . import exceptions, ionq_client, ionq_job
 from .helpers import GATESET_MAP
@@ -46,14 +46,23 @@
     This class is a simple wrapper for IonQ hardware calibration data.
     """
 
     def __init__(self, data):
         self._data = data
 
     @property
+    def uuid(self):
+        """The ID of the calibration.
+
+        Returns:
+           str: The ID.
+        """
+        return self._data["id"]
+
+    @property
     def num_qubits(self):
         """The number of qubits available.
 
         Returns:
             int: A number of qubits.
         """
         return int(self._data["qubits"])
@@ -61,24 +70,24 @@
     @property
     def target(self):
         """The target calibrated hardware.
 
         Returns:
             str: The name of the target hardware backend.
         """
-        return self._data["target"]
+        return self._data["backend"]
 
     @property
     def calibration_time(self):
         """Time of the measurement, in UTC.
 
         Returns:
             datetime.datetime: A datetime object with the time.
         """
-        return dateutil.parser.isoparse(self._data["date"])
+        return datetime.fromtimestamp(self._data["date"])
 
     @property
     def fidelities(self):
         """Fidelity for single-qubit (1q) and two-qubit (2q) gates, and State
         Preparation and Measurement (spam) operations.
 
         Currently provides only mean fidelity; additional statistical data will
@@ -121,15 +130,15 @@
 class IonQBackend(Backend):
     """IonQ Backend base class."""
 
     _client = None
 
     @classmethod
     def _default_options(cls):
-        return Options(shots=1024, job_settings=None)
+        return Options(shots=1024, job_settings=None, error_mitigation=None)
 
     @property
     def client(self):
         """A lazily populated IonQ API Client.
 
         Returns:
             IonQClient: An instance of a REST API client
@@ -167,15 +176,16 @@
             url = credentials["url"]
         except KeyError as ex:
             raise exceptions.IonQCredentialsError(
                 "Credentials `url` not present in provider."
             ) from ex
 
         if url is None:
-            raise exceptions.IonQCredentialsError("Credentials `url` may not be None!")
+            raise exceptions.IonQCredentialsError(
+                "Credentials `url` may not be None!")
 
         return ionq_client.IonQClient(token, url, self._provider.custom_headers)
 
     # pylint: disable=missing-type-doc,missing-param-doc,arguments-differ,arguments-renamed
     def run(self, circuit, **kwargs):
         """Create and run a job on an IonQ Backend.
 
@@ -196,14 +206,21 @@
             RuntimeError: If a multi-experiment circuit was provided.
         """
         if isinstance(circuit, (list, tuple)):
             if len(circuit) > 1:
                 raise RuntimeError("Multi-experiment jobs are not supported!")
             circuit = circuit[0]
 
+        if not self.has_valid_mapping(circuit):
+            warnings.warn(
+                f"Circuit {circuit.name} is not measuring any qubits",
+                UserWarning,
+                stacklevel=2,
+            )
+
         for kwarg in kwargs:
             if not hasattr(self.options, kwarg):
                 warnings.warn(
                     f"Option {kwarg} is not used by this backend",
                     UserWarning,
                     stacklevel=2,
                 )
@@ -232,14 +249,32 @@
         return ionq_job.IonQJob(self, job_id, self.client)
 
     def retrieve_jobs(self, job_ids):
         """get a list of jobs from a specific backend, job id"""
 
         return [ionq_job.IonQJob(self, job_id, self.client) for job_id in job_ids]
 
+    def has_valid_mapping(self, circuit) -> bool:
+        """checks if the circuit has at least one
+        valid qubit -> bit measurement.
+
+        Args:
+            circuit (:class:`QuantumCircuit <qiskit.circuit.QuantumCircuit>`):
+                A Qiskit QuantumCircuit object.
+
+        Returns:
+            boolean: if the circuit has valid mappings
+        """
+        # Check if a qubit is measured
+        for instruction, _, cargs in circuit.data:
+            if instruction.name == "measure" and len(cargs):
+                return True
+        # If no mappings are found, return False
+        return False
+
     # TODO: Implement backend status checks.
     def status(self):
         """Return a backend status object to the caller.
 
         Returns:
             BackendStatus: the status of the backend.
         """
@@ -343,14 +378,15 @@
                 "backend_version": "0.0.1",
                 "simulator": True,
                 "local": False,
                 "coupling_map": None,
                 "description": "IonQ simulator",
                 "basis_gates": GATESET_MAP[gateset],
                 "memory": False,
+                # Varied based on noise model, but enforced server-side.
                 "n_qubits": 32,
                 "conditional": False,
                 "max_shots": 1,
                 "max_experiments": 1,
                 "open_pulse": False,
                 "gates": [{"name": "TODO", "parameters": [], "qasm_def": "TODO"}],
             }
```

### Comparing `qiskit-ionq-0.3.9/qiskit_ionq/ionq_client.py` & `qiskit-ionq-0.4.0.dev0/qiskit_ionq/ionq_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 from .exceptions import IonQRetriableError
 
 
 class IonQClient:
     """IonQ API Client
 
     Attributes:
-        _url(str): A URL base to use for API calls, e.g. ``"https://api.ionq.co/v0.1"``
+        _url(str): A URL base to use for API calls, e.g. ``"https://api.ionq.co/v0.3"``
         _token(str): An API Access Token to use with the IonQ API.
         _custom_headers(dict): Extra headers to add to the request.
     """
 
     def __init__(self, token=None, url=None, custom_headers=None):
         self._token = token
         self._custom_headers = custom_headers or {}
@@ -149,63 +149,79 @@
             IonQAPIError: When the API returns a non-200 status code.
 
         Returns:
             dict: A :mod:`requests <requests>` response :meth:`json <requests.Response.json>` dict.
         """
         req_path = self.make_path("jobs", job_id)
         res = requests.delete(req_path, headers=self.api_headers, timeout=30)
-        exceptions.IonQAPIError.raise_for_status(requests)
+        exceptions.IonQAPIError.raise_for_status(res)
         return res.json()
 
     @retry(exceptions=IonQRetriableError, max_delay=60, backoff=2, jitter=1)
     def get_calibration_data(self, backend_name: str) -> dict:
         """Retrieve calibration data for a specified backend.
 
         Args:
             backend_name (str): The IonQ backend to fetch data for.
 
         Calibration::
 
             {
-                "pages": <int>,
-                "calibrations": [
-                    {
-                        "id": <str>,
-                        "date": <int>,
-                        "target": <str>,
-                        "qubits": <int>,
-                        "connectivity": [<int>, ...],
-                        "fidelity": {
-                            "spam": {
-                                "mean": <int>,
-                                "stderr": <int>
-                            }
-                        },
-                        "timing": {
-                            "readout": <int>,
-                            "reset": <int>
-                        }
+                "id": <str>,
+                "calibration_time": <int>,
+                "target": <str>,
+                "num_qubits": <int>,
+                "connectivity": [<int>, ...],
+                "fidelity": {
+                    "spam": {
+                        "mean": <int>,
+                        "stderr": <int>
                     }
-                ]
+                },
+                "timing": {
+                    "readout": <int>,
+                    "reset": <int>
+                }
             }
 
         Returns:
             dict: A dictionary of an IonQ backend's calibration data.
         """
-        req_path = self.make_path("calibrations")
+        req_path = self.make_path("/".join([
+            "characterizations/backends",
+            backend_name[5:],
+            "current"
+        ]))
         res = requests.get(req_path, headers=self.api_headers, timeout=30)
-        exceptions.IonQAPIError.raise_for_status(requests)
+        exceptions.IonQAPIError.raise_for_status(res)
+
+        return res.json()
 
-        # Get calibrations and filter down to the target
-        response = res.json()
-        calibrations = response.get("calibrations") or []
-        calibrations = [c for c in calibrations if c.get("target") == backend_name]
-
-        # If nothing was found, just return None.
-        if len(calibrations) == 0:
-            return None
+    @retry(exceptions=IonQRetriableError, max_delay=60, backoff=2, jitter=1)
+    def get_results(self, job_id: str, aggregation=None):
+        """Retrieve job results from the IonQ API.
 
-        # Calibrations are in most recent order in the response, so get the first.
-        return calibrations[0]
+        The returned JSON dict will only have data if job has completed.
+
+        Args:
+            job_id (str): The ID of a job to retrieve.
+            aggregation (str): type of results aggregation
+
+        Raises:
+            IonQAPIError: When the API returns a non-200 status code.
+
+        Returns:
+            dict: A :mod:`requests <requests>` response :meth:`json <requests.Response.json>` dict.
+        """
+
+        params = {}
+
+        if aggregation:
+            params["aggregation"] = aggregation
+
+        req_path = self.make_path("jobs", job_id, "results")
+        res = requests.get(req_path, params, headers=self.api_headers, timeout=30)
+        exceptions.IonQAPIError.raise_for_status(res)
+        return res.json()
 
 
 __all__ = ["IonQClient"]
```

### Comparing `qiskit-ionq-0.3.9/qiskit_ionq/ionq_gates.py` & `qiskit-ionq-0.4.0.dev0/qiskit_ionq/ionq_gates.py`

 * *Files identical despite different names*

### Comparing `qiskit-ionq-0.3.9/qiskit_ionq/ionq_job.py` & `qiskit-ionq-0.4.0.dev0/qiskit_ionq/ionq_job.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,31 +37,58 @@
 
 import warnings
 import numpy as np
 
 from qiskit.providers import JobV1, jobstatus
 from qiskit.providers.exceptions import JobTimeoutError
 from .ionq_result import IonQResult as Result
+from .constants import AggregationType
 from .helpers import decompress_metadata_string_to_dict
 
 
 from . import constants, exceptions
 
 
-def _build_counts(result, use_sampler=False, sampler_seed=None):
+def map_output(data, clbits, num_qubits):
+    """Map histogram according to measured bits"""
+
+    if not clbits:
+        return {}
+
+    mapped_output = {}
+
+    def get_bitvalue(bitstring, bit):
+        if bit is not None and 0 <= bit < len(bitstring):
+            return bitstring[bit]
+        return '0'
+
+    for value, probability in data.items():
+        bitstring = bin(int(value))[2:].rjust(num_qubits, "0")[::-1]
+
+        outvalue = int(''.join([get_bitvalue(bitstring, bit) for bit in clbits])[::-1], 2)
+
+        mapped_output[outvalue] = mapped_output.get(outvalue, 0) + probability
+
+    return mapped_output
+
+
+def _build_counts(data, num_qubits, clbits, shots, use_sampler=False, sampler_seed=None):
     """Map IonQ's ``counts`` onto qiskit's ``counts`` model.
 
     .. NOTE:: For simulator jobs, this method builds counts using a randomly
         generated sampling of the probabilities returned from the API. Because
         this is a random process, rebuilding the results object (by e.g.
         restarting the kernel and getting the job again) without providing a
         sampler_seed in the run method may result in slightly different counts.
 
     Args:
-        result (dict): A REST API response.
+        data (dict): histogram as returned by the API.
+        num_qubits (int): number of qubits
+        clbits (List[int]): array of classical bits for measurements
+        shots (int): number of shots
         use_sampler (bool): for counts generation, whether to use
             simple shots * probabilities (for qpu) or a sampler (for simulator)
         sampler_seed (int): ability to provide a seed for the randomness in the
             sampler for repeatable results. passed as
             `np.random.RandomState(seed)`. If none, `np.random` is used
 
     Returns:
@@ -71,39 +98,19 @@
             simulator work.
 
     Raises:
         IonQJobError: In the event that ``result`` has missing or invalid job
             properties.
     """
     # Short circuit when we don't have all the information we need.
-    if not result:
-        raise exceptions.IonQJobError("Cannot remap counts without an API response!")
-
-    # Check for required result dict keys:
-    if "qubits" not in result:
-        raise exceptions.IonQJobError("Cannot remap counts without qubits!")
-    if "metadata" not in result:
-        raise exceptions.IonQJobError("Cannot remap counts without metadata!")
-    if "data" not in result:
-        raise exceptions.IonQJobError("Cannot remap counts without result data!")
-
-    # Pull metadata, histogram, and num_qubits to perform the mapping.
-    metadata = result["metadata"]
-    num_qubits = result["qubits"]
-
-    # Get shot count.
-    shots = metadata.get("shots", "1024")
-    shots = (
-        int(shots) if shots.isdigit() else 1024
-    )  # We do this in case shots was 0 or None.
+    if not data:
+        raise exceptions.IonQJobError("Cannot remap counts without data!")
 
     # Grab the mapped output from response.
-    output_probs = (result["data"].get("registers", {}) or {}).get("meas_mapped", {})
-    if not output_probs:
-        output_probs = result["data"].get("histogram", {})
+    output_probs = map_output(data, clbits, num_qubits)
 
     sampled = {}
     if use_sampler:
         rand = np.random.RandomState(sampler_seed)
         outcomes, weights = zip(*output_probs.items())
         weights = np.array(weights).astype(float)
         # just in case the sum isn't exactly 1 — sometimes the API returns
@@ -146,26 +153,25 @@
     methods on sub-classe instances of IonQBackend to create and retrieve jobs
     (both methods return a job instance).
 
     Attributes:
         circuit(:mod:`QuantumCircuit <qiskit.QuantumCircuit>`): A possibly ``None``
             Qiskit quantum circuit.
         _result(:class:`Result <qiskit.result.Result>`):
-            The actual Qiskit Result of this job.
-            This attribute is only populated when :meth:`status` is called and
-            the job has reached a one of the status values in ``JOB_FINAL_STATES``
-            from ``qiskit.providers.jobstatus``
+            The actual Qiskit Result of this job when done.
     """
 
     def __init__(self, backend, job_id, client=None, circuit=None, passed_args=None):
         super().__init__(backend, job_id)
         self._client = client or backend.client
         self._passed_args = passed_args or {"shots": 1024, "sampler_seed": None}
         self._result = None
         self._status = None
+        self._execution_time = None
+        self._metadata = {}
 
         if circuit is not None:
             self.circuit = circuit
             self._status = jobstatus.JobStatus.INITIALIZING
         else:  # retrieve existing job
             self.circuit = None
             self._status = jobstatus.JobStatus.INITIALIZING
@@ -223,15 +229,15 @@
             circuit (str or QuantumCircuit or int or None): Optional.
 
         Returns:
             tuple(dict[str, float], dict[str, float]): A tuple counts, probabilities.
         """
         return self.result().get_probabilities()
 
-    def result(self):
+    def result(self, aggregation: AggregationType = None):
         """Retrieve job result data.
 
         .. NOTE::
            :attr:`_result` is populated by :meth:`status`, when the job
            status has reached a "final" state.
 
         This method calls the
@@ -245,37 +251,46 @@
             IonQJobError: If the job has reached a final state but
                 the job itself was never converted to a
                 :class:`Result <qiskit.result.Result>`.
 
         Returns:
             Result: A Qiskit :class:`Result <qiskit.result.Result>` representation of this job.
         """
-        # Short-circuit if we have already cached the result for this job.
-        if self._result is not None:
-            return self._result
+        # TODO: cache results by aggregation type
+
+        if aggregation is not None and not isinstance(aggregation, AggregationType):
+            warnings.warn("Invalid aggregation type")
 
         # Wait for the job to complete.
         try:
             self.wait_for_final_state()
         except JobTimeoutError as ex:
             raise exceptions.IonQJobTimeoutError(
                 "Timed out waiting for job to complete."
             ) from ex
 
+        if self._status is jobstatus.JobStatus.DONE:
+            agg_type = (
+                aggregation.value
+                if isinstance(aggregation, AggregationType)
+                else aggregation
+            )
+            response = self._client.get_results(self._job_id, agg_type)
+            self._result = self._format_result(response)
+
         return self._result
 
     def status(self):
         """Retrieve the status of a job
 
-        This will also populate :attr:`_result` with a :class:`Result <qiskit.result.Result>`
-        object, if the job's status has reached a "final" state.
-
         Raises:
             IonQJobError: If the IonQ job status was unknown or otherwise
                 unmappable to a qiskit job status.
+            IonQJobFailureError: If the job fails
+            IonQJobStateError: If the job was cancelled
 
         Returns:
             JobStatus: An enum value from Qiskit's :class:`JobStatus <qiskit.providers.JobStatus>`.
         """
         # Return early if we have no job id yet.
         if self._job_id is None:
             return self._status
@@ -306,22 +321,46 @@
         try:
             self._status = jobstatus.JobStatus[status_enum.value]
         except KeyError as ex:
             raise exceptions.IonQJobError(
                 f"Qiskit has no JobStatus named '{status_enum}'"
             ) from ex
 
-        # if done, also put the result on the job obj
-        # so we don't have to make an API call again if user wants results
         if self._status in jobstatus.JOB_FINAL_STATES:
-            self._result = self._format_result(response)
+            self._metadata = response.get("metadata") or {}
+
+        if self._status == jobstatus.JobStatus.DONE:
+            self._num_qubits = response.get("qubits")
+            default_map = list(range(self._num_qubits))
+            self._clbits = (response.get("registers") or {}).get("meas_mapped", default_map)
+            self._execution_time = response.get("execution_time") / 1000
+
+        if self._status == jobstatus.JobStatus.ERROR:
+            failure = response.get("failure") or {}
+            failure_type = failure.get("code", "")
+            failure_message = failure.get("error", "")
+            error_message = (
+                f"Unable to retreive result for job {self.job_id()}. "
+                f'Failure from IonQ API "{failure_type}: {failure_message}"'
+            )
+            raise exceptions.IonQJobFailureError(error_message)
+
+        if self._status == jobstatus.JobStatus.CANCELLED:
+            error_message = (
+                f'Unable to retreive result for job {self.job_id()}. Job was cancelled"'
+            )
+            raise exceptions.IonQJobStateError(error_message)
+
+        if "warning" in response and "messages" in response["warning"]:
+            for warning in response["warning"]["messages"]:
+                warnings.warn(warning)
 
         return self._status
 
-    def _format_result(self, result):
+    def _format_result(self, data):
         """Translate IonQ's result format into a qiskit Result instance.
 
         TODO: If result is (failure, cancelled), this method may fail.
 
         Args:
             result (dict): A JSON body response from a REST API call.
 
@@ -339,71 +378,55 @@
         backend_version = backend.configuration().backend_version
         is_ideal_simulator = (
             backend_name == "ionq_simulator" and backend.options.noise_model == "ideal"
         )
 
         # Format the inner result payload.
         success = self._status == jobstatus.JobStatus.DONE
-        time_taken = (result.get("execution_time") / 1000) if success else None
-        metadata = result.get("metadata") or {}
+        metadata = self._metadata
         sampler_seed = (
             int(metadata.get("sampler_seed", ""))
             if metadata.get("sampler_seed", "").isdigit()
             else None
         )
         qiskit_header = decompress_metadata_string_to_dict(
             metadata.get("qiskit_header", None)
         )
+
+        shots = int(
+            metadata.get("shots") if metadata.get("shots").isdigit() else 1024
+        )
         job_result = {
             "data": {},
-            "shots": int(
-                metadata.get("shots") if metadata.get("shots").isdigit() else 1024
-            ),
+            "shots": shots,
             "header": qiskit_header or {},
             "success": success,
         }
         if self._status == jobstatus.JobStatus.DONE:
             (counts, probabilities) = _build_counts(
-                result, use_sampler=is_ideal_simulator, sampler_seed=sampler_seed
+                data, self._num_qubits, self._clbits, shots,
+                use_sampler=is_ideal_simulator, sampler_seed=sampler_seed
             )
             job_result["data"] = {
                 "counts": counts,
                 "probabilities": probabilities,
                 # Qiskit/experiments relies on this being present in this location in the
                 # ExperimentData class.
                 "metadata": qiskit_header or {},
             }
-        if self._status == jobstatus.JobStatus.ERROR:
-            failure = result.get("failure") or {}
-            failure_type = failure.get("code", "")
-            failure_message = failure.get("error", "")
-            error_message = (
-                f"Unable to retreive result for job {self.job_id()}. "
-                f'Failure from IonQ API "{failure_type}: {failure_message}"'
-            )
-            raise exceptions.IonQJobFailureError(error_message)
-        if self._status == jobstatus.JobStatus.CANCELLED:
-            error_message = (
-                f'Unable to retreive result for job {self.job_id()}. Job was cancelled"'
-            )
-            raise exceptions.IonQJobStateError(error_message)
-
-        if "warning" in job_result and "messages" in job_result["warning"]:
-            for warning in job_result["warning"]["messages"]:
-                warnings.warn(warning)
 
         # Create a qiskit result to express the IonQ job result data.
         backend = self.backend()
         return Result.from_dict(
             {
                 "results": [job_result],
                 "job_id": self.job_id(),
                 "backend_name": backend_name,
                 "backend_version": backend_version,
                 "qobj_id": metadata.get("qobj_id"),
                 "success": success,
-                "time_taken": time_taken,
+                "time_taken": self._execution_time,
             }
         )
 
 
 __all__ = ["IonQJob"]
```

### Comparing `qiskit-ionq-0.3.9/qiskit_ionq/ionq_provider.py` & `qiskit-ionq-0.4.0.dev0/qiskit_ionq/ionq_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,28 +40,28 @@
 def resolve_credentials(token: str = None, url: str = None):
     """Resolve credentials for use in IonQ Client API calls.
 
     If the provided ``token`` and ``url`` are both ``None``, then these values
     are loaded from the ``QISKIT_IONQ_API_TOKEN`` and ``QISKIT_IONQ_API_URL``
     environment variables, respectively.
 
-    If no url is discovered, then ``https://api.ionq.co/v0.1`` is used.
+    If no url is discovered, then ``https://api.ionq.co/v0.3`` is used.
 
     Args:
         token (str): IonQ API access token.
         url (str, optional): IonQ API url. Defaults to ``None``.
 
     Returns:
         dict[str]: A dict with "token" and "url" keys, for use by a client.
     """
     env_token = os.environ.get("QISKIT_IONQ_API_TOKEN")
     env_url = os.environ.get("QISKIT_IONQ_API_URL")
     return {
         "token": token or env_token,
-        "url": url or env_url or "https://api.ionq.co/v0.1",
+        "url": url or env_url or "https://api.ionq.co/v0.3",
     }
 
 
 class IonQProvider:
     """Provider for interacting with IonQ backends
 
     Attributes:
```

### Comparing `qiskit-ionq-0.3.9/qiskit_ionq/ionq_result.py` & `qiskit-ionq-0.4.0.dev0/qiskit_ionq/ionq_result.py`

 * *Files identical despite different names*

### Comparing `qiskit-ionq-0.3.9/qiskit_ionq/version.py` & `qiskit-ionq-0.4.0.dev0/qiskit_ionq/version.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 import pathlib
 import subprocess
 from typing import List
 
 pkg_parent = pathlib.Path(__file__).parent.parent.absolute()
 
 # major, minor, micro
-VERSION_INFO = ".".join([str(x) for x in (0, 3, 9)])
+VERSION_INFO = ".".join(map(str, (0, 4, 0, "dev0")))
 
 
 def _minimal_ext_cmd(cmd: List[str]) -> bytes:
     # construct minimal environment
     env = {
         "LANGUAGE": "C",  # LANGUAGE is used on win32
         "LANG": "C",
@@ -86,15 +86,17 @@
     try:
         release = _minimal_ext_cmd(["git", "tag", "-l", "--points-at", "HEAD"])
     except Exception:  # pylint: disable=broad-except
         return full_version
 
     if not release:
         git_revision = git_version()
-        full_version += ".dev0+" + git_revision[:7]
+        if ".dev" not in full_version:
+            full_version += ".dev0"
+        full_version += "+" + git_revision[:7]
 
     return full_version
 
 
 __version__ = get_version_info()
 
 __all__ = ["__version__"]
```

### Comparing `qiskit-ionq-0.3.9/qiskit_ionq.egg-info/PKG-INFO` & `qiskit-ionq-0.4.0.dev0/qiskit_ionq.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-ionq
-Version: 0.3.9
+Version: 0.4.0.dev0
 Summary: Qiskit provider for IonQ backends
 Home-page: https://github.com/qiskit-partners/qiskit-ionq
 Author: IonQ
 Author-email: info@ionq.com
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/qiskit-partners/qiskit-ionq/issues
 Project-URL: Source Code, https://github.com/qiskit-partners/qiskit-ionq
@@ -97,30 +97,35 @@
 ### Submitting a Circuit
 
 Once a backend has been specified, it may be used to submit circuits.
 For example, running a Bell State:
 
 ```python
 from qiskit import QuantumCircuit
+from qiskit_ionq.constants import AggregationType
 
 # Create a basic Bell State circuit:
 qc = QuantumCircuit(2, 2)
 qc.h(0)
 qc.cx(0, 1)
 qc.measure([0, 1], [0, 1])
 
 # Run the circuit on IonQ's platform:
 job = simulator_backend.run(qc)
 
 # Print the results.
-print(job.get_counts())
+print(job.result().get_counts())
+
+# Get results with a different aggregation method when symmetrization
+# is applied as an error mitigation strategy
+print(job.result(AggregationType.AVERAGE).get_counts())
 
 # The simulator specifically provides the the ideal probabilities and creates
 # counts by sampling from these probabilities. The raw probabilities are also accessible:
-print(job.get_probabilities())
+print(job.result().get_probabilities())
 ```
 
 ### Basis gates and transpilation
 
 The IonQ provider provides access to the full IonQ Cloud backend, which includes its own transpilation and compilation pipeline. As such, IonQ provider backends have a broad set of "basis gates" that they will accept — effectively anything the IonQ API will accept. They are `ccx, ch, cnot, cp, crx, cry, crz, csx, cx, cy, cz, h, i, id, mcp, mct, mcx, measure, p, rx, rxx, ry, ryy, rz, rzz, s, sdg, swap, sx, sxdg, t, tdg, toffoli, x, y` and `z`.
 
 If you have circuits that you'd like to run on IonQ backends that use other gates than this (`u` or `iswap` for example), you will either need to manually rewrite the circuit to only use the above list, or use the Qiskit transpiler, per the example below. Please note that not all circuits can be automatically transpiled.
```

### Comparing `qiskit-ionq-0.3.9/qiskit_ionq.egg-info/SOURCES.txt` & `qiskit-ionq-0.4.0.dev0/qiskit_ionq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qiskit-ionq-0.3.9/setup.py` & `qiskit-ionq-0.4.0.dev0/setup.py`

 * *Files identical despite different names*

### Comparing `qiskit-ionq-0.3.9/test/test_mock.py` & `qiskit-ionq-0.4.0.dev0/test/test_mock.py`

 * *Files identical despite different names*

