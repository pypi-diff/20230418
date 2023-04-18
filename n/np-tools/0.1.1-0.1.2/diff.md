# Comparing `tmp/np_tools-0.1.1.tar.gz` & `tmp/np_tools-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "np_tools-0.1.1.tar", last modified: Tue Apr 18 02:01:10 2023, max compression
+gzip compressed data, was "np_tools-0.1.2.tar", last modified: Tue Apr 18 21:31:18 2023, max compression
```

## Comparing `np_tools-0.1.1.tar` & `np_tools-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      273 2023-04-13 18:32:03.410128 np_tools-0.1.1/README.md
--rw-r--r--   0        0        0     2273 2023-04-18 02:01:10.205599 np_tools-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      279 2023-04-13 18:53:01.173171 np_tools-0.1.1/src/np_tools/__init__.py
--rw-r--r--   0        0        0      268 2023-04-13 18:53:25.697520 np_tools-0.1.1/src/np_tools/config.py
--rw-r--r--   0        0        0     4352 2023-04-18 01:59:18.463852 np_tools-0.1.1/src/np_tools/remote.py
--rw-r--r--   0        0        0     1683 1970-01-01 00:00:00.000000 np_tools-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      273 2023-04-13 18:32:03.410128 np_tools-0.1.2/README.md
+-rw-r--r--   0        0        0     2344 2023-04-18 21:31:18.505373 np_tools-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      238 2023-04-18 21:29:53.450239 np_tools-0.1.2/src/np_tools/__init__.py
+-rw-r--r--   0        0        0      268 2023-04-13 18:53:25.697520 np_tools-0.1.2/src/np_tools/config.py
+-rw-r--r--   0        0        0     4195 2023-04-18 21:29:53.558658 np_tools-0.1.2/src/np_tools/remote.py
+-rw-r--r--   0        0        0     1683 1970-01-01 00:00:00.000000 np_tools-0.1.2/PKG-INFO
```

### Comparing `np_tools-0.1.1/pyproject.toml` & `np_tools-0.1.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -27,14 +27,20 @@
 [tool.pdm.scripts.publish]
 composite = [
     "prebuild",
     "pdm build",
     "pdm publish --no-build",
 ]
 
+[tool.pdm.scripts.pub]
+composite = [
+    "bump",
+    "pdm publish",
+]
+
 [tool.ruff]
 ignore-init-module-imports = true
 
 [tool.pytest.ini_options]
 addopts = [
     "--import-mode=importlib",
     "--doctest-modules",
@@ -61,15 +67,15 @@
 ]
 
 [tool.coverage.report]
 show_missing = true
 
 [project]
 name = "np_tools"
-version = "0.1.1"
+version = "0.1.2"
 description = "General-purpose tools for common tasks encountered in Mindscope Neuropixels workflows."
 authors = [
     { name = "bjhardcastle", email = "ben.hardcastle@alleninstitute.org" },
 ]
 dependencies = [
     "fabric>=3.0.0",
     "np-config>=0.4.17",
```

### Comparing `np_tools-0.1.1/src/np_tools/remote.py` & `np_tools-0.1.2/src/np_tools/remote.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,22 +33,16 @@
     return fabric.Connection(
         host=host,
         user=HPC_CREDENTIALS['user'],
         connect_kwargs=dict(password=HPC_CREDENTIALS['password']),
     )
 
 
-def hpc() -> fabric.Connection:
-    """Fabric connection to `hpc-login` using `svc_neuropix` creds.
-
-    >>> with hpc() as connection:
-    ...     response = connection.run('echo "hello world"', hide=True)
-
-    """
-    return ssh('hpc-login')
+hpc = ssh('hpc-login')
+"""Fabric connection to `hpc-login` using `svc_neuropix` creds."""
 
 
 def run_cmd_on_host(
     host: str,
     cmd: str,
     *,
     hide_output: bool = True,  # suppresses stdout
@@ -59,15 +53,15 @@
     If `host` is 'localhost', run `cmd` locally in a subprocess.
 
     >>> print(run_cmd_on_host('w10svad0139', 'hostname').stdout.strip())
     W10SVAD0139
     >>> run_cmd_on_host('localhost', 'echo hello world').stdout.strip()
     b'hello world'
     >>> _ = run_cmd_on_host('localhost', 'echo hello world', hide_output=False)
-    
+
     # prints 'hello world'
     """
     if host == 'localhost':
         logger.debug('Running command on localhost: %r', cmd)
         result = subprocess.run(
             cmd,
             shell=True,
```

### Comparing `np_tools-0.1.1/PKG-INFO` & `np_tools-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: np-tools
-Version: 0.1.1
+Version: 0.1.2
 Summary: General-purpose tools for common tasks encountered in Mindscope Neuropixels workflows.
 Author-Email: bjhardcastle <ben.hardcastle@alleninstitute.org>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

