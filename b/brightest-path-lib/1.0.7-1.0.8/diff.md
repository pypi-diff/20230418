# Comparing `tmp/brightest-path-lib-1.0.7.tar.gz` & `tmp/brightest-path-lib-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/runner/work/brightest-path-lib/brightest-path-lib/dist/.tmp-k4kvgj40/brightest-path-lib-1.0.7.tar", last modified: Tue Apr 18 13:44:38 2023, max compression
+gzip compressed data, was "brightest-path-lib-1.0.8.tar", last modified: Tue Apr 18 17:50:50 2023, max compression
```

## Comparing `brightest-path-lib-1.0.7.tar` & `brightest-path-lib-1.0.8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-18 13:44:38.000000 brightest-path-lib-1.0.7/
--rw-r--r--   0 runner     (501) staff       (20)    35148 2023-04-18 13:43:51.000000 brightest-path-lib-1.0.7/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)      115 2023-04-18 13:43:51.000000 brightest-path-lib-1.0.7/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)      601 2023-04-18 13:44:38.000000 brightest-path-lib-1.0.7/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     1493 2023-04-18 13:43:51.000000 brightest-path-lib-1.0.7/README.md
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-18 13:44:38.000000 brightest-path-lib-1.0.7/brightest_path_lib/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-18 13:44:38.000000 brightest-path-lib-1.0.7/brightest_path_lib/cost/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-18 13:44:38.000000 brightest-path-lib-1.0.7/brightest_path_lib/cost/__pythran__/
--rw-------   0 runner     (501) staff       (20)    19226 2023-04-18 13:44:38.000000 brightest-path-lib-1.0.7/brightest_path_lib/cost/__pythran__/reciprocal_transonic.cpp
--rw-r--r--   0 runner     (501) staff       (20)     2739 2023-04-18 13:43:51.000000 brightest-path-lib-1.0.7/brightest_path_lib/cost/reciprocal_transonic.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-18 13:44:38.000000 brightest-path-lib-1.0.7/brightest_path_lib/heuristic/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-18 13:44:38.000000 brightest-path-lib-1.0.7/brightest_path_lib/heuristic/__pythran__/
--rw-------   0 runner     (501) staff       (20)    34397 2023-04-18 13:44:37.000000 brightest-path-lib-1.0.7/brightest_path_lib/heuristic/__pythran__/euclidean_transonic.cpp
--rw-r--r--   0 runner     (501) staff       (20)     3309 2023-04-18 13:43:51.000000 brightest-path-lib-1.0.7/brightest_path_lib/heuristic/euclidean_transonic.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-18 13:44:38.000000 brightest-path-lib-1.0.7/brightest_path_lib.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)      601 2023-04-18 13:44:37.000000 brightest-path-lib-1.0.7/brightest_path_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)      710 2023-04-18 13:44:38.000000 brightest-path-lib-1.0.7/brightest_path_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2023-04-18 13:44:37.000000 brightest-path-lib-1.0.7/brightest_path_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)      146 2023-04-18 13:44:37.000000 brightest-path-lib-1.0.7/brightest_path_lib.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)       19 2023-04-18 13:44:37.000000 brightest-path-lib-1.0.7/brightest_path_lib.egg-info/top_level.txt
--rw-r--r--   0 runner     (501) staff       (20)      121 2023-04-18 13:43:51.000000 brightest-path-lib-1.0.7/pyproject.toml
--rw-r--r--   0 runner     (501) staff       (20)       38 2023-04-18 13:44:38.000000 brightest-path-lib-1.0.7/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)     2568 2023-04-18 13:43:51.000000 brightest-path-lib-1.0.7/setup.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-18 13:44:38.000000 brightest-path-lib-1.0.7/tests/
--rw-r--r--   0 runner     (501) staff       (20)     4514 2023-04-18 13:43:51.000000 brightest-path-lib-1.0.7/tests/test_astar.py
--rw-r--r--   0 runner     (501) staff       (20)     1874 2023-04-18 13:43:51.000000 brightest-path-lib-1.0.7/tests/test_bidirectional_node.py
--rw-r--r--   0 runner     (501) staff       (20)      611 2023-04-18 13:43:51.000000 brightest-path-lib-1.0.7/tests/test_brightest_path_lib.py
--rw-r--r--   0 runner     (501) staff       (20)     1919 2023-04-18 13:43:51.000000 brightest-path-lib-1.0.7/tests/test_euclidean_heuristic.py
--rw-r--r--   0 runner     (501) staff       (20)     1586 2023-04-18 13:43:51.000000 brightest-path-lib-1.0.7/tests/test_image_stats.py
--rw-r--r--   0 runner     (501) staff       (20)     4700 2023-04-18 13:43:51.000000 brightest-path-lib-1.0.7/tests/test_nbastar.py
--rw-r--r--   0 runner     (501) staff       (20)     1065 2023-04-18 13:43:51.000000 brightest-path-lib-1.0.7/tests/test_node.py
--rw-r--r--   0 runner     (501) staff       (20)     1591 2023-04-18 13:43:51.000000 brightest-path-lib-1.0.7/tests/test_reciprocal_cost_func.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-18 17:50:50.461558 brightest-path-lib-1.0.8/
+-rw-r--r--   0 runner     (501) staff       (20)    35148 2023-04-18 17:50:00.000000 brightest-path-lib-1.0.8/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)      115 2023-04-18 17:50:00.000000 brightest-path-lib-1.0.8/MANIFEST.in
+-rw-r--r--   0 runner     (501) staff       (20)      601 2023-04-18 17:50:50.461182 brightest-path-lib-1.0.8/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     1493 2023-04-18 17:50:00.000000 brightest-path-lib-1.0.8/README.md
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-18 17:50:50.449508 brightest-path-lib-1.0.8/brightest_path_lib/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-18 17:50:50.455358 brightest-path-lib-1.0.8/brightest_path_lib/cost/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-18 17:50:50.455839 brightest-path-lib-1.0.8/brightest_path_lib/cost/__pythran__/
+-rw-------   0 runner     (501) staff       (20)    19226 2023-04-18 17:50:50.000000 brightest-path-lib-1.0.8/brightest_path_lib/cost/__pythran__/reciprocal_transonic.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     2739 2023-04-18 17:50:00.000000 brightest-path-lib-1.0.8/brightest_path_lib/cost/reciprocal_transonic.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-18 17:50:50.456400 brightest-path-lib-1.0.8/brightest_path_lib/heuristic/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-18 17:50:50.456848 brightest-path-lib-1.0.8/brightest_path_lib/heuristic/__pythran__/
+-rw-------   0 runner     (501) staff       (20)    34397 2023-04-18 17:50:50.000000 brightest-path-lib-1.0.8/brightest_path_lib/heuristic/__pythran__/euclidean_transonic.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     3309 2023-04-18 17:50:00.000000 brightest-path-lib-1.0.8/brightest_path_lib/heuristic/euclidean_transonic.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-18 17:50:50.454824 brightest-path-lib-1.0.8/brightest_path_lib.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)      601 2023-04-18 17:50:49.000000 brightest-path-lib-1.0.8/brightest_path_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)      710 2023-04-18 17:50:50.000000 brightest-path-lib-1.0.8/brightest_path_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2023-04-18 17:50:49.000000 brightest-path-lib-1.0.8/brightest_path_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)      146 2023-04-18 17:50:49.000000 brightest-path-lib-1.0.8/brightest_path_lib.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)       19 2023-04-18 17:50:49.000000 brightest-path-lib-1.0.8/brightest_path_lib.egg-info/top_level.txt
+-rw-r--r--   0 runner     (501) staff       (20)      121 2023-04-18 17:50:00.000000 brightest-path-lib-1.0.8/pyproject.toml
+-rw-r--r--   0 runner     (501) staff       (20)       38 2023-04-18 17:50:50.461671 brightest-path-lib-1.0.8/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)     2568 2023-04-18 17:50:00.000000 brightest-path-lib-1.0.8/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-18 17:50:50.460630 brightest-path-lib-1.0.8/tests/
+-rw-r--r--   0 runner     (501) staff       (20)     4514 2023-04-18 17:50:00.000000 brightest-path-lib-1.0.8/tests/test_astar.py
+-rw-r--r--   0 runner     (501) staff       (20)     1874 2023-04-18 17:50:00.000000 brightest-path-lib-1.0.8/tests/test_bidirectional_node.py
+-rw-r--r--   0 runner     (501) staff       (20)      611 2023-04-18 17:50:00.000000 brightest-path-lib-1.0.8/tests/test_brightest_path_lib.py
+-rw-r--r--   0 runner     (501) staff       (20)     1919 2023-04-18 17:50:00.000000 brightest-path-lib-1.0.8/tests/test_euclidean_heuristic.py
+-rw-r--r--   0 runner     (501) staff       (20)     1586 2023-04-18 17:50:00.000000 brightest-path-lib-1.0.8/tests/test_image_stats.py
+-rw-r--r--   0 runner     (501) staff       (20)     4700 2023-04-18 17:50:00.000000 brightest-path-lib-1.0.8/tests/test_nbastar.py
+-rw-r--r--   0 runner     (501) staff       (20)     1065 2023-04-18 17:50:00.000000 brightest-path-lib-1.0.8/tests/test_node.py
+-rw-r--r--   0 runner     (501) staff       (20)     1591 2023-04-18 17:50:00.000000 brightest-path-lib-1.0.8/tests/test_reciprocal_cost_func.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `brightest-path-lib-1.0.7/LICENSE` & `brightest-path-lib-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `brightest-path-lib-1.0.7/PKG-INFO` & `brightest-path-lib-1.0.8/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brightest-path-lib
-Version: 1.0.7
+Version: 1.0.8
 Summary: A library of path-finding algorithms to find the brightest path between two points.
 Home-page: https://github.com/mapmanager/brightest-path-lib
 Author: Vasudha Jha
 License: GNU General Public License, Version 3
 Project-URL: Issues, https://github.com/mapmanager/brightest-path-lib/issues
 Project-URL: CI, https://github.com/mapmanager/brightest-path-lib/actions
 Project-URL: Changelog, https://github.com/mapmanager/brightest-path-lib/releases
```

### Comparing `brightest-path-lib-1.0.7/README.md` & `brightest-path-lib-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `brightest-path-lib-1.0.7/brightest_path_lib/cost/__pythran__/reciprocal_transonic.cpp` & `brightest-path-lib-1.0.8/brightest_path_lib/cost/__pythran__/reciprocal_transonic.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -298,15 +298,15 @@
 
 
 static PyMethodDef Methods[] = {
     {
     "__for_method__ReciprocalTransonic__minimum_step_cost",
     (PyCFunction)__pythran_wrapall___for_method__ReciprocalTransonic__minimum_step_cost,
     METH_VARARGS | METH_KEYWORDS,
-    "calculates the minimum step cost\n""\n""        Returns\n""        -------\n""        float\n""            the minimum step cost\n""\n""\n""    Supported prototypes:\n""\n""    - __for_method__ReciprocalTransonic__minimum_step_cost(float64)"},{
+    "calculates the minimum step cost\n""\n""    Supported prototypes:\n""\n""    - __for_method__ReciprocalTransonic__minimum_step_cost(float64)\n""\n""        Returns\n""        -------\n""        float\n""            the minimum step cost\n"""},{
     "__for_method__ReciprocalTransonic__cost_of_moving_to",
     (PyCFunction)__pythran_wrapall___for_method__ReciprocalTransonic__cost_of_moving_to,
     METH_VARARGS | METH_KEYWORDS,
     "calculates the cost of moving to a point\n""\n""    Supported prototypes:\n""\n""    - __for_method__ReciprocalTransonic__cost_of_moving_to(float64, float64, float64, float64, float64)\n""\n""        Parameters\n""        ----------\n""        intensity_at_new_point : float\n""            The intensity of the new point under consideration\n""\n""        Returns\n""        -------\n""        float\n""            the cost of moving to the new point\n""\n""        Notes\n""        -----\n""        - To cope with zero intensities, RECIPROCAL_MIN is added to the intensities in the range before reciprocal calculation\n""        - We set the maximum intensity <= RECIPROCAL_MAX so that the intensity is between RECIPROCAL MIN and RECIPROCAL_MAX\n""\n"""},
     {NULL, NULL, 0, NULL}
 };
 
@@ -349,16 +349,16 @@
                                                      ""
                 );
                 #endif
                 if(! theModule)
                     PYTHRAN_RETURN;
                 PyObject * theDoc = Py_BuildValue("(sss)",
                                                   "0.12.1",
-                                                  "2023-04-18 13:44:38.025710",
-                                                  "437594492678aa5480d24b4e8550f8810fb608091fdbb308aa7037a9dc92c24f");
+                                                  "2023-04-18 17:50:50.438816",
+                                                  "837ab9168b906b083b44ff44080768d36d3cd2f0bf45a5bc7adc69f2e573c716");
                 if(! theDoc)
                     PYTHRAN_RETURN;
                 PyModule_AddObject(theModule,
                                    "__pythran__",
                                    theDoc);
 
                 PyModule_AddObject(theModule, "__transonic__", __transonic__);
```

### Comparing `brightest-path-lib-1.0.7/brightest_path_lib/cost/reciprocal_transonic.py` & `brightest-path-lib-1.0.8/brightest_path_lib/cost/reciprocal_transonic.py`

 * *Files identical despite different names*

### Comparing `brightest-path-lib-1.0.7/brightest_path_lib/heuristic/__pythran__/euclidean_transonic.cpp` & `brightest-path-lib-1.0.8/brightest_path_lib/heuristic/__pythran__/euclidean_transonic.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 #include <pythonic/types/int.hpp>
 #ifdef _OPENMP
 #include <omp.h>
 #endif
 #include <pythonic/include/types/ndarray.hpp>
 #include <pythonic/include/types/float64.hpp>
 #include <pythonic/include/types/int64.hpp>
-#include <pythonic/types/int64.hpp>
 #include <pythonic/types/float64.hpp>
 #include <pythonic/types/ndarray.hpp>
+#include <pythonic/types/int64.hpp>
 #include <pythonic/include/builtins/TypeError.hpp>
 #include <pythonic/include/builtins/ValueError.hpp>
 #include <pythonic/include/builtins/len.hpp>
 #include <pythonic/include/builtins/pythran/is_none.hpp>
 #include <pythonic/include/builtins/pythran/or_.hpp>
 #include <pythonic/include/builtins/pythran/static_if.hpp>
 #include <pythonic/include/builtins/tuple.hpp>
@@ -509,16 +509,16 @@
                                                      ""
                 );
                 #endif
                 if(! theModule)
                     PYTHRAN_RETURN;
                 PyObject * theDoc = Py_BuildValue("(sss)",
                                                   "0.12.1",
-                                                  "2023-04-18 13:44:37.900584",
-                                                  "c851a0a3829d72e9a86f3c46e4c833fc15e1ae5d90eab8ca29115df81a059458");
+                                                  "2023-04-18 17:50:50.344238",
+                                                  "c05d11336916ffc5577dc142faff358aeb635b45ebb631a4918a6d5f79c4c890");
                 if(! theDoc)
                     PYTHRAN_RETURN;
                 PyModule_AddObject(theModule,
                                    "__pythran__",
                                    theDoc);
 
                 PyModule_AddObject(theModule, "__transonic__", __transonic__);
```

### Comparing `brightest-path-lib-1.0.7/brightest_path_lib/heuristic/euclidean_transonic.py` & `brightest-path-lib-1.0.8/brightest_path_lib/heuristic/euclidean_transonic.py`

 * *Files identical despite different names*

### Comparing `brightest-path-lib-1.0.7/brightest_path_lib.egg-info/PKG-INFO` & `brightest-path-lib-1.0.8/brightest_path_lib.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brightest-path-lib
-Version: 1.0.7
+Version: 1.0.8
 Summary: A library of path-finding algorithms to find the brightest path between two points.
 Home-page: https://github.com/mapmanager/brightest-path-lib
 Author: Vasudha Jha
 License: GNU General Public License, Version 3
 Project-URL: Issues, https://github.com/mapmanager/brightest-path-lib/issues
 Project-URL: CI, https://github.com/mapmanager/brightest-path-lib/actions
 Project-URL: Changelog, https://github.com/mapmanager/brightest-path-lib/releases
```

### Comparing `brightest-path-lib-1.0.7/brightest_path_lib.egg-info/SOURCES.txt` & `brightest-path-lib-1.0.8/brightest_path_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `brightest-path-lib-1.0.7/setup.py` & `brightest-path-lib-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 import sys
 from transonic.dist import ParallelBuildExt, make_backend_files, init_transonic_extensions
 
 here = Path(__file__).parent.absolute()
 sys.path.insert(0, ".")
 
-VERSION = "1.0.7"
+VERSION = "1.0.8"
 TRANSONIC_BACKEND = "pythran"
 
 build_dependencies_backends = {
     "pythran": ["pythran"],
     "cython": ["cython"],
     "python": [],
     "numba": ["numba"],
```

### Comparing `brightest-path-lib-1.0.7/tests/test_astar.py` & `brightest-path-lib-1.0.8/tests/test_astar.py`

 * *Files identical despite different names*

### Comparing `brightest-path-lib-1.0.7/tests/test_bidirectional_node.py` & `brightest-path-lib-1.0.8/tests/test_bidirectional_node.py`

 * *Files identical despite different names*

### Comparing `brightest-path-lib-1.0.7/tests/test_brightest_path_lib.py` & `brightest-path-lib-1.0.8/tests/test_brightest_path_lib.py`

 * *Files identical despite different names*

### Comparing `brightest-path-lib-1.0.7/tests/test_euclidean_heuristic.py` & `brightest-path-lib-1.0.8/tests/test_euclidean_heuristic.py`

 * *Files identical despite different names*

### Comparing `brightest-path-lib-1.0.7/tests/test_image_stats.py` & `brightest-path-lib-1.0.8/tests/test_image_stats.py`

 * *Files identical despite different names*

### Comparing `brightest-path-lib-1.0.7/tests/test_nbastar.py` & `brightest-path-lib-1.0.8/tests/test_nbastar.py`

 * *Files identical despite different names*

### Comparing `brightest-path-lib-1.0.7/tests/test_node.py` & `brightest-path-lib-1.0.8/tests/test_node.py`

 * *Files identical despite different names*

### Comparing `brightest-path-lib-1.0.7/tests/test_reciprocal_cost_func.py` & `brightest-path-lib-1.0.8/tests/test_reciprocal_cost_func.py`

 * *Files identical despite different names*

