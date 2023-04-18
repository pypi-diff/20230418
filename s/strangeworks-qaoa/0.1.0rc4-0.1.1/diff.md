# Comparing `tmp/strangeworks_qaoa-0.1.0rc4.tar.gz` & `tmp/strangeworks_qaoa-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strangeworks_qaoa-0.1.0rc4.tar", max compression
+gzip compressed data, was "strangeworks_qaoa-0.1.1.tar", max compression
```

## Comparing `strangeworks_qaoa-0.1.0rc4.tar` & `strangeworks_qaoa-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0    11357 2023-03-10 14:52:38.652457 strangeworks_qaoa-0.1.0rc4/LICENSE
--rw-r--r--   0        0        0      573 2023-03-10 14:52:38.652457 strangeworks_qaoa-0.1.0rc4/README.md
--rw-r--r--   0        0        0      663 2023-03-10 14:52:54.436717 strangeworks_qaoa-0.1.0rc4/pyproject.toml
--rw-r--r--   0        0        0       39 2023-03-10 14:52:38.652457 strangeworks_qaoa-0.1.0rc4/strangeworks_qaoa/__init__.py
--rw-r--r--   0        0        0      117 2023-03-10 14:52:38.656456 strangeworks_qaoa-0.1.0rc4/strangeworks_qaoa/qaoa-jobs.py
--rw-r--r--   0        0        0    15868 2023-03-10 14:52:38.656456 strangeworks_qaoa-0.1.0rc4/strangeworks_qaoa/sdk.py
--rw-r--r--   0        0        0      691 2023-03-10 14:52:38.656456 strangeworks_qaoa-0.1.0rc4/strangeworks_qaoa/serializer.py
--rw-r--r--   0        0        0    10780 2023-03-10 14:52:38.656456 strangeworks_qaoa-0.1.0rc4/strangeworks_qaoa/utils.py
--rw-r--r--   0        0        0     1224 1970-01-01 00:00:00.000000 strangeworks_qaoa-0.1.0rc4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-18 11:13:51.737443 strangeworks_qaoa-0.1.1/LICENSE
+-rw-r--r--   0        0        0      576 2023-04-18 11:13:51.737443 strangeworks_qaoa-0.1.1/README.md
+-rw-r--r--   0        0        0      792 2023-04-18 11:14:10.737308 strangeworks_qaoa-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      128 2023-04-18 11:13:51.737443 strangeworks_qaoa-0.1.1/strangeworks_qaoa/__init__.py
+-rw-r--r--   0        0        0    15787 2023-04-18 11:13:51.737443 strangeworks_qaoa-0.1.1/strangeworks_qaoa/sdk.py
+-rw-r--r--   0        0        0      691 2023-04-18 11:13:51.737443 strangeworks_qaoa-0.1.1/strangeworks_qaoa/serializer.py
+-rw-r--r--   0        0        0    10780 2023-04-18 11:13:51.737443 strangeworks_qaoa-0.1.1/strangeworks_qaoa/utils.py
+-rw-r--r--   0        0        0     1228 1970-01-01 00:00:00.000000 strangeworks_qaoa-0.1.1/PKG-INFO
```

### Comparing `strangeworks_qaoa-0.1.0rc4/LICENSE` & `strangeworks_qaoa-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `strangeworks_qaoa-0.1.0rc4/README.md` & `strangeworks_qaoa-0.1.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -4,27 +4,29 @@
 
 ## Installation
 
 Install using `poetry`
 
 ```
 pip install poetry
-poetry install 
+poetry install
 ```
 
 ## Tests
 
 Test using pytest
+
 ```
 poetry run pytest tests
 ```
 
 ## Lint
 
 Lint with black
+
 ```
 poetry run black .
 ```
 
 ## Bump version
 
 Bump version with [poetry](https://python-poetry.org/docs/cli/#version).
@@ -32,15 +34,17 @@
 ```
 poetry version [patch, minor, major]
 ```
 
 ## Update packages
 
 Update <package> version
+
 ```
 poetry update <package>
 ```
 
 Update all packages
+
 ```
 poetry update
 ```
```

### Comparing `strangeworks_qaoa-0.1.0rc4/pyproject.toml` & `strangeworks_qaoa-0.1.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 [tool.poetry]
 name = "strangeworks-qaoa"
-version = "0.1.0rc4"
+version = "0.1.1"
 description = "Extension to strangeworks sdk to allow user to run qaoa service"
 authors = ["SFlann <stuart@strangeworks.com>"]
 readme = "README.md"
 packages = [{include = "strangeworks_qaoa"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 networkx = "^3.0"
 numpy = "1.23.2"
 qiskit = "^0.41.0"
-strangeworks = "0.4.0rc2" 
+strangeworks = "^0.4.0" 
 dimod = "^0.12.4"
 
 [tool.poetry.group.dev.dependencies]
 black = "22.10.0"
 flake8 = "^6.0.0"
 isort = "^5.12.0"
 pytest = "^7.2.1"
 pre-commit = "^3.0.4"
 ipykernel = "^6.21.1"
 python-dotenv = "^0.21.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.flake8]
+max-line-length = 88
+ignore = "E203, E501, E722, E741, F401, F841, W503"
+per-file-ignores = [
+    "__init__.py:F401"
+]
```

### Comparing `strangeworks_qaoa-0.1.0rc4/strangeworks_qaoa/sdk.py` & `strangeworks_qaoa-0.1.1/strangeworks_qaoa/sdk.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import copy
 from typing import Optional
 
 import dimod
 import networkx as nx
 import numpy as np
 import qiskit
 import strangeworks
@@ -293,16 +292,14 @@
             If results file is not there, run the function to produce the results file
             and plots for the platform
             """
             result = strangeworks.execute(
                 self.rsc, {"payload": {"job_slug": job_slug}}, "result"
             )
 
-            result = serializer.pickle_deserializer(result, "json")
-
             if result.strip().upper() == "COMPLETED":
                 result_url = strangeworks.execute(
                     self.rsc, {"payload": {"job_slug": job_slug}}, "get_results_url"
                 )
                 if result_url:
                     result_file = strangeworks.download_job_files([result_url])[0]
                 else:
```

### Comparing `strangeworks_qaoa-0.1.0rc4/strangeworks_qaoa/serializer.py` & `strangeworks_qaoa-0.1.1/strangeworks_qaoa/serializer.py`

 * *Files identical despite different names*

### Comparing `strangeworks_qaoa-0.1.0rc4/strangeworks_qaoa/utils.py` & `strangeworks_qaoa-0.1.1/strangeworks_qaoa/utils.py`

 * *Files identical despite different names*

### Comparing `strangeworks_qaoa-0.1.0rc4/PKG-INFO` & `strangeworks_qaoa-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,50 @@
 Metadata-Version: 2.1
 Name: strangeworks-qaoa
-Version: 0.1.0rc4
+Version: 0.1.1
 Summary: Extension to strangeworks sdk to allow user to run qaoa service
 Author: SFlann
 Author-email: stuart@strangeworks.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dimod (>=0.12.4,<0.13.0)
 Requires-Dist: networkx (>=3.0,<4.0)
 Requires-Dist: numpy (==1.23.2)
 Requires-Dist: qiskit (>=0.41.0,<0.42.0)
-Requires-Dist: strangeworks (==0.4.0rc2)
+Requires-Dist: strangeworks (>=0.4.0,<0.5.0)
 Description-Content-Type: text/markdown
 
 # Strangeworks QAOA SDK Extension
 
 This extension provides access to the Strangeworks QAOA service through the SDK.
 
 ## Installation
 
 Install using `poetry`
 
 ```
 pip install poetry
-poetry install 
+poetry install
 ```
 
 ## Tests
 
 Test using pytest
+
 ```
 poetry run pytest tests
 ```
 
 ## Lint
 
 Lint with black
+
 ```
 poetry run black .
 ```
 
 ## Bump version
 
 Bump version with [poetry](https://python-poetry.org/docs/cli/#version).
@@ -50,16 +52,18 @@
 ```
 poetry version [patch, minor, major]
 ```
 
 ## Update packages
 
 Update <package> version
+
 ```
 poetry update <package>
 ```
 
 Update all packages
+
 ```
 poetry update
 ```
```

