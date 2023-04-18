# Comparing `tmp/prometheus_http_sd-1.1.8.tar.gz` & `tmp/prometheus_http_sd-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prometheus_http_sd-1.1.8.tar", max compression
+gzip compressed data, was "prometheus_http_sd-1.1.9.tar", max compression
```

## Comparing `prometheus_http_sd-1.1.8.tar` & `prometheus_http_sd-1.1.9.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0    11357 2022-11-21 10:26:58.675992 prometheus_http_sd-1.1.8/LICENSE
--rw-r--r--   0        0        0     9153 2022-11-21 10:26:58.675992 prometheus_http_sd-1.1.8/README.md
--rw-r--r--   0        0        0        0 2022-11-21 10:26:58.679992 prometheus_http_sd-1.1.8/prometheus_http_sd/__init__.py
--rw-r--r--   0        0        0     3272 2022-11-21 10:26:58.679992 prometheus_http_sd-1.1.8/prometheus_http_sd/app.py
--rw-r--r--   0        0        0     2153 2022-11-21 10:26:58.679992 prometheus_http_sd-1.1.8/prometheus_http_sd/cli.py
--rw-r--r--   0        0        0      110 2022-11-21 10:26:58.679992 prometheus_http_sd-1.1.8/prometheus_http_sd/config.py
--rw-r--r--   0        0        0        0 2022-11-21 10:26:58.679992 prometheus_http_sd-1.1.8/prometheus_http_sd/exceptions.py
--rw-r--r--   0        0        0     4433 2022-11-21 10:26:58.679992 prometheus_http_sd-1.1.8/prometheus_http_sd/sd.py
--rw-r--r--   0        0        0      147 2022-11-21 10:26:58.679992 prometheus_http_sd-1.1.8/prometheus_http_sd/targets.py
--rw-r--r--   0        0        0     1148 2022-11-21 10:26:58.679992 prometheus_http_sd-1.1.8/prometheus_http_sd/templates/admin.html
--rw-r--r--   0        0        0     2037 2022-11-21 10:26:58.679992 prometheus_http_sd-1.1.8/prometheus_http_sd/validate.py
--rw-r--r--   0        0        0       18 2022-11-21 10:26:58.679992 prometheus_http_sd-1.1.8/prometheus_http_sd/version.py
--rw-r--r--   0        0        0      566 2022-11-21 10:26:58.679992 prometheus_http_sd-1.1.8/pyproject.toml
--rw-r--r--   0        0        0    10361 1970-01-01 00:00:00.000000 prometheus_http_sd-1.1.8/setup.py
--rw-r--r--   0        0        0     9843 1970-01-01 00:00:00.000000 prometheus_http_sd-1.1.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-03-29 06:26:30.458391 prometheus_http_sd-1.1.9/LICENSE
+-rw-r--r--   0        0        0     9192 2023-03-29 06:26:30.458391 prometheus_http_sd-1.1.9/README.md
+-rw-r--r--   0        0        0        0 2023-03-29 06:26:30.462391 prometheus_http_sd-1.1.9/prometheus_http_sd/__init__.py
+-rw-r--r--   0        0        0     3400 2023-03-29 06:26:30.462391 prometheus_http_sd-1.1.9/prometheus_http_sd/app.py
+-rw-r--r--   0        0        0     2153 2023-03-29 06:26:30.462391 prometheus_http_sd-1.1.9/prometheus_http_sd/cli.py
+-rw-r--r--   0        0        0      110 2023-03-29 06:26:30.462391 prometheus_http_sd-1.1.9/prometheus_http_sd/config.py
+-rw-r--r--   0        0        0        0 2023-03-29 06:26:30.462391 prometheus_http_sd-1.1.9/prometheus_http_sd/exceptions.py
+-rw-r--r--   0        0        0     4515 2023-03-29 06:26:30.462391 prometheus_http_sd-1.1.9/prometheus_http_sd/sd.py
+-rw-r--r--   0        0        0      147 2023-03-29 06:26:30.462391 prometheus_http_sd-1.1.9/prometheus_http_sd/targets.py
+-rw-r--r--   0        0        0     1148 2023-03-29 06:26:30.462391 prometheus_http_sd-1.1.9/prometheus_http_sd/templates/admin.html
+-rw-r--r--   0        0        0     2037 2023-03-29 06:26:30.462391 prometheus_http_sd-1.1.9/prometheus_http_sd/validate.py
+-rw-r--r--   0        0        0       18 2023-03-29 06:26:30.462391 prometheus_http_sd-1.1.9/prometheus_http_sd/version.py
+-rw-r--r--   0        0        0      566 2023-03-29 06:26:30.462391 prometheus_http_sd-1.1.9/pyproject.toml
+-rw-r--r--   0        0        0     9882 1970-01-01 00:00:00.000000 prometheus_http_sd-1.1.9/PKG-INFO
```

### Comparing `prometheus_http_sd-1.1.8/LICENSE` & `prometheus_http_sd-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `prometheus_http_sd-1.1.8/README.md` & `prometheus_http_sd-1.1.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 
 Then you can run `prometheus-http-sd serve -h 0.0.0.0 -p 8080 /tmp/targets`,
 prometheus-http-sd will start to expose targets at: http://0.0.0.0:8080/targets
 
 The `-h` and `-p` is optional, defaults to `127.0.0.1` and `8080`.
 
 ```shell
-$ prometheus-http-sd /tmp/good_root
+$ prometheus-http-sd serve /tmp/targets # replace this to your target path
 [2022-07-24 00:52:03,896] {wasyncore.py:486} INFO - Serving on http://127.0.0.1:8080
 ```
 
 Finally, you can tell your Prometheus to find targets under
 http://127.0.0.1:8080/targets, by adding this into your Prometheus config:
 
 ```yaml
```

### Comparing `prometheus_http_sd-1.1.8/prometheus_http_sd/app.py` & `prometheus_http_sd-1.1.9/prometheus_http_sd/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import logging
 from pathlib import Path
 
 
-from flask import Flask, jsonify, abort, render_template
+from flask import Flask, jsonify, abort, render_template, request
 from .sd import generate
 from .version import VERSION
 from .config import config
 from prometheus_client import Gauge, Counter, Histogram, Info
 from werkzeug.middleware.dispatcher import DispatcherMiddleware
 from prometheus_client import make_wsgi_app
 
@@ -55,20 +55,25 @@
     )
 
     @app.route(f"{prefix}/targets", defaults={"rest_path": ""})
     @app.route(f"{prefix}/targets/", defaults={"rest_path": ""})
     # match the rest of the path
     @app.route(f"{prefix}/targets/<path:rest_path>")
     def get_targets(rest_path):
-        logger.info("request target path: {}".format(rest_path))
+        logger.info(
+            "request target path: {} with parameters: {}".format(
+                rest_path,
+                request.args,
+            )
+        )
         with target_path_request_duration_seconds.labels(
             path=rest_path
         ).time():
             try:
-                targets = generate(config.root_dir, rest_path)
+                targets = generate(config.root_dir, rest_path, **request.args)
             except FileNotFoundError:
                 logger.error(f"Didn't found {config.root_dir}/{rest_path}!")
                 abort(404)
             except:  # noqa: E722
                 target_path_requests_total.labels(
                     path=rest_path, status="fail"
                 ).inc()
```

### Comparing `prometheus_http_sd-1.1.8/prometheus_http_sd/cli.py` & `prometheus_http_sd-1.1.9/prometheus_http_sd/cli.py`

 * *Files identical despite different names*

### Comparing `prometheus_http_sd-1.1.8/prometheus_http_sd/sd.py` & `prometheus_http_sd-1.1.9/prometheus_http_sd/sd.py`

 * *Files 3% similar despite different names*

```diff
@@ -88,25 +88,25 @@
 
             generators.append(full_path)
 
     logger.debug(f"{generators=}")
     return generators
 
 
-def generate(root: str, path: str = "") -> TargetList:
+def generate(root: str, path: str = "", **extra_args) -> TargetList:
     generators = get_generator_list(root, path)
     all_targets = []
     for generator in generators:
-        target_list = run_generator(generator)
+        target_list = run_generator(generator, **extra_args)
         all_targets.extend(target_list)
 
     return all_targets
 
 
-def run_generator(generator_path: str) -> TargetList:
+def run_generator(generator_path: str, **extra_args) -> TargetList:
     if generator_path.endswith(".json"):
         executor = run_json
     elif generator_path.endswith(".py"):
         executor = run_python
     elif generator_path.endswith(".yaml"):
         executor = run_yaml
     else:
@@ -115,15 +115,15 @@
         ).inc()
         raise Exception(f"Unknown File Type: {generator_path}")
 
     with generator_run_duration_seconds.labels(
         generator=generator_path
     ).time():
         try:
-            result = executor(generator_path)
+            result = executor(generator_path, **extra_args)
         except:  # noqa: E722
             generator_requests_total.labels(
                 generator=generator_path, status="fail"
             ).inc()
             raise
         else:
             generator_requests_total.labels(
@@ -138,26 +138,26 @@
 
 
 def run_json(file_path: str) -> TargetList:
     with open(file_path) as jsonf:
         return json.load(jsonf)
 
 
-def run_python(generator_path) -> TargetList:
+def run_python(generator_path, **extra_args) -> TargetList:
     logger.debug(f"start to import module {generator_path}...")
 
     loader = importlib.machinery.SourceFileLoader("mymodule", generator_path)
     spec = importlib.util.spec_from_loader("mymodule", loader)
     if spec:
         mymodule = importlib.util.module_from_spec(spec)
         loader.exec_module(mymodule)
     else:
         raise Exception("Load a None module!")
 
-    return mymodule.generate_targets()
+    return mymodule.generate_targets(**extra_args)
 
 
 def run_yaml(file_path: str):
     with open(file_path) as yamlf:
         data = yaml.load(yamlf, Loader=Loader)
         return data
```

### Comparing `prometheus_http_sd-1.1.8/prometheus_http_sd/templates/admin.html` & `prometheus_http_sd-1.1.9/prometheus_http_sd/templates/admin.html`

 * *Files identical despite different names*

### Comparing `prometheus_http_sd-1.1.8/prometheus_http_sd/validate.py` & `prometheus_http_sd-1.1.9/prometheus_http_sd/validate.py`

 * *Files identical despite different names*

### Comparing `prometheus_http_sd-1.1.8/pyproject.toml` & `prometheus_http_sd-1.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prometheus-http-sd"
-version = "1.1.8"
+version = "1.1.9"
 description = "Prometheus HTTP SD framework."
 authors = ["laixintao <laixintaoo@gmail.com>"]
 readme = 'README.md'
 
 [tool.poetry.dependencies]
 python = "^3.7"
 Flask = "^2.1.3"
@@ -13,15 +13,15 @@
 PyYAML = "^6.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 flake8 = "^4.0.1"
 
 [build-system]
-requires = ["poetry-core>=1.1.8"]
+requires = ["poetry-core>=1.1.9"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 79
 
 [tool.poetry.scripts]
 prometheus-http-sd = 'prometheus_http_sd.cli:main'
```

### Comparing `prometheus_http_sd-1.1.8/setup.py` & `prometheus_http_sd-1.1.9/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,326 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: prometheus-http-sd
+Version: 1.1.9
+Summary: Prometheus HTTP SD framework.
+Author: laixintao
+Author-email: laixintaoo@gmail.com
+Requires-Python: >=3.7,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: Flask (>=2.1.3,<3.0.0)
+Requires-Dist: PyYAML (>=6.0,<7.0)
+Requires-Dist: prometheus-client (>=0.14.1,<0.15.0)
+Requires-Dist: waitress (>=2.1.2,<3.0.0)
+Description-Content-Type: text/markdown
 
-packages = \
-['prometheus_http_sd']
+# prometheus-http-sd
 
-package_data = \
-{'': ['*'], 'prometheus_http_sd': ['templates/*']}
+This is a
+[Prometheus HTTP SD](https://prometheus.io/docs/prometheus/latest/http_sd/)
+framework.
 
-install_requires = \
-['Flask>=2.1.3,<3.0.0',
- 'PyYAML>=6.0,<7.0',
- 'prometheus-client>=0.14.1,<0.15.0',
- 'waitress>=2.1.2,<3.0.0']
-
-entry_points = \
-{'console_scripts': ['prometheus-http-sd = prometheus_http_sd.cli:main']}
-
-setup_kwargs = {
-    'name': 'prometheus-http-sd',
-    'version': '1.1.8',
-    'description': 'Prometheus HTTP SD framework.',
-    'long_description': '# prometheus-http-sd\n\nThis is a\n[Prometheus HTTP SD](https://prometheus.io/docs/prometheus/latest/http_sd/)\nframework.\n\n[![Test](https://github.com/laixintao/prometheus-http-sd/actions/workflows/test.yaml/badge.svg)](https://github.com/laixintao/prometheus-http-sd/actions/workflows/test.yaml)\n\n<!-- vim-markdown-toc GFM -->\n\n- [Features](#features)\n- [Installation](#installation)\n- [Usage](#usage)\n  - [Manage prometheus-http-sd by systemd](#manage-prometheus-http-sd-by-systemd)\n  - [Admin Page](#admin-page)\n  - [Serve under a different root path](#serve-under-a-different-root-path)\n- [Define you targets](#define-you-targets)\n  - [Your target generator](#your-target-generator)\n  - [The Target Path](#the-target-path)\n  - [Overwriting `job_name` labels](#overwriting-job_name-labels)\n  - [Check and Validate your Targets](#check-and-validate-your-targets)\n  - [Script Dependencies](#script-dependencies)\n- [Update Your Scripts](#update-your-scripts)\n- [Best Practice](#best-practice)\n\n<!-- vim-markdown-toc -->\n\n## Features\n\n- Support static targets from Json file;\n- Support static targets from Yaml file;\n- Support generating target list using Python script;\n- Support `check` command, to testing the generated target is as expected, and\n  counting the targets;\n- You can monitoring your target generator via `/metrics`, see\n  [metrics](./docs/metrics.txt);\n- Admin page to list all target paths;\n- Auto reload when generator or targets changed;\n- Support managing targets in a hierarchy way;\n\n## Installation\n\n```shell\npip install prometheus-http-sd\n```\n\n## Usage\n\nFirst, you need a directory, everything in this directory will be used to\ngenerate targets for prometheus-http-sd.\n\n```shell\n$ mkdir targets\n```\n\nIn this directory, every file is called a target "generator":\n\n- Filename that ending with `.json` will be exposed directly\n- Filename that ending with `.yaml` will be exposed directly\n- Filename that ending with `.py` must include a `generate_targets()` function,\n  the function will be run, and it must return a `TargetList` (Type helper in\n  `prometheus_http_sd.targets.`)\n- Filename that starts with `_` will be ignored, so you can have some python\n  utils there, for e.g. `_utils/__init__.py` that you can import in you\n  `generate_targets()`\n- Filename that starts with `.` (hidden file in Linux) will also be ignored\n\nLet write our first target generator by yaml, put this into your\n`targets/first_target.yaml`:\n\n```yaml\n---\n- targets:\n    - "10.1.1.9:9100"\n    - "10.1.1.10:9100"\n  labels:\n    job: node\n    datacenter: nyc\n    group: g1\n- targets:\n    - "10.2.1.9:9100"\n    - "10.2.1.10:9100"\n  labels:\n    job: node\n    datacenter: sg\n    group: g2\n```\n\nIf you use json, the data structure is the same, just in Json format.\n\nLet\'s put another generator using Python:\n\nPut this into your `targets/by_python.py`:\n\n```python\ndef generate_targets():\n  return {"targets": "10.1.1.22:2379", "labels": {"app": "etcd"}}\n```\n\nThen you can run `prometheus-http-sd serve -h 0.0.0.0 -p 8080 /tmp/targets`,\nprometheus-http-sd will start to expose targets at: http://0.0.0.0:8080/targets\n\nThe `-h` and `-p` is optional, defaults to `127.0.0.1` and `8080`.\n\n```shell\n$ prometheus-http-sd /tmp/good_root\n[2022-07-24 00:52:03,896] {wasyncore.py:486} INFO - Serving on http://127.0.0.1:8080\n```\n\nFinally, you can tell your Prometheus to find targets under\nhttp://127.0.0.1:8080/targets, by adding this into your Prometheus config:\n\n```yaml\nscrape_configs:\n  - job_name: "etcd"\n    http_sd_config:\n      url: http://127.0.0.1:8080/targets/\n```\n\n### Manage prometheus-http-sd by systemd\n\nJust put this file under `/lib/systemd/system/http-sd.service` (remember to\nchange your installation path and root_dir path):\n\n```\n# /lib/systemd/system/http-sd.service\n[Unit]\nDescription=Prometheus HTTP SD Service\nWants=network-online.target\nAfter=network-online.target\n\n[Service]\nType=simple\nExecStart=/opt/httpsd_env/bin/prometheus-http-sd serve \\\n    -h 0.0.0.0                                         \\\n    -p 8080                                            \\\n    /opt/httpsd_targets\n\nRestart=always\nRestartSec=90\n\n[Install]\nWantedBy=multi-user.target\n```\n\n### Admin Page\n\nYou can open the root path, `http://127.0.0.1:8080/` in this example, and you\nwill see all of the available paths list in the admin page.\n\n![](./docs/admin1.png)\n\n### Serve under a different root path\n\nIf you put prometheus-http-sd behind a reverse proxy like Nginx, like this:\n\n```\nlocation /http_sd/ {\n      proxy_pass http://prometheus_http_sd;\n}\n```\n\nThen you need to tell prometheus_http_sd to serve all HTTP requests under this\npath, by using the `--url_prefix /http_sd` cli option, (or `-r /http_sd` for\nshort).\n\n## Define you targets\n\n### Your target generator\n\nPlease see the [Usage](#usage) to know how to define your generator.\n\n### The Target Path\n\nprometheus-http-sd support sub-pathes.\n\nFor example, if we use `prometheus-http-sd serve gateway`, and the `gateway`\ndirectory\'s structure is as follows:\n\n```shell\ngateway\n├── nginx\n│\xa0\xa0 ├── edge.py\n│\xa0\xa0 └── targets.json\n└── targets.json\n```\n\nThen:\n\n- `/targets/gateway` will return the targets from:\n  - `gateway/nginx/edge.py`\n  - `gateway/nginx/targets.json`\n  - `gateway/targets.json`\n- `/targets/gateway/nginx` will return the targets from:\n  - `gateway/nginx/edge.py`\n  - `gateway/nginx/targets.json`\n\nThis is very useful when you use vertical scaling. Say you have 5 Prometheus\ninstances, and you want each one of them scrape for different targets, then you\ncan use the sub-path feature of prometheus-http-sd.\n\nFor example, in one Prometheus\'s scrape config:\n\n```yaml\nscrape_configs:\n  - job_name: "nginx"\n    http_sd_config:\n      url: http://prometheus-http-sd:8080/targets/nginx\n\n  - job_name: "etcd"\n    http_sd_config:\n      url: http://prometheus-http-sd:8080/targets/etcd\n```\n\nAnd in another one:\n\n```yaml\nscrape_configs:\n  - job_name: "nginx"\n    http_sd_config:\n      url: http://prometheus-http-sd:8080/targets/database\n\n  - job_name: "etcd"\n    http_sd_config:\n      url: http://prometheus-http-sd:8080/targets/application\n```\n\n### Overwriting `job_name` labels\n\nYou may want to put all of etcd targets in one generator, including port 2379\nfor etcd metrics and 9100 for node_exporter metrics of the etcd server. But the\n`job_name` setting was based on per URL.\n\nThe trick is that, you can overwrite the `job` label in the target labels, like\nthis:\n\n```yaml\n---\n- targets:\n    - "10.1.1.9:9100"\n  labels:\n    job: node\n    datacenter: nyc\n    group: g1\n- targets:\n    - "10.1.1.9:2379"\n  labels:\n    job: etcd\n    datacenter: nyc\n    group: g1\n```\n\n### Check and Validate your Targets\n\nYou can use `prometheus-http-sd check` command to test your targets dir. It will\nrun all of you generators, validate the targets, and print the targets count\nthat each generator generates.\n\n```shell\n$ prometheus-http-sd check test/test_generator/root\n[2022-08-06 00:50:11,095] {validate.py:16} INFO - Run generator test/test_generator/root/json/target.json, took 0.0011398792266845703s, generated 1 targets.\n[2022-08-06 00:50:11,100] {validate.py:16} INFO - Run generator test/test_generator/root/yaml/target.yaml, took 0.0043718814849853516s, generated 2 targets.\n[2022-08-06 00:50:11,100] {validate.py:22} INFO - Done! Generated {total_targets} in total.\n```\n\nIt\'s a good idea to use `prometheus-http-sd check` in your CI system to validate\nyour targets generator scripts and target files.\n\n### Script Dependencies\n\nIf you want your scripts to use some other python library, just install them\ninto the **same virtualenv** that you install prometheus-http-sd, so that\nprometheus-http-sd can import them.\n\n## Update Your Scripts\n\nIf you want to update your script file or target json file, just upload and\noverwrite with your new version, it will take effect immediately after you\nmaking changes, **there is no need to restart** prometheus-http-sd,\nprometheus-http-sd will read the file (or reload the python script) every time\nserving a request.\n\nIt is worth noting that restarting is safe because if Prometheus failed to get\nthe target list via HTTP request, it won\'t update its current target list to\nempty, instead,\n[it will keep using the current list](https://prometheus.io/docs/prometheus/latest/http_sd/).\n\n> Prometheus caches target lists. If an error occurs while fetching an updated\n> targets list, Prometheus keeps using the current targets list.\n\nFor the same reason, if there are 3 scripts under `/targets/mysystem` and only\none failed for a request, prometheus-http-sd will return a HTTP 500 Error for\nthe whole request instead of returning the partial targets from the other two\nscripts.\n\nAlso for the same reason, if your script met any error, you should throw out\n`Exception` all the way to the top instead of catch it in your script and return\na null `TargetList`, if you return a null `TargetList`, prometheus-http-sd will\nthink that your script run successfully and empty the target list as well.\n\nYou can notice this error from stdout logs or `/metrics` from\nprometheus-http-sd.\n\n## Best Practice\n\nYou can use a git repository to manage your target generator.\n',
-    'author': 'laixintao',
-    'author_email': 'laixintaoo@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
+[![Test](https://github.com/laixintao/prometheus-http-sd/actions/workflows/test.yaml/badge.svg)](https://github.com/laixintao/prometheus-http-sd/actions/workflows/test.yaml)
+
+<!-- vim-markdown-toc GFM -->
+
+- [Features](#features)
+- [Installation](#installation)
+- [Usage](#usage)
+  - [Manage prometheus-http-sd by systemd](#manage-prometheus-http-sd-by-systemd)
+  - [Admin Page](#admin-page)
+  - [Serve under a different root path](#serve-under-a-different-root-path)
+- [Define you targets](#define-you-targets)
+  - [Your target generator](#your-target-generator)
+  - [The Target Path](#the-target-path)
+  - [Overwriting `job_name` labels](#overwriting-job_name-labels)
+  - [Check and Validate your Targets](#check-and-validate-your-targets)
+  - [Script Dependencies](#script-dependencies)
+- [Update Your Scripts](#update-your-scripts)
+- [Best Practice](#best-practice)
+
+<!-- vim-markdown-toc -->
+
+## Features
+
+- Support static targets from Json file;
+- Support static targets from Yaml file;
+- Support generating target list using Python script;
+- Support `check` command, to testing the generated target is as expected, and
+  counting the targets;
+- You can monitoring your target generator via `/metrics`, see
+  [metrics](./docs/metrics.txt);
+- Admin page to list all target paths;
+- Auto reload when generator or targets changed;
+- Support managing targets in a hierarchy way;
+
+## Installation
+
+```shell
+pip install prometheus-http-sd
+```
+
+## Usage
+
+First, you need a directory, everything in this directory will be used to
+generate targets for prometheus-http-sd.
+
+```shell
+$ mkdir targets
+```
+
+In this directory, every file is called a target "generator":
+
+- Filename that ending with `.json` will be exposed directly
+- Filename that ending with `.yaml` will be exposed directly
+- Filename that ending with `.py` must include a `generate_targets()` function,
+  the function will be run, and it must return a `TargetList` (Type helper in
+  `prometheus_http_sd.targets.`)
+- Filename that starts with `_` will be ignored, so you can have some python
+  utils there, for e.g. `_utils/__init__.py` that you can import in you
+  `generate_targets()`
+- Filename that starts with `.` (hidden file in Linux) will also be ignored
+
+Let write our first target generator by yaml, put this into your
+`targets/first_target.yaml`:
+
+```yaml
+---
+- targets:
+    - "10.1.1.9:9100"
+    - "10.1.1.10:9100"
+  labels:
+    job: node
+    datacenter: nyc
+    group: g1
+- targets:
+    - "10.2.1.9:9100"
+    - "10.2.1.10:9100"
+  labels:
+    job: node
+    datacenter: sg
+    group: g2
+```
+
+If you use json, the data structure is the same, just in Json format.
+
+Let's put another generator using Python:
+
+Put this into your `targets/by_python.py`:
+
+```python
+def generate_targets():
+  return {"targets": "10.1.1.22:2379", "labels": {"app": "etcd"}}
+```
+
+Then you can run `prometheus-http-sd serve -h 0.0.0.0 -p 8080 /tmp/targets`,
+prometheus-http-sd will start to expose targets at: http://0.0.0.0:8080/targets
+
+The `-h` and `-p` is optional, defaults to `127.0.0.1` and `8080`.
+
+```shell
+$ prometheus-http-sd serve /tmp/targets # replace this to your target path
+[2022-07-24 00:52:03,896] {wasyncore.py:486} INFO - Serving on http://127.0.0.1:8080
+```
+
+Finally, you can tell your Prometheus to find targets under
+http://127.0.0.1:8080/targets, by adding this into your Prometheus config:
+
+```yaml
+scrape_configs:
+  - job_name: "etcd"
+    http_sd_config:
+      url: http://127.0.0.1:8080/targets/
+```
+
+### Manage prometheus-http-sd by systemd
+
+Just put this file under `/lib/systemd/system/http-sd.service` (remember to
+change your installation path and root_dir path):
+
+```
+# /lib/systemd/system/http-sd.service
+[Unit]
+Description=Prometheus HTTP SD Service
+Wants=network-online.target
+After=network-online.target
+
+[Service]
+Type=simple
+ExecStart=/opt/httpsd_env/bin/prometheus-http-sd serve \
+    -h 0.0.0.0                                         \
+    -p 8080                                            \
+    /opt/httpsd_targets
+
+Restart=always
+RestartSec=90
+
+[Install]
+WantedBy=multi-user.target
+```
+
+### Admin Page
+
+You can open the root path, `http://127.0.0.1:8080/` in this example, and you
+will see all of the available paths list in the admin page.
+
+![](./docs/admin1.png)
+
+### Serve under a different root path
+
+If you put prometheus-http-sd behind a reverse proxy like Nginx, like this:
+
+```
+location /http_sd/ {
+      proxy_pass http://prometheus_http_sd;
 }
+```
+
+Then you need to tell prometheus_http_sd to serve all HTTP requests under this
+path, by using the `--url_prefix /http_sd` cli option, (or `-r /http_sd` for
+short).
+
+## Define you targets
+
+### Your target generator
+
+Please see the [Usage](#usage) to know how to define your generator.
+
+### The Target Path
+
+prometheus-http-sd support sub-pathes.
+
+For example, if we use `prometheus-http-sd serve gateway`, and the `gateway`
+directory's structure is as follows:
+
+```shell
+gateway
+├── nginx
+│   ├── edge.py
+│   └── targets.json
+└── targets.json
+```
+
+Then:
+
+- `/targets/gateway` will return the targets from:
+  - `gateway/nginx/edge.py`
+  - `gateway/nginx/targets.json`
+  - `gateway/targets.json`
+- `/targets/gateway/nginx` will return the targets from:
+  - `gateway/nginx/edge.py`
+  - `gateway/nginx/targets.json`
+
+This is very useful when you use vertical scaling. Say you have 5 Prometheus
+instances, and you want each one of them scrape for different targets, then you
+can use the sub-path feature of prometheus-http-sd.
+
+For example, in one Prometheus's scrape config:
+
+```yaml
+scrape_configs:
+  - job_name: "nginx"
+    http_sd_config:
+      url: http://prometheus-http-sd:8080/targets/nginx
+
+  - job_name: "etcd"
+    http_sd_config:
+      url: http://prometheus-http-sd:8080/targets/etcd
+```
+
+And in another one:
+
+```yaml
+scrape_configs:
+  - job_name: "nginx"
+    http_sd_config:
+      url: http://prometheus-http-sd:8080/targets/database
+
+  - job_name: "etcd"
+    http_sd_config:
+      url: http://prometheus-http-sd:8080/targets/application
+```
+
+### Overwriting `job_name` labels
+
+You may want to put all of etcd targets in one generator, including port 2379
+for etcd metrics and 9100 for node_exporter metrics of the etcd server. But the
+`job_name` setting was based on per URL.
+
+The trick is that, you can overwrite the `job` label in the target labels, like
+this:
+
+```yaml
+---
+- targets:
+    - "10.1.1.9:9100"
+  labels:
+    job: node
+    datacenter: nyc
+    group: g1
+- targets:
+    - "10.1.1.9:2379"
+  labels:
+    job: etcd
+    datacenter: nyc
+    group: g1
+```
+
+### Check and Validate your Targets
+
+You can use `prometheus-http-sd check` command to test your targets dir. It will
+run all of you generators, validate the targets, and print the targets count
+that each generator generates.
+
+```shell
+$ prometheus-http-sd check test/test_generator/root
+[2022-08-06 00:50:11,095] {validate.py:16} INFO - Run generator test/test_generator/root/json/target.json, took 0.0011398792266845703s, generated 1 targets.
+[2022-08-06 00:50:11,100] {validate.py:16} INFO - Run generator test/test_generator/root/yaml/target.yaml, took 0.0043718814849853516s, generated 2 targets.
+[2022-08-06 00:50:11,100] {validate.py:22} INFO - Done! Generated {total_targets} in total.
+```
+
+It's a good idea to use `prometheus-http-sd check` in your CI system to validate
+your targets generator scripts and target files.
+
+### Script Dependencies
+
+If you want your scripts to use some other python library, just install them
+into the **same virtualenv** that you install prometheus-http-sd, so that
+prometheus-http-sd can import them.
+
+## Update Your Scripts
+
+If you want to update your script file or target json file, just upload and
+overwrite with your new version, it will take effect immediately after you
+making changes, **there is no need to restart** prometheus-http-sd,
+prometheus-http-sd will read the file (or reload the python script) every time
+serving a request.
+
+It is worth noting that restarting is safe because if Prometheus failed to get
+the target list via HTTP request, it won't update its current target list to
+empty, instead,
+[it will keep using the current list](https://prometheus.io/docs/prometheus/latest/http_sd/).
+
+> Prometheus caches target lists. If an error occurs while fetching an updated
+> targets list, Prometheus keeps using the current targets list.
+
+For the same reason, if there are 3 scripts under `/targets/mysystem` and only
+one failed for a request, prometheus-http-sd will return a HTTP 500 Error for
+the whole request instead of returning the partial targets from the other two
+scripts.
+
+Also for the same reason, if your script met any error, you should throw out
+`Exception` all the way to the top instead of catch it in your script and return
+a null `TargetList`, if you return a null `TargetList`, prometheus-http-sd will
+think that your script run successfully and empty the target list as well.
+
+You can notice this error from stdout logs or `/metrics` from
+prometheus-http-sd.
+
+## Best Practice
 
+You can use a git repository to manage your target generator.
 
-setup(**setup_kwargs)
```

