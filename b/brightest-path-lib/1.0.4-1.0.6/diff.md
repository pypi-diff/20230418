# Comparing `tmp/brightest-path-lib-1.0.4.tar.gz` & `tmp/brightest-path-lib-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brightest-path-lib-1.0.4.tar", last modified: Tue Apr 18 05:38:56 2023, max compression
+gzip compressed data, was "brightest-path-lib-1.0.6.tar", last modified: Tue Apr 18 13:37:31 2023, max compression
```

## Comparing `brightest-path-lib-1.0.4.tar` & `brightest-path-lib-1.0.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-18 05:38:56.078734 brightest-path-lib-1.0.4/
--rw-r--r--   0 runner     (501) staff       (20)    35148 2023-04-18 05:38:01.000000 brightest-path-lib-1.0.4/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)      115 2023-04-18 05:38:01.000000 brightest-path-lib-1.0.4/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)      601 2023-04-18 05:38:56.078347 brightest-path-lib-1.0.4/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     1502 2023-04-18 05:38:01.000000 brightest-path-lib-1.0.4/README.md
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-18 05:38:56.066569 brightest-path-lib-1.0.4/brightest_path_lib/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-18 05:38:56.072269 brightest-path-lib-1.0.4/brightest_path_lib/cost/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-18 05:38:56.072737 brightest-path-lib-1.0.4/brightest_path_lib/cost/__pythran__/
--rw-------   0 runner     (501) staff       (20)    19226 2023-04-18 05:38:56.000000 brightest-path-lib-1.0.4/brightest_path_lib/cost/__pythran__/reciprocal_transonic.cpp
--rw-r--r--   0 runner     (501) staff       (20)     2739 2023-04-18 05:38:01.000000 brightest-path-lib-1.0.4/brightest_path_lib/cost/reciprocal_transonic.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-18 05:38:56.073289 brightest-path-lib-1.0.4/brightest_path_lib/heuristic/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-18 05:38:56.073776 brightest-path-lib-1.0.4/brightest_path_lib/heuristic/__pythran__/
--rw-------   0 runner     (501) staff       (20)    34397 2023-04-18 05:38:55.000000 brightest-path-lib-1.0.4/brightest_path_lib/heuristic/__pythran__/euclidean_transonic.cpp
--rw-r--r--   0 runner     (501) staff       (20)     3309 2023-04-18 05:38:01.000000 brightest-path-lib-1.0.4/brightest_path_lib/heuristic/euclidean_transonic.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-18 05:38:56.071804 brightest-path-lib-1.0.4/brightest_path_lib.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)      601 2023-04-18 05:38:55.000000 brightest-path-lib-1.0.4/brightest_path_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)      710 2023-04-18 05:38:56.000000 brightest-path-lib-1.0.4/brightest_path_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2023-04-18 05:38:55.000000 brightest-path-lib-1.0.4/brightest_path_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)      146 2023-04-18 05:38:55.000000 brightest-path-lib-1.0.4/brightest_path_lib.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)       19 2023-04-18 05:38:55.000000 brightest-path-lib-1.0.4/brightest_path_lib.egg-info/top_level.txt
--rw-r--r--   0 runner     (501) staff       (20)      121 2023-04-18 05:38:01.000000 brightest-path-lib-1.0.4/pyproject.toml
--rw-r--r--   0 runner     (501) staff       (20)       38 2023-04-18 05:38:56.078848 brightest-path-lib-1.0.4/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)     2568 2023-04-18 05:38:01.000000 brightest-path-lib-1.0.4/setup.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-18 05:38:56.077767 brightest-path-lib-1.0.4/tests/
--rw-r--r--   0 runner     (501) staff       (20)     4514 2023-04-18 05:38:01.000000 brightest-path-lib-1.0.4/tests/test_astar.py
--rw-r--r--   0 runner     (501) staff       (20)     1874 2023-04-18 05:38:01.000000 brightest-path-lib-1.0.4/tests/test_bidirectional_node.py
--rw-r--r--   0 runner     (501) staff       (20)      611 2023-04-18 05:38:01.000000 brightest-path-lib-1.0.4/tests/test_brightest_path_lib.py
--rw-r--r--   0 runner     (501) staff       (20)     1919 2023-04-18 05:38:01.000000 brightest-path-lib-1.0.4/tests/test_euclidean_heuristic.py
--rw-r--r--   0 runner     (501) staff       (20)     1586 2023-04-18 05:38:01.000000 brightest-path-lib-1.0.4/tests/test_image_stats.py
--rw-r--r--   0 runner     (501) staff       (20)     4700 2023-04-18 05:38:01.000000 brightest-path-lib-1.0.4/tests/test_nbastar.py
--rw-r--r--   0 runner     (501) staff       (20)     1065 2023-04-18 05:38:01.000000 brightest-path-lib-1.0.4/tests/test_node.py
--rw-r--r--   0 runner     (501) staff       (20)     1591 2023-04-18 05:38:01.000000 brightest-path-lib-1.0.4/tests/test_reciprocal_cost_func.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-18 13:37:31.528571 brightest-path-lib-1.0.6/
+-rw-r--r--   0 runner     (501) staff       (20)    35148 2023-04-18 13:36:40.000000 brightest-path-lib-1.0.6/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)      115 2023-04-18 13:36:40.000000 brightest-path-lib-1.0.6/MANIFEST.in
+-rw-r--r--   0 runner     (501) staff       (20)      601 2023-04-18 13:37:31.528118 brightest-path-lib-1.0.6/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     1493 2023-04-18 13:36:40.000000 brightest-path-lib-1.0.6/README.md
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-18 13:37:31.515623 brightest-path-lib-1.0.6/brightest_path_lib/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-18 13:37:31.521641 brightest-path-lib-1.0.6/brightest_path_lib/cost/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-18 13:37:31.522146 brightest-path-lib-1.0.6/brightest_path_lib/cost/__pythran__/
+-rw-------   0 runner     (501) staff       (20)    19226 2023-04-18 13:37:31.000000 brightest-path-lib-1.0.6/brightest_path_lib/cost/__pythran__/reciprocal_transonic.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     2739 2023-04-18 13:36:40.000000 brightest-path-lib-1.0.6/brightest_path_lib/cost/reciprocal_transonic.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-18 13:37:31.522729 brightest-path-lib-1.0.6/brightest_path_lib/heuristic/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-18 13:37:31.523285 brightest-path-lib-1.0.6/brightest_path_lib/heuristic/__pythran__/
+-rw-------   0 runner     (501) staff       (20)    34397 2023-04-18 13:37:31.000000 brightest-path-lib-1.0.6/brightest_path_lib/heuristic/__pythran__/euclidean_transonic.cpp
+-rw-r--r--   0 runner     (501) staff       (20)     3309 2023-04-18 13:36:40.000000 brightest-path-lib-1.0.6/brightest_path_lib/heuristic/euclidean_transonic.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-18 13:37:31.521122 brightest-path-lib-1.0.6/brightest_path_lib.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)      601 2023-04-18 13:37:30.000000 brightest-path-lib-1.0.6/brightest_path_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)      710 2023-04-18 13:37:31.000000 brightest-path-lib-1.0.6/brightest_path_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2023-04-18 13:37:30.000000 brightest-path-lib-1.0.6/brightest_path_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)      146 2023-04-18 13:37:30.000000 brightest-path-lib-1.0.6/brightest_path_lib.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)       19 2023-04-18 13:37:30.000000 brightest-path-lib-1.0.6/brightest_path_lib.egg-info/top_level.txt
+-rw-r--r--   0 runner     (501) staff       (20)      121 2023-04-18 13:36:40.000000 brightest-path-lib-1.0.6/pyproject.toml
+-rw-r--r--   0 runner     (501) staff       (20)       38 2023-04-18 13:37:31.528675 brightest-path-lib-1.0.6/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)     2568 2023-04-18 13:36:40.000000 brightest-path-lib-1.0.6/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-04-18 13:37:31.527528 brightest-path-lib-1.0.6/tests/
+-rw-r--r--   0 runner     (501) staff       (20)     4514 2023-04-18 13:36:40.000000 brightest-path-lib-1.0.6/tests/test_astar.py
+-rw-r--r--   0 runner     (501) staff       (20)     1874 2023-04-18 13:36:40.000000 brightest-path-lib-1.0.6/tests/test_bidirectional_node.py
+-rw-r--r--   0 runner     (501) staff       (20)      611 2023-04-18 13:36:40.000000 brightest-path-lib-1.0.6/tests/test_brightest_path_lib.py
+-rw-r--r--   0 runner     (501) staff       (20)     1919 2023-04-18 13:36:40.000000 brightest-path-lib-1.0.6/tests/test_euclidean_heuristic.py
+-rw-r--r--   0 runner     (501) staff       (20)     1586 2023-04-18 13:36:40.000000 brightest-path-lib-1.0.6/tests/test_image_stats.py
+-rw-r--r--   0 runner     (501) staff       (20)     4700 2023-04-18 13:36:40.000000 brightest-path-lib-1.0.6/tests/test_nbastar.py
+-rw-r--r--   0 runner     (501) staff       (20)     1065 2023-04-18 13:36:40.000000 brightest-path-lib-1.0.6/tests/test_node.py
+-rw-r--r--   0 runner     (501) staff       (20)     1591 2023-04-18 13:36:40.000000 brightest-path-lib-1.0.6/tests/test_reciprocal_cost_func.py
```

### Comparing `brightest-path-lib-1.0.4/LICENSE` & `brightest-path-lib-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `brightest-path-lib-1.0.4/PKG-INFO` & `brightest-path-lib-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brightest-path-lib
-Version: 1.0.4
+Version: 1.0.6
 Summary: A library of path-finding algorithms to find the brightest path between two points.
 Home-page: https://github.com/mapmanager/brightest-path-lib
 Author: Vasudha Jha
 License: GNU General Public License, Version 3
 Project-URL: Issues, https://github.com/mapmanager/brightest-path-lib/issues
 Project-URL: CI, https://github.com/mapmanager/brightest-path-lib/actions
 Project-URL: Changelog, https://github.com/mapmanager/brightest-path-lib/releases
```

### Comparing `brightest-path-lib-1.0.4/README.md` & `brightest-path-lib-1.0.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # brightest-path-lib
 
 [![Python](https://img.shields.io/badge/python-3.7|3.8|3.9|3.10|3.11-blue.svg)](https://www.python.org/downloads/release/python-3111/)
 [![tests](https://github.com/mapmanager/brightest-path-lib/workflows/Test/badge.svg)](https://github.com/mapmanager/brightest-path-lib/actions)
 [![codecov](https://codecov.io/github/mapmanager/brightest-path-lib/branch/main/graph/badge.svg?token=0ZR226588I)](https://codecov.io/github/mapmanager/brightest-path-lib)
 [![OS](https://img.shields.io/badge/OS-Linux|Windows|macOS-blue.svg)]()
 [![License](https://img.shields.io/badge/license-GPLv3-blue)](https://github.com/mapmanager/brightest-path-lib/blob/main/LICENSE)
-<!-- [![PyPI](https://img.shields.io/pypi/v/brightest-path-lib.svg)](https://pypi.org/project/brightest-path-lib/) -->
+[![PyPI](https://img.shields.io/pypi/v/brightest-path-lib.svg)](https://pypi.org/project/brightest-path-lib/)
 <!-- [![Changelog](https://img.shields.io/github/v/release/mapmanager/brightest-path-lib?include_prereleases&label=changelog)](https://github.com/mapmanager/brightest-path-lib/releases) -->
 
 A library of path-finding algorithms to find the brightest path between two points.
 
 ## Installation
 
 Install this library using `pip`:
```

### Comparing `brightest-path-lib-1.0.4/brightest_path_lib/cost/__pythran__/reciprocal_transonic.cpp` & `brightest-path-lib-1.0.6/brightest_path_lib/cost/__pythran__/reciprocal_transonic.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -349,15 +349,15 @@
                                                      ""
                 );
                 #endif
                 if(! theModule)
                     PYTHRAN_RETURN;
                 PyObject * theDoc = Py_BuildValue("(sss)",
                                                   "0.12.1",
-                                                  "2023-04-18 05:38:56.055066",
+                                                  "2023-04-18 13:37:31.504770",
                                                   "837ab9168b906b083b44ff44080768d36d3cd2f0bf45a5bc7adc69f2e573c716");
                 if(! theDoc)
                     PYTHRAN_RETURN;
                 PyModule_AddObject(theModule,
                                    "__pythran__",
                                    theDoc);
```

### Comparing `brightest-path-lib-1.0.4/brightest_path_lib/cost/reciprocal_transonic.py` & `brightest-path-lib-1.0.6/brightest_path_lib/cost/reciprocal_transonic.py`

 * *Files identical despite different names*

### Comparing `brightest-path-lib-1.0.4/brightest_path_lib/heuristic/__pythran__/euclidean_transonic.cpp` & `brightest-path-lib-1.0.6/brightest_path_lib/heuristic/__pythran__/euclidean_transonic.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #include <pythonic/core.hpp>
 #include <pythonic/python/core.hpp>
 #include <pythonic/types/bool.hpp>
 #include <pythonic/types/int.hpp>
 #ifdef _OPENMP
 #include <omp.h>
 #endif
-#include <pythonic/include/types/float64.hpp>
 #include <pythonic/include/types/ndarray.hpp>
 #include <pythonic/include/types/int64.hpp>
-#include <pythonic/types/int64.hpp>
+#include <pythonic/include/types/float64.hpp>
 #include <pythonic/types/float64.hpp>
+#include <pythonic/types/int64.hpp>
 #include <pythonic/types/ndarray.hpp>
 #include <pythonic/include/builtins/TypeError.hpp>
 #include <pythonic/include/builtins/ValueError.hpp>
 #include <pythonic/include/builtins/len.hpp>
 #include <pythonic/include/builtins/pythran/is_none.hpp>
 #include <pythonic/include/builtins/pythran/or_.hpp>
 #include <pythonic/include/builtins/pythran/static_if.hpp>
@@ -509,16 +509,16 @@
                                                      ""
                 );
                 #endif
                 if(! theModule)
                     PYTHRAN_RETURN;
                 PyObject * theDoc = Py_BuildValue("(sss)",
                                                   "0.12.1",
-                                                  "2023-04-18 05:38:55.932951",
-                                                  "382fe1c27a9cbb319156cd007f8ecb665ae3896e0c8d0815a4d13005e11057e4");
+                                                  "2023-04-18 13:37:31.411785",
+                                                  "c05d11336916ffc5577dc142faff358aeb635b45ebb631a4918a6d5f79c4c890");
                 if(! theDoc)
                     PYTHRAN_RETURN;
                 PyModule_AddObject(theModule,
                                    "__pythran__",
                                    theDoc);
 
                 PyModule_AddObject(theModule, "__transonic__", __transonic__);
```

### Comparing `brightest-path-lib-1.0.4/brightest_path_lib/heuristic/euclidean_transonic.py` & `brightest-path-lib-1.0.6/brightest_path_lib/heuristic/euclidean_transonic.py`

 * *Files identical despite different names*

### Comparing `brightest-path-lib-1.0.4/brightest_path_lib.egg-info/PKG-INFO` & `brightest-path-lib-1.0.6/brightest_path_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brightest-path-lib
-Version: 1.0.4
+Version: 1.0.6
 Summary: A library of path-finding algorithms to find the brightest path between two points.
 Home-page: https://github.com/mapmanager/brightest-path-lib
 Author: Vasudha Jha
 License: GNU General Public License, Version 3
 Project-URL: Issues, https://github.com/mapmanager/brightest-path-lib/issues
 Project-URL: CI, https://github.com/mapmanager/brightest-path-lib/actions
 Project-URL: Changelog, https://github.com/mapmanager/brightest-path-lib/releases
```

### Comparing `brightest-path-lib-1.0.4/brightest_path_lib.egg-info/SOURCES.txt` & `brightest-path-lib-1.0.6/brightest_path_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `brightest-path-lib-1.0.4/setup.py` & `brightest-path-lib-1.0.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 import sys
 from transonic.dist import ParallelBuildExt, make_backend_files, init_transonic_extensions
 
 here = Path(__file__).parent.absolute()
 sys.path.insert(0, ".")
 
-VERSION = "1.0.4"
+VERSION = "1.0.6"
 TRANSONIC_BACKEND = "pythran"
 
 build_dependencies_backends = {
     "pythran": ["pythran"],
     "cython": ["cython"],
     "python": [],
     "numba": ["numba"],
```

### Comparing `brightest-path-lib-1.0.4/tests/test_astar.py` & `brightest-path-lib-1.0.6/tests/test_astar.py`

 * *Files identical despite different names*

### Comparing `brightest-path-lib-1.0.4/tests/test_bidirectional_node.py` & `brightest-path-lib-1.0.6/tests/test_bidirectional_node.py`

 * *Files identical despite different names*

### Comparing `brightest-path-lib-1.0.4/tests/test_brightest_path_lib.py` & `brightest-path-lib-1.0.6/tests/test_brightest_path_lib.py`

 * *Files identical despite different names*

### Comparing `brightest-path-lib-1.0.4/tests/test_euclidean_heuristic.py` & `brightest-path-lib-1.0.6/tests/test_euclidean_heuristic.py`

 * *Files identical despite different names*

### Comparing `brightest-path-lib-1.0.4/tests/test_image_stats.py` & `brightest-path-lib-1.0.6/tests/test_image_stats.py`

 * *Files identical despite different names*

### Comparing `brightest-path-lib-1.0.4/tests/test_nbastar.py` & `brightest-path-lib-1.0.6/tests/test_nbastar.py`

 * *Files identical despite different names*

### Comparing `brightest-path-lib-1.0.4/tests/test_node.py` & `brightest-path-lib-1.0.6/tests/test_node.py`

 * *Files identical despite different names*

### Comparing `brightest-path-lib-1.0.4/tests/test_reciprocal_cost_func.py` & `brightest-path-lib-1.0.6/tests/test_reciprocal_cost_func.py`

 * *Files identical despite different names*

