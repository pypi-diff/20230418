# Comparing `tmp/efemarai-0.3.3.tar.gz` & `tmp/efemarai-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "efemarai-0.3.3.tar", last modified: Thu Mar 30 15:00:03 2023, max compression
+gzip compressed data, was "efemarai-0.3.4.tar", last modified: Tue Apr 18 19:18:36 2023, max compression
```

## Comparing `efemarai-0.3.3.tar` & `efemarai-0.3.4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 15:00:03.896661 efemarai-0.3.3/
--rw-r--r--   0 root         (0) root         (0)     2783 2023-03-30 15:00:03.896661 efemarai-0.3.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2459 2023-02-10 13:56:21.000000 efemarai-0.3.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 15:00:03.896661 efemarai-0.3.3/efemarai/
--rw-r--r--   0 root         (0) root         (0)      363 2023-03-30 14:59:21.000000 efemarai-0.3.3/efemarai/__init__.py
--rw-r--r--   0 root         (0) root         (0)      931 2023-03-30 13:28:06.000000 efemarai-0.3.3/efemarai/base_checker.py
--rw-r--r--   0 root         (0) root         (0)     4509 2023-03-30 13:28:06.000000 efemarai-0.3.3/efemarai/baseline.py
--rw-r--r--   0 root         (0) root         (0)    34680 2023-03-30 14:36:50.000000 efemarai-0.3.3/efemarai/cli.py
--rw-r--r--   0 root         (0) root         (0)       54 2022-08-02 18:24:10.000000 efemarai-0.3.3/efemarai/console.py
--rw-r--r--   0 root         (0) root         (0)    17423 2023-03-30 14:36:50.000000 efemarai-0.3.3/efemarai/dataset.py
--rw-r--r--   0 root         (0) root         (0)    12412 2023-02-15 17:42:16.000000 efemarai-0.3.3/efemarai/definition_checker.py
--rw-r--r--   0 root         (0) root         (0)     3243 2023-03-07 14:11:53.000000 efemarai-0.3.3/efemarai/domain.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 15:00:03.896661 efemarai-0.3.3/efemarai/fields/
--rw-r--r--   0 root         (0) root         (0)     2032 2023-03-30 13:28:06.000000 efemarai-0.3.3/efemarai/fields/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21636 2023-03-30 13:28:06.000000 efemarai-0.3.3/efemarai/fields/annotation_fields.py
--rw-r--r--   0 root         (0) root         (0)     3606 2023-03-02 12:33:13.000000 efemarai-0.3.3/efemarai/fields/base_fields.py
--rw-r--r--   0 root         (0) root         (0)    16157 2023-03-30 13:28:06.000000 efemarai-0.3.3/efemarai/fields/data_fields.py
--rw-r--r--   0 root         (0) root         (0)     9110 2023-03-30 13:28:06.000000 efemarai-0.3.3/efemarai/fields/datapoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 15:00:03.896661 efemarai-0.3.3/efemarai/formats/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-20 14:12:18.000000 efemarai-0.3.3/efemarai/formats/__init__.py
--rw-r--r--   0 root         (0) root         (0)      757 2023-01-16 10:19:03.000000 efemarai-0.3.3/efemarai/formats/config.py
--rw-r--r--   0 root         (0) root         (0)     6736 2023-03-30 13:28:06.000000 efemarai-0.3.3/efemarai/formats/dataset_coco.py
--rw-r--r--   0 root         (0) root         (0)     2012 2023-02-08 13:57:13.000000 efemarai-0.3.3/efemarai/formats/dataset_imagenet.py
--rw-r--r--   0 root         (0) root         (0)      515 2023-03-28 09:34:44.000000 efemarai-0.3.3/efemarai/job_state.py
--rw-r--r--   0 root         (0) root         (0)    12955 2023-03-30 13:28:06.000000 efemarai-0.3.3/efemarai/model.py
--rw-rw-rw-   0 root         (0) root         (0)      557 2022-06-21 09:32:32.000000 efemarai-0.3.3/efemarai/problem_type.py
--rw-r--r--   0 root         (0) root         (0)    25493 2023-03-30 13:28:06.000000 efemarai-0.3.3/efemarai/project.py
--rw-r--r--   0 root         (0) root         (0)    13777 2022-11-22 13:33:10.000000 efemarai-0.3.3/efemarai/runtime_checker.py
--rw-r--r--   0 root         (0) root         (0)    13203 2023-03-02 13:11:49.000000 efemarai-0.3.3/efemarai/session.py
--rw-r--r--   0 root         (0) root         (0)     8995 2023-03-30 13:28:06.000000 efemarai-0.3.3/efemarai/stress_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 15:00:03.896661 efemarai-0.3.3/efemarai.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2783 2023-03-30 15:00:03.000000 efemarai-0.3.3/efemarai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      855 2023-03-30 15:00:03.000000 efemarai-0.3.3/efemarai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-30 15:00:03.000000 efemarai-0.3.3/efemarai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       71 2023-03-30 15:00:03.000000 efemarai-0.3.3/efemarai.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-05 14:06:34.000000 efemarai-0.3.3/efemarai.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      348 2023-03-30 15:00:03.000000 efemarai-0.3.3/efemarai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-03-30 15:00:03.000000 efemarai-0.3.3/efemarai.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-30 15:00:03.896661 efemarai-0.3.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1421 2023-03-20 14:12:18.000000 efemarai-0.3.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 19:18:36.086872 efemarai-0.3.4/
+-rw-r--r--   0 root         (0) root         (0)     2763 2023-04-18 19:18:36.086872 efemarai-0.3.4/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     2459 2023-04-18 12:01:21.000000 efemarai-0.3.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 19:18:36.086872 efemarai-0.3.4/efemarai/
+-rw-rw-r--   0 root         (0) root         (0)      363 2023-04-18 19:17:37.000000 efemarai-0.3.4/efemarai/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      931 2023-04-18 12:01:21.000000 efemarai-0.3.4/efemarai/base_checker.py
+-rw-rw-r--   0 root         (0) root         (0)     4484 2023-04-18 12:01:21.000000 efemarai-0.3.4/efemarai/baseline.py
+-rw-rw-r--   0 root         (0) root         (0)    34699 2023-04-18 12:01:21.000000 efemarai-0.3.4/efemarai/cli.py
+-rw-rw-r--   0 root         (0) root         (0)       54 2022-08-08 14:41:49.000000 efemarai-0.3.4/efemarai/console.py
+-rw-rw-r--   0 root         (0) root         (0)    17571 2023-04-18 12:01:21.000000 efemarai-0.3.4/efemarai/dataset.py
+-rw-rw-r--   0 root         (0) root         (0)    12675 2023-04-18 12:01:21.000000 efemarai-0.3.4/efemarai/definition_checker.py
+-rw-rw-r--   0 root         (0) root         (0)     3204 2023-04-18 12:01:21.000000 efemarai-0.3.4/efemarai/domain.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 19:18:36.086872 efemarai-0.3.4/efemarai/fields/
+-rw-rw-r--   0 root         (0) root         (0)     2037 2023-04-18 12:01:21.000000 efemarai-0.3.4/efemarai/fields/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    22788 2023-04-18 16:53:02.000000 efemarai-0.3.4/efemarai/fields/annotation_fields.py
+-rw-rw-r--   0 root         (0) root         (0)     3605 2023-04-18 12:01:21.000000 efemarai-0.3.4/efemarai/fields/base_fields.py
+-rw-rw-r--   0 root         (0) root         (0)    16180 2023-04-18 12:01:21.000000 efemarai-0.3.4/efemarai/fields/data_fields.py
+-rw-rw-r--   0 root         (0) root         (0)     9485 2023-04-18 12:01:21.000000 efemarai-0.3.4/efemarai/fields/datapoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 19:18:36.086872 efemarai-0.3.4/efemarai/formats/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-04-18 12:01:21.000000 efemarai-0.3.4/efemarai/formats/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      757 2023-04-18 12:01:21.000000 efemarai-0.3.4/efemarai/formats/config.py
+-rw-rw-r--   0 root         (0) root         (0)     6690 2023-04-18 12:01:21.000000 efemarai-0.3.4/efemarai/formats/dataset_coco.py
+-rw-rw-r--   0 root         (0) root         (0)     2023 2023-04-18 12:01:21.000000 efemarai-0.3.4/efemarai/formats/dataset_imagenet.py
+-rw-rw-r--   0 root         (0) root         (0)      505 2023-04-18 12:01:21.000000 efemarai-0.3.4/efemarai/job_state.py
+-rw-rw-r--   0 root         (0) root         (0)    13695 2023-04-18 12:01:21.000000 efemarai-0.3.4/efemarai/model.py
+-rw-rw-r--   0 root         (0) root         (0)      547 2023-04-18 12:01:21.000000 efemarai-0.3.4/efemarai/problem_type.py
+-rw-rw-r--   0 root         (0) root         (0)    25413 2023-04-18 12:01:21.000000 efemarai-0.3.4/efemarai/project.py
+-rw-rw-r--   0 root         (0) root         (0)    13777 2023-03-20 16:49:10.000000 efemarai-0.3.4/efemarai/runtime_checker.py
+-rw-rw-r--   0 root         (0) root         (0)    13047 2023-04-18 12:01:21.000000 efemarai-0.3.4/efemarai/session.py
+-rw-rw-r--   0 root         (0) root         (0)     8960 2023-04-18 12:01:21.000000 efemarai-0.3.4/efemarai/stress_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 19:18:36.086872 efemarai-0.3.4/efemarai.egg-info/
+-rw-rw-r--   0 root         (0) root         (0)     2763 2023-04-18 19:18:36.000000 efemarai-0.3.4/efemarai.egg-info/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      855 2023-04-18 19:18:36.000000 efemarai-0.3.4/efemarai.egg-info/SOURCES.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2023-04-18 19:18:36.000000 efemarai-0.3.4/efemarai.egg-info/dependency_links.txt
+-rw-rw-r--   0 root         (0) root         (0)       70 2023-04-18 19:18:36.000000 efemarai-0.3.4/efemarai.egg-info/entry_points.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2022-07-25 12:08:08.000000 efemarai-0.3.4/efemarai.egg-info/not-zip-safe
+-rw-rw-r--   0 root         (0) root         (0)      348 2023-04-18 19:18:36.000000 efemarai-0.3.4/efemarai.egg-info/requires.txt
+-rw-rw-r--   0 root         (0) root         (0)        9 2023-04-18 19:18:36.000000 efemarai-0.3.4/efemarai.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-18 19:18:36.086872 efemarai-0.3.4/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1421 2023-04-18 12:01:21.000000 efemarai-0.3.4/setup.py
```

### Comparing `efemarai-0.3.3/PKG-INFO` & `efemarai-0.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: efemarai
-Version: 0.3.3
+Version: 0.3.4
 Summary: A CLI and SDK for interacting with the Efemarai ML testing platform.
 Home-page: https://www.efemarai.com/
 Author: Efemarai
 Author-email: support@efemarai.com
 License: MIT license
-Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 A CLI and SDK for interacting with the [Efemarai ML testing platform](https://efemarai.com).
 
 ## Setup
 
@@ -101,9 +100,7 @@
 
 # access the created entities
 project = result["project"]
 models = result["models"]
 domains = result["domains"]
 datasets = result["datasets"]
 ```
-
-
```

### Comparing `efemarai-0.3.3/README.md` & `efemarai-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `efemarai-0.3.3/efemarai/base_checker.py` & `efemarai-0.3.4/efemarai/base_checker.py`

 * *Files identical despite different names*

### Comparing `efemarai-0.3.3/efemarai/baseline.py` & `efemarai-0.3.4/efemarai/baseline.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,23 +9,22 @@
     def create(
         project,
         name,
         model,
         dataset,
     ):
         """Create a baseline. A more convenient way is to use :func:`project.create_baseline`"""
-
         if isinstance(model, str):
             model = project.model(model)
 
         if isinstance(dataset, str):
             dataset = project.dataset(dataset)
 
         response = project._put(
-            f"api/baselineRunById",
+            "api/baselineRunById",
             json={
                 "name": name,
                 "model": model.id,
                 "dataset": dataset.id,
             },
         )
         return Baseline(
@@ -35,20 +34,18 @@
             model,
             dataset,
             "NotStarted",
             None,
             {},
         )
 
-    """Create a standard baseline evaluation."""
-
     def __init__(
         self, project, id, name, model, dataset, state, state_message, reports
     ):
-
+        """Create a standard baseline evaluation."""
         self.project = (
             project  #: (:class:`efemarai.project.Project`) Associated project.
         )
         self.id = id
         self.name = name  #: (str) Name of the baseline.
 
         if isinstance(model, str):
@@ -86,76 +83,68 @@
         res += f"\n  id={self.id}"
         res += f"\n  name={self.name}"
         res += f"\n  model={self.model.name}"
         res += f"\n  dataset={self.dataset.name}"
         res += f"\n  state={self.state}"
         res += f"\n  state_message={self.state_message}"
         res += f"\n  len(reports)={len(self._reports)}"
-        res += f"\n)"
+        res += "\n)"
         return res
 
     @property
     def model(self):
         """Returns the model associated with the baseline."""
-
         if self._model is None:
             self._model = next(m for m in self.project.models if m.id == self._model_id)
         return self._model
 
     @property
     def dataset(self):
         """Returns the dataset associated with the baseline."""
-
         if self._dataset is None:
             self._dataset = next(
                 d for d in self.project.datasets if d.id == self._dataset_id
             )
         return self._dataset
 
     @property
     def finished(self):
         """Returns if the baseline has successfully finished.
 
         :rtype: bool
         """
-
         return self.state == JobState.Finished
 
     @property
     def failed(self):
         """Returns if the baseline has failed.
 
         :rtype: bool
         """
-
         return self.state == JobState.Failed
 
     @property
     def running(self):
         """Returns if the baseline is still running - not failed or finished.
 
         :rtype: bool
         """
-
         return self.state not in (JobState.Finished, JobState.Failed)
 
     def delete(self, delete_dependants=False):
-        """
-        Deletes a baseline run. This cannot be undone.
-        """
+        """Deletes a baseline run. This cannot be undone."""
         self.project._delete(f"api/baselineRunById/{self.id}/{delete_dependants}")
 
     def reload(self):
         """
         Reloads the baseline *in place* from the remote endpoint and return it.
 
         Rerturns:
             The updated baseline object.
         """
-
         response = self.project._get(f"api/baselineRunById/{self.id}")["value"]
 
         self.name = response["name"]
         self.state = JobState(response["states"][-1]["name"])
         self.state_message = response["states"][-1].get("message")
         self._reports = response.get("reports", {})
```

### Comparing `efemarai-0.3.3/efemarai/cli.py` & `efemarai-0.3.4/efemarai/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,15 +176,15 @@
         _wait_for_runs(result["datasets"])
 
 
 @project.command("list", aliases=["ls"])
 def project_list():
     """Lists the projects associated with the current user."""
     table = Table(box=None)
-    [table.add_column(x) for x in ["Id", "Name", "Problem Type"]]
+    _ = [table.add_column(x) for x in ["Id", "Name", "Problem Type"]]
     for m in ef.Session().projects:
         table.add_row(m.id, m.name, str(m.problem_type))
     console.print(table)
 
 
 @project.command("delete")
 @click.argument("project", required=True)
@@ -220,39 +220,38 @@
     "-f", "--file", help=f"Name of the Efemarai file (Default is '{default_yaml}')"
 )
 def model_list(file):
     """Lists the models in the current project."""
     project = _get_project(efemarai_file=file)
 
     table = Table(box=None)
-    [table.add_column(x) for x in ["Id", "Name"]]
+    _ = [table.add_column(x) for x in ["Id", "Name"]]
     for m in project.models:
         table.add_row(m.id, m.name)
     console.print(table)
 
 
 @model.command("log")
 @click.argument("model", required=True)
 def model_version_list(model):
     """Lists the model versions of a particular model / definition file."""
-
     if model.endswith((".yaml", ".yml", ".")):
         if model.endswith("."):
             model = default_yaml
         project = _get_project(efemarai_file=model)
         models_yaml = [m["name"] for m in checker.load_definition(model)["models"]]
         models = [model for model in project.models if model.name in models_yaml]
     else:
         project = _get_project(efemarai_file=default_yaml)
         models = [m for m in project.models if model in (m.name, m.id)]
 
     model_versions = [model.versions() for model in models]
 
     table = Table(box=None)
-    [table.add_column(x) for x in ["Id", "Name", "Description", "Version"]]
+    _ = [table.add_column(x) for x in ["Id", "Name", "Description", "Version"]]
     for model_v in model_versions:
         for m in model_v["objects"]:
             table.add_row(m["id"], m["name"], m["description"], m["version"][:7])
     console.print(table)
 
 
 @model.command("create")
@@ -275,15 +274,14 @@
 @click.option(
     "--warnings/--no-warnings",
     default=True,
     help="Print warnings when checking the model definition.",
 )
 def model_create(definition_file, file, verbose, exists_ok, check_runtime, warnings):
     """Create a model in the current project."""
-
     if definition_file == ".":
         definition_file = default_yaml
 
     checker.print_warnings(warnings)
 
     definition = checker.load_definition(definition_file)
 
@@ -334,15 +332,14 @@
 @click.option(
     "-m",
     "--message",
     help="Model version message.",
 )
 def model_push(definition_file, file, verbose, check_runtime, warnings, message):
     """Pushes a model version in the current project."""
-
     if definition_file == ".":
         definition_file = default_yaml
 
     checker.print_warnings(warnings)
 
     definition = checker.load_definition(definition_file)
 
@@ -416,15 +413,15 @@
     "-f", "--file", help=f"Name of the Efemarai file (Default is '{default_yaml}')"
 )
 def domain_list(file):
     """Lists the domains in the current project."""
     project = _get_project(efemarai_file=file)
 
     table = Table(box=None)
-    [table.add_column(x) for x in ["Id", "Name"]]
+    _ = [table.add_column(x) for x in ["Id", "Name"]]
     for d in project.domains:
         table.add_row(d.id, d.name)
     console.print(table)
 
 
 @domain.command("create")
 @click.argument("definition-file", required=True)
@@ -442,15 +439,14 @@
     default=True,
     help="Print warnings when checking the domain definition.",
 )
 def domain_create(definition_file, file, verbose, exists_ok, warnings):
     """Create a domain in the current project.
 
     definition_file (str): YAML file containing domain definition."""
-
     checker.print_warnings(warnings)
 
     definition = checker.load_definition(definition_file)
 
     if not checker.check(
         definition,
         definition_filename=definition_file,
@@ -542,15 +538,15 @@
 def domain_apply(domain_name, image, output, file):
     with console.status("Applying domain transformations...", spinner_style="green"):
         project = _get_project(efemarai_file=file)
 
         domain = project.domain(domain_name)
         if not domain:
             console.print(f":poop: Domain '{domain_name}' does not exist.", style="red")
-            exit(1)
+            sys.exit(1)
 
         image = cv2.imread(image)
 
         if image.shape[-1] == 1:
             image = cv2.cvtColor(image, cv2.COLOR_GRAY2RGB)
         elif image.shape[-1] == 3:
             image = cv2.cvtColor(image, cv2.COLOR_BGR2RGB)
@@ -622,15 +618,14 @@
     default=True,
     help="Print warnings when checking the dataset definition.",
 )
 def dataset_create(definition_file, file, wait, verbose, exists_ok, warnings):
     """Create a dataset in the current project.
 
     definition_file (str): YAML file containing dataset definition."""
-
     checker.print_warnings(warnings)
 
     if definition_file == ".":
         definition_file = default_yaml
 
     definition = checker.load_definition(definition_file)
 
@@ -690,15 +685,15 @@
         console.print(
             f"\nRun the command with a specific dataset id: [bold green]$ efemarai dataset delete {datasets[-1].id}",
         )
         sys.exit(1)
 
     dataset_name = dataset
     dataset = project.dataset(dataset)
-    if not dataset:
+    if dataset is None:
         console.print(f":poop: Dataset '{dataset_name}' does not exist.", style="red")
         sys.exit(1)
 
     dataset.delete(delete_dependants)
 
 
 @dataset.command("download")
@@ -792,21 +787,21 @@
     """Enhance a dataset by applying a domain from the current project."""
     project = _get_project(efemarai_file=file)
 
     dataset_name = dataset
     dataset = project.dataset(dataset)
     if not dataset:
         console.print(f":poop: Dataset '{dataset_name}' does not exist.", style="red")
-        exit(1)
+        sys.exit(1)
 
     domain_name = domain
     domain = project.domain(domain)
     if not domain:
         console.print(f":poop: Domain '{domain_name}' does not exist.", style="red")
-        exit(1)
+        sys.exit(1)
 
     enhanced_dataset = dataset.enhance(domain, samples_per_datapoint, new_name)
 
     if not wait:
         return
 
     _wait_for_runs([enhanced_dataset])
@@ -1132,15 +1127,15 @@
             table.add_column(c.capitalize())
     for t in tests:
         row = []
         for c in columns_list:
             if hasattr(t, c):
                 obj = getattr(t, c)
                 if hasattr(obj, "name"):
-                    obj = getattr(obj, "name")
+                    obj = obj.name
                 row.append(str(obj))
         table.add_row(*row)
     console.print(table)
 
 
 def _check_for_multiple_entities(entities, name):
     return len([x for x in entities if x.name == name]) > 1
@@ -1155,17 +1150,18 @@
                 f":poop: Project '{efemarai_file}' does not exist.", style="red"
             )
             sys.exit(1)
 
         return project
 
     # Check if definition needs to be overwritten from file
-    if definition is not None:
-        if "project" not in definition or "name" not in definition["project"]:
-            definition = None
+    if definition is not None and (
+        "project" not in definition or "name" not in definition["project"]
+    ):
+        definition = None
 
     if definition is None or efemarai_file is not None:
         if efemarai_file is None:
             efemarai_file = default_yaml
 
         if not os.path.exists(efemarai_file):
             console.print(
```

### Comparing `efemarai-0.3.3/efemarai/dataset.py` & `efemarai-0.3.4/efemarai/dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,17 +11,15 @@
 from efemarai.console import console
 from efemarai.fields import AnnotationClass, sdk_deserialize
 from efemarai.job_state import JobState
 from efemarai.problem_type import ProblemType
 
 
 class DatasetFormat(str, Enum):
-    """
-    Possible dataset formats.
-    """
+    """Possible dataset formats."""
 
     COCO = "COCO"
     ImageRegression = "ImageRegression"
     ImageNet = "ImageNet"
     TFRecord = "tfrecord"
     Custom = "Custom"
 
@@ -92,37 +90,37 @@
         format=None,
         data_url=None,
         annotations_url=None,
         credentials=None,
         upload=None,
         num_datapoints=None,
         mask_generation=None,
-        min_asset_size=None,
+        min_asset_area=None,
     ):
-        """
-        Create a dataset. A more convenient way is to use `project.create_model(...)`.
-        """
-
+        """Create a dataset. A more convenient way is to use `project.create_dataset(...)`."""
         if stage is not None and data_url is not None:
             # Remote dataset
-            assert DatasetFormat.has(
-                format
-            ), f"Dataset format '{format}' should be in {DatasetFormat.list()}."
-
-            assert DatasetStage.has(
-                stage
-            ), f"Dataset stage '{stage}' should be in {DatasetStage.list()}."
+            if not DatasetFormat.has(format):
+                raise AssertionError(
+                    f"Dataset format '{format}' should be in {DatasetFormat.list()}."
+                )
+
+            if not DatasetStage.has(stage):
+                raise AssertionError(
+                    f"Dataset stage '{stage}' should be in {DatasetStage.list()}."
+                )
 
             if name is None or data_url is None:
                 return None
 
-            assert mask_generation in (None, "Simple", "Advanced")
+            if mask_generation not in (None, "Simple", "Advanced"):
+                raise AssertionError("Mask generation not in (None, Simple, Advanced)")
 
             response = project._put(
-                f"api/dataset",
+                "api/dataset",
                 json={
                     "name": name,
                     "format": format,
                     "stage": stage,
                     "data_url": data_url,
                     "annotations_url": annotations_url,
                     "access_token": credentials,
@@ -138,15 +136,15 @@
                     project._upload(annotations_url, endpoint)
                 project._upload(data_url, endpoint)
                 project._post(
                     endpoint,
                     json={
                         "num_samples": num_datapoints,
                         "mask_generation": mask_generation,
-                        "min_asset_size": min_asset_size,
+                        "min_asset_area": min_asset_area,
                     },
                 )
 
             return Dataset(
                 project=project,
                 name=name,
                 stage=stage,
@@ -154,15 +152,15 @@
                 format=format,
                 data_url=data_url,
                 annotations_url=annotations_url,
                 state="NotStarted",
                 classes=[],
             )
         response = project._put(
-            f"api/dataset",
+            "api/dataset",
             json={
                 "name": name,
                 "format": format,
                 "stage": stage,
                 # "data_url": data_url,
                 # "annotations_url": annotations_url,
                 "access_token": credentials,
@@ -179,15 +177,15 @@
                 project._upload(annotations_url, endpoint)
             project._upload(data_url, endpoint)
             project._post(
                 endpoint,
                 json={
                     "num_samples": num_datapoints,
                     "mask_generation": mask_generation,
-                    "min_asset_size": min_asset_size,
+                    "min_asset_area": min_asset_area,
                 },
             )
 
         # Custom dataset to be uploaded
         return Dataset(
             project=project,
             name=name,
@@ -259,25 +257,25 @@
             f"\n  annotations_url={self.annotations_url}"
             if self.annotations_url
             else ""
         )
         res += f"\n  state={self.state}"
         res += f"\n  state_message={self.state_message}"
         res += f"\n  classes={self.classes}"
-        res += f"\n)"
+        res += "\n)"
         return res
 
     @staticmethod
     def deserialize_datapoint(data):
         """Returns a datapoint from the data field."""
         datapoint = sdk_deserialize(data)
         datapoint.inputs = [sdk_deserialize(json.loads(i)) for i in datapoint.inputs]
         # Dereference target ref_fields
-        for i in range(len(datapoint.targets)):
-            data = json.loads(datapoint.targets[i])
+        for i, target in enumerate(datapoint.targets):
+            data = json.loads(target)
             if "ref_field" in data and len(data["ref_field"]) > 0:
                 data["ref_field"] = [
                     di
                     for ref in data["ref_field"]
                     for di in datapoint.inputs
                     if str(di.id) in str(ref)
                 ]
@@ -408,15 +406,15 @@
         """
         Reloads the dataset *in place* from the remote endpoint and return it.
 
         Returns:
             The updated dataset object.
         """
         if self.id is None:
-            return
+            return None
 
         endpoint = f"api/dataset/{self.id}"
         dataset_details = self.project._get(endpoint)
 
         self.name = dataset_details["name"]
         self.format = dataset_details["format"]
         self.stage = dataset_details["stage"]
@@ -442,15 +440,14 @@
         Args:
             num_samples (int): Number of samples to download. Leave `None` for all.
             dataset_format (str): What format to download the dataset. Currently supported include `COCO`, `YOLO`, `VOC`, `ImageNet`, `CSV`.
             path (str): The path where to download the data.
             unzip (bool): Should the downloaded zip be unzipped.
             ignore_cache (bool): Force regeneration of the dataset by ignoring the cache. May lead to slower subsequent calls.
         """
-
         if self.id is None:
             return
 
         if self.running:
             console.print(":poop: Dataset has not finished loading.", style="red")
             return None
```

### Comparing `efemarai-0.3.3/efemarai/definition_checker.py` & `efemarai-0.3.4/efemarai/definition_checker.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from efemarai.dataset import DatasetFormat, DatasetStage
 from efemarai.runtime_checker import RuntimeChecker
 
 # from efemarai.problem_type import ProblemType
 
 
 class DefinitionChecker(BaseChecker):
-    _allowed_vars = set(["datapoints"])
+    _allowed_vars = {"datapoints"}
 
     def __init__(self):
         super().__init__()
         self._status = console.status("Checking...")
 
     @staticmethod
     def is_path_remote(path):
@@ -114,15 +114,15 @@
         )
 
     def check_project(self, definition):
         self._status.update("Checking project...")
 
         project = self._get_required_item(definition, "project")
 
-        name = self._get_required_item(project, "name", "project")
+        # name = self._get_required_item(project, "name", "project")
 
         # problem_type = self._get_required_item(project, "problem_type", "project")
 
         # if not ProblemType.has(problem_type):
         #     self._error(f"Unsupported problem type '{problem_type}' (in 'project')")
 
     def check_datasets(self, definition):
@@ -297,18 +297,23 @@
                     except git.exc.GitError:
                         self._error(
                             f"Commit '{hash}' does not exist (in '{repo_parent}')"
                         )
 
                 yield repo.working_dir
         else:
+            # Local path - convert to absolute path
+            url = os.path.abspath(url)
             if not os.path.isdir(url):
                 self._error(
                     f"Repository path '{url}' (in '{repo_parent}') must be a folder."
                 )
+            # Check if the directory is empty
+            if len(os.listdir(url)) == 0:
+                self._error(f"Repository path '{url}' (in '{repo_parent}') is empty.")
             yield url
 
     def _check_files(self, model, parent):
         files = model.get("files", [])
         known_files = set()
         for i, file in enumerate(files):
             file_parent = parent + f".files[{i}]"
```

### Comparing `efemarai-0.3.3/efemarai/domain.py` & `efemarai-0.3.4/efemarai/domain.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,22 +7,20 @@
     """
     Provides domain related functionality. The easiest way to interact with this object is through the UI.
     It can be created through the :class:`efemarai.project.Project.create_domain` method.
     """
 
     @staticmethod
     def create(project, name, transformations):
-        """
-        Create a domain. A more convenient way is to use `project.create_domain(...)`.
-        """
+        """Create a domain. A more convenient way is to use `project.create_domain(...)`."""
         if name is None or name is None or transformations is None:
             return None
 
         response = project._put(
-            f"api/domain",
+            "api/domain",
             json={"name": name, "projectId": project.id},
         )
         domain_id = response["id"]
 
         response = project._put(
             f"api/domain/{domain_id}/import-flow",
             json={
@@ -44,15 +42,15 @@
         return self.apply(image)
 
     def __repr__(self):
         res = f"{self.__module__}.{self.__class__.__name__}("
         res += f"\n  id={self.id}"
         res += f"\n  name={self.name}"
         res += f"\n  transformations={self.transformations}"
-        res += f"\n)"
+        res += "\n)"
         return res
 
     def download(self, filename=None) -> str:
         """
         Downalod the domain specifications to a local file.
 
         Args:
@@ -73,24 +71,22 @@
         response = self.project._get(f"api/domain/{self.id}/export")
         with open(filename, "w") as f:
             f.write(response["definition"])
 
         return filename
 
     def delete(self, delete_dependants=False):
-        """
-        Delete the domain. You cannot delete an object that is used in a stress test or a baseline (delete those first). This cannot be undone.
-        """
+        """Delete the domain. You cannot delete an object that is used in a stress test or a baseline (delete those first). This cannot be undone."""
         self.project._delete(
             f"api/domain/{self.id}/{delete_dependants}",
         )
 
     def apply(self, image):
         response = self.project._post(
-            f"api/generateImageSdk",
+            "api/generateImageSdk",
             json={
                 "domainId": str(self.id),
                 "image": _encode_ndarray(image),
                 "inputKeyName": "image",
             },
         )
```

### Comparing `efemarai-0.3.3/efemarai/fields/__init__.py` & `efemarai-0.3.4/efemarai/fields/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 SDK_CLASS_STRUCTURE = dict(inspect.getmembers(sys.modules[__name__], inspect.isclass))
 
 
 def sdk_deserialize(data):
     if "_cls" not in data:
         print(f":poop: Cannot locate class from the data {data.keys()}.")
-        return
+        return None
 
     c = SDK_CLASS_STRUCTURE[data["_cls"]]
     sdk_type = data.pop("_cls")
 
     # "data" stores the loaded image in an np.ndarray
     if (
         "data" in data
```

### Comparing `efemarai-0.3.3/efemarai/fields/annotation_fields.py` & `efemarai-0.3.4/efemarai/fields/annotation_fields.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,20 +59,19 @@
         id: int = None,
         confidence: float = None,
         color: str = None,
         text_color: str = None,
         category: str = None,
         slug: str = None,
     ):
-        assert not (
-            name is None and id is None
-        ), "'name' and 'id' cannot be None at the same time."
+        if name is None and id is None:
+            raise AssertionError("'name' and 'id' cannot be None at the same time.")
 
         self.name = name
-        self.id = id
+        self.id = int(id)
         self.confidence = confidence
         self.category = category
         self.color = color if color is not None else self.get_random_color()
         self.text_color = (
             text_color if text_color is not None else self.get_random_color()
         )
         self.slug = slug if slug is not None else self.get_slug()
@@ -83,29 +82,29 @@
     @staticmethod
     def get_random_color():
         import random
 
         def r():
             return random.randint(0, 255)
 
-        return "#%02X%02X%02X" % (r(), r(), r())
+        return f"#{r():02X}{r():02X}{r():02X}"
 
     def _serialize(self):
         return sdk_serialize(self)
 
     def __repr__(self):
         res = f"{self.__module__}.{self.__class__.__name__}("
         res += f"\n  name={self.name}"
         res += f"\n  id={self.id}"
         res += f"\n  confidence={self.confidence}"
         res += f"\n  color={self.color}" if self.color else ""
         res += f"\n  text_color={self.text_color}" if self.text_color else ""
         res += f"\n  category={self.category}" if self.category else ""
         res += f"\n  slug={self.slug}"
-        res += f"\n)"
+        res += "\n)"
         return res
 
 
 class Tag(BaseField):
     """
     Represents an annotation that can be used for classification.
 
@@ -174,15 +173,15 @@
         res = f"{self.__module__}.{self.__class__.__name__}("
         res += f"\n  label={self.label}"
         res += f"\n  probabilities={self.probabilities}"
         res += f"\n  confidence={self.confidence}"
         res += f"\n  description={self.description}"
         res += f"\n  ref_field={self.ref_field}"
         res += f"\n  key_name={self.key_name}"
-        res += f"\n)"
+        res += "\n)"
         return res
 
 
 class Value(BaseField):
     """
     Represents an annotation that can be used for regression.
 
@@ -233,15 +232,15 @@
 
     def __repr__(self):
         res = f"{self.__module__}.{self.__class__.__name__}("
         res += f"\n  value={self.value}"
         res += f"\n  description={self.description}"
         res += f"\n  ref_field={self.ref_field}"
         res += f"\n  key_name={self.key_name}"
-        res += f"\n)"
+        res += "\n)"
         return res
 
 
 class InstanceField(BaseField):
     """
     This is a base class. Represents an annotation of an instance that can be
     attached to any other field and can act as a label.
@@ -325,29 +324,34 @@
             confidence=confidence,
             id=id,
             description=description,
             ref_field=ref_field,
             key_name=key_name,
             user_attributes=user_attributes,
         )
-        self.xyxy = xyxy
+
+        self.xyxy = tuple(
+            i if not isinstance(i, (np.int64, np.int32)) else i.item() for i in xyxy
+        )
         self.area = (
-            area if area is not None else (xyxy[2] - xyxy[0]) * (xyxy[3] - xyxy[1])
+            area
+            if area is not None
+            else (self.xyxy[2] - self.xyxy[0]) * (self.xyxy[3] - self.xyxy[1])
         )
 
     def __repr__(self):
         res = f"{self.__module__}.{self.__class__.__name__}("
         res += f"\n  xyxy={self.xyxy}"
         res += f"\n  area={self.area}"
         res += f"\n  instance_id={self.instance_id}"
         res += f"\n  description={self.description}"
         res += f"\n  ref_field={self.ref_field}"
         res += f"\n  label={self.label}"
         res += f"\n  key_name={self.key_name}"
-        res += f"\n)"
+        res += "\n)"
         return res
 
     @property
     def width(self):
         return self.xyxy[2] - self.xyxy[0] + 1
 
     @property
@@ -364,24 +368,27 @@
 
 
 class Polygon(InstanceField):
     """
     Represents a polygon annotation.
 
     Args:
-        vertices List[List[Tuple[float]]]: Coordinates of the polygon absolute values in format [[[point]...],[[point]...]]
-            where the first list contains all instances of the polygon, the second contains lists of single points.
+        vertices List[List[Tuple[float]]]: Coordinates of the polygon. The
+            values in are in format [[[point]...],[[point]...]] in image dimensions,
+            where the first list contains all contours of the polygon, the internal
+            ones - lists of single points of that contour.
         label (AnnotationClass): An AnnotationClass associated with the instance
         area (Optional[float]): Area of the polygon
         instance_id (Optional[id]): Id of the instance within the dataset
         confidence (Optional[float]): Confidence level of the field.
         description (Optional[str]): A description of the object or annotation information.
         ref_field (List[object]): A list of objects the current BaseField is refering to.
         key_name (Optional[str]): A string key, by which the field can be identified.
-        user_attributes (Optional[Dict[str, object]]): Dictionary containing additional data regarding the field.
+        user_attributes (Optional[Dict[str, object]]): Dictionary containing
+            additional data regarding the field.
 
     Returns:
         :class: `efemarai.fields.annotation_fields.Polygon`: A Polygon object.
 
     You can construct a polygon from the output of a model that is a mask:
 
     .. code-block:: python
@@ -392,15 +399,15 @@
         mask = np.zeros((100, 100), dtype=np.uint8)
         mask[10:30, 10:50] = 255
 
         label = ef.AnnotationClass(id=1)
         polygon = ef.InstanceMask(label=label, data=mask).to_polygon()
         print(label, polygon)
 
-        new_poly = ef.Polygon(label=label, vertices=polygon.certices)
+        new_poly = ef.Polygon(label=label, vertices=polygon.vertices)
         print(new_poly)
     """
 
     def __init__(
         self,
         vertices: List[List[Tuple[float, float]]],
         label: AnnotationClass,
@@ -419,28 +426,46 @@
             confidence=confidence,
             id=id,
             description=description,
             ref_field=ref_field,
             key_name=key_name,
             user_attributes=user_attributes,
         )
+
+        if not (
+            isinstance(vertices, (list, tuple))
+            and all(
+                (isinstance(v, (list, tuple)))
+                and all(
+                    (isinstance(p, (tuple, list)))
+                    and len(p) == 2
+                    and all(isinstance(f, (float, int)) for f in p)
+                    for p in v
+                )
+                for v in vertices
+            )
+        ):
+            raise ValueError(
+                "Polygon vertices are not of type List[List[List[float/int, float/int], ...]] or Tuple[Tuple[Tuple[float/int, float/int], ...]]"
+            )
+
         self.vertices = vertices
         self.area = area
 
     def __repr__(self):
         res = f"{self.__module__}.{self.__class__.__name__}("
         res += f"\n  vertices={self.vertices}"
         res += f"\n  area={self.area}"
         res += f"\n  instance_id={self.instance_id}"
         res += f"\n  description={self.description}"
         res += f"\n  label={self.label}"
         res += f"\n  confidence={self.confidence}"
         res += f"\n  ref_field={self.ref_field}"
         res += f"\n  key_name={self.key_name}"
-        res += f"\n)"
+        res += "\n)"
         return res
 
 
 class Keypoint(InstanceField):
     """
     Represents a keypoint annotation.
 
@@ -486,16 +511,16 @@
             confidence=confidence,
             id=id,
             description=description,
             ref_field=ref_field,
             key_name=key_name,
             user_attributes=user_attributes,
         )
-        self.x = x
-        self.y = y
+        self.x = x if not isinstance(i, (np.int64, np.int32)) else i.item()
+        self.y = y if not isinstance(i, (np.int64, np.int32)) else i.item()
         self.name = name
         self.index = index
         self.annotated = annotated
         self.occluded = occluded
 
     def __repr__(self):
         res = f"{self.__module__}.{self.__class__.__name__}("
@@ -504,15 +529,15 @@
         res += f"\n  occluded={self.occluded}"
         res += f"\n  instance_id={self.instance_id}"
         res += f"\n  description={self.description}"
         res += f"\n  label={self.label}"
         res += f"\n  ref_field={self.ref_field}"
         res += f"\n  key_name={self.key_name}"
         res += f"\n  id={self.id}"
-        res += f"\n)"
+        res += "\n)"
         return res
 
     @staticmethod
     def chunks(lst, n):
         """Yield successive n-sized chunks from lst."""
         for i in range(0, len(lst), n):
             yield lst[i : i + n]
@@ -583,15 +608,15 @@
                     confidence=1,
                 )
             )
     """
 
     def __init__(
         self,
-        keypoints: list,
+        keypoints: List[Keypoint],
         label: AnnotationClass,
         edges: list = None,
         instance_id: int = None,
         confidence: float = None,
         id: ObjectId = None,
         description: str = None,
         ref_field: list = None,
@@ -605,20 +630,26 @@
             id=id,
             description=description,
             ref_field=ref_field,
             key_name=key_name,
             user_attributes=user_attributes,
         )
         self.keypoints = keypoints
-        self.edges = edges
+        self.edges = [
+            (f, t)
+            if not isinstance(f, (np.int64, np.int32))
+            or not isinstance(t, (np.int64, np.int32))
+            else (int(f), int(t))
+            for (f, t) in edges
+        ]
 
     def __repr__(self):
         res = f"{self.__module__}.{self.__class__.__name__}("
         res += f"\n  keypoints={self.keypoints}"
-        res += f"\n)"
+        res += "\n)"
         return res
 
 
 class PolarVector:
     def __init__(self, angle: float, length: float):
 
         self.angle = angle
```

### Comparing `efemarai-0.3.3/efemarai/fields/base_fields.py` & `efemarai-0.3.4/efemarai/fields/base_fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,9 +99,9 @@
         res = f"{self.__module__}.{self.__class__.__name__}("
         res += f"\n  id={self.id}"
         res += f"\n  description={self.description}"
         res += f"\n  ref_field={self.ref_field}"
         res += f"\n  key_name={self.key_name}"
         res += f"\n  confidence={self.confidence}"
         res += f"\n  user_attributes={self.user_attributes}"
-        res += f"\n)"
+        res += "\n)"
         return res
```

### Comparing `efemarai-0.3.3/efemarai/fields/data_fields.py` & `efemarai-0.3.4/efemarai/fields/data_fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,18 +7,17 @@
 from bson.objectid import ObjectId
 from PIL import Image as pil_image
 
 from efemarai.fields.annotation_fields import AnnotationClass, InstanceField, Polygon
 from efemarai.fields.base_fields import BaseField, sdk_serialize
 
 
-def create_polygons_from_mask(mask_img):
-    # TODO: Remove from DatapointStore (v1)
+def create_polygons_from_mask(mask_img, threshold_value=127):
     # Get contours as polygons and the area of the polygons
-    ret, thresh = cv2.threshold(mask_img, 127, 255, 0)
+    ret, thresh = cv2.threshold(mask_img, threshold_value, 255, 0)
     (
         contours,
         hierarchy,
     ) = cv2.findContours(  # Format: [[[[x1, y1]], [[x2, y2]]...], ...]
         thresh, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE
     )
     if not contours:
@@ -99,17 +98,18 @@
             id=id,
             description=description,
             ref_field=ref_field,
             key_name=key_name,
             user_attributes=user_attributes,
         )
 
-        assert not (
-            file_path is None and data is None
-        ), f"You need to specify either a 'file_path'({file_path}) or 'data'({data})."
+        if file_path is None and data is None:
+            raise AssertionError(
+                f"You need to specify either a 'file_path'({file_path}) or 'data'({data})."
+            )
 
         self.file_path = file_path
         self.width = width
         self.height = height
         self._raw = data
 
         # Skip check for 0-1 images (TODO: give warning)
@@ -136,37 +136,36 @@
         if self._raw is None:
             self._raw = np.asarray(pil_image.open(self.file_path))
             self.height = self._raw.shape[0]
             self.width = self._raw.shape[1]
         return self._raw
 
     def set_data(self, data: np.ndarray):
-        assert (
-            self._raw.dtype == np.uint8
-        ), f"Expected format {np.uint8}. Received {data.dtype}."
+        if self._raw.dtype != np.uint8:
+            raise AssertionError(f"Expected format {np.uint8}. Received {data.dtype}.")
 
         self._raw = data
         self.height = self._raw.shape[0]
         self.width = self._raw.shape[1]
 
     def __repr__(self):
         res = f"{self.__module__}.{self.__class__.__name__}("
         res += f"\n  id={self.id}"
         res += f"\n  file_path={self.file_path}"
-        res += f"\n  data=" + (
+        res += "\n  data=" + (
             f"{self._raw.shape}, {self._raw.dtype}, min({np.min(self._raw)}), max({np.max(self._raw)})"
             if self._raw is not None
             else "<not-loaded>"
         )
         res += f"\n  width={self.width}"
         res += f"\n  height={self.height}"
         res += f"\n  description={self.description}"
         res += f"\n  ref_field={self.ref_field}"
         res += f"\n  key_name={self.key_name}"
-        res += f"\n)"
+        res += "\n)"
         return res
 
 
 class Mask(Image):
     """Used for Semantic Segmentation. Same as Image class, but whenever rescaled, Image.Nearest strategy is used."""
 
     pass
@@ -241,27 +240,27 @@
             user_attributes=user_attributes,
         )
 
     def __repr__(self):
         res = f"{self.__module__}.{self.__class__.__name__}("
         res += f"\n  id={self.id}"
         res += f"\n  file_path={self.file_path}"
-        res += f"\n  data=" + (
+        res += "\n  data=" + (
             f"{self._raw.shape}, {self._raw.dtype}, min({np.min(self._raw)}), max({np.max(self._raw)})"
             if self._raw is not None
             else "<not-loaded>"
         )
         res += f"\n  confidence={self.confidence}"
         res += f"\n  label={self.label}"
         res += f"\n  width={self.width}"
         res += f"\n  height={self.height}"
         res += f"\n  description={self.description}"
         res += f"\n  ref_field={self.ref_field}"
         res += f"\n  key_name={self.key_name}"
-        res += f"\n)"
+        res += "\n)"
         return res
 
     def to_polygon(self):
         """
         Converts `efemarai.fields.data_fields.InstanceMask` to `efemarai.fields.annotation_fields.Polygon`
 
         Returns:
```

### Comparing `efemarai-0.3.3/efemarai/fields/datapoint.py` & `efemarai-0.3.4/efemarai/fields/datapoint.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 import os
+import tempfile
 from glob import glob
 from typing import Union
 
 import ffmpeg
 from bson.objectid import ObjectId
 
 from efemarai.console import console
@@ -19,36 +20,31 @@
     images, text, etc) and the annotations (bounding boxes, polygons, etc).
 
     Args:
         dataset (efemarai.dataset.Dataset): Instance of a Dataset object
         inputs (list[BaseFields]): List of Basefields to represent the inputs to the datapoint.
         targets (list[BaseFields]): List of Basefields to represent the targets to the inputs datapoint.
         id (Optional[ObjectId]): A valid ObjectId for the datapoint
-        info (Optional[dict]): Any additional information that needs to be stored in the datapoint
     Returns:
         :class: `efemarai.fields.datapoint.Datapoint`
     """
 
-    def __init__(
-        self, dataset, inputs=None, targets=None, id=None, info: dict = None
-    ) -> None:
+    def __init__(self, dataset, inputs=None, targets=None, id=None) -> None:
         self.inputs = self.sanitize_format(inputs)
         self.targets = self.sanitize_format(targets)
         self.dataset = dataset
         self.id = id if id is not None else ObjectId()
-        self.info = info
 
     def __repr__(self):
         res = f"{self.__module__}.{self.__class__.__name__}("
         res += f"\n  id={self.id}"
         res += f"\n  dataset={self.dataset}"
         res += f"\n  inputs={self.inputs}"
         res += f"\n  targets={self.targets}"
-        res += f"\n  info={self.info}"
-        res += f"\n)"
+        res += "\n)"
         return res
 
     @staticmethod
     def sanitize_format(data):
         if data is None:
             return []
 
@@ -77,15 +73,15 @@
             or not len(_target.vertices) > 0
             or not isinstance(_target.vertices[0][0][0], (float, int))
         ):
             console.print(
                 ":poop: We do not support empty polygons or RLE style polygons yet. Please pass a list of lists of floats.",
                 style="red",
             )
-            return
+            return None
 
         self.targets.append(_target)
         return self.targets
 
     def add_inputs(self, _input: Union[BaseField, InstanceField]):
         """
         Used to add inputs to the datapoint.
@@ -103,51 +99,51 @@
     def _post(self, endpoint, json=None, params=None):
         return self.dataset.project._session._post(endpoint, json, params)
 
     def _put(self, endpoint, json=None, params=None):
         return self.dataset.project._put(endpoint, json, params)
 
     def _handle_video(self, ef_video):
-        TMP_VIDEO_FRAME_DIR = "/tmp/"
-        video_info = ffmpeg.probe(ef_video.file_path)["streams"]
-        width = [info["width"] for info in video_info if info.get("width")][0]
-        height = [info["height"] for info in video_info if info.get("height")][0]
-
-        basename = os.path.basename(ef_video.file_path)
-        out_path = os.path.join(TMP_VIDEO_FRAME_DIR, basename)
-        os.makedirs(out_path, exist_ok=True)
-        ffmpeg.input(ef_video.file_path).output(
-            f"{out_path}/{basename}_frame_%08d.png", **{"qscale:v": 2}
-        ).run(quiet=True)
-
-        frames = sorted(glob(f"{out_path}/{basename}_frame_*.png"))
-        # ffmpeg r_frame_rate is a string in decimal format -> "12/1"
-        r_frame_rate = [
-            info["r_frame_rate"] for info in video_info if info.get("width")
-        ][0].split("/")
-        fps = int(r_frame_rate[0]) / int(r_frame_rate[1])
-        ef_video.width = width
-        ef_video.height = height
-        ef_video.fps = fps
-        ef_video.frame_count = len(frames)
-        for frame in frames:
-            ef_video.frames.append(
-                VideoFrame(
-                    index=frame.split("_")[-1].strip(".png"),
-                    file_path=frame,
-                    width=width,
-                    height=height,
+        with tempfile.TemporaryDirectory() as TMP_VIDEO_FRAME_DIR:
+            video_info = ffmpeg.probe(ef_video.file_path)["streams"]
+            width = [info["width"] for info in video_info if info.get("width")][0]
+            height = [info["height"] for info in video_info if info.get("height")][0]
+
+            basename = os.path.basename(ef_video.file_path)
+            out_path = os.path.join(TMP_VIDEO_FRAME_DIR, basename)
+            os.makedirs(out_path, exist_ok=True)
+            ffmpeg.input(ef_video.file_path).output(
+                f"{out_path}/{basename}_frame_%08d.png", **{"qscale:v": 2}
+            ).run(quiet=True)
+
+            frames = sorted(glob(f"{out_path}/{basename}_frame_*.png"))
+            # ffmpeg r_frame_rate is a string in decimal format -> "12/1"
+            r_frame_rate = [
+                info["r_frame_rate"] for info in video_info if info.get("width")
+            ][0].split("/")
+            fps = int(r_frame_rate[0]) / int(r_frame_rate[1])
+            ef_video.width = width
+            ef_video.height = height
+            ef_video.fps = fps
+            ef_video.frame_count = len(frames)
+            for frame in frames:
+                ef_video.frames.append(
+                    VideoFrame(
+                        index=frame.split("_")[-1].strip(".png"),
+                        file_path=frame,
+                        width=width,
+                        height=height,
+                    )
                 )
-            )
-            self.dataset.project._upload(
-                frame,
-                f"api/datapoint/{self.dataset.id}/upload",
-                verbose=False,
-            )
-            os.remove(frame)
+                self.dataset.project._upload(
+                    frame,
+                    f"api/datapoint/{self.dataset.id}/upload",
+                    verbose=False,
+                )
+                os.remove(frame)
 
     def upload(self, copy_files=True):
         """
         Used to upload a datapoint to the system.
 
         Args:
             copy_files (bool): Whether to copy the files or to upload them
@@ -183,21 +179,20 @@
 
         serialized_targets = [
             json.loads(target._serialize()) for target in self.targets
         ]
         serialized_inputs = [json.loads(_input._serialize()) for _input in self.inputs]
 
         response = self._put(
-            f"api/datapoint/undefined",
+            "api/datapoint/undefined",
             json={
                 "access_token": self.dataset.project._session.token,
                 "datasetId": self.dataset.id,
                 "targets": serialized_targets,
                 "inputs": serialized_inputs,
-                "info": self.info,
             },
         )
 
         datapoint_id = response["id"]
         if not copy_files:
             return datapoint_id
 
@@ -235,15 +230,14 @@
 
             import efemarai as ef
 
             images = datapoints[0].get_inputs_with_type(ef.Image)
             # images is a list of all of the ef.Image elements in datapoints[0].
             # each of those images can be accessed by datapoints[0].get_input(images[0].key_name)
         """
-
         res = []
         for _input in self.inputs:
             if ef_type is type(Video):
                 res.append(_input)
                 continue
             if isinstance(_input, ef_type):
                 res.append(_input)
@@ -260,13 +254,29 @@
 
         Args:
             ef_type (BaseField): An instance of `efemarai.fields.base_fields.BaseField`.
 
         Returns:
             list[BaseField] - a list of inputs of the ef_type
         """
-
         res = []
         for target in self.targets:
             if isinstance(target, ef_type):
                 res.append(target)
         return res
+
+    def get_input_refs(self, ids):
+        """
+        Returns a list of field in input that refer to id.
+
+        Args:
+            ids (List[ObjectId]): Ids when referenced to return object, or [] if not found.
+
+        Returns:
+            An instance of BaseField
+        """
+        refs = []
+        for _input in self.inputs:
+            if _input.id in ids:
+                refs.append(_input)
+
+        return refs
```

### Comparing `efemarai-0.3.3/efemarai/formats/config.py` & `efemarai-0.3.4/efemarai/formats/config.py`

 * *Files identical despite different names*

### Comparing `efemarai-0.3.3/efemarai/formats/dataset_coco.py` & `efemarai-0.3.4/efemarai/formats/dataset_coco.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,17 +109,15 @@
                     polygons, polygons_area = create_polygons_from_mask(mask_img)
                     polygons = [list(itertools.chain(*polygon)) for polygon in polygons]
                     cocoAnn["segmentation"] = polygons
                     cocoAnn["area"] = polygons_area
 
                 vertices = []
                 for polygon in cocoAnn["segmentation"]:
-                    vertices.append(
-                        list(zip(polygon[:-1][::2], polygon[1:][::2]))
-                    )
+                    vertices.append(list(zip(polygon[:-1][::2], polygon[1:][::2])))
 
                 datapoint.add_target(
                     Polygon(
                         label=label,
                         vertices=vertices,
                         area=cocoAnn["area"],
                         instance_id=instance_id,
```

### Comparing `efemarai-0.3.3/efemarai/formats/dataset_imagenet.py` & `efemarai-0.3.4/efemarai/formats/dataset_imagenet.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,18 +25,18 @@
     dataset = project.create_dataset(
         name=name, stage=stage, format=DatasetFormat.Custom
     )
 
     # Creating classes based on folders
     classes = sorted(next(os.walk(data_url.replace("file://", "", 1)))[1])
 
-    for i in range(len(classes)):
+    for i, class_name in enumerate(classes):
         dataset.add_annotation_class(
             id=i,
-            name=classes[i],
+            name=class_name,
             color=CLASS_COLORS[i % len(CLASS_COLORS)],
         )
 
     # Loading images into datapoints for each folder
     for class_id, class_name in enumerate(classes):
         for ext in IMAGE_EXTENSIONS:
             for image_file in islice(
```

### Comparing `efemarai-0.3.3/efemarai/model.py` & `efemarai-0.3.4/efemarai/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 class ModelRepository:
     def __init__(self, url=None, branch=None, hash=None, access_token=None):
         self.url = url if url is not None else "."
         self.branch = branch
         self.hash = hash
         self.access_token = access_token
-        self.files = self.get_all_files()
+        self.files = self.get_all_files() if not self.is_remote else []
 
     def __repr__(self):
         res = f"{self.__module__}.{self.__class__.__name__}("
         res += f"\n      url={self.url}"
         res += f"\n      branch={self.branch}"
         res += "\n    )"
         return res
@@ -49,14 +49,15 @@
         ignore_spec = pathspec.PathSpec.from_lines("gitwildmatch", ignore_lines)
 
         files = [
             file
             for file in list(Path(self.url).glob("**/*"))
             if not ignore_spec.match_file(str(file))
         ]
+
         return files
 
     @staticmethod
     def calculate_file_hash(filepath):
         return ModelHasher._calculate_file_hash(filepath=filepath)
 
     def get_last_commit(self, access_token):
@@ -67,15 +68,14 @@
             ),
             heads=True,
         )
         return remote_heads.split(f"\trefs/heads/{self.branch}")[0]
 
     @contextmanager
     def archive(self, name):
-
         with tempfile.TemporaryDirectory() as dirpath:
             zip_name = os.path.join(dirpath, name)
 
             with ZipFile(zip_name, "w") as zip:
                 for file in self.files:
                     zip.write(file)
 
@@ -101,33 +101,38 @@
 
     def __repr__(self):
         res = f"{self.__module__}.{self.__class__.__name__}("
         res += f"\n      name={self.name}"
         res += f"\n      url={self.url}"
         res += f"\n      upload={self.upload}"
         res += f"\n      hash_code={self.hash_code}"
-        res += f"\n    )"
+        res += "\n    )"
         return res
 
 
 class ModelHasher:
     @staticmethod
     def _calculate_file_hash(filepath, hashing_algorithm="sha1"):
         """This function returns the SHA-1 hash
         of the file passed into it."""
-
         # make a hash object
         if hashing_algorithm == "md5":
             h = hashlib.md5()
         elif hashing_algorithm == "sha1":
             h = hashlib.sha1()
 
         if str(filepath).startswith("http"):
             return hashlib.sha1(str(filepath).encode("utf-8")).hexdigest()
 
+        if not os.path.exists(filepath):
+            console.print(
+                f":poop: File/folder under '{filepath}' does not exist.", style="red"
+            )
+            raise ValueError()
+
         if os.path.isdir(filepath):
             filenames = [
                 filename
                 for filename in glob(os.path.join(filepath, "**/*"), recursive=True)
                 if os.path.isfile(filename)
             ]
             file_hashes = [ModelHasher._calculate_file_hash(file) for file in filenames]
@@ -193,17 +198,23 @@
         # Remote repo case
         if repository.is_remote:
             repo_hash = (
                 repository.hash
                 if repository.hash is not None
                 else repository.get_last_commit(repository.access_token)
             )
-
-        # Local repo case
         else:
+            # Local repo case
+            if len(repository.files) == 0:
+                console.print(
+                    f"No files in '{repository.url}'. "
+                    "Confirm path and ignore rules in '.gitignore', '.efignore'."
+                )
+                raise ValueError()
+
             repo_hash = "".join(
                 [
                     ModelHasher._calculate_file_hash(filepath=i)
                     for i in repository.files
                     if i.is_file()
                 ]
             )
@@ -211,15 +222,15 @@
         version = hashlib.sha1(
             (repo_hash + model_files_hashes).encode("utf-8")
         ).hexdigest()  # Model hash
 
         files = [ModelFile(**f) if not isinstance(f, ModelFile) else f for f in files]
 
         response = project._put(
-            f"api/model",
+            "api/model",
             json={
                 "name": name,
                 "description": description,
                 "version": version,
                 "repository": {
                     "url": repository.url,
                     "branch": repository.branch,
@@ -286,14 +297,21 @@
             repo_hash = (
                 repository.hash
                 if repository.hash is not None
                 else repository.get_last_commit(repository.access_token)
             )
         else:
             # Local repo
+            if len(repository.files) == 0:
+                console.print(
+                    f"No files in '{repository.url}'. "
+                    "Confirm path and ignore rules in '.gitignore', '.efignore'."
+                )
+                raise ValueError()
+
             repo_hash = "".join(
                 [
                     ModelHasher._calculate_file_hash(filepath=f)
                     for f in repository.files
                     if f.is_file()
                 ]
             )
@@ -301,26 +319,26 @@
         version = hashlib.sha1(
             (repo_hash + model_files_hashes).encode("utf-8")
         ).hexdigest()  # Model hash
 
         # Do not create a new model version if there are no changes
         if version == existing_model.version:
             console.print(
-                f":face_with_monocle: "
-                f"There are were no changes found in the files. Skipping...",
+                ":face_with_monocle: "
+                "There are were no changes found in the files. Skipping...",
                 style="orange1",
             )
             return existing_model
 
         files = [ModelFile(**f) if not isinstance(f, ModelFile) else f for f in files]
         files = Model._point_to_existing_model_files(
             new_model_files=files, existing_model=existing_model
         )
         response = project._put(
-            f"api/model",
+            "api/model",
             json={
                 "name": name,
                 "description": description,
                 "version": version,
                 "repository": {
                     "url": repository.url,
                     "branch": repository.branch,
@@ -368,15 +386,15 @@
         res = f"{self.__module__}.{self.__class__.__name__}("
         res += f"\n  id={self.id}"
         res += f"\n  name={self.name}"
         res += f"\n  description={self.description}"
         res += f"\n  version={self.version}"
         res += f"\n  repository={self.repository}"
         res += f"\n  files={self.files}"
-        res += f"\n)"
+        res += "\n)"
         return res
 
     def delete(self, delete_dependants=False):
         """
         Deletes the model.
 
         You cannot delete an object that is used in a stress test or a baseline
@@ -400,11 +418,9 @@
                     if file.hash_code == f.hash_code
                 ][0]
                 f.upload = False
 
         return new_model_files
 
     def versions(self):
-        """
-        Returns all model versions.
-        """
+        """Returns all model versions."""
         return self.project._get(f"api/modelVersions/{self.id}")
```

### Comparing `efemarai-0.3.3/efemarai/project.py` & `efemarai-0.3.4/efemarai/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
     def __repr__(self):
         res = f"{self.__module__}.{self.__class__.__name__}("
         res += f"\n  id={self.id}"
         res += f"\n  name={self.name}"
         res += f"\n  description={self.description}"
         res += f"\n  problem_type={self.problem_type}"
-        res += f"\n)"
+        res += "\n)"
         return res
 
     def _get(self, endpoint, json=None, params=None):
         return self._session._get(endpoint, json, params, self.id)
 
     def _post(self, endpoint, json=None, params=None):
         return self._session._post(endpoint, json, params, self.id)
@@ -87,15 +87,14 @@
 
     def _upload(self, from_url, endpoint, verbose=True):
         return self._session._upload(from_url, endpoint, self.id, verbose)
 
     @property
     def models(self):
         """Returns a list of the models associated with the project."""
-
         return [
             Model(
                 project=self,
                 id=model["id"],
                 name=model["name"],
                 description=model.get("description"),
                 version=model.get("version"),
@@ -110,27 +109,26 @@
                         url=f["url"],
                         upload=f["upload"],
                         hash_code=f["hash"],
                     )
                     for f in model["files"]
                 ],
             )
-            for model in self._get(f"api/models")
+            for model in self._get("api/models")
         ]
 
     def model(self, model) -> Model:
         """Returns the model specified by the name.
 
         Args:
             model (str): A model identifier. It can either be the name of the model or its id.
 
         Returns:
             :class:`efemarai.model.Model`: A model object or `None` if it doesn't exist.
         """
-
         model = next((m for m in self.models if model in (m.name, m.id)), None)
         return model
 
     def create_model(
         self,
         name,
         description=None,
@@ -152,15 +150,14 @@
 
         Raises:
             ValueError: If the model exists and `exists_ok` is set to `False`.
 
         Returns:
             :class:`efemarai.model.Model`: The created model.
         """
-
         existing_model = next((m for m in self.models if m.name == name), None)
         if existing_model is not None:
             if exists_ok:
                 return existing_model
             raise ValueError(f"Model {name} already exists and exists_ok=False.")
 
         model = Model.create(self, name, description, repository, files)
@@ -182,15 +179,14 @@
             repository (dict, optional): Model repository info. See `ef.model.ModelRepository`.
             files (list[dict]): Files needed to load the model e.g. weights or config
                 files. See `ef.model.ModelFile`.
 
         Returns:
             :class:`efemarai.model.Model`: The created model.
         """
-
         existing_model = next((m for m in self.models if m.name == name), None)
         if existing_model is not None:
             model = Model.push(
                 project=self,
                 name=name,
                 description=description,
                 repository=repository,
@@ -210,41 +206,39 @@
     def datasets(self):
         """
         Returns a list of the datasets associated with the project.
 
         Returns:
             list[:class:`efemarai.dataset.Dataset`]: A list of available datasets.
         """
-
         return [
             Dataset(
                 project=self,
                 name=dataset["name"],
                 stage=dataset["stage"],
                 id=dataset["id"],
                 format=dataset["format"],
                 data_url=dataset.get("data_url"),
                 annotations_url=dataset.get("annotations_url"),
                 state=dataset["states"][-1]["name"],
                 classes=Dataset._parse_classes(dataset["classes"]),
             )
-            for dataset in self._get(f"api/datasets")
+            for dataset in self._get("api/datasets")
         ]
 
     def dataset(self, dataset) -> Dataset:
         """
         Returns the dataset specified by the name or id.
 
         Args:
             dataset (str): A dataset identifier. It can either be the name of the dataset or its id.
 
         Returns:
             :class:`efemarai.dataset.Dataset`: A dataset object or `None` if it doesn't exist.
         """
-
         dataset = next((d for d in self.datasets if dataset in (d.name, d.id)), None)
         return dataset
 
     def create_dataset(
         self,
         name,
         stage,
@@ -252,15 +246,15 @@
         data_url=None,
         annotations_url=None,
         credentials=None,
         upload=False,
         num_datapoints=None,
         mask_generation=None,
         exists_ok=False,
-        min_asset_size=15,
+        min_asset_area=15,
         **kwargs,
     ) -> Dataset:
         """Creates a dataset.
 
         Args:
             name (str): A dataset name.
             format (str): A format of the dataset. Possible formats are specified under `ef.dataset.DatasetFormat`.
@@ -268,23 +262,22 @@
             data_url (str): A url to fetch data. Can be local or remote.
             annotations_url (str, optional): A url that specifies the annotation file. Can be local or remote.
             credentials (str, optional): If the dataset if remote, Specify the `access token` or `{username}:{password}` to access.
             upload (bool, optional): Should the data be uploaded to Efemarai? This would make evaluation and testing much faster.
             num_datapoints (int, optional): Should a subset of the datapoints be loaded as a dataset? Specify the number of dataponts. Useful for quick testing. Use `None` to load all.
             mask_generation (str): What strategy should be used for mask generation.
             exists_ok (bool, optional): If the current named dataset exist, should it be returned or an exception raised.
-            min_asset_size (int, optional): Assets with width and hight smaller than this will be ignored. Default value of 15.
+            min_asset_area (int, optional): Assets with area smaller than this will be ignored. Default value of 15.
 
         Raises:
             ValueError: If the dataset exists and `exists_ok` is set to `False`.
 
         Returns:
             :class:`efemarai.dataset.Dataset`: The created dataset.
         """
-
         existing_dataset = next((d for d in self.datasets if d.name == name), None)
         if existing_dataset is not None:
             if exists_ok:
                 return existing_dataset
             raise ValueError(f"Dataset {name} already exists and exists_ok=False.")
 
         if isinstance(format, str):
@@ -298,28 +291,28 @@
                 stage=stage,
                 data_url=data_url,
                 annotations_url=annotations_url,
                 credentials=credentials,
                 upload=upload,
                 num_datapoints=num_datapoints,
                 mask_generation=mask_generation,
-                min_asset_size=min_asset_size,
+                min_asset_area=min_asset_area,
             )
         elif format == DatasetFormat.COCO:
             from efemarai.formats.dataset_coco import create_coco_dataset
 
             dataset = create_coco_dataset(
                 project=self,
                 name=name,
                 stage=stage,
                 data_url=data_url,
                 annotations_url=annotations_url,
                 num_datapoints=num_datapoints,
                 mask_generation=mask_generation,
-                min_asset_area=min_asset_size,  # TODO: Change all to area
+                min_asset_area=min_asset_area,
             )
         elif format == DatasetFormat.ImageNet:
             from efemarai.formats.dataset_imagenet import create_imagenet_dataset
 
             dataset = create_imagenet_dataset(
                 project=self,
                 name=name,
@@ -340,36 +333,34 @@
     def domains(self):
         """
         Returns a list of the domains associated with the project.
 
         Returns:
             list [:class:`efemarai.domain.Domain`]: A list of available domains.
         """
-
         return [
             Domain(
                 project=self,
                 id=domain["id"],
                 name=domain["name"],
                 transformations=domain["transformations"],
             )
-            for domain in self._get(f"api/domains")
+            for domain in self._get("api/domains")
         ]
 
     def domain(self, domain) -> Domain:
         """
         Returns the domain specified by the name or id.
 
         Args:
             domain (str): A domain identifier. It can either be the name of the domain or its id.
 
         Returns:
             :class:`efemarai.domain.Domain`: A domain object or `None` if it doesn't exist.
         """
-
         domain = next((d for d in self.domains if domain in (d.name, d.id)), None)
         return domain
 
     def create_domain(self, name, transformations, exists_ok=False, **kwargs) -> Domain:
         """
         Creates a domain. **The recommended strategy** is to use the UI to build up the domain visually.
         The domain then can be exported to a yaml configuration file for storage and loaded/reused through `ef.Session().load(...)`.
@@ -381,15 +372,14 @@
 
         Raises:
             ValueError: If the domain exists and `exists_ok` is set to `False`.
 
         Returns:
             :class:`efemarai.domain.Domain`: The created domain.
         """
-
         existing_domain = next((d for d in self.domains if d.name == name), None)
         if existing_domain is not None:
             if exists_ok:
                 return existing_domain
             raise ValueError(f"Domain {name} already exists and exists_ok=False.")
 
         domain = Domain.create(self, name, transformations)
@@ -399,27 +389,26 @@
     def baselines(self):
         """
         Returns a list of the baselines associated with the project.
 
         Returns:
             list [:class:`efemarai.baseline.Baseline`]: A list of available baselines.
         """
-
         return [
             Baseline(
                 project=self,
                 id=baseline["id"],
                 name=baseline["name"],
                 model=baseline["model"],
                 dataset=baseline["dataset"]["id"],
                 state=baseline["states"][-1]["name"],
                 state_message=baseline["states"][-1].get("message"),
                 reports=baseline["reports"],
             )
-            for baseline in self._get(f"api/baselineRuns")["objects"]
+            for baseline in self._get("api/baselineRuns")["objects"]
         ]
 
     def baseline(self, baseline_run) -> Baseline:
         """
         Returns the baseline specified by the name or id.
 
         Args:
@@ -448,15 +437,14 @@
             model (str, :class:`efemarai.model.Model`): The model to stress test.
             domain (str, :class:`efemarai.domain.Domain`): The domain from which to generate samples.
             dataset (str, :class:`efemarai.dataset.Dataset`): The dataset with which to generate samples.
 
         Returns:
             :class:`efemarai.baseline.Baseline`: A baseline object.
         """
-
         baseline = Baseline.create(
             project=self,
             name=name,
             model=model,
             dataset=dataset,
         )
 
@@ -466,28 +454,27 @@
     def stress_tests(self):
         """
         Returns a list of the stress tests associated with the project.
 
         Returns:
             list [:class:`efemarai.stress_test.StressTest`]: A list of available stress tests.
         """
-
         return [
             StressTest(
                 project=self,
                 id=test["id"],
                 name=test["name"],
                 model=test["model"],
                 domain=test["domain"]["id"],
                 dataset=test["dataset"]["id"],
                 state=test["states"][-1]["name"],
                 state_message=test["states"][-1].get("message"),
                 reports=test["reports"],
             )
-            for test in self._get(f"api/getRuns")["objects"]
+            for test in self._get("api/getRuns")["objects"]
         ]
 
     def stress_test(self, test) -> StressTest:
         """
         Returns the stress test specified by the name or id.
 
         Args:
@@ -521,33 +508,29 @@
             num_samples (int, optional): Sample count to generate.
             num_runs (int, optional): Number of searches to run.
             concurrent_runs (int, optional): Number of concurrent searches.
 
         Returns:
             :class:`efemarai.stress_test.StressTest`: A stress test object.
         """
-
         test = StressTest.create(
             project=self,
             name=name,
             model=model,
             domain=domain,
             dataset=dataset,
             num_samples=num_samples,
             num_runs=num_runs,
             concurrent_runs=concurrent_runs,
         )
 
         return test
 
     def delete(self, delete_dependants=False):
-        """
-        Deletes a project, including the domains, datasets, models, stress tests. Cannot be undone.
-        """
-
+        """Deletes a project, including the domains, datasets, models, stress tests. Cannot be undone."""
         self._delete(f"api/project/{self.id}/{delete_dependants}")
 
     def export_datasets(
         self,
         test_run_ids: list = None,
         min_score=0.0,
         include_dataset=False,
@@ -567,15 +550,14 @@
             unzip (bool, optional): If the zip file should be unzipped.
             ignore_cache (bool, optional): Force regeneration of the dataset by ignoring the cache. May lead to slower subsequent calls.
             export_format (str): The format of the output vulnerabilities dataset.
 
         Returns:
             str: The filename of the resulting object.
         """
-
         if export_format is None:
             if self.problem_type == ProblemType.Classification:
                 export_format = "imagenet"
             elif self.problem_type == ProblemType.ObjectDetection:
                 export_format = "coco"
             elif self.problem_type == ProblemType.InstanceSegmentation:
                 export_format = "coco"
@@ -681,15 +663,14 @@
             unzip (bool, optional): If the zip file should be unzipped.
             ignore_cache (bool, optional): Force regeneration of the dataset by ignoring the cache. May lead to slower subsequent calls.
             export_format (str): The format of the output vulnerabilities dataset.
 
         Returns:
             str: The filename of the resulting object.
         """
-
         stress_tests = [self.stress_test(test_id) for test_id in test_run_ids]
         for stress_test in stress_tests:
             if not stress_test.finished:
                 console.print(
                     (
                         ":warning: Cannot export vulnerabilities "
                         "dataset as stress test is still running"
```

### Comparing `efemarai-0.3.3/efemarai/runtime_checker.py` & `efemarai-0.3.4/efemarai/runtime_checker.py`

 * *Files identical despite different names*

### Comparing `efemarai-0.3.3/efemarai/session.py` & `efemarai-0.3.4/efemarai/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,23 +54,23 @@
         else:
             console.print("URL: ", existing_config["url"])
             console.print("User: ", existing_config["username"])
             console.print()
             if not Confirm.ask(
                 "Do you want to overwrite existing config?", default=False
             ):
-                return
+                return None
 
         console.print()
 
         username = Prompt.ask("Username")
         password = Prompt.ask("Password", password=True)
 
         while True:
-            url = Prompt.ask("Platform URL", default=f"https://ci.efemarai.com")
+            url = Prompt.ask("Platform URL", default="https://ci.efemarai.com")
 
             if not re.match(r"^https?://", url):
                 url = "https://" + url
 
             if not url.endswith("/"):
                 url += "/"
 
@@ -111,19 +111,14 @@
 
         if not os.path.isfile(config_file):
             return None
 
         return Session._load_config_file(config_file)
 
     @staticmethod
-    def _save_config_file(data, filename):
-        with open(filename, "w") as f:
-            yaml.dump(data, f)
-
-    @staticmethod
     def _load_config_file(filename):
         checker = DefinitionChecker()
         return checker.load_definition(filename)
 
     @staticmethod
     def _progress_bar(verbose):
         return Progress(
@@ -169,15 +164,14 @@
 
         .. code-block:: python
 
             import efemarai as ef
             result = ef.Session().load("efemarai.yaml")
             print(result)
         """
-
         config = self._load_config_file(filename)
 
         project = None
         if "project" in config:
             project = self.create_project(**config["project"], exists_ok=exists_ok)
 
         if project_only:
@@ -210,15 +204,14 @@
     def projects(self):
         """
         Returns the list of projects.
 
         Returns:
             list [:class:`efemarai.project.Project`]: A list of the available projects.
         """
-
         return [
             Project(
                 self,
                 project["id"],
                 project["name"],
                 project.get("description", ""),
                 project["problem_type"],
@@ -240,15 +233,14 @@
 
         .. code-block:: python
 
             import efemarai as ef
             project = ef.Session().project("Name")
             print(project)
         """
-
         project = next((p for p in self.projects if name in (p.name, p.id)), None)
         return project
 
     def create_project(
         self,
         name,
         description=None,
@@ -268,15 +260,14 @@
 
         Raises:
             ValueError: If the project exists and `exists_ok` is set to `False`.
 
         Returns:
             :class:`efemarai.project.Project`: A project object.
         """
-
         project = Project.create(
             self, name, description, problem_type, private, exists_ok
         )
         return project
 
     def _get(self, endpoint, json=None, params=None, project_id=None):
         return self._make_request(requests.get, endpoint, json, params, project_id)
@@ -367,29 +358,29 @@
 
         s3, bucket, prefix = self._get_access(endpoint, project_id)
 
         with self._progress_bar(verbose) as progress:
             task = progress.add_task(
                 f"Uploading '{dirname}' ", total=float(len(filenames))
             )
-            for index, filename in enumerate(filenames):
+            for filename in filenames:
                 object_key = os.path.join(
                     dirname, os.path.relpath(filename, start=from_url)
                 ).replace(ntpath.sep, posixpath.sep)
 
                 with smart_open(filename, "rb") as f:
                     s3.upload_fileobj(f, bucket, prefix + object_key)
 
                 progress.advance(task)
 
         if verbose:
             console.print(f":heavy_check_mark: Uploaded '{from_url}'", style="green")
 
     def _get_access(self, endpoint, project_id):
-        access = self._access_requests.get(endpoint, None)
+        access = self._access_requests.get(endpoint)
 
         if access is None or access["Expiration"] <= datetime.now():
             access = self._get(endpoint, project_id=project_id)
             access["Expiration"] = datetime.strptime(
                 access["Expiration"], "%Y-%m-%dT%H:%M:%SZ"
             )
             self._access_requests[endpoint] = access
```

### Comparing `efemarai-0.3.3/efemarai/stress_test.py` & `efemarai-0.3.4/efemarai/stress_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,15 +45,14 @@
         domain,
         dataset,
         num_samples,
         num_runs,
         concurrent_runs,
     ):
         """Create a stress test. A more convenient way is to use :func:`project.create_stress_test`"""
-
         if isinstance(model, str):
             model = project.model(model)
 
         if isinstance(dataset, str):
             dataset = project.dataset(dataset)
 
         if isinstance(domain, str):
@@ -136,15 +135,15 @@
         res += f"\n  name={self.name}"
         res += f"\n  model={self.model.name}"
         res += f"\n  domain={self.domain.name}"
         res += f"\n  dataset={self.dataset.name}"
         res += f"\n  state={self.state}"
         res += f"\n  state_message={self.state_message}"
         res += f"\n  len(reports)={len(self.reports)}"
-        res += f"\n)"
+        res += "\n)"
         return res
 
     @property
     def reports(self):
         """Returns the stress test reports. This can be slow as is potentially fetching a large object."""
         if not self._reports:
             response = self.project._get(
@@ -154,80 +153,71 @@
             self._reports = response["reports"]
 
         return self._reports
 
     @property
     def model(self):
         """Returns the model associated with the stress test."""
-
         if self._model is None:
             self._model = next(m for m in self.project.models if m.id == self._model_id)
         return self._model
 
     @property
     def domain(self):
         """Returns the domain associated with the stress test."""
-
         if self._domain is None:
             self._domain = next(
                 d for d in self.project.domains if d.id == self._domain_id
             )
         return self._domain
 
     @property
     def dataset(self):
         """Returns the dataset associated with the stress test."""
-
         if self._dataset is None:
             self._dataset = next(
                 d for d in self.project.datasets if d.id == self._dataset_id
             )
         return self._dataset
 
     @property
     def finished(self):
         """Returns if the stress test has successfully finished.
 
         :rtype: bool
         """
-
         return self.state == JobState.Finished
 
     @property
     def failed(self):
         """Returns if the stress test has failed.
 
         :rtype: bool
         """
-
         return self.state == JobState.Failed
 
     @property
     def running(self):
         """Returns if the stress test is still running - not failed or finished.
 
         :rtype: bool
         """
-
         return self.state not in (JobState.Finished, JobState.Failed)
 
     def delete(self):
-        """
-        Deletes a stress test. This cannot be undone.
-        """
+        """Deletes a stress test. This cannot be undone."""
         self.project._delete("api/stressTest?id=" + self.id)
 
     def reload(self):
         """
         Reloads the stress test *in place* from the remote endpoint and return it.
 
         Rerturns:
             The updated stress test object.
         """
-
         response = self.project._get("api/getTestRun", params={"testRunId": self.id})
 
         self.state = JobState(response["states"][-1]["name"])
         self.state_message = response["states"][-1].get("message")
         self._reports = response.get("reports", {})
 
         return self
@@ -248,15 +238,15 @@
             # Collapse repeating spaces
             filename = re.sub(r"  +", r" ", filename)
             # Replace spaces with dashes and convert to lowercase
             filename = filename.replace(" ", "_").lower()
             filename += ".json"
 
         with open(filename, "w") as f:
-            f.write(json.dumps(self.reports))
+            json.dump(self.reports, f)
 
         return filename
 
     def vulnerabilities_dataset(
         self,
         min_score=0.0,
         include_dataset=False,
@@ -275,15 +265,14 @@
             unzip (bool, optional): If the zip file should be unzipped.
             ignore_cache (bool, optional): Force regeneration of the dataset by ignoring the cache. May lead to slower subsequent calls.
             export_format (str): The format of the output vulnerabilities dataset.
 
         Returns:
             str: The filename of the resulting object.
         """
-
         if not self.finished:
             console.print(
                 (
                     ":warning: Cannot export vulnerabilities "
                     "dataset as stress test is still running"
                 ),
                 style="yellow",
```

### Comparing `efemarai-0.3.3/efemarai.egg-info/PKG-INFO` & `efemarai-0.3.4/efemarai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: efemarai
-Version: 0.3.3
+Version: 0.3.4
 Summary: A CLI and SDK for interacting with the Efemarai ML testing platform.
 Home-page: https://www.efemarai.com/
 Author: Efemarai
 Author-email: support@efemarai.com
 License: MIT license
-Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 A CLI and SDK for interacting with the [Efemarai ML testing platform](https://efemarai.com).
 
 ## Setup
 
@@ -101,9 +100,7 @@
 
 # access the created entities
 project = result["project"]
 models = result["models"]
 domains = result["domains"]
 datasets = result["datasets"]
 ```
-
-
```

### Comparing `efemarai-0.3.3/efemarai.egg-info/SOURCES.txt` & `efemarai-0.3.4/efemarai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `efemarai-0.3.3/setup.py` & `efemarai-0.3.4/setup.py`

 * *Files identical despite different names*

