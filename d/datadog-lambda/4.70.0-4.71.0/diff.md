# Comparing `tmp/datadog_lambda-4.70.0.tar.gz` & `tmp/datadog_lambda-4.71.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datadog_lambda-4.70.0.tar", max compression
+gzip compressed data, was "datadog_lambda-4.71.0.tar", max compression
```

## Comparing `datadog_lambda-4.70.0.tar` & `datadog_lambda-4.71.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    11379 2022-08-04 20:47:28.483033 datadog_lambda-4.70.0/LICENSE
--rw-r--r--   0        0        0      394 2023-02-13 18:56:36.618770 datadog_lambda-4.70.0/LICENSE-3rdparty.csv
--rw-r--r--   0        0        0     3416 2023-02-13 18:56:36.619028 datadog_lambda-4.70.0/README.md
--rw-r--r--   0        0        0      538 2023-02-17 16:21:55.265937 datadog_lambda-4.70.0/datadog_lambda/__init__.py
--rw-r--r--   0        0        0     3653 2023-02-13 18:56:36.619460 datadog_lambda-4.70.0/datadog_lambda/api.py
--rw-r--r--   0        0        0     7232 2023-04-12 18:23:27.980925 datadog_lambda-4.70.0/datadog_lambda/cold_start.py
--rw-r--r--   0        0        0     1669 2023-02-13 18:56:36.620125 datadog_lambda-4.70.0/datadog_lambda/constants.py
--rw-r--r--   0        0        0     4769 2023-02-13 18:56:36.620241 datadog_lambda-4.70.0/datadog_lambda/dogstatsd.py
--rw-r--r--   0        0        0     1199 2023-02-13 18:56:36.620396 datadog_lambda-4.70.0/datadog_lambda/extension.py
--rw-r--r--   0        0        0      994 2022-08-04 20:47:28.483885 datadog_lambda-4.70.0/datadog_lambda/handler.py
--rw-r--r--   0        0        0     4707 2023-03-15 15:25:33.105333 datadog_lambda-4.70.0/datadog_lambda/metric.py
--rw-r--r--   0        0        0      139 2023-02-13 18:56:36.620660 datadog_lambda-4.70.0/datadog_lambda/module_name.py
--rw-r--r--   0        0        0     4641 2023-02-13 18:56:36.620808 datadog_lambda-4.70.0/datadog_lambda/patch.py
--rw-r--r--   0        0        0      243 2023-02-13 18:56:36.620890 datadog_lambda-4.70.0/datadog_lambda/stats_writer.py
--rw-r--r--   0        0        0      403 2023-02-13 18:56:36.620968 datadog_lambda-4.70.0/datadog_lambda/statsd_writer.py
--rw-r--r--   0        0        0     1751 2023-02-13 18:56:36.621061 datadog_lambda-4.70.0/datadog_lambda/tag_object.py
--rw-r--r--   0        0        0     3240 2023-02-13 18:56:36.621201 datadog_lambda-4.70.0/datadog_lambda/tags.py
--rw-r--r--   0        0        0     2522 2023-02-13 18:56:36.621290 datadog_lambda-4.70.0/datadog_lambda/thread_stats_writer.py
--rw-r--r--   0        0        0    45292 2023-04-12 18:23:27.981500 datadog_lambda-4.70.0/datadog_lambda/tracing.py
--rw-r--r--   0        0        0    12082 2023-04-12 18:23:27.981977 datadog_lambda-4.70.0/datadog_lambda/trigger.py
--rw-r--r--   0        0        0    13237 2023-03-15 15:25:33.105870 datadog_lambda-4.70.0/datadog_lambda/wrapper.py
--rw-r--r--   0        0        0     3449 2023-04-12 15:37:46.255654 datadog_lambda-4.70.0/datadog_lambda/xray.py
--rw-r--r--   0        0        0     1205 2023-04-12 18:30:35.665688 datadog_lambda-4.70.0/pyproject.toml
--rw-r--r--   0        0        0     4549 1970-01-01 00:00:00.000000 datadog_lambda-4.70.0/setup.py
--rw-r--r--   0        0        0     4912 1970-01-01 00:00:00.000000 datadog_lambda-4.70.0/PKG-INFO
+-rw-r--r--   0        0        0    11379 2022-08-04 20:47:28.483033 datadog_lambda-4.71.0/LICENSE
+-rw-r--r--   0        0        0      394 2023-02-13 18:56:36.618770 datadog_lambda-4.71.0/LICENSE-3rdparty.csv
+-rw-r--r--   0        0        0     3422 2023-04-17 18:27:24.481065 datadog_lambda-4.71.0/README.md
+-rw-r--r--   0        0        0      538 2023-02-17 16:21:55.265937 datadog_lambda-4.71.0/datadog_lambda/__init__.py
+-rw-r--r--   0        0        0     3653 2023-02-13 18:56:36.619460 datadog_lambda-4.71.0/datadog_lambda/api.py
+-rw-r--r--   0        0        0     7232 2023-04-12 18:23:27.980925 datadog_lambda-4.71.0/datadog_lambda/cold_start.py
+-rw-r--r--   0        0        0     1669 2023-02-13 18:56:36.620125 datadog_lambda-4.71.0/datadog_lambda/constants.py
+-rw-r--r--   0        0        0     4769 2023-02-13 18:56:36.620241 datadog_lambda-4.71.0/datadog_lambda/dogstatsd.py
+-rw-r--r--   0        0        0     1199 2023-02-13 18:56:36.620396 datadog_lambda-4.71.0/datadog_lambda/extension.py
+-rw-r--r--   0        0        0      994 2022-08-04 20:47:28.483885 datadog_lambda-4.71.0/datadog_lambda/handler.py
+-rw-r--r--   0        0        0     4707 2023-03-15 15:25:33.105333 datadog_lambda-4.71.0/datadog_lambda/metric.py
+-rw-r--r--   0        0        0      139 2023-02-13 18:56:36.620660 datadog_lambda-4.71.0/datadog_lambda/module_name.py
+-rw-r--r--   0        0        0     4641 2023-02-13 18:56:36.620808 datadog_lambda-4.71.0/datadog_lambda/patch.py
+-rw-r--r--   0        0        0      243 2023-02-13 18:56:36.620890 datadog_lambda-4.71.0/datadog_lambda/stats_writer.py
+-rw-r--r--   0        0        0      403 2023-02-13 18:56:36.620968 datadog_lambda-4.71.0/datadog_lambda/statsd_writer.py
+-rw-r--r--   0        0        0     1751 2023-02-13 18:56:36.621061 datadog_lambda-4.71.0/datadog_lambda/tag_object.py
+-rw-r--r--   0        0        0     3240 2023-02-13 18:56:36.621201 datadog_lambda-4.71.0/datadog_lambda/tags.py
+-rw-r--r--   0        0        0     2522 2023-02-13 18:56:36.621290 datadog_lambda-4.71.0/datadog_lambda/thread_stats_writer.py
+-rw-r--r--   0        0        0    45292 2023-04-12 18:23:27.981500 datadog_lambda-4.71.0/datadog_lambda/tracing.py
+-rw-r--r--   0        0        0    12082 2023-04-12 18:23:27.981977 datadog_lambda-4.71.0/datadog_lambda/trigger.py
+-rw-r--r--   0        0        0    13237 2023-04-17 15:01:22.537628 datadog_lambda-4.71.0/datadog_lambda/wrapper.py
+-rw-r--r--   0        0        0     3449 2023-04-12 15:37:46.255654 datadog_lambda-4.71.0/datadog_lambda/xray.py
+-rw-r--r--   0        0        0     1251 2023-04-17 19:45:09.828867 datadog_lambda-4.71.0/pyproject.toml
+-rw-r--r--   0        0        0     4555 1970-01-01 00:00:00.000000 datadog_lambda-4.71.0/setup.py
+-rw-r--r--   0        0        0     4969 1970-01-01 00:00:00.000000 datadog_lambda-4.71.0/PKG-INFO
```

### Comparing `datadog_lambda-4.70.0/LICENSE` & `datadog_lambda-4.71.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.70.0/README.md` & `datadog_lambda-4.71.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 ![build](https://github.com/DataDog/datadog-lambda-python/workflows/build/badge.svg)
 [![PyPI](https://img.shields.io/pypi/v/datadog-lambda)](https://pypi.org/project/datadog-lambda/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/datadog-lambda)
 [![Slack](https://chat.datadoghq.com/badge.svg?bg=632CA6)](https://chat.datadoghq.com/)
 [![License](https://img.shields.io/badge/license-Apache--2.0-blue)](https://github.com/DataDog/datadog-lambda-python/blob/main/LICENSE)
 
-Datadog Lambda Library for Python (3.7, 3.8, and 3.9) enables [enhanced Lambda metrics](https://docs.datadoghq.com/serverless/enhanced_lambda_metrics), [distributed tracing](https://docs.datadoghq.com/serverless/distributed_tracing), and [custom metric submission](https://docs.datadoghq.com/serverless/custom_metrics) from AWS Lambda functions.
+Datadog Lambda Library for Python (3.7, 3.8, 3.9, and 3.10) enables [enhanced Lambda metrics](https://docs.datadoghq.com/serverless/enhanced_lambda_metrics), [distributed tracing](https://docs.datadoghq.com/serverless/distributed_tracing), and [custom metric submission](https://docs.datadoghq.com/serverless/custom_metrics) from AWS Lambda functions.
 
 ## Installation
 
 Follow the [installation instructions](https://docs.datadoghq.com/serverless/installation/python/), and view your function's enhanced metrics, traces and logs in Datadog.
 
 ## Configuration
```

### Comparing `datadog_lambda-4.70.0/datadog_lambda/__init__.py` & `datadog_lambda-4.71.0/datadog_lambda/__init__.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.70.0/datadog_lambda/api.py` & `datadog_lambda-4.71.0/datadog_lambda/api.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.70.0/datadog_lambda/cold_start.py` & `datadog_lambda-4.71.0/datadog_lambda/cold_start.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.70.0/datadog_lambda/constants.py` & `datadog_lambda-4.71.0/datadog_lambda/constants.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.70.0/datadog_lambda/dogstatsd.py` & `datadog_lambda-4.71.0/datadog_lambda/dogstatsd.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.70.0/datadog_lambda/extension.py` & `datadog_lambda-4.71.0/datadog_lambda/extension.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.70.0/datadog_lambda/handler.py` & `datadog_lambda-4.71.0/datadog_lambda/handler.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.70.0/datadog_lambda/metric.py` & `datadog_lambda-4.71.0/datadog_lambda/metric.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.70.0/datadog_lambda/patch.py` & `datadog_lambda-4.71.0/datadog_lambda/patch.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.70.0/datadog_lambda/tag_object.py` & `datadog_lambda-4.71.0/datadog_lambda/tag_object.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.70.0/datadog_lambda/tags.py` & `datadog_lambda-4.71.0/datadog_lambda/tags.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.70.0/datadog_lambda/thread_stats_writer.py` & `datadog_lambda-4.71.0/datadog_lambda/thread_stats_writer.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.70.0/datadog_lambda/tracing.py` & `datadog_lambda-4.71.0/datadog_lambda/tracing.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.70.0/datadog_lambda/trigger.py` & `datadog_lambda-4.71.0/datadog_lambda/trigger.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.70.0/datadog_lambda/wrapper.py` & `datadog_lambda-4.71.0/datadog_lambda/wrapper.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.70.0/datadog_lambda/xray.py` & `datadog_lambda-4.71.0/datadog_lambda/xray.py`

 * *Files identical despite different names*

### Comparing `datadog_lambda-4.70.0/pyproject.toml` & `datadog_lambda-4.71.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datadog_lambda"
-version = "4.70.0"
+version = "4.71.0"
 description = "The Datadog AWS Lambda Library"
 authors = ["Datadog, Inc. <dev@datadoghq.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/DataDog/datadog-lambda-python"
 keywords = [
     "datadog",
@@ -15,14 +15,15 @@
 packages = [
     { include = "datadog_lambda" }
 ]
 classifiers = [
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.7.0,<4"
 datadog = ">=0.41.0,<1.0.0"
 wrapt = "^1.11.2"
 ddtrace = "^1.6.4"
```

### Comparing `datadog_lambda-4.70.0/setup.py` & `datadog_lambda-4.71.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,17 +17,17 @@
          'requests>=2.22.0,<3.0.0',
          'nose2>=0.9.1,<0.10.0',
          'flake8>=3.7.9,<4.0.0',
          'httpretty>=0.9.7,<0.10.0']}
 
 setup_kwargs = {
     'name': 'datadog-lambda',
-    'version': '4.70.0',
+    'version': '4.71.0',
     'description': 'The Datadog AWS Lambda Library',
-    'long_description': "# datadog-lambda-python\n\n![build](https://github.com/DataDog/datadog-lambda-python/workflows/build/badge.svg)\n[![PyPI](https://img.shields.io/pypi/v/datadog-lambda)](https://pypi.org/project/datadog-lambda/)\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/datadog-lambda)\n[![Slack](https://chat.datadoghq.com/badge.svg?bg=632CA6)](https://chat.datadoghq.com/)\n[![License](https://img.shields.io/badge/license-Apache--2.0-blue)](https://github.com/DataDog/datadog-lambda-python/blob/main/LICENSE)\n\nDatadog Lambda Library for Python (3.7, 3.8, and 3.9) enables [enhanced Lambda metrics](https://docs.datadoghq.com/serverless/enhanced_lambda_metrics), [distributed tracing](https://docs.datadoghq.com/serverless/distributed_tracing), and [custom metric submission](https://docs.datadoghq.com/serverless/custom_metrics) from AWS Lambda functions.\n\n## Installation\n\nFollow the [installation instructions](https://docs.datadoghq.com/serverless/installation/python/), and view your function's enhanced metrics, traces and logs in Datadog.\n\n## Configuration\n\nFollow the [configuration instructions](https://docs.datadoghq.com/serverless/configuration) to tag your telemetry, capture request/response payloads, filter or scrub sensitive information from logs or traces, and more.\n\n## Opening Issues\n\nIf you encounter a bug with this package, we want to hear about it. Before opening a new issue, search the existing issues to avoid duplicates.\n\nWhen opening an issue, include the Datadog Lambda Library version, Python version, and stack trace if available. In addition, include the steps to reproduce when appropriate.\n\nYou can also open an issue for a feature request.\n\n## Lambda Profiling Beta\n\nDatadog's [Continuous Profiler](https://www.datadoghq.com/product/code-profiling/) is now available in beta for Python in version 4.62.0 and layer version 62 and above. This optional feature is enabled by setting the `DD_PROFILING_ENABLED` environment variable to `true`. During the beta period, profiling is available at no additional cost.\n\nThe Continuous Profiler works by spawning a thread which periodically wakes up and takes a snapshot of the CPU and Heap of all running python code. This can include the profiler itself. If you want the Profiler to ignore itself, set `DD_PROFILING_IGNORE_PROFILER` to `true`.\n\n## Major Version Notes\n\n### 4.x / Layer version 61+\n\n- Python3.6 support has been [deprecated](https://docs.aws.amazon.com/lambda/latest/dg/lambda-runtimes.html) by AWS, and support removed from this library.\n- `dd-trace` upgraded from 0.61 to 1.4, full release notes are available [here](https://ddtrace.readthedocs.io/en/stable/release_notes.html#v1-0-0)\n  - `get_correlation_ids()` has been changed to `get_log_correlation_context()`, which now returns a dictionary containing the active `span_id`, `trace_id`, as well as `service` and `env`.\n\n## Contributing\n\nIf you find an issue with this package and have a fix, please feel free to open a pull request following the [procedures](CONTRIBUTING.md).\n\n## Community\n\nFor product feedback and questions, join the `#serverless` channel in the [Datadog community on Slack](https://chat.datadoghq.com/).\n\n## License\n\nUnless explicitly stated otherwise all files in this repository are licensed under the Apache License Version 2.0.\n\nThis product includes software developed at Datadog (https://www.datadoghq.com/). Copyright 2019 Datadog, Inc.\n",
+    'long_description': "# datadog-lambda-python\n\n![build](https://github.com/DataDog/datadog-lambda-python/workflows/build/badge.svg)\n[![PyPI](https://img.shields.io/pypi/v/datadog-lambda)](https://pypi.org/project/datadog-lambda/)\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/datadog-lambda)\n[![Slack](https://chat.datadoghq.com/badge.svg?bg=632CA6)](https://chat.datadoghq.com/)\n[![License](https://img.shields.io/badge/license-Apache--2.0-blue)](https://github.com/DataDog/datadog-lambda-python/blob/main/LICENSE)\n\nDatadog Lambda Library for Python (3.7, 3.8, 3.9, and 3.10) enables [enhanced Lambda metrics](https://docs.datadoghq.com/serverless/enhanced_lambda_metrics), [distributed tracing](https://docs.datadoghq.com/serverless/distributed_tracing), and [custom metric submission](https://docs.datadoghq.com/serverless/custom_metrics) from AWS Lambda functions.\n\n## Installation\n\nFollow the [installation instructions](https://docs.datadoghq.com/serverless/installation/python/), and view your function's enhanced metrics, traces and logs in Datadog.\n\n## Configuration\n\nFollow the [configuration instructions](https://docs.datadoghq.com/serverless/configuration) to tag your telemetry, capture request/response payloads, filter or scrub sensitive information from logs or traces, and more.\n\n## Opening Issues\n\nIf you encounter a bug with this package, we want to hear about it. Before opening a new issue, search the existing issues to avoid duplicates.\n\nWhen opening an issue, include the Datadog Lambda Library version, Python version, and stack trace if available. In addition, include the steps to reproduce when appropriate.\n\nYou can also open an issue for a feature request.\n\n## Lambda Profiling Beta\n\nDatadog's [Continuous Profiler](https://www.datadoghq.com/product/code-profiling/) is now available in beta for Python in version 4.62.0 and layer version 62 and above. This optional feature is enabled by setting the `DD_PROFILING_ENABLED` environment variable to `true`. During the beta period, profiling is available at no additional cost.\n\nThe Continuous Profiler works by spawning a thread which periodically wakes up and takes a snapshot of the CPU and Heap of all running python code. This can include the profiler itself. If you want the Profiler to ignore itself, set `DD_PROFILING_IGNORE_PROFILER` to `true`.\n\n## Major Version Notes\n\n### 4.x / Layer version 61+\n\n- Python3.6 support has been [deprecated](https://docs.aws.amazon.com/lambda/latest/dg/lambda-runtimes.html) by AWS, and support removed from this library.\n- `dd-trace` upgraded from 0.61 to 1.4, full release notes are available [here](https://ddtrace.readthedocs.io/en/stable/release_notes.html#v1-0-0)\n  - `get_correlation_ids()` has been changed to `get_log_correlation_context()`, which now returns a dictionary containing the active `span_id`, `trace_id`, as well as `service` and `env`.\n\n## Contributing\n\nIf you find an issue with this package and have a fix, please feel free to open a pull request following the [procedures](CONTRIBUTING.md).\n\n## Community\n\nFor product feedback and questions, join the `#serverless` channel in the [Datadog community on Slack](https://chat.datadoghq.com/).\n\n## License\n\nUnless explicitly stated otherwise all files in this repository are licensed under the Apache License Version 2.0.\n\nThis product includes software developed at Datadog (https://www.datadoghq.com/). Copyright 2019 Datadog, Inc.\n",
     'author': 'Datadog, Inc.',
     'author_email': 'dev@datadoghq.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/DataDog/datadog-lambda-python',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `datadog_lambda-4.70.0/PKG-INFO` & `datadog_lambda-4.71.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: datadog-lambda
-Version: 4.70.0
+Version: 4.71.0
 Summary: The Datadog AWS Lambda Library
 Home-page: https://github.com/DataDog/datadog-lambda-python
 License: Apache-2.0
 Keywords: datadog,aws,lambda,layer
 Author: Datadog, Inc.
 Author-email: dev@datadoghq.com
 Requires-Python: >=3.7.0,<4
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: dev
 Requires-Dist: boto3 (>=1.10.33,<2.0.0) ; extra == "dev"
 Requires-Dist: datadog (>=0.41.0,<1.0.0)
 Requires-Dist: ddtrace (>=1.6.4,<2.0.0)
@@ -36,15 +37,15 @@
 
 ![build](https://github.com/DataDog/datadog-lambda-python/workflows/build/badge.svg)
 [![PyPI](https://img.shields.io/pypi/v/datadog-lambda)](https://pypi.org/project/datadog-lambda/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/datadog-lambda)
 [![Slack](https://chat.datadoghq.com/badge.svg?bg=632CA6)](https://chat.datadoghq.com/)
 [![License](https://img.shields.io/badge/license-Apache--2.0-blue)](https://github.com/DataDog/datadog-lambda-python/blob/main/LICENSE)
 
-Datadog Lambda Library for Python (3.7, 3.8, and 3.9) enables [enhanced Lambda metrics](https://docs.datadoghq.com/serverless/enhanced_lambda_metrics), [distributed tracing](https://docs.datadoghq.com/serverless/distributed_tracing), and [custom metric submission](https://docs.datadoghq.com/serverless/custom_metrics) from AWS Lambda functions.
+Datadog Lambda Library for Python (3.7, 3.8, 3.9, and 3.10) enables [enhanced Lambda metrics](https://docs.datadoghq.com/serverless/enhanced_lambda_metrics), [distributed tracing](https://docs.datadoghq.com/serverless/distributed_tracing), and [custom metric submission](https://docs.datadoghq.com/serverless/custom_metrics) from AWS Lambda functions.
 
 ## Installation
 
 Follow the [installation instructions](https://docs.datadoghq.com/serverless/installation/python/), and view your function's enhanced metrics, traces and logs in Datadog.
 
 ## Configuration
```

