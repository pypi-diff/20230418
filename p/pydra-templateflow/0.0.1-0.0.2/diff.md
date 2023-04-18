# Comparing `tmp/pydra_templateflow-0.0.1.tar.gz` & `tmp/pydra_templateflow-0.0.2.tar.gz`

## Comparing `pydra_templateflow-0.0.1.tar` & `pydra_templateflow-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 pydra_templateflow-0.0.1/.github/dependabot.yaml
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 pydra_templateflow-0.0.1/.github/workflows/publish.yaml
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 pydra_templateflow-0.0.1/.github/workflows/test.yaml
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 pydra_templateflow-0.0.1/src/pydra/tasks/templateflow/__init__.py
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 pydra_templateflow-0.0.1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pydra_templateflow-0.0.1/LICENSE
--rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 pydra_templateflow-0.0.1/README.md
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 pydra_templateflow-0.0.1/hatch.toml
--rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 pydra_templateflow-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3151 2020-02-02 00:00:00.000000 pydra_templateflow-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 pydra_templateflow-0.0.2/.github/dependabot.yaml
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 pydra_templateflow-0.0.2/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 pydra_templateflow-0.0.2/.github/workflows/test.yaml
+-rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 pydra_templateflow-0.0.2/src/pydra/tasks/templateflow/__init__.py
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 pydra_templateflow-0.0.2/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pydra_templateflow-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2554 2020-02-02 00:00:00.000000 pydra_templateflow-0.0.2/README.md
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 pydra_templateflow-0.0.2/hatch.toml
+-rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 pydra_templateflow-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3788 2020-02-02 00:00:00.000000 pydra_templateflow-0.0.2/PKG-INFO
```

### Comparing `pydra_templateflow-0.0.1/.github/workflows/publish.yaml` & `pydra_templateflow-0.0.2/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `pydra_templateflow-0.0.1/.github/workflows/test.yaml` & `pydra_templateflow-0.0.2/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `pydra_templateflow-0.0.1/.gitignore` & `pydra_templateflow-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pydra_templateflow-0.0.1/LICENSE` & `pydra_templateflow-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydra_templateflow-0.0.1/README.md` & `pydra_templateflow-0.0.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # pydra-templateflow
 
+[![PyPI - Version][pypi-version]][pypi-project]
+[![PyPI - Python Version][pypi-pyversions]][pypi-project]
+[![PyPI - Downloads][pypi-downloads]][pypi-project]
+![][status-test]
+
 ----
 
 Pydra tasks for TemplateFlow.
 
 [Pydra][pydra] is a dataflow engine which provides
 a set of lightweight abstractions for DAG
 construction, manipulation, and distributed execution.
@@ -30,20 +35,24 @@
 ```python
 from pydra.tasks import templateflow
 
 task = templateflow.get_template(
     template_id="MNI152Lin",
     output_queries={
         "brain_mask": {"resolution": "1", "suffix": "mask", "desc": "head"},
-        "head_mask": {"resolution": 1, "suffix": "mask", "desc": "brain"},
+        "head_mask": {"resolution": "1", "suffix": "mask", "desc": "brain"},
         "t1w_image": {"resolution": "1", "suffix": "T1w"},
     },
 )
 
 result = task()
+
+# result.output.brain_mask
+# result.output.head_mask
+# result.output.t1w_image
 ```
 
 Please check the list of available templates [here][templateflow-browse].  
 
 ## Installation
 
 ```console
@@ -70,12 +79,17 @@
 hatch run lint:fix
 ```
 
 ## License
 
 This project is distributed under the terms of the [Apache License, Version 2.0][license].
 
+[pypi-project]: https://pypi.org/project/pydra-templateflow/
+[pypi-version]: https://img.shields.io/pypi/v/pydra-templateflow.svg
+[pypi-pyversions]: https://img.shields.io/pypi/pyversions/pydra-templateflow.svg
+[pypi-downloads]: https://static.pepy.tech/badge/pydra-templateflow
+[status-test]: https://github.com/ghisvail/pydra-templateflow/actions/workflows/test.yaml/badge.svg
 [pydra]: https://pydra.readthedocs.io/
 [templateflow]: https://www.templateflow.org/
 [templateflow-browse]: https://www.templateflow.org/browse/
 [hatch]: https://hatch.pypa.io/
 [license]: https://spdx.org/licenses/Apache-2.0.html
```

### Comparing `pydra_templateflow-0.0.1/pyproject.toml` & `pydra_templateflow-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pydra-templateflow"
-version = "0.0.1"
+version = "0.0.2"
 description = 'Pydra tasks for TemplateFlow'
 readme = "README.md"
 requires-python = ">=3.7"
 license = "Apache-2.0"
 keywords = [
   "atlas",
   "brain",
```

### Comparing `pydra_templateflow-0.0.1/PKG-INFO` & `pydra_templateflow-0.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydra-templateflow
-Version: 0.0.1
+Version: 0.0.2
 Summary: Pydra tasks for TemplateFlow
 Project-URL: Documentation, https://github.com/ghisvail/pydra-templateflow#readme
 Project-URL: Issues, https://github.com/ghisvail/pydra-templateflow/issues
 Project-URL: Source, https://github.com/ghisvail/pydra-templateflow
 Author-email: Ghislain Vaillant <ghisvail@gmail.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
@@ -24,14 +24,19 @@
 Requires-Python: >=3.7
 Requires-Dist: pydra>=0.22
 Requires-Dist: templateflow>=23.0.0
 Description-Content-Type: text/markdown
 
 # pydra-templateflow
 
+[![PyPI - Version][pypi-version]][pypi-project]
+[![PyPI - Python Version][pypi-pyversions]][pypi-project]
+[![PyPI - Downloads][pypi-downloads]][pypi-project]
+![][status-test]
+
 ----
 
 Pydra tasks for TemplateFlow.
 
 [Pydra][pydra] is a dataflow engine which provides
 a set of lightweight abstractions for DAG
 construction, manipulation, and distributed execution.
@@ -58,20 +63,24 @@
 ```python
 from pydra.tasks import templateflow
 
 task = templateflow.get_template(
     template_id="MNI152Lin",
     output_queries={
         "brain_mask": {"resolution": "1", "suffix": "mask", "desc": "head"},
-        "head_mask": {"resolution": 1, "suffix": "mask", "desc": "brain"},
+        "head_mask": {"resolution": "1", "suffix": "mask", "desc": "brain"},
         "t1w_image": {"resolution": "1", "suffix": "T1w"},
     },
 )
 
 result = task()
+
+# result.output.brain_mask
+# result.output.head_mask
+# result.output.t1w_image
 ```
 
 Please check the list of available templates [here][templateflow-browse].  
 
 ## Installation
 
 ```console
@@ -98,12 +107,17 @@
 hatch run lint:fix
 ```
 
 ## License
 
 This project is distributed under the terms of the [Apache License, Version 2.0][license].
 
+[pypi-project]: https://pypi.org/project/pydra-templateflow/
+[pypi-version]: https://img.shields.io/pypi/v/pydra-templateflow.svg
+[pypi-pyversions]: https://img.shields.io/pypi/pyversions/pydra-templateflow.svg
+[pypi-downloads]: https://static.pepy.tech/badge/pydra-templateflow
+[status-test]: https://github.com/ghisvail/pydra-templateflow/actions/workflows/test.yaml/badge.svg
 [pydra]: https://pydra.readthedocs.io/
 [templateflow]: https://www.templateflow.org/
 [templateflow-browse]: https://www.templateflow.org/browse/
 [hatch]: https://hatch.pypa.io/
 [license]: https://spdx.org/licenses/Apache-2.0.html
```

