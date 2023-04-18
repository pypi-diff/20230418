# Comparing `tmp/eons-2.3.6.tar.gz` & `tmp/eons-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eons-2.3.6.tar", last modified: Tue Apr 18 14:54:08 2023, max compression
+gzip compressed data, was "eons-2.4.0.tar", last modified: Tue Apr 18 14:58:37 2023, max compression
```

## Comparing `eons-2.3.6.tar` & `eons-2.4.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:54:08.061581 eons-2.3.6/
--rw-r--r--   0 runner    (1001) docker     (123)    16886 2023-04-18 14:54:08.061581 eons-2.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16599 2023-04-18 14:53:49.000000 eons-2.3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:54:08.057581 eons-2.3.6/pkg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:54:08.057581 eons-2.3.6/pkg/eons/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-18 14:53:58.000000 eons-2.3.6/pkg/eons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    82395 2023-04-18 14:53:58.000000 eons-2.3.6/pkg/eons/eons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:54:08.057581 eons-2.3.6/pkg/eons/method/
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-18 14:53:24.000000 eons-2.3.6/pkg/eons/method/External.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 14:53:58.000000 eons-2.3.6/pkg/eons/method/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:54:08.061581 eons-2.3.6/pkg/eons/resolve/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 14:53:58.000000 eons-2.3.6/pkg/eons/resolve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-04-18 14:53:24.000000 eons-2.3.6/pkg/eons/resolve/resolve_find_by_fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-18 14:53:24.000000 eons-2.3.6/pkg/eons/resolve/resolve_import_module.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-18 14:53:24.000000 eons-2.3.6/pkg/eons/resolve/resolve_install_from_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-18 14:53:24.000000 eons-2.3.6/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-18 14:53:24.000000 eons-2.3.6/pkg/eons/resolve/resolve_install_with_pip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:54:08.057581 eons-2.3.6/pkg/eons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16886 2023-04-18 14:54:08.000000 eons-2.3.6/pkg/eons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-18 14:54:08.000000 eons-2.3.6/pkg/eons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 14:54:08.000000 eons-2.3.6/pkg/eons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-18 14:54:08.000000 eons-2.3.6/pkg/eons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-18 14:54:08.000000 eons-2.3.6/pkg/eons.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-18 14:53:58.000000 eons-2.3.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-18 14:54:08.061581 eons-2.3.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:58:37.088723 eons-2.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16886 2023-04-18 14:58:37.088723 eons-2.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16599 2023-04-18 14:58:20.000000 eons-2.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:58:37.084723 eons-2.4.0/pkg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:58:37.084723 eons-2.4.0/pkg/eons/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-18 14:58:28.000000 eons-2.4.0/pkg/eons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82395 2023-04-18 14:58:28.000000 eons-2.4.0/pkg/eons/eons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:58:37.084723 eons-2.4.0/pkg/eons/method/
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-18 14:58:09.000000 eons-2.4.0/pkg/eons/method/External.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 14:58:28.000000 eons-2.4.0/pkg/eons/method/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:58:37.088723 eons-2.4.0/pkg/eons/resolve/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 14:58:28.000000 eons-2.4.0/pkg/eons/resolve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-04-18 14:58:09.000000 eons-2.4.0/pkg/eons/resolve/resolve_find_by_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-18 14:58:09.000000 eons-2.4.0/pkg/eons/resolve/resolve_import_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-18 14:58:09.000000 eons-2.4.0/pkg/eons/resolve/resolve_install_from_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-18 14:58:09.000000 eons-2.4.0/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-18 14:58:09.000000 eons-2.4.0/pkg/eons/resolve/resolve_install_with_pip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:58:37.084723 eons-2.4.0/pkg/eons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16886 2023-04-18 14:58:37.000000 eons-2.4.0/pkg/eons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-18 14:58:37.000000 eons-2.4.0/pkg/eons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 14:58:37.000000 eons-2.4.0/pkg/eons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-18 14:58:37.000000 eons-2.4.0/pkg/eons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-18 14:58:37.000000 eons-2.4.0/pkg/eons.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-18 14:58:28.000000 eons-2.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-18 14:58:37.088723 eons-2.4.0/setup.cfg
```

### Comparing `eons-2.3.6/PKG-INFO` & `eons-2.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eons
-Version: 2.3.6
+Version: 2.4.0
 Summary: Eons Python Framework
 Home-page: https://github.com/eons-dev/eons.lib
 Author: Eons
 Author-email: support@eons.llc
 Project-URL: Bug Tracker, https://github.com/eons-dev/eons.lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eons-2.3.6/README.md` & `eons-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `eons-2.3.6/pkg/eons/eons.py` & `eons-2.4.0/pkg/eons/eons.py`

 * *Files identical despite different names*

### Comparing `eons-2.3.6/pkg/eons/method/External.py` & `eons-2.4.0/pkg/eons/method/External.py`

 * *Files identical despite different names*

### Comparing `eons-2.3.6/pkg/eons/resolve/resolve_find_by_fetch.py` & `eons-2.4.0/pkg/eons/resolve/resolve_find_by_fetch.py`

 * *Files identical despite different names*

### Comparing `eons-2.3.6/pkg/eons/resolve/resolve_import_module.py` & `eons-2.4.0/pkg/eons/resolve/resolve_import_module.py`

 * *Files identical despite different names*

### Comparing `eons-2.3.6/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py` & `eons-2.4.0/pkg/eons/resolve/resolve_install_from_repo_with_default_package_type.py`

 * *Files identical despite different names*

### Comparing `eons-2.3.6/pkg/eons.egg-info/PKG-INFO` & `eons-2.4.0/pkg/eons.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eons
-Version: 2.3.6
+Version: 2.4.0
 Summary: Eons Python Framework
 Home-page: https://github.com/eons-dev/eons.lib
 Author: Eons
 Author-email: support@eons.llc
 Project-URL: Bug Tracker, https://github.com/eons-dev/eons.lib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `eons-2.3.6/pkg/eons.egg-info/SOURCES.txt` & `eons-2.4.0/pkg/eons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eons-2.3.6/setup.cfg` & `eons-2.4.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = eons
-version = 2.3.6
+version = 2.4.0
 author = Eons
 author_email = support@eons.llc
 description = Eons Python Framework
 license_files = LICENSE.txt
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/eons-dev/eons.lib
@@ -18,18 +18,18 @@
 
 [options]
 package_dir = 
 	= pkg
 packages = find:
 python_requires = >=3.7
 install_requires = 
-	pyyaml
-	requests
 	tqdm
+	pyyaml
 	jsonpickle
+	requests
 
 [options.packages.find]
 where = pkg
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

