# Comparing `tmp/petab_select-0.1.4.tar.gz` & `tmp/petab_select-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "petab_select-0.1.4.tar", last modified: Thu Apr 13 16:13:11 2023, max compression
+gzip compressed data, was "petab_select-0.1.5.tar", last modified: Mon Apr 17 22:52:49 2023, max compression
```

## Comparing `petab_select-0.1.4.tar` & `petab_select-0.1.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 dilan     (1001) dilan     (1001)        0 2023-04-13 16:13:11.128681 petab_select-0.1.4/
--rw-rw-r--   0 dilan     (1001) dilan     (1001)     1602 2021-08-31 13:20:42.000000 petab_select-0.1.4/LICENSE
--rw-rw-r--   0 dilan     (1001) dilan     (1001)     9746 2023-04-13 16:13:11.128681 petab_select-0.1.4/PKG-INFO
--rw-rw-r--   0 dilan     (1001) dilan     (1001)     9256 2023-04-13 16:12:57.000000 petab_select-0.1.4/README.md
-drwxrwxr-x   0 dilan     (1001) dilan     (1001)        0 2023-04-13 16:13:11.124681 petab_select-0.1.4/petab_select/
--rw-rw-r--   0 dilan     (1001) dilan     (1001)      263 2023-04-13 08:28:52.000000 petab_select-0.1.4/petab_select/__init__.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)    51676 2022-09-30 16:40:04.000000 petab_select-0.1.4/petab_select/candidate_space.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)    13247 2022-09-30 16:40:04.000000 petab_select-0.1.4/petab_select/cli.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)     4460 2022-09-30 16:40:04.000000 petab_select-0.1.4/petab_select/constants.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)     7225 2022-09-30 16:40:04.000000 petab_select-0.1.4/petab_select/criteria.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)     2443 2021-11-02 20:14:39.000000 petab_select-0.1.4/petab_select/descriptors.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)     1076 2022-09-30 16:40:04.000000 petab_select-0.1.4/petab_select/handlers.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)     2438 2022-09-30 16:40:04.000000 petab_select-0.1.4/petab_select/misc.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)    25962 2023-04-13 16:12:57.000000 petab_select-0.1.4/petab_select/model.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)    11415 2022-09-30 16:40:04.000000 petab_select-0.1.4/petab_select/model_space.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)    38364 2022-09-30 16:40:04.000000 petab_select-0.1.4/petab_select/model_subspace.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)     2254 2022-09-30 16:40:04.000000 petab_select-0.1.4/petab_select/petab.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)     8571 2023-04-13 08:28:52.000000 petab_select-0.1.4/petab_select/problem.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)    10109 2023-04-13 16:12:57.000000 petab_select-0.1.4/petab_select/ui.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)      295 2021-11-03 18:08:02.000000 petab_select-0.1.4/petab_select/validators.py
--rw-rw-r--   0 dilan     (1001) dilan     (1001)       80 2023-04-13 16:12:57.000000 petab_select-0.1.4/petab_select/version.py
-drwxrwxr-x   0 dilan     (1001) dilan     (1001)        0 2023-04-13 16:13:11.124681 petab_select-0.1.4/petab_select.egg-info/
--rw-rw-r--   0 dilan     (1001) dilan     (1001)     9746 2023-04-13 16:13:11.000000 petab_select-0.1.4/petab_select.egg-info/PKG-INFO
--rw-rw-r--   0 dilan     (1001) dilan     (1001)      658 2023-04-13 16:13:11.000000 petab_select-0.1.4/petab_select.egg-info/SOURCES.txt
--rw-rw-r--   0 dilan     (1001) dilan     (1001)        1 2023-04-13 16:13:11.000000 petab_select-0.1.4/petab_select.egg-info/dependency_links.txt
--rw-rw-r--   0 dilan     (1001) dilan     (1001)       54 2023-04-13 16:13:11.000000 petab_select-0.1.4/petab_select.egg-info/entry_points.txt
--rw-rw-r--   0 dilan     (1001) dilan     (1001)      136 2023-04-13 16:13:11.000000 petab_select-0.1.4/petab_select.egg-info/requires.txt
--rw-rw-r--   0 dilan     (1001) dilan     (1001)       13 2023-04-13 16:13:11.000000 petab_select-0.1.4/petab_select.egg-info/top_level.txt
--rw-rw-r--   0 dilan     (1001) dilan     (1001)      281 2022-09-30 16:40:04.000000 petab_select-0.1.4/pyproject.toml
--rw-rw-r--   0 dilan     (1001) dilan     (1001)       38 2023-04-13 16:13:11.128681 petab_select-0.1.4/setup.cfg
--rw-rw-r--   0 dilan     (1001) dilan     (1001)     2961 2023-04-13 16:12:57.000000 petab_select-0.1.4/setup.py
+drwxrwxr-x   0 dilan     (1001) dilan     (1001)        0 2023-04-17 22:52:49.704084 petab_select-0.1.5/
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)     1602 2021-08-31 13:20:42.000000 petab_select-0.1.5/LICENSE
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)     9746 2023-04-17 22:52:49.700084 petab_select-0.1.5/PKG-INFO
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)     9256 2023-04-13 16:12:57.000000 petab_select-0.1.5/README.md
+drwxrwxr-x   0 dilan     (1001) dilan     (1001)        0 2023-04-17 22:52:49.700084 petab_select-0.1.5/petab_select/
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)      263 2023-04-13 08:28:52.000000 petab_select-0.1.5/petab_select/__init__.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)    51676 2022-09-30 16:40:04.000000 petab_select-0.1.5/petab_select/candidate_space.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)    13247 2022-09-30 16:40:04.000000 petab_select-0.1.5/petab_select/cli.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)     4460 2022-09-30 16:40:04.000000 petab_select-0.1.5/petab_select/constants.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)     7225 2022-09-30 16:40:04.000000 petab_select-0.1.5/petab_select/criteria.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)     2443 2021-11-02 20:14:39.000000 petab_select-0.1.5/petab_select/descriptors.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)     1076 2022-09-30 16:40:04.000000 petab_select-0.1.5/petab_select/handlers.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)     2438 2022-09-30 16:40:04.000000 petab_select-0.1.5/petab_select/misc.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)    25969 2023-04-17 22:48:13.000000 petab_select-0.1.5/petab_select/model.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)    11415 2022-09-30 16:40:04.000000 petab_select-0.1.5/petab_select/model_space.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)    38364 2022-09-30 16:40:04.000000 petab_select-0.1.5/petab_select/model_subspace.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)     2254 2022-09-30 16:40:04.000000 petab_select-0.1.5/petab_select/petab.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)     8571 2023-04-13 08:28:52.000000 petab_select-0.1.5/petab_select/problem.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)    10109 2023-04-13 16:12:57.000000 petab_select-0.1.5/petab_select/ui.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)      295 2021-11-03 18:08:02.000000 petab_select-0.1.5/petab_select/validators.py
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)       80 2023-04-17 22:52:18.000000 petab_select-0.1.5/petab_select/version.py
+drwxrwxr-x   0 dilan     (1001) dilan     (1001)        0 2023-04-17 22:52:49.700084 petab_select-0.1.5/petab_select.egg-info/
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)     9746 2023-04-17 22:52:49.000000 petab_select-0.1.5/petab_select.egg-info/PKG-INFO
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)      658 2023-04-17 22:52:49.000000 petab_select-0.1.5/petab_select.egg-info/SOURCES.txt
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)        1 2023-04-17 22:52:49.000000 petab_select-0.1.5/petab_select.egg-info/dependency_links.txt
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)       54 2023-04-17 22:52:49.000000 petab_select-0.1.5/petab_select.egg-info/entry_points.txt
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)      136 2023-04-17 22:52:49.000000 petab_select-0.1.5/petab_select.egg-info/requires.txt
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)       13 2023-04-17 22:52:49.000000 petab_select-0.1.5/petab_select.egg-info/top_level.txt
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)      281 2022-09-30 16:40:04.000000 petab_select-0.1.5/pyproject.toml
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)       38 2023-04-17 22:52:49.704084 petab_select-0.1.5/setup.cfg
+-rw-rw-r--   0 dilan     (1001) dilan     (1001)     2961 2023-04-13 16:12:57.000000 petab_select-0.1.5/setup.py
```

### Comparing `petab_select-0.1.4/LICENSE` & `petab_select-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.4/PKG-INFO` & `petab_select-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petab_select
-Version: 0.1.4
+Version: 0.1.5
 Summary: PEtab Select: an extension to PEtab for model selection.
 Home-page: https://github.com/PEtab-dev/petab_select
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `petab_select-0.1.4/README.md` & `petab_select-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.4/petab_select/candidate_space.py` & `petab_select-0.1.5/petab_select/candidate_space.py`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.4/petab_select/cli.py` & `petab_select-0.1.5/petab_select/cli.py`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.4/petab_select/constants.py` & `petab_select-0.1.5/petab_select/constants.py`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.4/petab_select/criteria.py` & `petab_select-0.1.5/petab_select/criteria.py`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.4/petab_select/descriptors.py` & `petab_select-0.1.5/petab_select/descriptors.py`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.4/petab_select/handlers.py` & `petab_select-0.1.5/petab_select/handlers.py`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.4/petab_select/misc.py` & `petab_select-0.1.5/petab_select/misc.py`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.4/petab_select/model.py` & `petab_select-0.1.5/petab_select/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,15 @@
         # can provide type `np.float64`, which causes issues when writing to
         # YAML.
         # ESTIMATED_PARAMETERS: lambda x: x,
         ESTIMATED_PARAMETERS: lambda x: {
             str(id): float(value) for id, value in x.items()
         },
         CRITERIA: lambda x: {
-            criterion_id.value: criterion_value
+            criterion_id.value: float(criterion_value)
             for criterion_id, criterion_value in x.items()
         },
     }
     hash_attributes = {
         # MODEL_ID: lambda x: hash(x),  # possible circular dependency on hash
         # MODEL_SUBSPACE_ID: lambda x: hash(x),
         # MODEL_SUBSPACE_INDICES: hash_list,
```

### Comparing `petab_select-0.1.4/petab_select/model_space.py` & `petab_select-0.1.5/petab_select/model_space.py`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.4/petab_select/model_subspace.py` & `petab_select-0.1.5/petab_select/model_subspace.py`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.4/petab_select/petab.py` & `petab_select-0.1.5/petab_select/petab.py`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.4/petab_select/problem.py` & `petab_select-0.1.5/petab_select/problem.py`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.4/petab_select/ui.py` & `petab_select-0.1.5/petab_select/ui.py`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.4/petab_select.egg-info/PKG-INFO` & `petab_select-0.1.5/petab_select.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petab-select
-Version: 0.1.4
+Version: 0.1.5
 Summary: PEtab Select: an extension to PEtab for model selection.
 Home-page: https://github.com/PEtab-dev/petab_select
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `petab_select-0.1.4/petab_select.egg-info/SOURCES.txt` & `petab_select-0.1.5/petab_select.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `petab_select-0.1.4/setup.py` & `petab_select-0.1.5/setup.py`

 * *Files identical despite different names*

