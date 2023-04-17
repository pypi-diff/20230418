# Comparing `tmp/rustimport-1.2.4.tar.gz` & `tmp/rustimport-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rustimport-1.2.4.tar", last modified: Sun Apr  9 14:33:55 2023, max compression
+gzip compressed data, was "rustimport-1.2.5.tar", last modified: Mon Apr 17 23:08:31 2023, max compression
```

## Comparing `rustimport-1.2.4.tar` & `rustimport-1.2.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:33:55.872160 rustimport-1.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-09 14:33:44.000000 rustimport-1.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-09 14:33:44.000000 rustimport-1.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13693 2023-04-09 14:33:55.872160 rustimport-1.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13070 2023-04-09 14:33:44.000000 rustimport-1.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-09 14:33:44.000000 rustimport-1.2.4/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:33:55.872160 rustimport-1.2.4/rustimport/
--rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-04-09 14:33:44.000000 rustimport-1.2.4/rustimport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6951 2023-04-09 14:33:44.000000 rustimport-1.2.4/rustimport/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-04-09 14:33:44.000000 rustimport-1.2.4/rustimport/checksum.py
--rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-04-09 14:33:44.000000 rustimport-1.2.4/rustimport/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-09 14:33:44.000000 rustimport-1.2.4/rustimport/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-09 14:33:44.000000 rustimport-1.2.4/rustimport/find.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-04-09 14:33:44.000000 rustimport-1.2.4/rustimport/import_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)    12584 2023-04-09 14:33:44.000000 rustimport-1.2.4/rustimport/importable.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-09 14:33:44.000000 rustimport-1.2.4/rustimport/load.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:33:55.872160 rustimport-1.2.4/rustimport/pre_processing/
--rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-04-09 14:33:44.000000 rustimport-1.2.4/rustimport/pre_processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-09 14:33:44.000000 rustimport-1.2.4/rustimport/pre_processing/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-04-09 14:33:44.000000 rustimport-1.2.4/rustimport/pre_processing/pyo3_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-04-09 14:33:44.000000 rustimport-1.2.4/rustimport/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:33:55.872160 rustimport-1.2.4/rustimport.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13693 2023-04-09 14:33:55.000000 rustimport-1.2.4/rustimport.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-09 14:33:55.000000 rustimport-1.2.4/rustimport.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 14:33:55.000000 rustimport-1.2.4/rustimport.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 14:33:55.000000 rustimport-1.2.4/rustimport.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-09 14:33:55.000000 rustimport-1.2.4/rustimport.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-09 14:33:55.000000 rustimport-1.2.4/rustimport.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 14:33:55.872160 rustimport-1.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-09 14:33:44.000000 rustimport-1.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 14:33:55.872160 rustimport-1.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-09 14:33:44.000000 rustimport-1.2.4/tests/run_all.py
--rw-r--r--   0 runner    (1001) docker     (123)     7004 2023-04-09 14:33:44.000000 rustimport-1.2.4/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-04-09 14:33:44.000000 rustimport-1.2.4/tests/test_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:08:31.108228 rustimport-1.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-17 23:08:16.000000 rustimport-1.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-17 23:08:16.000000 rustimport-1.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13693 2023-04-17 23:08:31.108228 rustimport-1.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13070 2023-04-17 23:08:16.000000 rustimport-1.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-17 23:08:16.000000 rustimport-1.2.5/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:08:31.104227 rustimport-1.2.5/rustimport/
+-rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-04-17 23:08:16.000000 rustimport-1.2.5/rustimport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6951 2023-04-17 23:08:16.000000 rustimport-1.2.5/rustimport/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-04-17 23:08:16.000000 rustimport-1.2.5/rustimport/checksum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-04-17 23:08:16.000000 rustimport-1.2.5/rustimport/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-17 23:08:16.000000 rustimport-1.2.5/rustimport/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-17 23:08:16.000000 rustimport-1.2.5/rustimport/find.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-04-17 23:08:16.000000 rustimport-1.2.5/rustimport/import_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12656 2023-04-17 23:08:16.000000 rustimport-1.2.5/rustimport/importable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-17 23:08:16.000000 rustimport-1.2.5/rustimport/load.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:08:31.104227 rustimport-1.2.5/rustimport/pre_processing/
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-04-17 23:08:16.000000 rustimport-1.2.5/rustimport/pre_processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-17 23:08:16.000000 rustimport-1.2.5/rustimport/pre_processing/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-04-17 23:08:16.000000 rustimport-1.2.5/rustimport/pre_processing/pyo3_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-04-17 23:08:16.000000 rustimport-1.2.5/rustimport/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:08:31.104227 rustimport-1.2.5/rustimport.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13693 2023-04-17 23:08:31.000000 rustimport-1.2.5/rustimport.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-17 23:08:31.000000 rustimport-1.2.5/rustimport.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 23:08:31.000000 rustimport-1.2.5/rustimport.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 23:08:30.000000 rustimport-1.2.5/rustimport.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-17 23:08:31.000000 rustimport-1.2.5/rustimport.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-17 23:08:31.000000 rustimport-1.2.5/rustimport.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 23:08:31.108228 rustimport-1.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-17 23:08:16.000000 rustimport-1.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:08:31.108228 rustimport-1.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-17 23:08:16.000000 rustimport-1.2.5/tests/run_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7004 2023-04-17 23:08:16.000000 rustimport-1.2.5/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-04-17 23:08:16.000000 rustimport-1.2.5/tests/test_examples.py
```

### Comparing `rustimport-1.2.4/LICENSE` & `rustimport-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rustimport-1.2.4/PKG-INFO` & `rustimport-1.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rustimport
-Version: 1.2.4
+Version: 1.2.5
 Summary: Import Rust files directly from Python!
 Home-page: https://github.com/mityax/rustimport
 Author: mityax
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `rustimport-1.2.4/README.md` & `rustimport-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `rustimport-1.2.4/rustimport/__init__.py` & `rustimport-1.2.5/rustimport/__init__.py`

 * *Files identical despite different names*

### Comparing `rustimport-1.2.4/rustimport/__main__.py` & `rustimport-1.2.5/rustimport/__main__.py`

 * *Files identical despite different names*

### Comparing `rustimport-1.2.4/rustimport/checksum.py` & `rustimport-1.2.5/rustimport/checksum.py`

 * *Files identical despite different names*

### Comparing `rustimport-1.2.4/rustimport/compiler.py` & `rustimport-1.2.5/rustimport/compiler.py`

 * *Files identical despite different names*

### Comparing `rustimport-1.2.4/rustimport/error_handling.py` & `rustimport-1.2.5/rustimport/error_handling.py`

 * *Files identical despite different names*

### Comparing `rustimport-1.2.4/rustimport/find.py` & `rustimport-1.2.5/rustimport/find.py`

 * *Files identical despite different names*

### Comparing `rustimport-1.2.4/rustimport/import_hook.py` & `rustimport-1.2.5/rustimport/import_hook.py`

 * *Files identical despite different names*

### Comparing `rustimport-1.2.4/rustimport/importable.py` & `rustimport-1.2.5/rustimport/importable.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,17 +157,17 @@
     @property
     def __manifest_path(self) -> str:
         return self.path if self.path.lower().endswith("/cargo.toml") else os.path.join(self.path, 'Cargo.toml')
 
     @cached_property
     def __workspace_path(self) -> Optional[str]:
         """Returns the path of the cargo workspace this crate belongs to, if there is any."""
-
+        root_dir = os.path.abspath(".").split(os.path.sep)[0] + os.path.sep
         p = self.__crate_path
-        while os.path.dirname(p) != os.path.sep:  # loop through all parent directories...
+        while os.path.dirname(p) != root_dir:  # loop through all parent directories...
             p = os.path.dirname(p)
 
             if os.path.isfile(os.path.join(p, "Cargo.toml")):  # ... and check for a "Cargo.toml" file in each of them.
                 return p
 
         return None
```

### Comparing `rustimport-1.2.4/rustimport/load.py` & `rustimport-1.2.5/rustimport/load.py`

 * *Files identical despite different names*

### Comparing `rustimport-1.2.4/rustimport/pre_processing/__init__.py` & `rustimport-1.2.5/rustimport/pre_processing/__init__.py`

 * *Files identical despite different names*

### Comparing `rustimport-1.2.4/rustimport/pre_processing/base.py` & `rustimport-1.2.5/rustimport/pre_processing/base.py`

 * *Files identical despite different names*

### Comparing `rustimport-1.2.4/rustimport/pre_processing/pyo3_template.py` & `rustimport-1.2.5/rustimport/pre_processing/pyo3_template.py`

 * *Files identical despite different names*

### Comparing `rustimport-1.2.4/rustimport/settings.py` & `rustimport-1.2.5/rustimport/settings.py`

 * *Files identical despite different names*

### Comparing `rustimport-1.2.4/rustimport.egg-info/PKG-INFO` & `rustimport-1.2.5/rustimport.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rustimport
-Version: 1.2.4
+Version: 1.2.5
 Summary: Import Rust files directly from Python!
 Home-page: https://github.com/mityax/rustimport
 Author: mityax
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `rustimport-1.2.4/rustimport.egg-info/SOURCES.txt` & `rustimport-1.2.5/rustimport.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rustimport-1.2.4/setup.py` & `rustimport-1.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `rustimport-1.2.4/tests/test_cli.py` & `rustimport-1.2.5/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `rustimport-1.2.4/tests/test_examples.py` & `rustimport-1.2.5/tests/test_examples.py`

 * *Files identical despite different names*

