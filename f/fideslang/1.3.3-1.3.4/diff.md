# Comparing `tmp/fideslang-1.3.3.tar.gz` & `tmp/fideslang-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fideslang-1.3.3.tar", last modified: Tue Jan 24 15:48:32 2023, max compression
+gzip compressed data, was "fideslang-1.3.4.tar", last modified: Tue Apr 18 13:29:41 2023, max compression
```

## Comparing `fideslang-1.3.3.tar` & `fideslang-1.3.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 15:48:32.681625 fideslang-1.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)    18656 2023-01-24 15:48:26.000000 fideslang-1.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-01-24 15:48:26.000000 fideslang-1.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-01-24 15:48:32.681625 fideslang-1.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-01-24 15:48:26.000000 fideslang-1.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-01-24 15:48:26.000000 fideslang-1.3.3/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-01-24 15:48:26.000000 fideslang-1.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-01-24 15:48:26.000000 fideslang-1.3.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-01-24 15:48:32.681625 fideslang-1.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-01-24 15:48:26.000000 fideslang-1.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 15:48:32.673625 fideslang-1.3.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 15:48:32.681625 fideslang-1.3.3/src/fideslang/
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-01-24 15:48:26.000000 fideslang-1.3.3/src/fideslang/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-01-24 15:48:32.681625 fideslang-1.3.3/src/fideslang/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    12917 2023-01-24 15:48:26.000000 fideslang-1.3.3/src/fideslang/default_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)    32851 2023-01-24 15:48:26.000000 fideslang-1.3.3/src/fideslang/default_taxonomy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-01-24 15:48:26.000000 fideslang-1.3.3/src/fideslang/manifests.py
--rw-r--r--   0 runner    (1001) docker     (123)    35518 2023-01-24 15:48:26.000000 fideslang-1.3.3/src/fideslang/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-01-24 15:48:26.000000 fideslang-1.3.3/src/fideslang/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 15:48:26.000000 fideslang-1.3.3/src/fideslang/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-01-24 15:48:26.000000 fideslang-1.3.3/src/fideslang/relationships.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-01-24 15:48:26.000000 fideslang-1.3.3/src/fideslang/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-01-24 15:48:26.000000 fideslang-1.3.3/src/fideslang/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 15:48:32.681625 fideslang-1.3.3/src/fideslang.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-01-24 15:48:32.000000 fideslang-1.3.3/src/fideslang.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-01-24 15:48:32.000000 fideslang-1.3.3/src/fideslang.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-24 15:48:32.000000 fideslang-1.3.3/src/fideslang.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-01-24 15:48:32.000000 fideslang-1.3.3/src/fideslang.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-24 15:48:32.000000 fideslang-1.3.3/src/fideslang.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    57971 2023-01-24 15:48:26.000000 fideslang-1.3.3/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:29:41.948316 fideslang-1.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    18656 2023-04-18 13:29:36.000000 fideslang-1.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-18 13:29:36.000000 fideslang-1.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-04-18 13:29:41.948316 fideslang-1.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-04-18 13:29:36.000000 fideslang-1.3.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-18 13:29:36.000000 fideslang-1.3.4/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-04-18 13:29:36.000000 fideslang-1.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-18 13:29:36.000000 fideslang-1.3.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-18 13:29:41.952316 fideslang-1.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-04-18 13:29:36.000000 fideslang-1.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:29:41.948316 fideslang-1.3.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:29:41.952316 fideslang-1.3.4/src/fideslang/
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-18 13:29:36.000000 fideslang-1.3.4/src/fideslang/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-18 13:29:41.952316 fideslang-1.3.4/src/fideslang/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12917 2023-04-18 13:29:36.000000 fideslang-1.3.4/src/fideslang/default_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32851 2023-04-18 13:29:36.000000 fideslang-1.3.4/src/fideslang/default_taxonomy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-04-18 13:29:36.000000 fideslang-1.3.4/src/fideslang/manifests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35611 2023-04-18 13:29:36.000000 fideslang-1.3.4/src/fideslang/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-18 13:29:36.000000 fideslang-1.3.4/src/fideslang/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 13:29:36.000000 fideslang-1.3.4/src/fideslang/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-04-18 13:29:36.000000 fideslang-1.3.4/src/fideslang/relationships.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-18 13:29:36.000000 fideslang-1.3.4/src/fideslang/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-04-18 13:29:36.000000 fideslang-1.3.4/src/fideslang/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:29:41.948316 fideslang-1.3.4/src/fideslang.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-04-18 13:29:41.000000 fideslang-1.3.4/src/fideslang.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-18 13:29:41.000000 fideslang-1.3.4/src/fideslang.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 13:29:41.000000 fideslang-1.3.4/src/fideslang.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-18 13:29:41.000000 fideslang-1.3.4/src/fideslang.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-18 13:29:41.000000 fideslang-1.3.4/src/fideslang.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    57971 2023-04-18 13:29:36.000000 fideslang-1.3.4/versioneer.py
```

### Comparing `fideslang-1.3.3/LICENSE` & `fideslang-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fideslang-1.3.3/PKG-INFO` & `fideslang-1.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fideslang
-Version: 1.3.3
+Version: 1.3.4
 Summary: Fides Taxonomy Language
 Home-page: https://github.com/ethyca/fideslang
 Author: Ethyca, Inc.
 Author-email: fidesteam@ethyca.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `fideslang-1.3.3/README.md` & `fideslang-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `fideslang-1.3.3/pyproject.toml` & `fideslang-1.3.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fideslang-1.3.3/setup.cfg` & `fideslang-1.3.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `fideslang-1.3.3/setup.py` & `fideslang-1.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `fideslang-1.3.3/src/fideslang/__init__.py` & `fideslang-1.3.4/src/fideslang/__init__.py`

 * *Files identical despite different names*

### Comparing `fideslang-1.3.3/src/fideslang/default_fixtures.py` & `fideslang-1.3.4/src/fideslang/default_fixtures.py`

 * *Files identical despite different names*

### Comparing `fideslang-1.3.3/src/fideslang/default_taxonomy.py` & `fideslang-1.3.4/src/fideslang/default_taxonomy.py`

 * *Files identical despite different names*

### Comparing `fideslang-1.3.3/src/fideslang/manifests.py` & `fideslang-1.3.4/src/fideslang/manifests.py`

 * *Files identical despite different names*

### Comparing `fideslang-1.3.3/src/fideslang/models.py` & `fideslang-1.3.4/src/fideslang/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -820,14 +820,19 @@
             warn(
                 "The dataset_references field is deprecated, and will be removed in a future version of fideslang. Use the 'egress' and 'ingress` fields instead.",
                 DeprecationWarning,
             )
 
         return value
 
+    class Config:
+        """Config for the Privacy Declaration"""
+
+        orm_mode = True
+
 
 class SystemMetadata(BaseModel):
     """
     The SystemMetadata resource model.
 
     Object used to hold application specific metadata for a system
     """
```

### Comparing `fideslang-1.3.3/src/fideslang/parse.py` & `fideslang-1.3.4/src/fideslang/parse.py`

 * *Files identical despite different names*

### Comparing `fideslang-1.3.3/src/fideslang/relationships.py` & `fideslang-1.3.4/src/fideslang/relationships.py`

 * *Files identical despite different names*

### Comparing `fideslang-1.3.3/src/fideslang/utils.py` & `fideslang-1.3.4/src/fideslang/utils.py`

 * *Files identical despite different names*

### Comparing `fideslang-1.3.3/src/fideslang/validation.py` & `fideslang-1.3.4/src/fideslang/validation.py`

 * *Files identical despite different names*

### Comparing `fideslang-1.3.3/src/fideslang.egg-info/PKG-INFO` & `fideslang-1.3.4/src/fideslang.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fideslang
-Version: 1.3.3
+Version: 1.3.4
 Summary: Fides Taxonomy Language
 Home-page: https://github.com/ethyca/fideslang
 Author: Ethyca, Inc.
 Author-email: fidesteam@ethyca.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `fideslang-1.3.3/src/fideslang.egg-info/SOURCES.txt` & `fideslang-1.3.4/src/fideslang.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fideslang-1.3.3/versioneer.py` & `fideslang-1.3.4/versioneer.py`

 * *Files identical despite different names*

