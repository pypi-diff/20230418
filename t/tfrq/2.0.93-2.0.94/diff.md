# Comparing `tmp/tfrq-2.0.93.tar.gz` & `tmp/tfrq-2.0.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tfrq-2.0.93.tar", last modified: Wed Jan 25 07:15:48 2023, max compression
+gzip compressed data, was "tfrq-2.0.94.tar", last modified: Tue Apr 18 12:02:04 2023, max compression
```

## Comparing `tfrq-2.0.93.tar` & `tfrq-2.0.94.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-01-25 07:15:48.972481 tfrq-2.0.93/
--rw-rw-rw-   0        0        0    11558 2023-01-19 12:12:19.000000 tfrq-2.0.93/LICENSE
--rw-rw-rw-   0        0        0     3899 2023-01-25 07:15:48.971471 tfrq-2.0.93/PKG-INFO
--rw-rw-rw-   0        0        0     3531 2023-01-25 07:03:48.000000 tfrq-2.0.93/README.rst
--rw-rw-rw-   0        0        0       42 2023-01-25 07:15:48.972481 tfrq-2.0.93/setup.cfg
--rw-rw-rw-   0        0        0      452 2023-01-25 07:15:27.000000 tfrq-2.0.93/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-25 07:15:48.970479 tfrq-2.0.93/tfrq.egg-info/
--rw-rw-rw-   0        0        0     3899 2023-01-25 07:15:48.000000 tfrq-2.0.93/tfrq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      174 2023-01-25 07:15:48.000000 tfrq-2.0.93/tfrq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-25 07:15:48.000000 tfrq-2.0.93/tfrq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-01-25 07:15:48.000000 tfrq-2.0.93/tfrq.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-01-25 07:15:48.000000 tfrq-2.0.93/tfrq.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2560 2023-01-25 07:14:54.000000 tfrq-2.0.93/tfrq.py
+drwxrwxrwx   0        0        0        0 2023-04-18 12:02:04.846947 tfrq-2.0.94/
+-rw-rw-rw-   0        0        0    11558 2023-01-19 12:12:19.000000 tfrq-2.0.94/LICENSE
+-rw-rw-rw-   0        0        0     3840 2023-04-18 12:02:04.839885 tfrq-2.0.94/PKG-INFO
+-rw-rw-rw-   0        0        0     3531 2023-01-25 07:03:48.000000 tfrq-2.0.94/README.rst
+-rw-rw-rw-   0        0        0       42 2023-04-18 12:02:04.847945 tfrq-2.0.94/setup.cfg
+-rw-rw-rw-   0        0        0      452 2023-04-18 11:56:50.000000 tfrq-2.0.94/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 12:02:04.837886 tfrq-2.0.94/tfrq.egg-info/
+-rw-rw-rw-   0        0        0     3840 2023-04-18 12:02:04.000000 tfrq-2.0.94/tfrq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      174 2023-04-18 12:02:04.000000 tfrq-2.0.94/tfrq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 12:02:04.000000 tfrq-2.0.94/tfrq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-04-18 12:02:04.000000 tfrq-2.0.94/tfrq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-18 12:02:04.000000 tfrq-2.0.94/tfrq.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2826 2023-04-18 11:56:21.000000 tfrq-2.0.94/tfrq.py
```

### Comparing `tfrq-2.0.93/LICENSE` & `tfrq-2.0.94/LICENSE`

 * *Files identical despite different names*

### Comparing `tfrq-2.0.93/PKG-INFO` & `tfrq-2.0.94/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 Metadata-Version: 2.1
 Name: tfrq
-Version: 2.0.93
+Version: 2.0.94
 Summary: A library to parallelize the execution of a function in python
-Home-page: UNKNOWN
 Author: Foad Abo Dahood
 Author-email: Foad.ad5491@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 License-File: LICENSE
 
 tfrq - an easy way to parallelize processing a function
 =======================================================
 
 `tfrq on github! <https://github.com/masterFoad/tfrq>`_
 
@@ -101,8 +98,7 @@
 
     config = {"return_errors": False, "print_errors": True}
 
 
 tfrq is an arabic word meaning “To Split”, which is the purpose of this
 simple method, to split the work of a single function into multiple
 processes as easy as possible.
-
```

### Comparing `tfrq-2.0.93/README.rst` & `tfrq-2.0.94/README.rst`

 * *Files identical despite different names*

### Comparing `tfrq-2.0.93/tfrq.egg-info/PKG-INFO` & `tfrq-2.0.94/tfrq.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 Metadata-Version: 2.1
 Name: tfrq
-Version: 2.0.93
+Version: 2.0.94
 Summary: A library to parallelize the execution of a function in python
-Home-page: UNKNOWN
 Author: Foad Abo Dahood
 Author-email: Foad.ad5491@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 License-File: LICENSE
 
 tfrq - an easy way to parallelize processing a function
 =======================================================
 
 `tfrq on github! <https://github.com/masterFoad/tfrq>`_
 
@@ -101,8 +98,7 @@
 
     config = {"return_errors": False, "print_errors": True}
 
 
 tfrq is an arabic word meaning “To Split”, which is the purpose of this
 simple method, to split the work of a single function into multiple
 processes as easy as possible.
-
```

### Comparing `tfrq-2.0.93/tfrq.py` & `tfrq-2.0.94/tfrq.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,15 +31,15 @@
             if config["print_errors"]:
                 print(e)
             results.append(None)
             errors.append(e)
     return results, errors
 
 
-def tfrq(func: Callable, params: List, operator=None, num_cores=None, config=None):
+def tfrq(func: Callable, params: List, operator=None, num_cores=None, config=None, custom_executor=None):
     import math
     from concurrent.futures import ProcessPoolExecutor
     import os
 
     if num_cores is None:
         num_cores = os.cpu_count()
 
@@ -50,18 +50,23 @@
         for cfg in config_default_values:
             if cfg not in config:
                 config[cfg] = config_default_values[cfg]
 
     chunk_size = math.ceil(len(params) / num_cores)
     chunks = [params[i:i + chunk_size] for i in range(0, len(params), chunk_size)]
     print("Tfrq into", len(chunks), "Chunks for", num_cores, "cores.")
-    with ProcessPoolExecutor(max_workers=num_cores) as executor:
+    if custom_executor:
         results = list(
-            executor.map(param_list,
-                         [(func, chunk_num, chunk, operator, config) for chunk_num, chunk in enumerate(chunks)]))
+            custom_executor.map(param_list,
+                                [(func, chunk_num, chunk, operator, config) for chunk_num, chunk in enumerate(chunks)]))
+    else:
+        with ProcessPoolExecutor(max_workers=num_cores) as executor:
+            results = list(
+                executor.map(param_list,
+                             [(func, chunk_num, chunk, operator, config) for chunk_num, chunk in enumerate(chunks)]))
 
     errors = []
     final_results = []
     for res in results:
         final_results.append(res[0])
         errors.append(res[1])
```

