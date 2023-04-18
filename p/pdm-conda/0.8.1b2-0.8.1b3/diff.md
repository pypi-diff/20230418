# Comparing `tmp/pdm_conda-0.8.1b2.tar.gz` & `tmp/pdm_conda-0.8.1b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdm_conda-0.8.1b2.tar", last modified: Sun Apr 16 20:38:06 2023, max compression
+gzip compressed data, was "pdm_conda-0.8.1b3.tar", last modified: Sun Apr 16 21:55:24 2023, max compression
```

## Comparing `pdm_conda-0.8.1b2.tar` & `pdm_conda-0.8.1b3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1065 2022-12-16 23:52:20.043514 pdm_conda-0.8.1b2/LICENSE
--rw-r--r--   0        0        0     4832 2023-04-09 20:29:55.601420 pdm_conda-0.8.1b2/README.md
--rw-r--r--   0        0        0     2020 2023-04-16 20:38:07.194508 pdm_conda-0.8.1b2/pyproject.toml
--rw-r--r--   0        0        0      595 2023-04-15 20:17:55.377949 pdm_conda-0.8.1b2/src/pdm_conda/__init__.py
--rw-r--r--   0        0        0        0 2023-01-06 20:52:28.238706 pdm_conda-0.8.1b2/src/pdm_conda/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-01-06 20:52:59.837399 pdm_conda-0.8.1b2/src/pdm_conda/cli/commands/__init__.py
--rw-r--r--   0        0        0     3219 2023-04-09 20:29:55.603310 pdm_conda-0.8.1b2/src/pdm_conda/cli/commands/add.py
--rw-r--r--   0        0        0     1681 2023-04-09 20:29:55.604146 pdm_conda-0.8.1b2/src/pdm_conda/cli/commands/remove.py
--rw-r--r--   0        0        0     2183 2023-04-09 20:29:55.604925 pdm_conda-0.8.1b2/src/pdm_conda/cli/utils.py
--rw-r--r--   0        0        0    11223 2023-04-15 17:34:37.904070 pdm_conda-0.8.1b2/src/pdm_conda/conda.py
--rw-r--r--   0        0        0        0 2023-01-05 20:40:25.652497 pdm_conda-0.8.1b2/src/pdm_conda/installers/__init__.py
--rw-r--r--   0        0        0     2482 2023-04-09 20:29:55.606525 pdm_conda-0.8.1b2/src/pdm_conda/installers/manager.py
--rw-r--r--   0        0        0     2311 2023-04-15 20:38:24.832128 pdm_conda-0.8.1b2/src/pdm_conda/installers/synchronizers.py
--rw-r--r--   0        0        0     3132 2023-01-17 17:44:51.337923 pdm_conda-0.8.1b2/src/pdm_conda/mapping.py
--rw-r--r--   0        0        0        0 2023-01-02 22:45:44.891129 pdm_conda-0.8.1b2/src/pdm_conda/models/__init__.py
--rw-r--r--   0        0        0        0 2023-03-30 01:53:52.844040 pdm_conda-0.8.1b2/src/pdm_conda/models/__pycache__/candidates.cpython-310.pyc.281473776611248
--rw-r--r--   0        0        0     6776 2023-04-09 20:29:55.608074 pdm_conda-0.8.1b2/src/pdm_conda/models/candidates.py
--rw-r--r--   0        0        0     1818 2023-04-15 01:10:11.358619 pdm_conda-0.8.1b2/src/pdm_conda/models/conda.py
--rw-r--r--   0        0        0     7145 2023-04-10 20:13:29.271209 pdm_conda-0.8.1b2/src/pdm_conda/models/config.py
--rw-r--r--   0        0        0     3492 2023-04-15 19:31:29.818151 pdm_conda-0.8.1b2/src/pdm_conda/models/environment.py
--rw-r--r--   0        0        0     3863 2023-04-09 20:29:55.610491 pdm_conda-0.8.1b2/src/pdm_conda/models/repositories.py
--rw-r--r--   0        0        0    10806 2023-04-15 17:37:15.580889 pdm_conda-0.8.1b2/src/pdm_conda/models/requirements.py
--rw-r--r--   0        0        0      900 2023-04-09 20:29:55.611942 pdm_conda-0.8.1b2/src/pdm_conda/models/setup.py
--rw-r--r--   0        0        0     8413 2023-04-14 22:23:45.622217 pdm_conda-0.8.1b2/src/pdm_conda/project.py
--rw-r--r--   0        0        0        0 2023-02-18 20:09:32.663574 pdm_conda-0.8.1b2/src/pdm_conda/resolver/__init__.py
--rw-r--r--   0        0        0     1134 2023-02-23 00:47:35.312247 pdm_conda-0.8.1b2/src/pdm_conda/resolver/providers.py
--rw-r--r--   0        0        0     5455 2023-04-15 17:36:44.693219 pdm_conda-0.8.1b2/src/pdm_conda/resolvers.py
--rw-r--r--   0        0        0      784 2023-01-10 16:37:32.674613 pdm_conda-0.8.1b2/src/pdm_conda/utils.py
--rw-r--r--   0        0        0     6627 1970-01-01 00:00:00.000000 pdm_conda-0.8.1b2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2022-12-16 23:52:20.043514 pdm_conda-0.8.1b3/LICENSE
+-rw-r--r--   0        0        0     4832 2023-04-09 20:29:55.601420 pdm_conda-0.8.1b3/README.md
+-rw-r--r--   0        0        0     1962 2023-04-16 21:55:24.322209 pdm_conda-0.8.1b3/pyproject.toml
+-rw-r--r--   0        0        0      595 2023-04-16 21:54:51.001898 pdm_conda-0.8.1b3/src/pdm_conda/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-06 20:52:28.238706 pdm_conda-0.8.1b3/src/pdm_conda/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-06 20:52:59.837399 pdm_conda-0.8.1b3/src/pdm_conda/cli/commands/__init__.py
+-rw-r--r--   0        0        0     3219 2023-04-09 20:29:55.603310 pdm_conda-0.8.1b3/src/pdm_conda/cli/commands/add.py
+-rw-r--r--   0        0        0     1681 2023-04-09 20:29:55.604146 pdm_conda-0.8.1b3/src/pdm_conda/cli/commands/remove.py
+-rw-r--r--   0        0        0     2183 2023-04-09 20:29:55.604925 pdm_conda-0.8.1b3/src/pdm_conda/cli/utils.py
+-rw-r--r--   0        0        0    11223 2023-04-15 17:34:37.904070 pdm_conda-0.8.1b3/src/pdm_conda/conda.py
+-rw-r--r--   0        0        0        0 2023-01-05 20:40:25.652497 pdm_conda-0.8.1b3/src/pdm_conda/installers/__init__.py
+-rw-r--r--   0        0        0     2482 2023-04-09 20:29:55.606525 pdm_conda-0.8.1b3/src/pdm_conda/installers/manager.py
+-rw-r--r--   0        0        0     2311 2023-04-15 20:38:24.832128 pdm_conda-0.8.1b3/src/pdm_conda/installers/synchronizers.py
+-rw-r--r--   0        0        0     3132 2023-01-17 17:44:51.337923 pdm_conda-0.8.1b3/src/pdm_conda/mapping.py
+-rw-r--r--   0        0        0        0 2023-01-02 22:45:44.891129 pdm_conda-0.8.1b3/src/pdm_conda/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-30 01:53:52.844040 pdm_conda-0.8.1b3/src/pdm_conda/models/__pycache__/candidates.cpython-310.pyc.281473776611248
+-rw-r--r--   0        0        0     6776 2023-04-09 20:29:55.608074 pdm_conda-0.8.1b3/src/pdm_conda/models/candidates.py
+-rw-r--r--   0        0        0     1818 2023-04-15 01:10:11.358619 pdm_conda-0.8.1b3/src/pdm_conda/models/conda.py
+-rw-r--r--   0        0        0     7145 2023-04-10 20:13:29.271209 pdm_conda-0.8.1b3/src/pdm_conda/models/config.py
+-rw-r--r--   0        0        0     3606 2023-04-16 21:54:51.005272 pdm_conda-0.8.1b3/src/pdm_conda/models/environment.py
+-rw-r--r--   0        0        0     3863 2023-04-09 20:29:55.610491 pdm_conda-0.8.1b3/src/pdm_conda/models/repositories.py
+-rw-r--r--   0        0        0    10806 2023-04-15 17:37:15.580889 pdm_conda-0.8.1b3/src/pdm_conda/models/requirements.py
+-rw-r--r--   0        0        0      900 2023-04-09 20:29:55.611942 pdm_conda-0.8.1b3/src/pdm_conda/models/setup.py
+-rw-r--r--   0        0        0     8413 2023-04-14 22:23:45.622217 pdm_conda-0.8.1b3/src/pdm_conda/project.py
+-rw-r--r--   0        0        0        0 2023-02-18 20:09:32.663574 pdm_conda-0.8.1b3/src/pdm_conda/resolver/__init__.py
+-rw-r--r--   0        0        0     1134 2023-02-23 00:47:35.312247 pdm_conda-0.8.1b3/src/pdm_conda/resolver/providers.py
+-rw-r--r--   0        0        0     5455 2023-04-15 17:36:44.693219 pdm_conda-0.8.1b3/src/pdm_conda/resolvers.py
+-rw-r--r--   0        0        0      784 2023-01-10 16:37:32.674613 pdm_conda-0.8.1b3/src/pdm_conda/utils.py
+-rw-r--r--   0        0        0     6663 1970-01-01 00:00:00.000000 pdm_conda-0.8.1b3/PKG-INFO
```

### Comparing `pdm_conda-0.8.1b2/LICENSE` & `pdm_conda-0.8.1b3/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.1b2/README.md` & `pdm_conda-0.8.1b3/README.md`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.1b2/pyproject.toml` & `pdm_conda-0.8.1b3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -20,43 +20,37 @@
 dynamic = []
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3 :: Only",
 ]
 dependencies = [
-    "pytest",
+    "pdm~=2.4.0",
+    "requests>=2.28.1",
 ]
-version = "0.8.1b2"
+version = "0.8.1b3"
 
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 Homepage = "https://github.com/macro128/pdm-conda"
 Changelog = "https://github.com/macro128/pdm-conda/blob/main/CHANGELOG.md"
 
 [project.entry-points.pdm]
 conda = "pdm_conda:main"
 
-[tool.pdm.conda]
-runner = "micromamba"
-channels = [
-    "conda-forge",
+[tool.pdm.dev-dependencies]
+dev = [
+    "pytest>=7.2.0",
+    "pytest-mock>=3.10.0",
+    "pytest-cov>=4.0.0",
+    "pytest-random-num>=1.0.13",
+    "responses>=0.22.0",
 ]
-as-default-manager = true
-excludes = [
-    "streamlink",
-    "moto",
-    "python-telegram-bot-raw",
-    "fastapi-crudrouter",
-    "ormar",
-    "databases",
-]
-batched-commands = true
 
 [tool.pdm.version]
 source = "file"
 path = "src/pdm_conda/__init__.py"
 
 [tool.pdm.build]
 package-dir = "src"
```

### Comparing `pdm_conda-0.8.1b2/src/pdm_conda/__init__.py` & `pdm_conda-0.8.1b3/src/pdm_conda/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,8 +14,8 @@
     core.register_command(AddCommand)
     core.register_command(RemoveCommand)
 
     for name, config in CONFIGS:
         core.add_config(name, config)
 
 
-__version__ = "0.8.1b2"
+__version__ = "0.8.1b3"
```

### Comparing `pdm_conda-0.8.1b2/src/pdm_conda/cli/commands/add.py` & `pdm_conda-0.8.1b3/src/pdm_conda/cli/commands/add.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.1b2/src/pdm_conda/cli/commands/remove.py` & `pdm_conda-0.8.1b3/src/pdm_conda/cli/commands/remove.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.1b2/src/pdm_conda/cli/utils.py` & `pdm_conda-0.8.1b3/src/pdm_conda/cli/utils.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.1b2/src/pdm_conda/conda.py` & `pdm_conda-0.8.1b3/src/pdm_conda/conda.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.1b2/src/pdm_conda/installers/manager.py` & `pdm_conda-0.8.1b3/src/pdm_conda/installers/manager.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.1b2/src/pdm_conda/installers/synchronizers.py` & `pdm_conda-0.8.1b3/src/pdm_conda/installers/synchronizers.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.1b2/src/pdm_conda/mapping.py` & `pdm_conda-0.8.1b3/src/pdm_conda/mapping.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.1b2/src/pdm_conda/models/candidates.py` & `pdm_conda-0.8.1b3/src/pdm_conda/models/candidates.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.1b2/src/pdm_conda/models/conda.py` & `pdm_conda-0.8.1b3/src/pdm_conda/models/conda.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.1b2/src/pdm_conda/models/config.py` & `pdm_conda-0.8.1b3/src/pdm_conda/models/config.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.1b2/src/pdm_conda/models/environment.py` & `pdm_conda-0.8.1b3/src/pdm_conda/models/environment.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from pdm.exceptions import NoPythonVersion, ProjectError
 from pdm.models.environment import Environment, PrefixEnvironment
 from pdm.models.requirements import Requirement
 from pdm.models.working_set import WorkingSet
 from pdm.project import Project
 
-from pdm_conda.conda import conda_list, conda_search
+from pdm_conda.conda import conda_list, conda_search, logger
 from pdm_conda.mapping import pypi_to_conda
 from pdm_conda.models.candidates import CondaCandidate
 from pdm_conda.project import CondaProject
 from pdm_conda.utils import normalize_name
 
 _patched = False
 
@@ -35,16 +35,17 @@
 
     @property
     def packages_path(self) -> Path:
         return Path(ensure_conda_env())
 
     def get_paths(self) -> dict[str, str]:
         prefix = ensure_conda_env()
-        paths = sysconfig.get_paths(expand=True)
+        paths = sysconfig.get_paths(vars={k: prefix for k in ("base", "platbase", "installed_base")}, expand=True)
         paths.setdefault("prefix", prefix)
+        logger.debug(f"paths: {paths}")
         return paths
 
     def get_working_set(self) -> WorkingSet:
         """
         Get the working set based on local packages directory, include Conda managed packages.
         """
         working_set = super().get_working_set()
```

### Comparing `pdm_conda-0.8.1b2/src/pdm_conda/models/repositories.py` & `pdm_conda-0.8.1b3/src/pdm_conda/models/repositories.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.1b2/src/pdm_conda/models/requirements.py` & `pdm_conda-0.8.1b3/src/pdm_conda/models/requirements.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.1b2/src/pdm_conda/models/setup.py` & `pdm_conda-0.8.1b3/src/pdm_conda/models/setup.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.1b2/src/pdm_conda/project.py` & `pdm_conda-0.8.1b3/src/pdm_conda/project.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.1b2/src/pdm_conda/resolver/providers.py` & `pdm_conda-0.8.1b3/src/pdm_conda/resolver/providers.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.1b2/src/pdm_conda/resolvers.py` & `pdm_conda-0.8.1b3/src/pdm_conda/resolvers.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.1b2/src/pdm_conda/utils.py` & `pdm_conda-0.8.1b3/src/pdm_conda/utils.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.8.1b2/PKG-INFO` & `pdm_conda-0.8.1b3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdm-conda
-Version: 0.8.1b2
+Version: 0.8.1b3
 Summary:  A PDM plugin to install project dependencies with Conda
 Keywords: pdm plugin conda
 Author: Marcos Pastorini
 License: MIT License
         
         Copyright (c) 2022 macro128
         
@@ -27,15 +27,16 @@
         SOFTWARE.
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Project-URL: Homepage, https://github.com/macro128/pdm-conda
 Project-URL: Changelog, https://github.com/macro128/pdm-conda/blob/main/CHANGELOG.md
 Requires-Python: >=3.10
-Requires-Dist: pytest
+Requires-Dist: pdm~=2.4.0
+Requires-Dist: requests>=2.28.1
 Description-Content-Type: text/markdown
 
 # pdm-conda
 
 A PDM plugin to install project dependencies with Conda.
 
 ## Configuration
```

