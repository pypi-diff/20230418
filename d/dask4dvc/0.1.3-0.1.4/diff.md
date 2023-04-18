# Comparing `tmp/dask4dvc-0.1.3.tar.gz` & `tmp/dask4dvc-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dask4dvc-0.1.3.tar", max compression
+gzip compressed data, was "dask4dvc-0.1.4.tar", max compression
```

## Comparing `dask4dvc-0.1.3.tar` & `dask4dvc-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    13576 2023-01-25 13:10:23.183284 dask4dvc-0.1.3/LICENSE
--rw-r--r--   0        0        0     1456 2023-04-13 11:02:16.857294 dask4dvc-0.1.3/README.md
--rw-r--r--   0        0        0      521 2023-01-25 13:44:53.309679 dask4dvc-0.1.3/dask4dvc/__init__.py
--rw-r--r--   0        0        0       76 2023-01-25 13:44:53.309679 dask4dvc-0.1.3/dask4dvc/cli/__init__.py
--rw-r--r--   0        0        0     5896 2023-04-13 11:06:02.374819 dask4dvc-0.1.3/dask4dvc/cli/main.py
--rw-r--r--   0        0        0     3037 2023-01-25 13:44:53.309679 dask4dvc-0.1.3/dask4dvc/methods.py
--rw-r--r--   0        0        0      166 2023-01-25 13:44:53.309679 dask4dvc-0.1.3/dask4dvc/utils/__init__.py
--rw-r--r--   0        0        0      413 2023-01-25 13:44:53.309679 dask4dvc-0.1.3/dask4dvc/utils/config.py
--rw-r--r--   0        0        0     1055 2023-04-13 11:02:16.867293 dask4dvc-0.1.3/dask4dvc/utils/dask.py
--rw-r--r--   0        0        0     5807 2023-01-25 13:44:53.309679 dask4dvc-0.1.3/dask4dvc/utils/dvc.py
--rw-r--r--   0        0        0      951 2023-01-25 13:44:53.309679 dask4dvc-0.1.3/dask4dvc/utils/git.py
--rw-r--r--   0        0        0      903 2023-04-13 12:46:43.228695 dask4dvc-0.1.3/dask4dvc/utils/main.py
--rw-r--r--   0        0        0     1241 2023-04-13 12:45:20.249602 dask4dvc-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2350 1970-01-01 00:00:00.000000 dask4dvc-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    13576 2023-01-25 13:10:23.183284 dask4dvc-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1456 2023-04-13 11:02:16.857294 dask4dvc-0.1.4/README.md
+-rw-r--r--   0        0        0      521 2023-01-25 13:44:53.309679 dask4dvc-0.1.4/dask4dvc/__init__.py
+-rw-r--r--   0        0        0       76 2023-01-25 13:44:53.309679 dask4dvc-0.1.4/dask4dvc/cli/__init__.py
+-rw-r--r--   0        0        0     6243 2023-04-18 15:37:16.965339 dask4dvc-0.1.4/dask4dvc/cli/main.py
+-rw-r--r--   0        0        0     4447 2023-04-18 15:37:16.965339 dask4dvc-0.1.4/dask4dvc/methods.py
+-rw-r--r--   0        0        0      166 2023-01-25 13:44:53.309679 dask4dvc-0.1.4/dask4dvc/utils/__init__.py
+-rw-r--r--   0        0        0      413 2023-01-25 13:44:53.309679 dask4dvc-0.1.4/dask4dvc/utils/config.py
+-rw-r--r--   0        0        0     1055 2023-04-13 11:02:16.867293 dask4dvc-0.1.4/dask4dvc/utils/dask.py
+-rw-r--r--   0        0        0     5807 2023-04-18 13:10:44.129812 dask4dvc-0.1.4/dask4dvc/utils/dvc.py
+-rw-r--r--   0        0        0      951 2023-01-25 13:44:53.309679 dask4dvc-0.1.4/dask4dvc/utils/git.py
+-rw-r--r--   0        0        0      903 2023-04-13 12:46:43.228695 dask4dvc-0.1.4/dask4dvc/utils/main.py
+-rw-r--r--   0        0        0     1290 2023-04-18 15:37:16.975339 dask4dvc-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2395 1970-01-01 00:00:00.000000 dask4dvc-0.1.4/PKG-INFO
```

### Comparing `dask4dvc-0.1.3/LICENSE` & `dask4dvc-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dask4dvc-0.1.3/README.md` & `dask4dvc-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `dask4dvc-0.1.3/dask4dvc/__init__.py` & `dask4dvc-0.1.4/dask4dvc/__init__.py`

 * *Files identical despite different names*

### Comparing `dask4dvc-0.1.3/dask4dvc/cli/main.py` & `dask4dvc-0.1.4/dask4dvc/cli/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,16 @@
 def repro(
     address: str = typer.Option(None, help=Help.address),
     option: typing.List[str] = typer.Option(None, help=Help.option),
     leave: bool = typer.Option(True, help=Help.leave),
     detach: bool = typer.Option(False, "--detach", "-d", help=Help.detach),
     config: str = typer.Option(None, help=Help.config),
     target: list[str] = typer.Argument(None, help=Help.target, show_default=False),
+    parallel: bool = typer.Option(True, help=Help.parallel),
+    max_workers: int = typer.Option(None, help="Maximum number of workers to use."),
 ) -> None:
     """Replicate 'dvc repro' command using dask."""
     if detach:
         cmd = ["dask4dvc", "repro"]
         if address is not None:
             cmd += ["--address", address]
         if config is not None:
@@ -61,18 +63,23 @@
         return
 
     if config is not None:
         assert address is None, "Can not use address and config file"
         address = utils.dask.get_cluster_from_config(config)
 
     with dask.distributed.Client(address) as client:
+        if max_workers is not None:
+            client.cluster.adapt(minimum=1, maximum=max_workers)
         log.info(client)
-        result = client.submit(
-            utils.dvc.repro, targets=target, options=option, pure=False
-        )
+        if parallel:
+            result = methods.parallel_submit(client)
+        else:
+            result = client.submit(
+                utils.dvc.repro, targets=target, options=option, pure=False
+            )
 
         utils.dask.wait_for_futures(result)
         if not leave:
             utils.main.wait()
 
 
 @app.command()
```

### Comparing `dask4dvc-0.1.3/dask4dvc/utils/dask.py` & `dask4dvc-0.1.4/dask4dvc/utils/dask.py`

 * *Files identical despite different names*

### Comparing `dask4dvc-0.1.3/dask4dvc/utils/dvc.py` & `dask4dvc-0.1.4/dask4dvc/utils/dvc.py`

 * *Files identical despite different names*

### Comparing `dask4dvc-0.1.3/dask4dvc/utils/git.py` & `dask4dvc-0.1.4/dask4dvc/utils/git.py`

 * *Files identical despite different names*

### Comparing `dask4dvc-0.1.3/dask4dvc/utils/main.py` & `dask4dvc-0.1.4/dask4dvc/utils/main.py`

 * *Files identical despite different names*

### Comparing `dask4dvc-0.1.3/pyproject.toml` & `dask4dvc-0.1.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dask4dvc"
-version = "0.1.3"
+version = "0.1.4"
 description = "Use dask to run the DVC graph"
 authors = ["zincwarecode <zincwarecode@gmail.com>"]
 license = "Apache-2.0"
 keywords=["data-science", "HPC", "dask", "DVC"]
 readme = "README.md"
 
 [tool.poetry.urls]
@@ -12,17 +12,18 @@
 
 [tool.poetry.dependencies]
 python = "^3.8"
 dask = "^2022.7.1"
 distributed = "^2022.7.1"
 dask-jobqueue = "^0.8.1"
 dvc = "^2.34.3"
-typer = "^0.7.0"
+typer = {extras = ["all"], version = "^0.7.0"}
 bokeh = "^2"
 # for bokeh see https://distributed.dask.org/en/stable/changelog.html#v2022-11-1
+znflow = "^0.1.11"
 
 [tool.poetry.scripts]
 dask4dvc = 'dask4dvc.cli.main:app'
 
 [tool.poetry.group.dev.dependencies]
 jupyterlab = "^3.4.4"
 black = "^22.6.0"
```

### Comparing `dask4dvc-0.1.3/PKG-INFO` & `dask4dvc-0.1.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask4dvc
-Version: 0.1.3
+Version: 0.1.4
 Summary: Use dask to run the DVC graph
 License: Apache-2.0
 Keywords: data-science,HPC,dask,DVC
 Author: zincwarecode
 Author-email: zincwarecode@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -14,15 +14,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: bokeh (>=2,<3)
 Requires-Dist: dask (>=2022.7.1,<2023.0.0)
 Requires-Dist: dask-jobqueue (>=0.8.1,<0.9.0)
 Requires-Dist: distributed (>=2022.7.1,<2023.0.0)
 Requires-Dist: dvc (>=2.34.3,<3.0.0)
-Requires-Dist: typer (>=0.7.0,<0.8.0)
+Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
+Requires-Dist: znflow (>=0.1.11,<0.2.0)
 Project-URL: repository, https://github.com/zincware/dask4dvc
 Description-Content-Type: text/markdown
 
 [![Coverage Status](https://coveralls.io/repos/github/zincware/dask4dvc/badge.svg?branch=main)](https://coveralls.io/github/zincware/dask4dvc?branch=main)
 ![PyTest](https://github.com/zincware/dask4dvc/actions/workflows/pytest.yaml/badge.svg)
 [![PyPI version](https://badge.fury.io/py/dask4dvc.svg)](https://badge.fury.io/py/dask4dvc)
 [![zincware](https://img.shields.io/badge/Powered%20by-zincware-darkcyan)](https://github.com/zincware)
```

