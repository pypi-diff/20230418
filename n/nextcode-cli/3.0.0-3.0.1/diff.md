# Comparing `tmp/nextcode_cli-3.0.0.tar.gz` & `tmp/nextcode_cli-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nextcode_cli-3.0.0.tar", max compression
+gzip compressed data, was "nextcode_cli-3.0.1.tar", max compression
```

## Comparing `nextcode_cli-3.0.0.tar` & `nextcode_cli-3.0.1.tar`

### file list

```diff
@@ -1,46 +1,45 @@
--rw-r--r--   0        0        0     4544 2022-11-03 16:48:16.052640 nextcode_cli-3.0.0/README.md
--rw-r--r--   0        0        0       18 2022-11-03 16:48:16.056640 nextcode_cli-3.0.0/nextcodecli/VERSION
--rw-r--r--   0        0        0      423 2022-11-03 16:48:16.056640 nextcode_cli-3.0.0/nextcodecli/__init__.py
--rw-r--r--   0        0        0     3195 2022-11-03 16:48:16.056640 nextcode_cli-3.0.0/nextcodecli/__main__.py
--rw-r--r--   0        0        0       22 2022-11-03 16:48:16.056640 nextcode_cli-3.0.0/nextcodecli/commands/__init__.py
--rw-r--r--   0        0        0     5171 2022-11-03 16:48:16.056640 nextcode_cli-3.0.0/nextcodecli/commands/csa.py
--rw-r--r--   0        0        0     8709 2022-11-03 16:48:16.056640 nextcode_cli-3.0.0/nextcodecli/commands/keycloak.py
--rw-r--r--   0        0        0     2584 2022-11-03 16:48:16.056640 nextcode_cli-3.0.0/nextcodecli/commands/login.py
--rw-r--r--   0        0        0      755 2022-11-03 16:48:16.056640 nextcode_cli-3.0.0/nextcodecli/commands/pipelines/__init__.py
--rw-r--r--   0        0        0    18856 2022-11-03 16:48:16.056640 nextcode_cli-3.0.0/nextcodecli/commands/pipelines/instance.py
--rw-r--r--   0        0        0    21113 2022-11-03 16:48:16.056640 nextcode_cli-3.0.0/nextcodecli/commands/pipelines/job.py
--rw-r--r--   0        0        0     6491 2022-11-03 16:48:16.056640 nextcode_cli-3.0.0/nextcodecli/commands/pipelines/jobs.py
--rw-r--r--   0        0        0      901 2022-11-03 16:48:16.056640 nextcode_cli-3.0.0/nextcodecli/commands/pipelines/list.py
--rw-r--r--   0        0        0     4983 2022-11-03 16:48:16.056640 nextcode_cli-3.0.0/nextcodecli/commands/pipelines/run.py
--rw-r--r--   0        0        0     1169 2022-11-03 16:48:16.056640 nextcode_cli-3.0.0/nextcodecli/commands/pipelines/status.py
--rw-r--r--   0        0        0     5834 2022-11-03 16:48:16.056640 nextcode_cli-3.0.0/nextcodecli/commands/profile.py
--rw-r--r--   0        0        0     1324 2022-11-03 16:48:16.056640 nextcode_cli-3.0.0/nextcodecli/commands/project/__init__.py
--rw-r--r--   0        0        0     4272 2022-11-03 16:48:16.056640 nextcode_cli-3.0.0/nextcodecli/commands/project/fileaccess.py
--rw-r--r--   0        0        0     2914 2022-11-03 16:48:16.056640 nextcode_cli-3.0.0/nextcodecli/commands/project/status.py
--rw-r--r--   0        0        0     2238 2022-11-03 16:48:16.056640 nextcode_cli-3.0.0/nextcodecli/commands/project/users.py
--rw-r--r--   0        0        0     1926 2022-11-03 16:48:16.056640 nextcode_cli-3.0.0/nextcodecli/commands/query/__init__.py
--rw-r--r--   0        0        0    12181 2022-11-03 16:48:16.056640 nextcode_cli-3.0.0/nextcodecli/commands/query/run.py
--rw-r--r--   0        0        0     1135 2022-11-03 16:48:16.056640 nextcode_cli-3.0.0/nextcodecli/commands/query/status.py
--rw-r--r--   0        0        0     8361 2022-11-03 16:48:16.056640 nextcode_cli-3.0.0/nextcodecli/commands/query/templates.py
--rw-r--r--   0        0        0      472 2022-11-03 16:48:16.056640 nextcode_cli-3.0.0/nextcodecli/commands/setproject.py
--rw-r--r--   0        0        0     1134 2022-11-03 16:48:16.056640 nextcode_cli-3.0.0/nextcodecli/commands/token.py
--rw-r--r--   0        0        0      258 2022-11-03 16:48:16.056640 nextcode_cli-3.0.0/nextcodecli/commands/version.py
--rw-r--r--   0        0        0     1142 2022-11-03 16:48:16.056640 nextcode_cli-3.0.0/nextcodecli/commands/workflow/__init__.py
--rw-r--r--   0        0        0    27570 2022-11-03 16:48:16.056640 nextcode_cli-3.0.0/nextcodecli/commands/workflow/job.py
--rw-r--r--   0        0        0     4690 2022-11-03 16:48:16.056640 nextcode_cli-3.0.0/nextcodecli/commands/workflow/jobs.py
--rw-r--r--   0        0        0     3364 2022-11-03 16:48:16.056640 nextcode_cli-3.0.0/nextcodecli/commands/workflow/pipelines.py
--rw-r--r--   0        0        0      973 2022-11-03 16:48:16.056640 nextcode_cli-3.0.0/nextcodecli/commands/workflow/projects.py
--rw-r--r--   0        0        0     7468 2022-11-03 16:48:16.056640 nextcode_cli-3.0.0/nextcodecli/commands/workflow/run.py
--rw-r--r--   0        0        0     3658 2022-11-03 16:48:16.056640 nextcode_cli-3.0.0/nextcodecli/commands/workflow/status.py
--rwxr-xr-x   0        0        0     5244 2022-11-03 16:48:16.056640 nextcode_cli-3.0.0/nextcodecli/csa_import.py
--rw-r--r--   0        0        0        0 2022-11-03 16:48:16.084640 nextcode_cli-3.0.0/nextcodecli/pipelines/__init__.py
--rw-r--r--   0        0        0     2697 2022-11-03 16:48:16.056640 nextcode_cli-3.0.0/nextcodecli/pipelines/cmdutils.py
--rw-r--r--   0        0        0     6760 2022-11-03 16:48:16.060640 nextcode_cli-3.0.0/nextcodecli/pipelines/jobs.py
--rw-r--r--   0        0        0     3799 2022-11-03 16:48:16.060640 nextcode_cli-3.0.0/nextcodecli/pipelines/plot.py
--rw-r--r--   0        0        0     1892 2022-11-03 16:48:16.060640 nextcode_cli-3.0.0/nextcodecli/queryapi.py
--rw-r--r--   0        0        0     2565 2022-11-03 16:48:16.060640 nextcode_cli-3.0.0/nextcodecli/utils.py
--rw-r--r--   0        0        0        0 2022-11-03 16:48:16.084640 nextcode_cli-3.0.0/nextcodecli/workflow/__init__.py
--rw-r--r--   0        0        0     3498 2022-11-03 16:48:16.060640 nextcode_cli-3.0.0/nextcodecli/workflow/cmdutils.py
--rw-r--r--   0        0        0      807 2022-11-03 16:48:16.060640 nextcode_cli-3.0.0/pyproject.toml
--rw-r--r--   0        0        0     5897 1970-01-01 00:00:00.000000 nextcode_cli-3.0.0/setup.py
--rw-r--r--   0        0        0     5549 1970-01-01 00:00:00.000000 nextcode_cli-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0     4544 2023-04-18 16:40:05.085157 nextcode_cli-3.0.1/README.md
+-rw-r--r--   0        0        0       17 2023-04-18 16:40:05.089157 nextcode_cli-3.0.1/nextcodecli/VERSION
+-rw-r--r--   0        0        0      423 2023-04-18 16:40:05.089157 nextcode_cli-3.0.1/nextcodecli/__init__.py
+-rw-r--r--   0        0        0     3195 2023-04-18 16:40:05.089157 nextcode_cli-3.0.1/nextcodecli/__main__.py
+-rw-r--r--   0        0        0       22 2023-04-18 16:40:05.089157 nextcode_cli-3.0.1/nextcodecli/commands/__init__.py
+-rw-r--r--   0        0        0     5171 2023-04-18 16:40:05.089157 nextcode_cli-3.0.1/nextcodecli/commands/csa.py
+-rw-r--r--   0        0        0     8709 2023-04-18 16:40:05.089157 nextcode_cli-3.0.1/nextcodecli/commands/keycloak.py
+-rw-r--r--   0        0        0     2584 2023-04-18 16:40:05.089157 nextcode_cli-3.0.1/nextcodecli/commands/login.py
+-rw-r--r--   0        0        0      755 2023-04-18 16:40:05.089157 nextcode_cli-3.0.1/nextcodecli/commands/pipelines/__init__.py
+-rw-r--r--   0        0        0    18856 2023-04-18 16:40:05.089157 nextcode_cli-3.0.1/nextcodecli/commands/pipelines/instance.py
+-rw-r--r--   0        0        0    21113 2023-04-18 16:40:05.089157 nextcode_cli-3.0.1/nextcodecli/commands/pipelines/job.py
+-rw-r--r--   0        0        0     6491 2023-04-18 16:40:05.089157 nextcode_cli-3.0.1/nextcodecli/commands/pipelines/jobs.py
+-rw-r--r--   0        0        0      901 2023-04-18 16:40:05.089157 nextcode_cli-3.0.1/nextcodecli/commands/pipelines/list.py
+-rw-r--r--   0        0        0     4983 2023-04-18 16:40:05.089157 nextcode_cli-3.0.1/nextcodecli/commands/pipelines/run.py
+-rw-r--r--   0        0        0     1169 2023-04-18 16:40:05.089157 nextcode_cli-3.0.1/nextcodecli/commands/pipelines/status.py
+-rw-r--r--   0        0        0     5834 2023-04-18 16:40:05.089157 nextcode_cli-3.0.1/nextcodecli/commands/profile.py
+-rw-r--r--   0        0        0     1324 2023-04-18 16:40:05.089157 nextcode_cli-3.0.1/nextcodecli/commands/project/__init__.py
+-rw-r--r--   0        0        0     4272 2023-04-18 16:40:05.089157 nextcode_cli-3.0.1/nextcodecli/commands/project/fileaccess.py
+-rw-r--r--   0        0        0     2914 2023-04-18 16:40:05.093157 nextcode_cli-3.0.1/nextcodecli/commands/project/status.py
+-rw-r--r--   0        0        0     2238 2023-04-18 16:40:05.093157 nextcode_cli-3.0.1/nextcodecli/commands/project/users.py
+-rw-r--r--   0        0        0     1926 2023-04-18 16:40:05.093157 nextcode_cli-3.0.1/nextcodecli/commands/query/__init__.py
+-rw-r--r--   0        0        0    12181 2023-04-18 16:40:05.093157 nextcode_cli-3.0.1/nextcodecli/commands/query/run.py
+-rw-r--r--   0        0        0     1135 2023-04-18 16:40:05.093157 nextcode_cli-3.0.1/nextcodecli/commands/query/status.py
+-rw-r--r--   0        0        0     8361 2023-04-18 16:40:05.093157 nextcode_cli-3.0.1/nextcodecli/commands/query/templates.py
+-rw-r--r--   0        0        0      472 2023-04-18 16:40:05.093157 nextcode_cli-3.0.1/nextcodecli/commands/setproject.py
+-rw-r--r--   0        0        0     1134 2023-04-18 16:40:05.093157 nextcode_cli-3.0.1/nextcodecli/commands/token.py
+-rw-r--r--   0        0        0      258 2023-04-18 16:40:05.093157 nextcode_cli-3.0.1/nextcodecli/commands/version.py
+-rw-r--r--   0        0        0     1142 2023-04-18 16:40:05.093157 nextcode_cli-3.0.1/nextcodecli/commands/workflow/__init__.py
+-rw-r--r--   0        0        0    27570 2023-04-18 16:40:05.093157 nextcode_cli-3.0.1/nextcodecli/commands/workflow/job.py
+-rw-r--r--   0        0        0     4690 2023-04-18 16:40:05.093157 nextcode_cli-3.0.1/nextcodecli/commands/workflow/jobs.py
+-rw-r--r--   0        0        0     3364 2023-04-18 16:40:05.093157 nextcode_cli-3.0.1/nextcodecli/commands/workflow/pipelines.py
+-rw-r--r--   0        0        0      973 2023-04-18 16:40:05.093157 nextcode_cli-3.0.1/nextcodecli/commands/workflow/projects.py
+-rw-r--r--   0        0        0     7468 2023-04-18 16:40:05.093157 nextcode_cli-3.0.1/nextcodecli/commands/workflow/run.py
+-rw-r--r--   0        0        0     3658 2023-04-18 16:40:05.093157 nextcode_cli-3.0.1/nextcodecli/commands/workflow/status.py
+-rwxr-xr-x   0        0        0     5244 2023-04-18 16:40:05.093157 nextcode_cli-3.0.1/nextcodecli/csa_import.py
+-rw-r--r--   0        0        0        0 2023-04-18 16:40:05.165158 nextcode_cli-3.0.1/nextcodecli/pipelines/__init__.py
+-rw-r--r--   0        0        0     2697 2023-04-18 16:40:05.093157 nextcode_cli-3.0.1/nextcodecli/pipelines/cmdutils.py
+-rw-r--r--   0        0        0     6760 2023-04-18 16:40:05.093157 nextcode_cli-3.0.1/nextcodecli/pipelines/jobs.py
+-rw-r--r--   0        0        0     3799 2023-04-18 16:40:05.093157 nextcode_cli-3.0.1/nextcodecli/pipelines/plot.py
+-rw-r--r--   0        0        0     1892 2023-04-18 16:40:05.093157 nextcode_cli-3.0.1/nextcodecli/queryapi.py
+-rw-r--r--   0        0        0     2565 2023-04-18 16:40:05.093157 nextcode_cli-3.0.1/nextcodecli/utils.py
+-rw-r--r--   0        0        0        0 2023-04-18 16:40:05.169158 nextcode_cli-3.0.1/nextcodecli/workflow/__init__.py
+-rw-r--r--   0        0        0     3498 2023-04-18 16:40:05.093157 nextcode_cli-3.0.1/nextcodecli/workflow/cmdutils.py
+-rw-r--r--   0        0        0      807 2023-04-18 16:40:05.097157 nextcode_cli-3.0.1/pyproject.toml
+-rw-r--r--   0        0        0     5549 1970-01-01 00:00:00.000000 nextcode_cli-3.0.1/PKG-INFO
```

### Comparing `nextcode_cli-3.0.0/README.md` & `nextcode_cli-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.0/nextcodecli/__main__.py` & `nextcode_cli-3.0.1/nextcodecli/__main__.py`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.0/nextcodecli/commands/csa.py` & `nextcode_cli-3.0.1/nextcodecli/commands/csa.py`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.0/nextcodecli/commands/keycloak.py` & `nextcode_cli-3.0.1/nextcodecli/commands/keycloak.py`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.0/nextcodecli/commands/login.py` & `nextcode_cli-3.0.1/nextcodecli/commands/login.py`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.0/nextcodecli/commands/pipelines/__init__.py` & `nextcode_cli-3.0.1/nextcodecli/commands/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.0/nextcodecli/commands/pipelines/instance.py` & `nextcode_cli-3.0.1/nextcodecli/commands/pipelines/instance.py`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.0/nextcodecli/commands/pipelines/job.py` & `nextcode_cli-3.0.1/nextcodecli/commands/pipelines/job.py`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.0/nextcodecli/commands/pipelines/jobs.py` & `nextcode_cli-3.0.1/nextcodecli/commands/pipelines/jobs.py`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.0/nextcodecli/commands/pipelines/list.py` & `nextcode_cli-3.0.1/nextcodecli/commands/pipelines/list.py`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.0/nextcodecli/commands/pipelines/run.py` & `nextcode_cli-3.0.1/nextcodecli/commands/pipelines/run.py`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.0/nextcodecli/commands/pipelines/status.py` & `nextcode_cli-3.0.1/nextcodecli/commands/pipelines/status.py`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.0/nextcodecli/commands/profile.py` & `nextcode_cli-3.0.1/nextcodecli/commands/profile.py`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.0/nextcodecli/commands/project/__init__.py` & `nextcode_cli-3.0.1/nextcodecli/commands/project/__init__.py`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.0/nextcodecli/commands/project/fileaccess.py` & `nextcode_cli-3.0.1/nextcodecli/commands/project/fileaccess.py`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.0/nextcodecli/commands/project/status.py` & `nextcode_cli-3.0.1/nextcodecli/commands/project/status.py`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.0/nextcodecli/commands/project/users.py` & `nextcode_cli-3.0.1/nextcodecli/commands/project/users.py`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.0/nextcodecli/commands/query/__init__.py` & `nextcode_cli-3.0.1/nextcodecli/commands/query/__init__.py`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.0/nextcodecli/commands/query/run.py` & `nextcode_cli-3.0.1/nextcodecli/commands/query/run.py`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.0/nextcodecli/commands/query/status.py` & `nextcode_cli-3.0.1/nextcodecli/commands/query/status.py`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.0/nextcodecli/commands/query/templates.py` & `nextcode_cli-3.0.1/nextcodecli/commands/query/templates.py`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.0/nextcodecli/commands/token.py` & `nextcode_cli-3.0.1/nextcodecli/commands/token.py`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.0/nextcodecli/commands/workflow/__init__.py` & `nextcode_cli-3.0.1/nextcodecli/commands/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.0/nextcodecli/commands/workflow/job.py` & `nextcode_cli-3.0.1/nextcodecli/commands/workflow/job.py`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.0/nextcodecli/commands/workflow/jobs.py` & `nextcode_cli-3.0.1/nextcodecli/commands/workflow/jobs.py`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.0/nextcodecli/commands/workflow/pipelines.py` & `nextcode_cli-3.0.1/nextcodecli/commands/workflow/pipelines.py`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.0/nextcodecli/commands/workflow/projects.py` & `nextcode_cli-3.0.1/nextcodecli/commands/workflow/projects.py`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.0/nextcodecli/commands/workflow/run.py` & `nextcode_cli-3.0.1/nextcodecli/commands/workflow/run.py`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.0/nextcodecli/commands/workflow/status.py` & `nextcode_cli-3.0.1/nextcodecli/commands/workflow/status.py`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.0/nextcodecli/csa_import.py` & `nextcode_cli-3.0.1/nextcodecli/csa_import.py`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.0/nextcodecli/pipelines/cmdutils.py` & `nextcode_cli-3.0.1/nextcodecli/pipelines/cmdutils.py`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.0/nextcodecli/pipelines/jobs.py` & `nextcode_cli-3.0.1/nextcodecli/pipelines/jobs.py`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.0/nextcodecli/pipelines/plot.py` & `nextcode_cli-3.0.1/nextcodecli/pipelines/plot.py`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.0/nextcodecli/queryapi.py` & `nextcode_cli-3.0.1/nextcodecli/queryapi.py`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.0/nextcodecli/utils.py` & `nextcode_cli-3.0.1/nextcodecli/utils.py`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.0/nextcodecli/workflow/cmdutils.py` & `nextcode_cli-3.0.1/nextcodecli/workflow/cmdutils.py`

 * *Files identical despite different names*

### Comparing `nextcode_cli-3.0.0/pyproject.toml` & `nextcode_cli-3.0.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nextcode-cli"
-version = "3.0.0"
+version = "3.0.1"
 description = "WuXi Nextcode commandline utilities"
 license = "MIT"
 authors = ["WUXI NextCODE <support@wuxinextcode.com>"]
 maintainers = ["Genuity Science Software Development <sdev@genuitysci.com>"]
 readme = "README.md"
 homepage = "https://www.wuxinextcode.com"
 packages = [{include = "nextcodecli"}]
@@ -13,21 +13,21 @@
 nextcode = 'nextcodecli.__main__:cli'
 
 [tool.poetry.dependencies]
 python = "^3.8"
 click = "^8.1.3"
 python-dateutil = "^2.8.2"
 pyyaml = "^6.0"
-requests = "^2.28.1"
+requests = "^2.28.2"
 tabulate = "^0.9.0"
 hjson = "^3.1.0"
 jsonpath-rw = "^1.4.0"
-nextcode-sdk = "^2.0.0"
+nextcode-sdk = "^2.1.0"
 
 [tool.poetry.group.test.dependencies]
 pytest-cov = "^4.0.0"
-pytest = "^7.2.0"
+pytest = "^7.2.2"
 vulture = "^2.6"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nextcode_cli-3.0.0/setup.py` & `nextcode_cli-3.0.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,48 +1,156 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: nextcode-cli
+Version: 3.0.1
+Summary: WuXi Nextcode commandline utilities
+Home-page: https://www.wuxinextcode.com
+License: MIT
+Author: WUXI NextCODE
+Author-email: support@wuxinextcode.com
+Maintainer: Genuity Science Software Development
+Maintainer-email: sdev@genuitysci.com
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: hjson (>=3.1.0,<4.0.0)
+Requires-Dist: jsonpath-rw (>=1.4.0,<2.0.0)
+Requires-Dist: nextcode-sdk (>=2.1.0,<3.0.0)
+Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
+Requires-Dist: pyyaml (>=6.0,<7.0)
+Requires-Dist: requests (>=2.28.2,<3.0.0)
+Requires-Dist: tabulate (>=0.9.0,<0.10.0)
+Description-Content-Type: text/markdown
+
+# NextCODE Command Line Interface
+
+- [Requirements](#requirements)
+- [Installation](#installation)
+  * [End-user installation](#end-user-installation)
+  * [Developer installation](#developer-installation)
+  * [Set up a service profile](#set-up-a-service-profile)
+    + [Create a service profile](#create-a-service-profile)
+    + [Running the CLI for the first time](#running-the-cli-for-the-first-time)
+- [Releasing](#releasing)
+
+# Requirements
+ * Python 3.7
+
+# Installation
+
+## End-user installation
+
+**Prerequisites**
+Note that having `python3` (and a `pip3` that points to that python) is a prerequisite, the easist way to fullfil this is to install both via Homebrew.
+
+To install the package you have to run the following command:
+```bash
+$ pip3 install nextcode-cli -U
+```
+
+To verify that the installation was successful you can run the following command:
+```bash
+$ nextcode version
+nextcode-cli/x.y.z (yyyy.mm.dd)
+```
+
+## Developer installation
+Start by pulling the sourcecode from git (usually from develop to be on the bleeding edge).
+
+There are two ways to set up the CLI. We recommend trying to install it into your system python in `develop` mode by simply running the following command in the nextcode-cli folder (depending on your system setup you might need `sudo`)
+```bash
+$ pip3 install -e .
+```
+
+If you get any errors you can set up a local virtualenv in the nextcode-cli path:
+```bash
+$ source ./setup.sh
+$ pip3 install -e .
+```
+Using this method means that you will always need to do `source ./setup.sh` to enter the virtualenv before using the tool, so we would recommend getting the first method to work unless you intend on make edits to the code yourself.
+
+## Set up a service profile
+### Create a service profile
+For any work to happen a service profile must be defined. One example is the one here below, which is Platform Dev test specific. For QA purposes this is of course **test environment dependent**!:
+
+The command is:
+```bash
+$ nextcode profile add <profile-name>
+```
+
+Follow the prompts to enter a server name and then log in through the browser window that opens up.
+
+You can also set up the profile without a prompt like this:
+```bash
+$ nextcode profile add <profile-name> --domain=mydomain.wuxinextcode.com --api-key=<key>
+```
+
+### Running the CLI for the first time
+
+Once your installation has succeeded you can run the following command anywhere in your system:
+```bash
+nextcode status
+```
+Once you finish the authentication process you should be able to view workflow jobs:
+```bash
+nextcode workflow jobs
+```
+
+To start familiarizing yourself with the sdk you can use the --help option on all commands to see detailed information about their use.
+```bash
+$ nextcode --help
+Usage: nextcode [OPTIONS] COMMAND [ARGS]...
+
+  A utility for interfacing with WuXi Nextcode services.
+
+  This tool allows you to communicate with the pipelines service, CSA,
+  workflow service and GOR Query API. For all usage you will need to
+  authenticate against the specific service profile you are using.
+
+  Please look at the subcommands below for details.
+
+Options:
+  -v, --verbose [warning|error|info]
+                                  Output logs for debugging
+  -p, --profile TEXT              Use a specific profile for this command
+  --help                          Show this message and exit.
+
+Commands:
+  csa_authenticate  Authenticate against CSA (for import).
+  import            Import a TSV manifest into CSA.
+  keycloak          Manage keycloak users Requires the keycloak admin...
+  login             Authenticate against keycloak.
+  pipelines         Root subcommand for pipelines functionality
+  profile           Configure server profile to use.
+  query             Root subcommand for query api functionality
+  token             Print out an access token for the current profile
+  version           Show the Nextcode CLI version.
+  workflow          Root subcommand for workflow functionality
+
+$ nextcode workflow --help
+Usage: nextcode workflow [OPTIONS] COMMAND [ARGS]...
+
+  Root subcommand for workflow functionality
+
+Options:
+  --help  Show this message and exit.
+
+Commands:
+  job        View or manage individual jobs.
+  jobs       List jobs
+  pipelines  List pipelines
+  projects   List projects
+  run        Start a new nextflow job.
+  smoketest  Run a smoketest of the workflow service
+  status     Show the status of the workflow service
+```
+
+# Releasing
+* Bump version and update the a date in [nextcodecli/VERSION](nextcodecli/VERSION)
+* Merge to master
+* Tag in Gitlab
+* Watch the CI fireworks. 
 
-packages = \
-['nextcodecli',
- 'nextcodecli.commands',
- 'nextcodecli.commands.pipelines',
- 'nextcodecli.commands.project',
- 'nextcodecli.commands.query',
- 'nextcodecli.commands.workflow',
- 'nextcodecli.pipelines',
- 'nextcodecli.workflow']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['click>=8.1.3,<9.0.0',
- 'hjson>=3.1.0,<4.0.0',
- 'jsonpath-rw>=1.4.0,<2.0.0',
- 'nextcode-sdk>=2.0.0,<3.0.0',
- 'python-dateutil>=2.8.2,<3.0.0',
- 'pyyaml>=6.0,<7.0',
- 'requests>=2.28.1,<3.0.0',
- 'tabulate>=0.9.0,<0.10.0']
-
-entry_points = \
-{'console_scripts': ['nextcode = nextcodecli.__main__:cli']}
-
-setup_kwargs = {
-    'name': 'nextcode-cli',
-    'version': '3.0.0',
-    'description': 'WuXi Nextcode commandline utilities',
-    'long_description': '# NextCODE Command Line Interface\n\n- [Requirements](#requirements)\n- [Installation](#installation)\n  * [End-user installation](#end-user-installation)\n  * [Developer installation](#developer-installation)\n  * [Set up a service profile](#set-up-a-service-profile)\n    + [Create a service profile](#create-a-service-profile)\n    + [Running the CLI for the first time](#running-the-cli-for-the-first-time)\n- [Releasing](#releasing)\n\n# Requirements\n * Python 3.7\n\n# Installation\n\n## End-user installation\n\n**Prerequisites**\nNote that having `python3` (and a `pip3` that points to that python) is a prerequisite, the easist way to fullfil this is to install both via Homebrew.\n\nTo install the package you have to run the following command:\n```bash\n$ pip3 install nextcode-cli -U\n```\n\nTo verify that the installation was successful you can run the following command:\n```bash\n$ nextcode version\nnextcode-cli/x.y.z (yyyy.mm.dd)\n```\n\n## Developer installation\nStart by pulling the sourcecode from git (usually from develop to be on the bleeding edge).\n\nThere are two ways to set up the CLI. We recommend trying to install it into your system python in `develop` mode by simply running the following command in the nextcode-cli folder (depending on your system setup you might need `sudo`)\n```bash\n$ pip3 install -e .\n```\n\nIf you get any errors you can set up a local virtualenv in the nextcode-cli path:\n```bash\n$ source ./setup.sh\n$ pip3 install -e .\n```\nUsing this method means that you will always need to do `source ./setup.sh` to enter the virtualenv before using the tool, so we would recommend getting the first method to work unless you intend on make edits to the code yourself.\n\n## Set up a service profile\n### Create a service profile\nFor any work to happen a service profile must be defined. One example is the one here below, which is Platform Dev test specific. For QA purposes this is of course **test environment dependent**!:\n\nThe command is:\n```bash\n$ nextcode profile add <profile-name>\n```\n\nFollow the prompts to enter a server name and then log in through the browser window that opens up.\n\nYou can also set up the profile without a prompt like this:\n```bash\n$ nextcode profile add <profile-name> --domain=mydomain.wuxinextcode.com --api-key=<key>\n```\n\n### Running the CLI for the first time\n\nOnce your installation has succeeded you can run the following command anywhere in your system:\n```bash\nnextcode status\n```\nOnce you finish the authentication process you should be able to view workflow jobs:\n```bash\nnextcode workflow jobs\n```\n\nTo start familiarizing yourself with the sdk you can use the --help option on all commands to see detailed information about their use.\n```bash\n$ nextcode --help\nUsage: nextcode [OPTIONS] COMMAND [ARGS]...\n\n  A utility for interfacing with WuXi Nextcode services.\n\n  This tool allows you to communicate with the pipelines service, CSA,\n  workflow service and GOR Query API. For all usage you will need to\n  authenticate against the specific service profile you are using.\n\n  Please look at the subcommands below for details.\n\nOptions:\n  -v, --verbose [warning|error|info]\n                                  Output logs for debugging\n  -p, --profile TEXT              Use a specific profile for this command\n  --help                          Show this message and exit.\n\nCommands:\n  csa_authenticate  Authenticate against CSA (for import).\n  import            Import a TSV manifest into CSA.\n  keycloak          Manage keycloak users Requires the keycloak admin...\n  login             Authenticate against keycloak.\n  pipelines         Root subcommand for pipelines functionality\n  profile           Configure server profile to use.\n  query             Root subcommand for query api functionality\n  token             Print out an access token for the current profile\n  version           Show the Nextcode CLI version.\n  workflow          Root subcommand for workflow functionality\n\n$ nextcode workflow --help\nUsage: nextcode workflow [OPTIONS] COMMAND [ARGS]...\n\n  Root subcommand for workflow functionality\n\nOptions:\n  --help  Show this message and exit.\n\nCommands:\n  job        View or manage individual jobs.\n  jobs       List jobs\n  pipelines  List pipelines\n  projects   List projects\n  run        Start a new nextflow job.\n  smoketest  Run a smoketest of the workflow service\n  status     Show the status of the workflow service\n```\n\n# Releasing\n* Bump version and update the a date in [nextcodecli/VERSION](nextcodecli/VERSION)\n* Merge to master\n* Tag in Gitlab\n* Watch the CI fireworks. \n',
-    'author': 'WUXI NextCODE',
-    'author_email': 'support@wuxinextcode.com',
-    'maintainer': 'Genuity Science Software Development',
-    'maintainer_email': 'sdev@genuitysci.com',
-    'url': 'https://www.wuxinextcode.com',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

