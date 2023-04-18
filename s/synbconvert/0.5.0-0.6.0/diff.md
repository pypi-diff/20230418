# Comparing `tmp/synbconvert-0.5.0.tar.gz` & `tmp/synbconvert-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synbconvert-0.5.0.tar", max compression
+gzip compressed data, was "synbconvert-0.6.0.tar", max compression
```

## Comparing `synbconvert-0.5.0.tar` & `synbconvert-0.6.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1068 2023-03-14 13:21:27.250157 synbconvert-0.5.0/LICENSE
--rw-r--r--   0        0        0     2307 2023-03-14 13:21:27.250157 synbconvert-0.5.0/README.md
--rw-r--r--   0        0        0     1355 2023-03-14 13:21:27.254157 synbconvert-0.5.0/pyproject.toml
--rw-r--r--   0        0        0       64 2023-03-14 13:21:27.258157 synbconvert-0.5.0/synbconvert/__init__.py
--rw-r--r--   0        0        0      612 2023-03-14 13:21:27.258157 synbconvert-0.5.0/synbconvert/cli.py
--rw-r--r--   0        0        0    10988 2023-03-14 13:21:27.258157 synbconvert-0.5.0/synbconvert/python_file_handler.py
--rw-r--r--   0        0        0    11801 2023-03-14 13:21:27.258157 synbconvert-0.5.0/synbconvert/syn_notebook_handler.py
--rw-r--r--   0        0        0     2172 2023-03-14 13:21:27.258157 synbconvert-0.5.0/synbconvert/synbconvert.py
--rw-r--r--   0        0        0     3002 2023-03-14 13:21:27.258157 synbconvert-0.5.0/synbconvert/utils.py
--rw-r--r--   0        0        0     3357 1970-01-01 00:00:00.000000 synbconvert-0.5.0/setup.py
--rw-r--r--   0        0        0     3316 1970-01-01 00:00:00.000000 synbconvert-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-18 14:52:48.693014 synbconvert-0.6.0/LICENSE
+-rw-r--r--   0        0        0     2307 2023-04-18 14:52:48.693014 synbconvert-0.6.0/README.md
+-rw-r--r--   0        0        0     1355 2023-04-18 14:52:48.697014 synbconvert-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0       64 2023-04-18 14:52:48.697014 synbconvert-0.6.0/synbconvert/__init__.py
+-rw-r--r--   0        0        0      612 2023-04-18 14:52:48.697014 synbconvert-0.6.0/synbconvert/cli.py
+-rw-r--r--   0        0        0    10988 2023-04-18 14:52:48.697014 synbconvert-0.6.0/synbconvert/python_file_handler.py
+-rw-r--r--   0        0        0    11714 2023-04-18 14:52:48.697014 synbconvert-0.6.0/synbconvert/syn_notebook_handler.py
+-rw-r--r--   0        0        0     2172 2023-04-18 14:52:48.697014 synbconvert-0.6.0/synbconvert/synbconvert.py
+-rw-r--r--   0        0        0     3002 2023-04-18 14:52:48.697014 synbconvert-0.6.0/synbconvert/utils.py
+-rw-r--r--   0        0        0     3357 1970-01-01 00:00:00.000000 synbconvert-0.6.0/setup.py
+-rw-r--r--   0        0        0     3316 1970-01-01 00:00:00.000000 synbconvert-0.6.0/PKG-INFO
```

### Comparing `synbconvert-0.5.0/LICENSE` & `synbconvert-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `synbconvert-0.5.0/README.md` & `synbconvert-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `synbconvert-0.5.0/pyproject.toml` & `synbconvert-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "synbconvert"
-version = "0.5.0"
+version = "0.6.0"
 description = "A simple command line tool to convert Python files to Synapse Notebooks and vice versa."
 authors = ["Jan Bieser <janwithb@gmail.com>", "Michael Wellner <michael.wellner@gmail.com>"]
 keywords = ["python", "converter", "notebook", "azure", "synapse-analytics"]
 homepage = "https://github.com/alpine-data/synbconvert"
 repository = "https://github.com/alpine-data/synbconvert"
 documentation = "https://alpine-data.github.io/synbconvert/"
 readme = "README.md"
```

### Comparing `synbconvert-0.5.0/synbconvert/cli.py` & `synbconvert-0.6.0/synbconvert/cli.py`

 * *Files identical despite different names*

### Comparing `synbconvert-0.5.0/synbconvert/python_file_handler.py` & `synbconvert-0.6.0/synbconvert/python_file_handler.py`

 * *Files identical despite different names*

### Comparing `synbconvert-0.5.0/synbconvert/syn_notebook_handler.py` & `synbconvert-0.6.0/synbconvert/syn_notebook_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -289,15 +289,14 @@
         dynamicAllocationMaxExecutors = numExecutors
 
     result: dict = {
         "name": "",
         "properties": {
             "nbformat": 4,
             "nbformat_minor": 2,
-            "bigDataPool": {"referenceName": "poolS", "type": "BigDataPoolReference"},
             "sessionProperties": {
                 "driverMemory": "28g",
                 "driverCores": 4,
                 "executorMemory": "28g",
                 "executorCores": 4,
                 "numExecutors": numExecutors,
                 "runAsWorkspaceSystemIdentity": runAsWorkspaceSystemIdentity,
```

### Comparing `synbconvert-0.5.0/synbconvert/synbconvert.py` & `synbconvert-0.6.0/synbconvert/synbconvert.py`

 * *Files identical despite different names*

### Comparing `synbconvert-0.5.0/synbconvert/utils.py` & `synbconvert-0.6.0/synbconvert/utils.py`

 * *Files identical despite different names*

### Comparing `synbconvert-0.5.0/setup.py` & `synbconvert-0.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'mkdocstrings>=0.18.1,<0.19.0']
 
 entry_points = \
 {'console_scripts': ['synbconvert = synbconvert.cli:synbconvert']}
 
 setup_kwargs = {
     'name': 'synbconvert',
-    'version': '0.5.0',
+    'version': '0.6.0',
     'description': 'A simple command line tool to convert Python files to Synapse Notebooks and vice versa.',
     'long_description': '<p align="center"><img width="300" src="https://raw.githubusercontent.com/alpine-data/synbconvert/main/docs/img/logo.png"/></p>\n\n# synbconvert\n\n[![Documentation](https://img.shields.io/badge/Documentation-MkDocs-blue)](https://alpine-data.github.io/synbconvert/)\n[![Python Build](https://github.com/alpine-data/synbconvert/actions/workflows/python-build.yml/badge.svg)](https://github.com/alpine-data/synbconvert/actions/workflows/python-build.yml)\n\n**[Documentation](https://alpine-data.github.io/synbconvert/)**\n\nAzure Synapse Analytics uses notebooks for data preparation, data visualization, machine learning, and many other tasks. \nHowever, performing proper version control working with these notebooks is a pain. \nMerging long nested JSON documents with git is nearly impossible.\nIf you would like to use Azure Synapse Analytics for large scale projects while compling with the standards of good software engineering, synbconvert may be the tool you are looking for.\nYou will be able to develop code in your favorite IDE and colaborate with your team as usual.\n\n## Features\n\nsynbconvert is a simple command line tool and Python API to convert Python files to Azure Synapse Analytics notebooks and vice versa.\nThe main features of the tool include:\n\n- Lean annotation syntax for Python files\n- Conversion of Python files to Azure Synapse Analytics notebooks based on annotations\n- Conversion of Azure Synapse Analytics notebooks to annotated Python files\n\n## Workflow\n\n<p align="center"><img width="885" src="https://raw.githubusercontent.com/alpine-data/synbconvert/main/docs/img/workflow.png"/></p>\n\n## Installation\n\n### pip\n\nsynbconvert releases are available as source packages and binary wheels. Before you install synbconvert and its dependencies, make sure that your pip, setuptools and wheel are up to date. When using pip it is generally recommended to install packages in a virtual environment to avoid modifying system state. You can install synbconvert with:\n\n```console\n$ pip install synbconvert\n```\n\n<br>\n\n## Contribute\nThank you for taking the time to contribute to synbconvert. Before submitting a pull request, please make sure to bump the project version with:\n\n```console\n$ poetry version minor\n```\n\nfor minor releases or\n\n```console\n$ poetry version major\n```\n\nfor major releases.\n',
     'author': 'Jan Bieser',
     'author_email': 'janwithb@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/alpine-data/synbconvert',
```

### Comparing `synbconvert-0.5.0/PKG-INFO` & `synbconvert-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synbconvert
-Version: 0.5.0
+Version: 0.6.0
 Summary: A simple command line tool to convert Python files to Synapse Notebooks and vice versa.
 Home-page: https://github.com/alpine-data/synbconvert
 License: MIT
 Keywords: python,converter,notebook,azure,synapse-analytics
 Author: Jan Bieser
 Author-email: janwithb@gmail.com
 Requires-Python: >=3.9,<4.0
```

