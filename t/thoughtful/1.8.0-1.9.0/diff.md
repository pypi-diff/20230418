# Comparing `tmp/thoughtful-1.8.0.tar.gz` & `tmp/thoughtful-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thoughtful-1.8.0.tar", max compression
+gzip compressed data, was "thoughtful-1.9.0.tar", max compression
```

## Comparing `thoughtful-1.8.0.tar` & `thoughtful-1.9.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     4450 2022-10-21 22:43:56.240682 thoughtful-1.8.0/README.md
--rw-r--r--   0        0        0     2072 2022-10-21 22:43:56.274263 thoughtful-1.8.0/pyproject.toml
--rw-r--r--   0        0        0      184 2022-10-21 22:43:56.242740 thoughtful-1.8.0/supervisor/__init__.py
--rw-r--r--   0        0        0       54 2022-10-21 22:43:56.242850 thoughtful-1.8.0/supervisor/__version__.py
--rw-r--r--   0        0        0     5381 2022-10-21 22:43:56.242992 thoughtful-1.8.0/supervisor/default_instances.py
--rw-r--r--   0        0        0      888 2022-10-21 22:43:56.243100 thoughtful-1.8.0/supervisor/dynamic.py
--rw-r--r--   0        0        0     5785 2022-10-21 22:43:56.243196 thoughtful-1.8.0/supervisor/main_context.py
--rw-r--r--   0        0        0    13010 2022-10-21 22:43:56.243430 thoughtful-1.8.0/supervisor/manifest.py
--rw-r--r--   0        0        0        0 2022-10-21 22:43:56.243473 thoughtful-1.8.0/supervisor/py.typed
--rw-r--r--   0        0        0     6543 2022-10-21 22:43:56.243630 thoughtful-1.8.0/supervisor/recorder.py
--rw-r--r--   0        0        0        0 2022-10-21 22:43:56.243730 thoughtful-1.8.0/supervisor/reporting/__init__.py
--rw-r--r--   0        0        0     1010 2022-10-21 22:43:56.243862 thoughtful-1.8.0/supervisor/reporting/record.py
--rw-r--r--   0        0        0     2006 2022-10-21 22:43:56.243991 thoughtful-1.8.0/supervisor/reporting/report.py
--rw-r--r--   0        0        0     6809 2022-10-21 22:43:56.244136 thoughtful-1.8.0/supervisor/reporting/report_builder.py
--rw-r--r--   0        0        0      659 2022-10-21 22:43:56.244238 thoughtful-1.8.0/supervisor/reporting/status.py
--rw-r--r--   0        0        0     1496 2022-10-21 22:43:56.244336 thoughtful-1.8.0/supervisor/reporting/step_report.py
--rw-r--r--   0        0        0     1541 2022-10-21 22:43:56.244436 thoughtful-1.8.0/supervisor/reporting/timed_report.py
--rw-r--r--   0        0        0     1870 2022-10-21 22:43:56.244540 thoughtful-1.8.0/supervisor/reporting/timer.py
--rw-r--r--   0        0        0     8197 2022-10-21 22:43:56.244670 thoughtful-1.8.0/supervisor/step_context.py
--rw-r--r--   0        0        0     8140 2022-10-21 22:43:56.244825 thoughtful-1.8.0/supervisor/step_decorator_factory.py
--rw-r--r--   0        0        0     1764 2022-10-21 22:43:56.244933 thoughtful-1.8.0/supervisor/streaming_callback.py
--rw-r--r--   0        0        0     5630 2022-10-21 22:43:56.801440 thoughtful-1.8.0/setup.py
--rw-r--r--   0        0        0     5865 2022-10-21 22:43:56.801748 thoughtful-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0     4450 2022-10-21 22:43:49.374262 thoughtful-1.9.0/README.md
+-rw-r--r--   0        0        0     2088 2022-10-21 22:43:49.405760 thoughtful-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0      184 2022-10-21 22:43:49.375159 thoughtful-1.9.0/supervisor/__init__.py
+-rw-r--r--   0        0        0       54 2022-10-21 22:43:49.375253 thoughtful-1.9.0/supervisor/__version__.py
+-rw-r--r--   0        0        0     5370 2022-10-21 22:43:49.375384 thoughtful-1.9.0/supervisor/default_instances.py
+-rw-r--r--   0        0        0      888 2022-10-21 22:43:49.375490 thoughtful-1.9.0/supervisor/dynamic.py
+-rw-r--r--   0        0        0     7099 2022-10-21 22:43:49.375636 thoughtful-1.9.0/supervisor/main_context.py
+-rw-r--r--   0        0        0    13010 2022-10-21 22:43:49.375863 thoughtful-1.9.0/supervisor/manifest.py
+-rw-r--r--   0        0        0        0 2022-10-21 22:43:49.375905 thoughtful-1.9.0/supervisor/py.typed
+-rw-r--r--   0        0        0     6543 2022-10-21 22:43:49.376069 thoughtful-1.9.0/supervisor/recorder.py
+-rw-r--r--   0        0        0        0 2022-10-21 22:43:49.376170 thoughtful-1.9.0/supervisor/reporting/__init__.py
+-rw-r--r--   0        0        0     1010 2022-10-21 22:43:49.376288 thoughtful-1.9.0/supervisor/reporting/record.py
+-rw-r--r--   0        0        0     2006 2022-10-21 22:43:49.376417 thoughtful-1.9.0/supervisor/reporting/report.py
+-rw-r--r--   0        0        0     6809 2022-10-21 22:43:49.376554 thoughtful-1.9.0/supervisor/reporting/report_builder.py
+-rw-r--r--   0        0        0      659 2022-10-21 22:43:49.376648 thoughtful-1.9.0/supervisor/reporting/status.py
+-rw-r--r--   0        0        0     1496 2022-10-21 22:43:49.376743 thoughtful-1.9.0/supervisor/reporting/step_report.py
+-rw-r--r--   0        0        0     1541 2022-10-21 22:43:49.376843 thoughtful-1.9.0/supervisor/reporting/timed_report.py
+-rw-r--r--   0        0        0     1870 2022-10-21 22:43:49.376932 thoughtful-1.9.0/supervisor/reporting/timer.py
+-rw-r--r--   0        0        0     8197 2022-10-21 22:43:49.377063 thoughtful-1.9.0/supervisor/step_context.py
+-rw-r--r--   0        0        0     8140 2022-10-21 22:43:49.377227 thoughtful-1.9.0/supervisor/step_decorator_factory.py
+-rw-r--r--   0        0        0     1764 2022-10-21 22:43:49.377339 thoughtful-1.9.0/supervisor/streaming_callback.py
+-rw-r--r--   0        0        0     5653 2022-10-21 22:43:49.916624 thoughtful-1.9.0/setup.py
+-rw-r--r--   0        0        0     5902 2022-10-21 22:43:49.916929 thoughtful-1.9.0/PKG-INFO
```

### Comparing `thoughtful-1.8.0/README.md` & `thoughtful-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `thoughtful-1.8.0/pyproject.toml` & `thoughtful-1.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "thoughtful"
-version = "1.8.0"
+version = "1.9.0"
 description = "Supervisor is a Workflow Engine for Digital Workers that generates a detailed telemetric log at runtime called a Work Report"
 authors = ["Thoughtful Automation <engineering@thoughtfulautomation.com>"]
 license = "MIT"
 readme = 'README.md'
 homepage = "https://thoughtfulautomation.com"
 repository = "https://github.com/thoughtful-automation/supervisor"
 documentation = "https://thoughtful-automation.github.io/supervisor"
@@ -34,14 +34,15 @@
 pyconfs = "^0.5.5"
 pydantic = "^1.8.2"
 pre-commit = "^2.17.0"
 pydantic-yaml = "^0.6.3"
 isodate = "^0.6.1"
 boto3 = "^1.24.64"
 aws-requests-auth = "^0.4.3"
+moto = "^4.0.5"
 
 [tool.poetry.dev-dependencies]
 mkdocs = "^1.2.3"
 datamodel-code-generator = "^0.11.14"
 mkdocstrings = "^0.16.2"
 pytest = "^6.2.5"
 pytest-cov = "^2.12.1"
```

### Comparing `thoughtful-1.8.0/supervisor/default_instances.py` & `thoughtful-1.9.0/supervisor/default_instances.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     - a ``StepContext`` named ``step_context``,
     - a function to set step statuses called ``set_step_status``,
     - and a function to set record statuses called ``set_record_status``.
 
 See the quickstart for, well, quickstarts on each of these methods.
 """
 
+
 import logging
 import os
 import pathlib
 import warnings
 from typing import Optional, Union
 from urllib.parse import urlparse
 
@@ -60,16 +61,15 @@
 
 #: Expose the report builder's ability to override a step's record's status as a
 #: top-level call. Exposes ``report_builder.set_record_status``.
 set_record_status = report_builder.set_record_status
 
 # If callback url is in environment, we will stream to that url
 streaming_callback: Optional[StreamingCallback] = None
-callback_url = os.environ.get("SUPERVISOR_CALLBACK_URL")
-if callback_url:
+if callback_url := os.environ.get("SUPERVISOR_CALLBACK_URL"):
     credentials = boto3.Session().get_credentials()
     host = urlparse(callback_url).hostname
     aws_auth = AWSRequestsAuth(
         aws_access_key=credentials.access_key,
         aws_secret_access_key=credentials.secret_key,
         aws_token=credentials.token,
         aws_host=host,
```

### Comparing `thoughtful-1.8.0/supervisor/dynamic.py` & `thoughtful-1.9.0/supervisor/dynamic.py`

 * *Files identical despite different names*

### Comparing `thoughtful-1.8.0/supervisor/main_context.py` & `thoughtful-1.9.0/supervisor/main_context.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,17 +12,21 @@
 generated at the end of the process.
 """
 
 from __future__ import annotations
 
 import datetime
 import logging
+import os
 import pathlib
 from types import TracebackType
-from typing import Callable, Optional, Type, Union
+from typing import Callable, List, Optional, Type, Union
+from urllib.parse import urlparse
+
+import boto3
 
 from supervisor.manifest import Manifest
 from supervisor.recorder import Recorder
 from supervisor.reporting.report_builder import ReportBuilder
 from supervisor.reporting.status import Status
 
 logger = logging.getLogger(__name__)
@@ -79,14 +83,15 @@
                 parameters: the current context (as the `MainContext` instance)
                 and the `Report` generated from this digital worker's run.
         """
         self.report_builder = report_builder
         self.recorder = recorder
         self.manifest_path = pathlib.Path(manifest)
         self.output_path = pathlib.Path(output_dir)
+
         self.callback = callback
 
     def __enter__(self) -> MainContext:
         """
         Logic for when this context is first started. Attempts to load the
         manifest and returns itself as the context.
 
@@ -133,18 +138,49 @@
         manifest_json_path = self.output_path / "manifest.json"
         Manifest.yaml_to_json(self.manifest_path, manifest_json_path)
 
         # Run the user-defined callback
         if self.callback:
             self.callback(self, work_report)
 
+        # Upload output files to S3
+        if upload_uri := os.getenv("SUPERVISOR_ARTIFACT_UPLOAD_URI"):
+            try:
+                self.upload_output_files_to_s3(upload_uri)
+            except Exception:
+                logger.exception("Failed to upload output files to S3")
+        else:
+            logger.warning(
+                "SUPERVISOR_ARTIFACT_UPLOAD_URI is not set. Artifacts"
+                " will not be uploaded to S3."
+            )
+
         # Explicitly return false so that the parent caller above
         # this context sees the exception (if any)
         return False
 
+    def upload_output_files_to_s3(self, upload_uri: str) -> None:
+        """
+        It uploads all files in the output directory to S3. It requires the
+        environment variable `SUPERVISOR_ARTIFACT_UPLOAD_URI` to be set with
+        the S3 URI to upload the files to.
+        """
+        s3_client = boto3.client("s3")
+        upload_uri = urlparse(upload_uri.strip())
+        bucket = upload_uri.hostname
+        path = upload_uri.path.strip("/")
+
+        for file in self.output_path.glob("*"):
+            try:
+                if file.is_file():
+                    obj = f"{path}/{file.name}" if path else file.name
+                    s3_client.upload_file(str(file), bucket, obj)
+            except Exception:
+                logger.exception(f"Failed to upload {file} to S3")
+
     def _safe_report_path(self, file_prefix: str) -> pathlib.Path:
         """
         A ``pathlib.Path`` instance that points to a new work report writable
         location that is safe across all OSes.
 
         Returns:
             pathlib.Path: The path to the new report to be written.
```

### Comparing `thoughtful-1.8.0/supervisor/manifest.py` & `thoughtful-1.9.0/supervisor/manifest.py`

 * *Files identical despite different names*

### Comparing `thoughtful-1.8.0/supervisor/recorder.py` & `thoughtful-1.9.0/supervisor/recorder.py`

 * *Files identical despite different names*

### Comparing `thoughtful-1.8.0/supervisor/reporting/record.py` & `thoughtful-1.9.0/supervisor/reporting/record.py`

 * *Files identical despite different names*

### Comparing `thoughtful-1.8.0/supervisor/reporting/report.py` & `thoughtful-1.9.0/supervisor/reporting/report.py`

 * *Files identical despite different names*

### Comparing `thoughtful-1.8.0/supervisor/reporting/report_builder.py` & `thoughtful-1.9.0/supervisor/reporting/report_builder.py`

 * *Files identical despite different names*

### Comparing `thoughtful-1.8.0/supervisor/reporting/status.py` & `thoughtful-1.9.0/supervisor/reporting/status.py`

 * *Files identical despite different names*

### Comparing `thoughtful-1.8.0/supervisor/reporting/step_report.py` & `thoughtful-1.9.0/supervisor/reporting/step_report.py`

 * *Files identical despite different names*

### Comparing `thoughtful-1.8.0/supervisor/reporting/timed_report.py` & `thoughtful-1.9.0/supervisor/reporting/timed_report.py`

 * *Files identical despite different names*

### Comparing `thoughtful-1.8.0/supervisor/reporting/timer.py` & `thoughtful-1.9.0/supervisor/reporting/timer.py`

 * *Files identical despite different names*

### Comparing `thoughtful-1.8.0/supervisor/step_context.py` & `thoughtful-1.9.0/supervisor/step_context.py`

 * *Files identical despite different names*

### Comparing `thoughtful-1.8.0/supervisor/step_decorator_factory.py` & `thoughtful-1.9.0/supervisor/step_decorator_factory.py`

 * *Files identical despite different names*

### Comparing `thoughtful-1.8.0/supervisor/streaming_callback.py` & `thoughtful-1.9.0/supervisor/streaming_callback.py`

 * *Files identical despite different names*

### Comparing `thoughtful-1.8.0/setup.py` & `thoughtful-1.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,23 +8,24 @@
 {'': ['*']}
 
 install_requires = \
 ['aws-requests-auth>=0.4.3,<0.5.0',
  'boto3>=1.24.64,<2.0.0',
  'chevron>=0.14.0,<0.15.0',
  'isodate>=0.6.1,<0.7.0',
+ 'moto>=4.0.5,<5.0.0',
  'pre-commit>=2.17.0,<3.0.0',
  'pyconfs>=0.5.5,<0.6.0',
  'pydantic-yaml>=0.6.3,<0.7.0',
  'pydantic>=1.8.2,<2.0.0',
  'pyyaml>=5.4.1']
 
 setup_kwargs = {
     'name': 'thoughtful',
-    'version': '1.8.0',
+    'version': '1.9.0',
     'description': 'Supervisor is a Workflow Engine for Digital Workers that generates a detailed telemetric log at runtime called a Work Report',
     'long_description': '# 👷 Supervisor\n\n<img\n  title="Supervisor"\n  alt="Supervisor — Github Header"\n  width="262px"\n  height="179.5px"\n  align="right"\n  src="https://user-images.githubusercontent.com/1096881/147704110-3116d1e3-c278-45d6-b99a-209faf2b17e0.png"\n/>\n\n> **:warning: NOTE**: *Supervisor* is quite new.\n> We welcome and encourage you to help shape future\n> development by [reporting issues][git:issues] and\n> [making suggestions][url:notion-feedback] 💖\n\n---\n<big>Supervisor is a <u>Workflow Engine</u> for Digital Workers that constructs\nand broadcasts a detailed and structured telemetric log, called the <u>Run Report</u>.\n\nSupervisor is quick and easy to implement:</big>\n\n```python\nfrom supervisor import step, step_scope, supervise, set_step_status\n\n\n# using the step decorator\n@step("2")\ndef step_2(name: str) -> bool:\n    print(f\'Hello {name}\')\n    return True # some condition\n\ndef main() -> None:\n    # using the step_scope context manager\n    with step_scope(\'1\') as step_context:\n        try:\n            print("Getting credentials")\n            # ...\n        except Exception as e:\n            # set step status using method\n            step_context.set_status("warning")\n\n    if not step_2():\n        # set step status using function\n        set_step_status("2", "fail")\n\nif __name__ == \'__main__\':\n    with supervise():\n        main()\n```\n\n[![pre-commit](https://github.com/thoughtful-automation/supervisor/workflows/pre-commit/badge.svg?event=push)](https://github.com/thoughtful-automation/supervisor/actions?query=workflow%3Apre-commit+event%3Apush)\n[![test](https://github.com/thoughtful-automation/supervisor/workflows/test/badge.svg?event=push)](https://github.com/thoughtful-automation/supervisor/actions?query=workflow%3Atest+event%3Apush)\n\n<small>Supervisor supports `Python ≥ 3.7.5`</small>\n\n:books: 👉️ **[Read the Docs][url:readthedocs]**\n\n## Table of Contents\n\n- [Install](#install)\n- [Documentation](#documentation)\n- [Contributing](#contributing)\n- [Resources](#resources)\n\n## Installing Supervisor\n\nAt this time, Supervisor is a private package hosted only on CodeArtifact.\n\n1. Authenticate with `CodeArtifact`:\n\n   ```bash\n   aws codeartifact login \\\n     --tool pip \\\n     --repository thoughtful-automation \\\n     --domain thoughtful-automation \\\n     --domain-owner XXXXXXXXXXXX \\\n     --region us-east-1\n   ```\n\n2. Pip install\n\n   ```bash\n   pip install t-supervisor\n   ```\n\n   > or install a specific version: `pip install "t-supervisor==0.4.0"`\n\n## Documentation available on [Read the Docs][url:readthedocs]\n\nSee the [Read the Docs][url:readthedocs].\n\n## Contributing\n\nContributions to Supervisor are welcomed!\n\nTo get started, see the [contributing guide](CONTRIBUTING.md).\n\n## Resources\n\nLinks to related code, documentation, and applications.\n\n[**🖥 Empower**][url:dwm]\n\n> The digital Workforce Manager (*DWM*)\n\n[**👷 Supervisor**][url:supervisor] (this repo)\n\n> The Workflow Engine for Digital Workers that constructs\nand broadcasts a detailed and structured telemetric log, called the Work Report\n\n[**:robot: Foundry**][url:otto]\n\n> The initialization tool for Digital Workers.\n\n[**🔀 Prospector**][url:prospector]\n\n> The design tool for Digital Workers.\n\n[**:books: Schema Library**][url:schema-lib]\n\n  > The JSON-Schema-defined documents used to validate the **Manifest** and the\n  > runtime **Work Report**\n\n[**:eagle: Department of Digital\n  Labor**][url:dodl]\n\n> Documentation and Specifications for building Digital Workers in *TA\'s\n> ecosystem*, and **Empower**\n\n---\n\n<div align="center">\n\n  Made with ❤️ by\n\n  [![Thoughtful Automation](https://user-images.githubusercontent.com/1096881/141985289-317c2e72-3c2d-4e6b-800a-0def1a05f599.png)][url:ta]\n\n</div>\n\n<!--  Link References -->\n\n[url:ta]: https://www.thoughtfulautomation.com/\n[url:dwm]: https://app.thoughtfulautomation.com/\n[url:supervisor]: https://github.com/Thoughtful-Automation/supervisor\n[url:otto]: https://github.com/Thoughtful-Automation/otto\n[url:prospector]: https://github.com/Thoughtful-Automation/prospector\n[url:dodl]: https://github.com/Thoughtful-Automation/dodl\n[url:schema-lib]: https://github.com/Thoughtful-Automation/schemas\n[url:notion-feedback]:\n    https://www.notion.so/thoughtfulautomation/Feedback-Feature-Requests-5716a73769ea4e0cba398e921eab44b5\n[git:issues]: https://github.com/Thoughtful-Automation/supervisor/issues\n[url:readthedocs]: https://thoughtful-supervisor.readthedocs-hosted.com/en/latest/\n',
     'author': 'Thoughtful Automation',
     'author_email': 'engineering@thoughtfulautomation.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://thoughtfulautomation.com',
```

### Comparing `thoughtful-1.8.0/PKG-INFO` & `thoughtful-1.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thoughtful
-Version: 1.8.0
+Version: 1.9.0
 Summary: Supervisor is a Workflow Engine for Digital Workers that generates a detailed telemetric log at runtime called a Work Report
 Home-page: https://thoughtfulautomation.com
 License: MIT
 Keywords: rpa,robot-framework,robocorp,automation
 Author: Thoughtful Automation
 Author-email: engineering@thoughtfulautomation.com
 Requires-Python: >=3.8,<4.0
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Security :: Cryptography
 Requires-Dist: aws-requests-auth (>=0.4.3,<0.5.0)
 Requires-Dist: boto3 (>=1.24.64,<2.0.0)
 Requires-Dist: chevron (>=0.14.0,<0.15.0)
 Requires-Dist: isodate (>=0.6.1,<0.7.0)
+Requires-Dist: moto (>=4.0.5,<5.0.0)
 Requires-Dist: pre-commit (>=2.17.0,<3.0.0)
 Requires-Dist: pyconfs (>=0.5.5,<0.6.0)
 Requires-Dist: pydantic (>=1.8.2,<2.0.0)
 Requires-Dist: pydantic-yaml (>=0.6.3,<0.7.0)
 Requires-Dist: pyyaml (>=5.4.1)
 Project-URL: Documentation, https://thoughtful-automation.github.io/supervisor
 Project-URL: Repository, https://github.com/thoughtful-automation/supervisor
```

