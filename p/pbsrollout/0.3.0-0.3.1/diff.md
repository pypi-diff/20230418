# Comparing `tmp/pbsrollout-0.3.0.tar.gz` & `tmp/pbsrollout-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pbsrollout-0.3.0.tar", max compression
+gzip compressed data, was "pbsrollout-0.3.1.tar", max compression
```

## Comparing `pbsrollout-0.3.0.tar` & `pbsrollout-0.3.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0        0 2022-07-21 03:13:41.658475 pbsrollout-0.3.0/LICENSE
--rw-r--r--   0        0        0        0 2022-07-14 16:06:49.043912 pbsrollout-0.3.0/pbsrollout/__init__.py
--rw-r--r--   0        0        0        0 2023-04-05 21:41:28.936936 pbsrollout-0.3.0/pbsrollout/internal/__init__.py
--rw-r--r--   0        0        0     1231 2023-04-13 22:21:13.072224 pbsrollout-0.3.0/pbsrollout/internal/aws_utils.py
--rw-r--r--   0        0        0     2829 2023-04-05 21:42:20.098114 pbsrollout-0.3.0/pbsrollout/internal/check_cluster_ready.py
--rw-r--r--   0        0        0     3733 2023-02-23 22:56:56.612903 pbsrollout-0.3.0/pbsrollout/internal/k8s_utils.py
--rw-r--r--   0        0        0     9181 2023-04-05 21:42:20.105536 pbsrollout-0.3.0/pbsrollout/internal/process_cluster.py
--rw-r--r--   0        0        0      208 2023-04-13 22:19:08.544564 pbsrollout-0.3.0/pbsrollout/internal/test_aws_utils.py
--rw-r--r--   0        0        0     1217 2023-04-05 21:42:20.110740 pbsrollout-0.3.0/pbsrollout/internal/test_k8s_utils.py
--rw-r--r--   0        0        0      444 2023-04-05 21:42:20.121783 pbsrollout-0.3.0/pbsrollout/internal/test_process_cluster.py
--rw-r--r--   0        0        0      925 2022-07-27 23:18:57.505345 pbsrollout-0.3.0/pbsrollout/internal/utils.py
--rw-r--r--   0        0        0     4645 2023-04-13 22:01:13.155828 pbsrollout-0.3.0/pbsrollout/main.py
--rw-r--r--   0        0        0        0 2023-04-05 21:40:57.190004 pbsrollout-0.3.0/pbsrollout/pbs_release/__init__.py
--rw-r--r--   0        0        0     9374 2023-04-05 21:59:04.793955 pbsrollout-0.3.0/pbsrollout/pbs_release/main_view.py
--rw-r--r--   0        0        0        0 2023-04-05 21:40:57.190004 pbsrollout-0.3.0/pbsrollout/stg_release/__init__.py
--rw-r--r--   0        0        0     5907 2023-04-13 22:27:23.574087 pbsrollout-0.3.0/pbsrollout/stg_release/main_view.py
--rw-r--r--   0        0        0      522 2023-04-17 21:46:12.481295 pbsrollout-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      649 1970-01-01 00:00:00.000000 pbsrollout-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-07-21 03:13:41.658475 pbsrollout-0.3.1/LICENSE
+-rw-r--r--   0        0        0        0 2022-07-14 16:06:49.043912 pbsrollout-0.3.1/pbsrollout/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-05 21:41:28.936936 pbsrollout-0.3.1/pbsrollout/internal/__init__.py
+-rw-r--r--   0        0        0     1231 2023-04-13 22:21:13.072224 pbsrollout-0.3.1/pbsrollout/internal/aws_utils.py
+-rw-r--r--   0        0        0     2829 2023-04-05 21:42:20.098114 pbsrollout-0.3.1/pbsrollout/internal/check_cluster_ready.py
+-rw-r--r--   0        0        0     3733 2023-02-23 22:56:56.612903 pbsrollout-0.3.1/pbsrollout/internal/k8s_utils.py
+-rw-r--r--   0        0        0     9181 2023-04-05 21:42:20.105536 pbsrollout-0.3.1/pbsrollout/internal/process_cluster.py
+-rw-r--r--   0        0        0      208 2023-04-13 22:19:08.544564 pbsrollout-0.3.1/pbsrollout/internal/test_aws_utils.py
+-rw-r--r--   0        0        0     1217 2023-04-05 21:42:20.110740 pbsrollout-0.3.1/pbsrollout/internal/test_k8s_utils.py
+-rw-r--r--   0        0        0      444 2023-04-05 21:42:20.121783 pbsrollout-0.3.1/pbsrollout/internal/test_process_cluster.py
+-rw-r--r--   0        0        0      925 2022-07-27 23:18:57.505345 pbsrollout-0.3.1/pbsrollout/internal/utils.py
+-rw-r--r--   0        0        0     4667 2023-04-17 22:04:49.560368 pbsrollout-0.3.1/pbsrollout/main.py
+-rw-r--r--   0        0        0        0 2023-04-05 21:40:57.190004 pbsrollout-0.3.1/pbsrollout/pbs_release/__init__.py
+-rw-r--r--   0        0        0     9374 2023-04-05 21:59:04.793955 pbsrollout-0.3.1/pbsrollout/pbs_release/main_view.py
+-rw-r--r--   0        0        0        0 2023-04-05 21:40:57.190004 pbsrollout-0.3.1/pbsrollout/stg_release/__init__.py
+-rw-r--r--   0        0        0     5907 2023-04-13 22:27:23.574087 pbsrollout-0.3.1/pbsrollout/stg_release/main_view.py
+-rw-r--r--   0        0        0      522 2023-04-17 22:05:10.459171 pbsrollout-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      649 1970-01-01 00:00:00.000000 pbsrollout-0.3.1/PKG-INFO
```

### Comparing `pbsrollout-0.3.0/pbsrollout/internal/aws_utils.py` & `pbsrollout-0.3.1/pbsrollout/internal/aws_utils.py`

 * *Files identical despite different names*

### Comparing `pbsrollout-0.3.0/pbsrollout/internal/check_cluster_ready.py` & `pbsrollout-0.3.1/pbsrollout/internal/check_cluster_ready.py`

 * *Files identical despite different names*

### Comparing `pbsrollout-0.3.0/pbsrollout/internal/k8s_utils.py` & `pbsrollout-0.3.1/pbsrollout/internal/k8s_utils.py`

 * *Files identical despite different names*

### Comparing `pbsrollout-0.3.0/pbsrollout/internal/process_cluster.py` & `pbsrollout-0.3.1/pbsrollout/internal/process_cluster.py`

 * *Files identical despite different names*

### Comparing `pbsrollout-0.3.0/pbsrollout/internal/test_k8s_utils.py` & `pbsrollout-0.3.1/pbsrollout/internal/test_k8s_utils.py`

 * *Files identical despite different names*

### Comparing `pbsrollout-0.3.0/pbsrollout/internal/utils.py` & `pbsrollout-0.3.1/pbsrollout/internal/utils.py`

 * *Files identical despite different names*

### Comparing `pbsrollout-0.3.0/pbsrollout/main.py` & `pbsrollout-0.3.1/pbsrollout/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,18 +69,18 @@
                                  title="What do you want to do?",
                                  raise_error_on_interrupt=True)
     menu_entry_index = terminal_menu.show()
 
     # switch view depending on action
     if menu_entry_index == 0:
         # release_prebid
-        from pbs_release.main_view import entrypoint
+        from pbsrollout.pbs_release.main_view import entrypoint
         entrypoint(console)
     elif menu_entry_index == 1:
-        from stg_release.main_view import entrypoint
+        from pbsrollout.stg_release.main_view import entrypoint
         entrypoint(console)
 
 
 def main():
     """
     This main doesn't is not responsible for the main logic of the program.
     Instead, we:
```

### Comparing `pbsrollout-0.3.0/pbsrollout/pbs_release/main_view.py` & `pbsrollout-0.3.1/pbsrollout/pbs_release/main_view.py`

 * *Files identical despite different names*

### Comparing `pbsrollout-0.3.0/pbsrollout/stg_release/main_view.py` & `pbsrollout-0.3.1/pbsrollout/stg_release/main_view.py`

 * *Files identical despite different names*

### Comparing `pbsrollout-0.3.0/pyproject.toml` & `pbsrollout-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pbsrollout"
-version = "0.3.0"
+version = "0.3.1"
 description = ""
 authors = ["dimitri <dimitriwyzlic@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 shellpy = "^0.5.1"
 kubernetes = "^24.2.0"
```

### Comparing `pbsrollout-0.3.0/PKG-INFO` & `pbsrollout-0.3.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pbsrollout
-Version: 0.3.0
+Version: 0.3.1
 Summary: 
 Author: dimitri
 Author-email: dimitriwyzlic@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

