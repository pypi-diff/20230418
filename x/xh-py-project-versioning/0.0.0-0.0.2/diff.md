# Comparing `tmp/xh-py-project-versioning-0.0.0.tar.gz` & `tmp/xh-py-project-versioning-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xh-py-project-versioning-0.0.0.tar", last modified: Tue Apr 18 04:31:49 2023, max compression
+gzip compressed data, was "xh-py-project-versioning-0.0.2.tar", last modified: Tue Apr 18 06:58:51 2023, max compression
```

## Comparing `xh-py-project-versioning-0.0.0.tar` & `xh-py-project-versioning-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 xeth      (1000) xeth      (1000)        0 2023-04-18 04:31:49.143928 xh-py-project-versioning-0.0.0/
--rw-r--r--   0 xeth      (1000) xeth      (1000)    35821 2023-04-17 04:08:40.000000 xh-py-project-versioning-0.0.0/LICENSE.txt
--rw-r--r--   0 xeth      (1000) xeth      (1000)      817 2023-04-18 04:31:49.143928 xh-py-project-versioning-0.0.0/PKG-INFO
--rw-r--r--   0 xeth      (1000) xeth      (1000)      258 2023-04-17 04:08:45.000000 xh-py-project-versioning-0.0.0/README.md
--rw-r--r--   0 xeth      (1000) xeth      (1000)      629 2023-04-18 02:36:19.000000 xh-py-project-versioning-0.0.0/pyproject.toml
--rw-r--r--   0 xeth      (1000) xeth      (1000)       38 2023-04-18 04:31:49.143928 xh-py-project-versioning-0.0.0/setup.cfg
-drwxr-xr-x   0 xeth      (1000) xeth      (1000)        0 2023-04-18 04:31:49.143928 xh-py-project-versioning-0.0.0/src/
-drwxr-xr-x   0 xeth      (1000) xeth      (1000)        0 2023-04-18 04:31:49.143928 xh-py-project-versioning-0.0.0/src/xh_py_project_versioning/
--rw-r--r--   0 xeth      (1000) xeth      (1000)      419 2023-04-18 04:27:49.000000 xh-py-project-versioning-0.0.0/src/xh_py_project_versioning/PyPiRepo.py
--rw-r--r--   0 xeth      (1000) xeth      (1000)      809 2023-04-18 04:29:35.000000 xh-py-project-versioning-0.0.0/src/xh_py_project_versioning/PyProject.py
--rw-r--r--   0 xeth      (1000) xeth      (1000)      168 2023-04-18 04:27:49.000000 xh-py-project-versioning-0.0.0/src/xh_py_project_versioning/__init__.py
--rw-r--r--   0 xeth      (1000) xeth      (1000)     2717 2023-04-18 04:30:04.000000 xh-py-project-versioning-0.0.0/src/xh_py_project_versioning/__main__.py
--rw-r--r--   0 xeth      (1000) xeth      (1000)     1899 2023-04-18 04:27:49.000000 xh-py-project-versioning-0.0.0/src/xh_py_project_versioning/versioning.py
-drwxr-xr-x   0 xeth      (1000) xeth      (1000)        0 2023-04-18 04:31:49.143928 xh-py-project-versioning-0.0.0/src/xh_py_project_versioning.egg-info/
--rw-r--r--   0 xeth      (1000) xeth      (1000)      817 2023-04-18 04:31:49.000000 xh-py-project-versioning-0.0.0/src/xh_py_project_versioning.egg-info/PKG-INFO
--rw-r--r--   0 xeth      (1000) xeth      (1000)      452 2023-04-18 04:31:49.000000 xh-py-project-versioning-0.0.0/src/xh_py_project_versioning.egg-info/SOURCES.txt
--rw-r--r--   0 xeth      (1000) xeth      (1000)        1 2023-04-18 04:31:49.000000 xh-py-project-versioning-0.0.0/src/xh_py_project_versioning.egg-info/dependency_links.txt
--rw-r--r--   0 xeth      (1000) xeth      (1000)       25 2023-04-18 04:31:49.000000 xh-py-project-versioning-0.0.0/src/xh_py_project_versioning.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:58:51.688875 xh-py-project-versioning-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35821 2023-04-18 06:58:40.000000 xh-py-project-versioning-0.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-18 06:58:51.688875 xh-py-project-versioning-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-18 06:58:40.000000 xh-py-project-versioning-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-18 06:58:40.000000 xh-py-project-versioning-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 06:58:51.688875 xh-py-project-versioning-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:58:51.684875 xh-py-project-versioning-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:58:51.688875 xh-py-project-versioning-0.0.2/src/xh_py_project_versioning/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-18 06:58:40.000000 xh-py-project-versioning-0.0.2/src/xh_py_project_versioning/PyPiRepo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-18 06:58:40.000000 xh-py-project-versioning-0.0.2/src/xh_py_project_versioning/PyProject.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-18 06:58:40.000000 xh-py-project-versioning-0.0.2/src/xh_py_project_versioning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-04-18 06:58:40.000000 xh-py-project-versioning-0.0.2/src/xh_py_project_versioning/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-18 06:58:40.000000 xh-py-project-versioning-0.0.2/src/xh_py_project_versioning/versioning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:58:51.688875 xh-py-project-versioning-0.0.2/src/xh_py_project_versioning.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-18 06:58:51.000000 xh-py-project-versioning-0.0.2/src/xh_py_project_versioning.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-18 06:58:51.000000 xh-py-project-versioning-0.0.2/src/xh_py_project_versioning.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 06:58:51.000000 xh-py-project-versioning-0.0.2/src/xh_py_project_versioning.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-18 06:58:51.000000 xh-py-project-versioning-0.0.2/src/xh_py_project_versioning.egg-info/top_level.txt
```

### Comparing `xh-py-project-versioning-0.0.0/LICENSE.txt` & `xh-py-project-versioning-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xh-py-project-versioning-0.0.0/PKG-INFO` & `xh-py-project-versioning-0.0.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xh-py-project-versioning
-Version: 0.0.0
+Version: 0.0.2
 Summary: A library for increate version number and check version mismatch
 Author-email: xethhung <pypi@xethh.dev>
 Project-URL: Homepage, https://github.com/xh-dev/xh-py-project-versioning
 Project-URL: Bug Tracker, https://github.com/xh-dev/xh-py-project-versioning
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -18,7 +18,12 @@
 ```shell
 rm -fr dist
 python -m build
 # automate by following `-u {user} -p {token / password}`
 # api automate by following `-u __token__ -p {token / password}`
 python -m twine upload dist/*
 ```
+
+
+```shell
+PYTHONPATH=src python src/xh_py_project_versioning/__main__.py --project-file pyproject.toml --major -d
+```
```

### Comparing `xh-py-project-versioning-0.0.0/pyproject.toml` & `xh-py-project-versioning-0.0.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 [build-system]
 requires = [ "setuptools>=61.0",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "xh-py-project-versioning"
-version = "0.0.0"
+version = "0.0.2"
 description = "A library for increate version number and check version mismatch"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [ "Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent",]
-
 [[project.authors]]
 name = "xethhung"
 email = "pypi@xethh.dev"
 
 [project.urls]
 Homepage = "https://github.com/xh-dev/xh-py-project-versioning"
 "Bug Tracker" = "https://github.com/xh-dev/xh-py-project-versioning"
```

### Comparing `xh-py-project-versioning-0.0.0/src/xh_py_project_versioning/PyProject.py` & `xh-py-project-versioning-0.0.2/src/xh_py_project_versioning/PyProject.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import toml
 
 from xh_py_project_versioning.versioning import SemVer
 
 
-class PyProject():
+class PyProject:
     def __init__(self, data: dict):
         self.data = data
 
     def get_dict(self):
         return self.data
 
     def get_project_name(self):
         return self.data["project"]["name"]
 
     def get_version(self):
         return self.data["project"]["version"]
 
     def update_version(self, sem_ver: SemVer) -> 'PyProject':
-        self['info'].update({"version": str(sem_ver)})
+        self.data['project'].update({"version": str(sem_ver)})
         return self
 
     @staticmethod
     def from_toml(project_path: str) -> 'PyProject':
         d = toml.load(project_path)
         return PyProject(d)
 
     def persist(self, project_path: str) -> 'PyProject':
         with open(project_path, "w") as f:
-            toml.dump(self, f)
+            toml.dump(self.data, f)
         return self
```

### Comparing `xh-py-project-versioning-0.0.0/src/xh_py_project_versioning/versioning.py` & `xh-py-project-versioning-0.0.2/src/xh_py_project_versioning/versioning.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,34 +19,38 @@
 
     def increase_patch(self):
         self.patch = self.patch+1
 
     def set_pre_release(self, pre_release: str):
         self.pre_release = pre_release
 
+    def unset_pre_release(self):
+        self.set_pre_release(None)
+
     def increase_build(self):
-        self.build = 0 if self.build is None else self.build
+        self.build = 1 if self.build is None else self.build+1
 
     def set_build(self, build: Optional[int]):
         self.build = build
 
-    def is_not_dev(self):
-        return not self.is_dev()
+    def unset_build(self):
+        self.build = None
+
+    def is_pre_release_not_set(self):
+        return not self.is_pre_release_set()
 
-    def is_dev(self):
+    def is_pre_release_set(self):
         if self.pre_release is None:
             return False
-        elif self.pre_release == "dev":
-            return True
         else:
-            return False
+            return True
 
     def __str__(self):
-        pre_release_str = f"-{self.pre_release}" if self.pre_release is None else ""
-        build_str = f"-{self.build}" if self.build is None else ""
+        pre_release_str = f"-{self.pre_release}" if self.pre_release is not None else ""
+        build_str = f"+{self.build:03d}" if self.build is not None else ""
         return f"{self.major}.{self.minor}.{self.patch}{pre_release_str}{build_str}"
 
     def __repr__(self):
         self.__str__()
 
     @staticmethod
     def from_str(sem_ver_string: str) -> 'SemVer':
```

### Comparing `xh-py-project-versioning-0.0.0/src/xh_py_project_versioning.egg-info/PKG-INFO` & `xh-py-project-versioning-0.0.2/src/xh_py_project_versioning.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xh-py-project-versioning
-Version: 0.0.0
+Version: 0.0.2
 Summary: A library for increate version number and check version mismatch
 Author-email: xethhung <pypi@xethh.dev>
 Project-URL: Homepage, https://github.com/xh-dev/xh-py-project-versioning
 Project-URL: Bug Tracker, https://github.com/xh-dev/xh-py-project-versioning
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -18,7 +18,12 @@
 ```shell
 rm -fr dist
 python -m build
 # automate by following `-u {user} -p {token / password}`
 # api automate by following `-u __token__ -p {token / password}`
 python -m twine upload dist/*
 ```
+
+
+```shell
+PYTHONPATH=src python src/xh_py_project_versioning/__main__.py --project-file pyproject.toml --major -d
+```
```

