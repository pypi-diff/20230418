# Comparing `tmp/DLite-Python-0.3.8.tar.gz` & `tmp/DLite-Python-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DLite-Python-0.3.8.tar", last modified: Mon Mar 21 19:55:16 2022, max compression
+gzip compressed data, was "DLite-Python-0.3.9.tar", last modified: Wed Apr 27 08:44:43 2022, max compression
```

## Comparing `DLite-Python-0.3.8.tar` & `DLite-Python-0.3.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 19:55:16.888626 DLite-Python-0.3.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 19:55:16.888626 DLite-Python-0.3.8/DLite_Python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    19607 2022-03-21 19:55:16.000000 DLite-Python-0.3.8/DLite_Python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    18916 2022-03-21 19:55:16.000000 DLite-Python-0.3.8/DLite_Python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-21 19:55:16.000000 DLite-Python-0.3.8/DLite_Python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-21 19:55:14.000000 DLite-Python-0.3.8/DLite_Python.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-03-21 19:55:16.000000 DLite-Python-0.3.8/DLite_Python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-03-21 19:55:16.000000 DLite-Python-0.3.8/DLite_Python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       93 2022-03-21 19:55:00.000000 DLite-Python-0.3.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    19607 2022-03-21 19:55:16.888626 DLite-Python-0.3.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-21 19:55:16.888626 DLite-Python-0.3.8/dlite/
--rw-r--r--   0 runner    (1001) docker     (121)      264 2022-03-21 19:55:00.000000 DLite-Python-0.3.8/dlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1946 2022-03-21 19:55:00.000000 DLite-Python-0.3.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-21 19:55:16.888626 DLite-Python-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     7017 2022-03-21 19:55:00.000000 DLite-Python-0.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-27 08:44:43.795873 DLite-Python-0.3.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-27 08:44:43.795873 DLite-Python-0.3.9/DLite_Python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    19607 2022-04-27 08:44:43.000000 DLite-Python-0.3.9/DLite_Python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    18994 2022-04-27 08:44:43.000000 DLite-Python-0.3.9/DLite_Python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-27 08:44:43.000000 DLite-Python-0.3.9/DLite_Python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-27 08:44:41.000000 DLite-Python-0.3.9/DLite_Python.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       68 2022-04-27 08:44:43.000000 DLite-Python-0.3.9/DLite_Python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2022-04-27 08:44:43.000000 DLite-Python-0.3.9/DLite_Python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       93 2022-04-27 08:44:31.000000 DLite-Python-0.3.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)    19607 2022-04-27 08:44:43.795873 DLite-Python-0.3.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-27 08:44:43.795873 DLite-Python-0.3.9/dlite/
+-rw-r--r--   0 runner    (1001) docker     (121)      264 2022-04-27 08:44:31.000000 DLite-Python-0.3.9/dlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1800 2022-04-27 08:44:31.000000 DLite-Python-0.3.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-27 08:44:43.795873 DLite-Python-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     7017 2022-04-27 08:44:31.000000 DLite-Python-0.3.9/setup.py
```

### Comparing `DLite-Python-0.3.8/DLite_Python.egg-info/PKG-INFO` & `DLite-Python-0.3.9/DLite_Python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DLite-Python
-Version: 0.3.8
+Version: 0.3.9
 Summary: Lightweight data-centric framework for working with scientific data
 Home-page: https://github.com/SINTEF/dlite
 Author: SINTEF
 Author-email: jesper.friis@sintef.no
 License: MIT
 Platform: Windows
 Platform: Linux
```

### Comparing `DLite-Python-0.3.8/DLite_Python.egg-info/SOURCES.txt` & `DLite-Python-0.3.9/DLite_Python.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -31,21 +31,23 @@
 .././.git/hooks/pre-rebase.sample
 .././.git/hooks/pre-receive.sample
 .././.git/hooks/prepare-commit-msg.sample
 .././.git/hooks/push-to-checkout.sample
 .././.git/hooks/update.sample
 .././.git/info/exclude
 .././.git/logs/HEAD
-.././.git/objects/pack/pack-5e6e6cbb862dd4370d0b7581a60f179d09f254be.idx
-.././.git/objects/pack/pack-5e6e6cbb862dd4370d0b7581a60f179d09f254be.pack
-.././.git/refs/tags/v0.3.8
+.././.git/objects/pack/pack-e8f5277c9d0e1bf19900e4db409ae71d8d14c7d2.idx
+.././.git/objects/pack/pack-e8f5277c9d0e1bf19900e4db409ae71d8d14c7d2.pack
+.././.git/refs/tags/v0.3.9
 .././.github/.gitignore
 .././.github/docker/Dockerfile-manylinux.template
 .././.github/docker/Dockerfile-mingw
 .././.github/docker/Dockerfile-musllinux.template
+.././.github/docker/pgdg-91_i686.repo
+.././.github/docker/pgdg-91_x86_64.repo
 .././.github/docker/run_cibuildwheel.sh
 .././.github/utils/release_tag_msg.txt
 .././.github/workflows/cd_release.yml
 .././.github/workflows/ci_build_wheels.yml
 .././.github/workflows/ci_tests.yml
 .././.github/workflows/container_builds_weekly.yml
 .././.github/workflows/dockerimage.yml
```

### Comparing `DLite-Python-0.3.8/PKG-INFO` & `DLite-Python-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DLite-Python
-Version: 0.3.8
+Version: 0.3.9
 Summary: Lightweight data-centric framework for working with scientific data
 Home-page: https://github.com/SINTEF/dlite
 Author: SINTEF
 Author-email: jesper.friis@sintef.no
 License: MIT
 Platform: Windows
 Platform: Linux
```

### Comparing `DLite-Python-0.3.8/pyproject.toml` & `DLite-Python-0.3.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 [tool.cibuildwheel.linux]
 environment-pass = ["CI_BUILD_CMAKE_ARGS", "CI_PIP_CACHE_DIR"]
 before-build = [
   "rm -rf {project}/python/build/temp*",
   "export PYVER=$(python -c \"import sys; print(f'{sys.version_info.major}.{sys.version_info.minor}')\")",
   "export ABITAG=$(python -c \"import sys; cp=f'cp{sys.version_info.major}{sys.version_info.minor}'; print(f'{cp}-{cp}{sys.abiflags}')\")",
 ]
-before-test = "if [ -n \"${CI_PIP_CACHE_DIR}\" ]; then mkdir -p /host${CI_PIP_CACHE_DIR} && chown -R root /host${CI_PIP_CACHE_DIR} && python -m pip install --cache-dir /host${CI_PIP_CACHE_DIR} -U --upgrade-strategy=eager -r {project}/requirements.txt; fi"
+before-test = "python -m pip install --cache-dir /ci/pip_cache --prefer-binary -r {project}/requirements.txt"
 test-command = "python {package}/../bindings/python/tests/test_python_bindings.py"
 
 [tool.cibuildwheel.linux.environment]
 PYVER = "$(python -c \"import sys; print(f'{sys.version_info.major}.{sys.version_info.minor}')\")"
 PYABI = "$(python -c \"import sys; print(sys.abiflags)\")"
 ABITAG = "$(python -c \"import sys; cp=f'cp{sys.version_info.major}{sys.version_info.minor}'; print(f'{cp}-{cp}{sys.abiflags}')\")"
```

### Comparing `DLite-Python-0.3.8/setup.py` & `DLite-Python-0.3.9/setup.py`

 * *Files identical despite different names*

