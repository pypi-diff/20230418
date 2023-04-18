# Comparing `tmp/judo-0.0.8.tar.gz` & `tmp/judo-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "judo-0.0.8.tar", last modified: Mon Nov 29 12:41:29 2021, max compression
+gzip compressed data, was "judo-0.0.9.tar", last modified: Tue Nov 30 16:05:06 2021, max compression
```

## Comparing `judo-0.0.8.tar` & `judo-0.0.9.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-29 12:41:29.494722 judo-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1075 2021-11-29 12:41:17.000000 judo-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1584 2021-11-29 12:41:29.494722 judo-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      886 2021-11-29 12:41:17.000000 judo-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-29 12:41:29.486722 judo-0.0.8/judo/
--rw-r--r--   0 runner    (1001) docker     (121)     1489 2021-11-29 12:41:17.000000 judo-0.0.8/judo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       76 2021-11-29 12:41:17.000000 judo-0.0.8/judo/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-29 12:41:29.490722 judo-0.0.8/judo/data_structures/
--rw-r--r--   0 runner    (1001) docker     (121)      197 2021-11-29 12:41:17.000000 judo-0.0.8/judo/data_structures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11246 2021-11-29 12:41:17.000000 judo-0.0.8/judo/data_structures/bounds.py
--rw-r--r--   0 runner    (1001) docker     (121)     4222 2021-11-29 12:41:17.000000 judo-0.0.8/judo/data_structures/memory.py
--rw-r--r--   0 runner    (1001) docker     (121)    12503 2021-11-29 12:41:17.000000 judo-0.0.8/judo/data_structures/states.py
--rw-r--r--   0 runner    (1001) docker     (121)    29153 2021-11-29 12:41:17.000000 judo-0.0.8/judo/data_structures/tree.py
--rw-r--r--   0 runner    (1001) docker     (121)     3969 2021-11-29 12:41:17.000000 judo-0.0.8/judo/data_types.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-29 12:41:29.494722 judo-0.0.8/judo/functions/
--rw-r--r--   0 runner    (1001) docker     (121)      248 2021-11-29 12:41:17.000000 judo-0.0.8/judo/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1413 2021-11-29 12:41:17.000000 judo-0.0.8/judo/functions/api.py
--rw-r--r--   0 runner    (1001) docker     (121)     3010 2021-11-29 12:41:17.000000 judo-0.0.8/judo/functions/batching.py
--rw-r--r--   0 runner    (1001) docker     (121)     7222 2021-11-29 12:41:17.000000 judo-0.0.8/judo/functions/fractalai.py
--rw-r--r--   0 runner    (1001) docker     (121)     2092 2021-11-29 12:41:17.000000 judo-0.0.8/judo/functions/hashing.py
--rw-r--r--   0 runner    (1001) docker     (121)      818 2021-11-29 12:41:17.000000 judo-0.0.8/judo/functions/images.py
--rw-r--r--   0 runner    (1001) docker     (121)      792 2021-11-29 12:41:17.000000 judo-0.0.8/judo/functions/notebook.py
--rw-r--r--   0 runner    (1001) docker     (121)     1690 2021-11-29 12:41:17.000000 judo-0.0.8/judo/functions/numpy.py
--rw-r--r--   0 runner    (1001) docker     (121)     3013 2021-11-29 12:41:17.000000 judo-0.0.8/judo/functions/pytorch.py
--rw-r--r--   0 runner    (1001) docker     (121)     3090 2021-11-29 12:41:17.000000 judo-0.0.8/judo/functions/random.py
--rw-r--r--   0 runner    (1001) docker     (121)     6968 2021-11-29 12:41:17.000000 judo-0.0.8/judo/judo_backend.py
--rw-r--r--   0 runner    (1001) docker     (121)     6673 2021-11-29 12:41:17.000000 judo-0.0.8/judo/judo_tensor.py
--rw-r--r--   0 runner    (1001) docker     (121)      506 2021-11-29 12:41:17.000000 judo-0.0.8/judo/typing.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-11-29 12:41:17.000000 judo-0.0.8/judo/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-29 12:41:29.486722 judo-0.0.8/judo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1584 2021-11-29 12:41:29.000000 judo-0.0.8/judo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      947 2021-11-29 12:41:29.000000 judo-0.0.8/judo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-29 12:41:29.000000 judo-0.0.8/judo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       98 2021-11-29 12:41:29.000000 judo-0.0.8/judo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2021-11-29 12:41:29.000000 judo-0.0.8/judo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2337 2021-11-29 12:41:17.000000 judo-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-29 12:41:29.494722 judo-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1569 2021-11-29 12:41:17.000000 judo-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-29 12:41:29.494722 judo-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-29 12:41:17.000000 judo-0.0.8/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-29 12:41:29.494722 judo-0.0.8/tests/functions/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-29 12:41:17.000000 judo-0.0.8/tests/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      960 2021-11-29 12:41:17.000000 judo-0.0.8/tests/functions/test_images.py
--rw-r--r--   0 runner    (1001) docker     (121)      161 2021-11-29 12:41:17.000000 judo-0.0.8/tests/functions/test_notebook.py
--rw-r--r--   0 runner    (1001) docker     (121)      234 2021-11-29 12:41:17.000000 judo-0.0.8/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (121)      728 2021-11-29 12:41:17.000000 judo-0.0.8/tests/test_backend.py
--rw-r--r--   0 runner    (1001) docker     (121)     8463 2021-11-29 12:41:17.000000 judo-0.0.8/tests/test_bounds.py
--rw-r--r--   0 runner    (1001) docker     (121)     4689 2021-11-29 12:41:17.000000 judo-0.0.8/tests/test_states.py
--rw-r--r--   0 runner    (1001) docker     (121)     4205 2021-11-29 12:41:17.000000 judo-0.0.8/tests/test_tree.py
--rw-r--r--   0 runner    (1001) docker     (121)      353 2021-11-29 12:41:17.000000 judo-0.0.8/tests/test_types.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 16:05:06.911084 judo-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1075 2021-11-30 16:04:56.000000 judo-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     1754 2021-11-30 16:05:06.911084 judo-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      886 2021-11-30 16:04:56.000000 judo-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 16:05:06.911084 judo-0.0.9/judo/
+-rw-r--r--   0 runner    (1001) docker     (121)     1610 2021-11-30 16:04:56.000000 judo-0.0.9/judo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       76 2021-11-30 16:04:56.000000 judo-0.0.9/judo/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 16:05:06.911084 judo-0.0.9/judo/data_structures/
+-rw-r--r--   0 runner    (1001) docker     (121)      251 2021-11-30 16:04:56.000000 judo-0.0.9/judo/data_structures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11298 2021-11-30 16:04:56.000000 judo-0.0.9/judo/data_structures/bounds.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4222 2021-11-30 16:04:56.000000 judo-0.0.9/judo/data_structures/memory.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12515 2021-11-30 16:04:56.000000 judo-0.0.9/judo/data_structures/states.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29545 2021-11-30 16:04:56.000000 judo-0.0.9/judo/data_structures/tree.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3970 2021-11-30 16:04:56.000000 judo-0.0.9/judo/data_types.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 16:05:06.911084 judo-0.0.9/judo/functions/
+-rw-r--r--   0 runner    (1001) docker     (121)      248 2021-11-30 16:04:56.000000 judo-0.0.9/judo/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1413 2021-11-30 16:04:56.000000 judo-0.0.9/judo/functions/api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3010 2021-11-30 16:04:56.000000 judo-0.0.9/judo/functions/batching.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7222 2021-11-30 16:04:56.000000 judo-0.0.9/judo/functions/fractalai.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1604 2021-11-30 16:04:56.000000 judo-0.0.9/judo/functions/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (121)      818 2021-11-30 16:04:56.000000 judo-0.0.9/judo/functions/images.py
+-rw-r--r--   0 runner    (1001) docker     (121)      792 2021-11-30 16:04:56.000000 judo-0.0.9/judo/functions/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2203 2021-11-30 16:04:56.000000 judo-0.0.9/judo/functions/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3526 2021-11-30 16:04:56.000000 judo-0.0.9/judo/functions/pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3090 2021-11-30 16:04:56.000000 judo-0.0.9/judo/functions/random.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6968 2021-11-30 16:04:56.000000 judo-0.0.9/judo/judo_backend.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6673 2021-11-30 16:04:56.000000 judo-0.0.9/judo/judo_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (121)      506 2021-11-30 16:04:56.000000 judo-0.0.9/judo/typing.py
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2021-11-30 16:04:56.000000 judo-0.0.9/judo/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 16:05:06.911084 judo-0.0.9/judo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1754 2021-11-30 16:05:06.000000 judo-0.0.9/judo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      947 2021-11-30 16:05:06.000000 judo-0.0.9/judo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-30 16:05:06.000000 judo-0.0.9/judo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      210 2021-11-30 16:05:06.000000 judo-0.0.9/judo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       11 2021-11-30 16:05:06.000000 judo-0.0.9/judo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2337 2021-11-30 16:04:56.000000 judo-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-30 16:05:06.911084 judo-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1805 2021-11-30 16:04:56.000000 judo-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 16:05:06.911084 judo-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-30 16:04:56.000000 judo-0.0.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-30 16:05:06.911084 judo-0.0.9/tests/functions/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-30 16:04:56.000000 judo-0.0.9/tests/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      996 2021-11-30 16:04:56.000000 judo-0.0.9/tests/functions/test_images.py
+-rw-r--r--   0 runner    (1001) docker     (121)      441 2021-11-30 16:04:56.000000 judo-0.0.9/tests/functions/test_notebook.py
+-rw-r--r--   0 runner    (1001) docker     (121)      225 2021-11-30 16:04:56.000000 judo-0.0.9/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)      728 2021-11-30 16:04:56.000000 judo-0.0.9/tests/test_backend.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8503 2021-11-30 16:04:56.000000 judo-0.0.9/tests/test_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4724 2021-11-30 16:04:56.000000 judo-0.0.9/tests/test_states.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4389 2021-11-30 16:04:56.000000 judo-0.0.9/tests/test_tree.py
+-rw-r--r--   0 runner    (1001) docker     (121)      593 2021-11-30 16:04:56.000000 judo-0.0.9/tests/test_types.py
```

### Comparing `judo-0.0.8/LICENSE` & `judo-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `judo-0.0.8/PKG-INFO` & `judo-0.0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 Metadata-Version: 2.1
 Name: judo
-Version: 0.0.8
+Version: 0.0.9
 Summary: API and data structures for efficient AI research.
 Home-page: https://github.com/FragileTech/judo
 Author: FragileTech
 Author-email: info@fragile.tech
 License: MIT
 Keywords: Machine learning,artificial intelligence
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/markdown
+Provides-Extra: torch
+Provides-Extra: image
+Provides-Extra: ipython
+Provides-Extra: data-structures
+Provides-Extra: all
 License-File: LICENSE
 
 # judo
 [![Travis build status](https://travis-ci.com/fragiletech/judo.svg)](https://travis-ci.com/fragiletech/judo)
 [![Documentation Status](https://readthedocs.org/projects/fragile/badge/?version=latest)](https://judo.readthedocs.io/en/latest/?badge=latest)
 [![Code coverage](https://codecov.io/github/fragiletech/judo/coverage.svg)](https://codecov.io/github/fragiletech/judo)
 [![PyPI package](https://badgen.net/pypi/v/judo)](https://pypi.org/project/judo/)
```

### Comparing `judo-0.0.8/README.md` & `judo-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `judo-0.0.8/judo/__init__.py` & `judo-0.0.9/judo/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -40,14 +40,16 @@
             return __backend_wrap(val) if callable(val) else val
         elif Backend.is_torch():
             val = getattr(torch, name)
             return __backend_wrap(val) if callable(val) else val
         raise e
 
 
+# In python versions 3.7 + you don't need to import dtype,
+# and calling judo.float64 instead of dtype.float64 will work
 module = sys.modules[__name__]
 __old_getattr = getattr(module, "__getattr__", __base_getattr)
 module.__getattr__ = __new_getattr
 is_bool = dtype.is_bool
 is_int = dtype.is_int
 is_float = dtype.is_float
 is_tensor = dtype.is_tensor
```

### Comparing `judo-0.0.8/judo/data_structures/bounds.py` & `judo-0.0.9/judo/data_structures/bounds.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from collections.abc import Iterable as _Iterable
 from typing import Iterable, Optional, Tuple, Union
 
 import numpy
 
 import judo
+from judo.data_types import dtype
+from judo.functions.api import API
 from judo.judo_tensor import tensor
 from judo.typing import Scalar, Tensor
 
 
 class Bounds:
     """
     The :class:`Bounds` implements the logic for defining and managing closed intervals, \
@@ -63,19 +65,19 @@
             shape = high.shape
         elif shape is None and hasattr(low, "shape"):
             shape = low.shape
         elif shape is None:
             raise TypeError("If shape is None high or low need to have .shape attribute.")
         # High and low will be arrays of target shape
         if not judo.is_tensor(high):
-            high = tensor(high) if isinstance(high, _Iterable) else judo.ones(shape) * high
+            high = tensor(high) if isinstance(high, _Iterable) else API.ones(shape) * high
         if not judo.is_tensor(low):
-            low = tensor(low) if isinstance(low, _Iterable) else judo.ones(shape) * low
-        self.high = judo.astype(high, judo.float)
-        self.low = judo.astype(low, judo.float)
+            low = tensor(low) if isinstance(low, _Iterable) else API.ones(shape) * low
+        self.high = judo.astype(high, dtype)
+        self.low = judo.astype(low, dtype)
         if dtype is not None:
             self.dtype = dtype
         elif hasattr(high, "dtype"):
             self.dtype = high.dtype
         elif hasattr(low, "dtype"):
             self.dtype = low.dtype
         else:
@@ -125,15 +127,15 @@
             Bounds shape int64 dtype (3,) low [-1 -2  2] high [1 1 3]
 
         """
         low, high = [], []
         for lo, hi in bounds:
             low.append(lo)
             high.append(hi)
-        low, high = tensor(low, dtype=judo.float), tensor(high, dtype=judo.float)
+        low, high = tensor(low, dtype=dtype.float), tensor(high, dtype=dtype.float)
         return Bounds(low=low, high=high)
 
     @staticmethod
     def get_scaled_intervals(
         low: Union[Tensor, float, int],
         high: Union[Tensor, float, int],
         scale: float,
@@ -155,23 +157,23 @@
             minimum values of the array.
 
         Returns:
             :class:`Bounds` instance.
 
         """
         pct = tensor(scale - 1)
-        big_scale = 1 + judo.abs(pct)
-        small_scale = 1 - judo.abs(pct)
+        big_scale = 1 + API.abs(pct)
+        small_scale = 1 - API.abs(pct)
         zero = judo.astype(tensor(0.0), low.dtype)
         if pct > 0:
-            xmin_scaled = judo.where(low < zero, low * big_scale, low * small_scale)
-            xmax_scaled = judo.where(high < zero, high * small_scale, high * big_scale)
+            xmin_scaled = API.where(low < zero, low * big_scale, low * small_scale)
+            xmax_scaled = API.where(high < zero, high * small_scale, high * big_scale)
         else:
-            xmin_scaled = judo.where(low < zero, low * small_scale, low * small_scale)
-            xmax_scaled = judo.where(high < zero, high * big_scale, high * small_scale)
+            xmin_scaled = API.where(low < zero, low * small_scale, low * small_scale)
+            xmax_scaled = API.where(high < zero, high * big_scale, high * small_scale)
         return xmin_scaled, xmax_scaled
 
     @classmethod
     def from_array(cls, x: Tensor, scale: float = 1.0) -> "Bounds":
         """
         Instantiate a bounds compatible for bounding the given array. It also allows to set a \
         margin for the high and low values.
@@ -196,30 +198,30 @@
             >>> x = numpy.ones((3, 3))
             >>> x[1:-1, 1:-1] = -5
             >>> bounds = Bounds.from_array(x, scale=1.5)
             >>> print(bounds)
             Bounds shape float64 dtype (3,) low [ 0.5 -7.5  0.5] high [1.5 1.5 1.5]
 
         """
-        xmin, xmax = judo.min(x, axis=0), judo.max(x, axis=0)
+        xmin, xmax = API.min(x, axis=0), API.max(x, axis=0)
         xmin_scaled, xmax_scaled = cls.get_scaled_intervals(xmin, xmax, scale)
         return Bounds(low=xmin_scaled, high=xmax_scaled)
 
     def clip(self, x: Tensor) -> Tensor:
         """
         Clip the values of the target array to fall inside the bounds (closed interval).
 
         Args:
             x: Numpy array to be clipped.
 
         Returns:
             Clipped numpy array with all its values inside the defined bounds.
 
         """
-        return judo.clip(judo.astype(x, judo.float), self.low, self.high)
+        return API.clip(judo.astype(x, dtype.float), self.low, self.high)
 
     def points_in_bounds(self, x: Tensor) -> Union[Tensor, bool]:
         """
         Check if the rows of the target array have all their coordinates inside \
         specified bounds.
 
         If the array is one dimensional it will return a boolean, otherwise a vector of booleans.
@@ -227,15 +229,15 @@
         Args:
             x: Array to be checked against the bounds.
 
         Returns:
             Numpy array of booleans indicating if a row lies inside the bounds.
 
         """
-        match = self.clip(x) == judo.astype(x, judo.float)
+        match = self.clip(x) == judo.astype(x, dtype.float)
         return match.all(1).flatten() if len(match.shape) > 1 else match.all()
 
     def safe_margin(
         self,
         low: Union[Tensor, Scalar] = None,
         high: Optional[Union[Tensor, Scalar]] = None,
         scale: float = 1.0,
```

### Comparing `judo-0.0.8/judo/data_structures/memory.py` & `judo-0.0.9/judo/data_structures/memory.py`

 * *Files identical despite different names*

### Comparing `judo-0.0.8/judo/data_structures/states.py` & `judo-0.0.9/judo/data_structures/states.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import copy
 from typing import Dict, Generator, Iterable, List, Optional, Tuple, Union
 
 import numpy
 
 import judo
+from judo.functions.api import API
 from judo.functions.hashing import hasher
 from judo.judo_tensor import tensor
 from judo.typing import StateDict, Tensor
 
 
 class States:
     """
@@ -85,17 +86,15 @@
                     item,
                     type(item),
                 ),
             )
 
     def _ix(self, index: int):
         # TODO(guillemdb): Allow slicing
-        data = {
-            k: judo.unsqueeze(v[index], 0) if judo.is_tensor(v) else v for k, v in self.items()
-        }
+        data = {k: API.unsqueeze(v[index], 0) if judo.is_tensor(v) else v for k, v in self.items()}
         return self.__class__(batch_size=1, **data)
 
     def __setitem__(self, key, value: Union[Tuple, List, Tensor]):
         """
         Allow the class to set its attributes as if it was a dict.
 
         Args:
@@ -121,17 +120,17 @@
     def __hash__(self) -> int:
         return hasher.hash_state(self)
 
     def group_hash(self, name: str) -> int:
         """Return a unique id for a given attribute."""
         return hasher.hash_tensor(self[name])
 
-    def hash_walkers(self, name: str) -> List[int]:
+    def hash_attribute(self, name: str) -> List[int]:
         """Return a unique id for each walker attribute."""
-        return hasher.hash_walkers(self[name])
+        return hasher.hash_iterable(self[name])
 
     @staticmethod
     def merge_states(states: Iterable["States"]) -> "States":
         """
         Combine different states containing the same kind of data into a single \
         :class:`State` with batch size equal to the sum of all the state batch \
         sizes.
@@ -175,15 +174,15 @@
                     value = data
                 else:
                     raise ValueError(
                         "Could not infer data concatenation for attribute %s  with shape %s"
                         % (name, data.shape),
                     )
                 vals.append(value)
-            return judo.concatenate(vals)
+            return API.concatenate(vals)
 
         # Assumes all states have the same names.
         data = {name: merge_one_name(states, name) for name in states[0]._names}
         batch_size = sum(s.n for s in states)
         return states[0].__class__(batch_size=batch_size, **data)
 
     @property
@@ -259,15 +258,15 @@
         def get_chunck_size(state, start, end):
             for name in state._names:
                 attr = state[name]
                 if judo.is_tensor(attr):
                     return len(attr[start:end])
             return int(numpy.ceil(self.n / n_chunks))
 
-        for start, end in judo.similiar_chunks_indexes(self.n, n_chunks):
+        for start, end in API.similiar_chunks_indexes(self.n, n_chunks):
             chunk_size = get_chunck_size(self, start, end)
             data = {k: val[start:end] if judo.is_tensor(val) else val for k, val in self.items()}
             new_state = self.__class__(batch_size=chunk_size, **data)
             yield new_state
 
     def update(self, other: "States" = None, **kwargs):
         """
@@ -333,9 +332,9 @@
                 val_size = val.get("size")
             # Create appropriate shapes with current state's number of walkers.
             sizes = n_walkers if val_size is None else tuple([n_walkers]) + val_size
             if "size" in val:
                 del val["size"]
             if "shape" in val:
                 del val["shape"]
-            tensor_dict[key] = judo.zeros(sizes, **val)
+            tensor_dict[key] = API.zeros(sizes, **val)
         return tensor_dict
```

### Comparing `judo-0.0.8/judo/data_structures/tree.py` & `judo-0.0.9/judo/data_structures/tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,14 +145,15 @@
             if name.lstrip(next_prefix) in node_names
         ]
         self.edge_names = [
             name.lstrip(next_prefix)
             for name in self.names
             if name.lstrip(next_prefix) in edge_names
         ]
+        self._prune_sentinel = self.root_id
 
     def __len__(self) -> int:
         return self._node_count
 
     def __repr__(self) -> str:
         string = "%s \n" "Nodes: %s Leafs: %s " % (
             self.__class__.__name__,
@@ -184,19 +185,15 @@
             kwargs: Keyword arguments representing different :class:`States` instances.
 
         Returns:
             None
 
         """
         ids, id_states = self.get_states_ids(**kwargs)
-        if hasher.uses_true_hash:
-            leaf_ids = judo.to_numpy(ids)
-        else:
-            leaf_ids = hasher.get_array_of_ids(len(id_states))
-        parent_ids = judo.to_numpy(parent_ids)
+        leaf_ids, parent_ids = judo.to_numpy(ids), judo.to_numpy(parent_ids)
         # Keep track of nodes that are active to make sure that they are not pruned
         self.last_added = set(leaf_ids) | set(parent_ids)
         for i, (leaf, parent) in enumerate(zip(leaf_ids, parent_ids)):
             node_data, edge_data = self._extract_data_from_states(index=i, **kwargs)
             self.append_leaf(
                 leaf_id=leaf,
                 parent_id=parent,
@@ -219,14 +216,15 @@
             None.
 
         """
         if self.prune:
             alive_leafs = set(alive_leafs)
             dead_leafs = self.leafs - alive_leafs
             self.prune_dead_branches(dead_leafs=dead_leafs, alive_leafs=alive_leafs)
+        # self._update_prune_sentinel()
 
     def reset_graph(
         self,
         node_data: Dict[str, Any],
         root_id: NodeId = None,
         epoch: int = -1,
     ) -> None:
@@ -246,14 +244,15 @@
         Returns:
             None.
 
         """
         self.root_id = to_node_id(root_id) if root_id is not None else self.root_id
         self.data: nx.DiGraph = nx.DiGraph()
         self.data.add_node(self.root_id, epoch=epoch, **node_data)
+        self._prune_sentinel = self.root_id
         self._node_count = 1
         self.leafs = {self.root_id}
         self.last_added = set()
 
     def append_leaf(
         self,
         leaf_id: NodeId,
@@ -285,15 +284,17 @@
         Returns:
             None.
 
         """
         # Don't add any leaf that creates a cycle in the graph
         if leaf_id not in self.data.nodes:
             if parent_id not in self.data.nodes:
-                raise ValueError("Parent not in graph")
+                raise ValueError(
+                    f"Parent {parent_id} of leaf {leaf_id} not in graph.",
+                )
             import copy
 
             self.data.add_node(leaf_id, epoch=epoch, **copy.deepcopy(node_data))
             self.data.add_edge(parent_id, leaf_id, **copy.deepcopy(edge_data))
             # self.data.add_node(leaf_id, epoch=epoch, **node_data)
             # self.data.add_edge(parent_id, leaf_id, **edge_data)
             self.leafs.add(leaf_id)
@@ -339,15 +340,15 @@
 
         Returns:
             None
 
         """
         leaf_id = to_node_id(leaf_id)
         if (
-            leaf_id == self.root_id
+            leaf_id == self._prune_sentinel
             or leaf_id in alive_nodes  # Remove only old nodes (inserted for 2+ epochs)
             or len(self.data.out_edges([leaf_id])) > 0  # Has children -> It's not a leaf
         ):
             return
         parent = self.get_parent(leaf_id)
         if parent in alive_nodes:
             return
@@ -426,14 +427,20 @@
 
         Returns:
             None
 
         """
         self.data = nx.compose(self.data, other.data)
 
+    def _update_prune_sentinel(self):
+        children_edges = self.data.out_edges([self._prune_sentinel])
+        while len(children_edges) == 1:
+            self._prune_sentinel = tuple(children_edges)[0][1]  # Update to child node
+            children_edges = self.data.out_edges([self._prune_sentinel])
+
     def _extract_data_from_states(
         self,
         index,
         env_states,
         model_states,
         walkers_states,
         only_node_data: bool = False,
```

### Comparing `judo-0.0.8/judo/data_types.py` & `judo-0.0.9/judo/data_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 def float64():
     funcs = {"numpy": lambda x: numpy.float64, "torch": lambda x: torch.float64}
     return Backend.execute(None, funcs)
 
 
 def hash_type():
     funcs = {
-        "numpy": lambda x: numpy.dtype("<U64") if Backend.use_true_hash() else numpy.int64,
+        "numpy": lambda x: numpy.dtype("<U64") if Backend.use_true_hash() else numpy.uint64,
         "torch": lambda x: torch.int64,
     }
     return Backend.execute(None, funcs)
 
 
 class MetaScalar(type):
     @property
```

### Comparing `judo-0.0.8/judo/functions/api.py` & `judo-0.0.9/judo/functions/api.py`

 * *Files identical despite different names*

### Comparing `judo-0.0.8/judo/functions/batching.py` & `judo-0.0.9/judo/functions/batching.py`

 * *Files identical despite different names*

### Comparing `judo-0.0.8/judo/functions/fractalai.py` & `judo-0.0.9/judo/functions/fractalai.py`

 * *Files identical despite different names*

### Comparing `judo-0.0.8/judo/functions/hashing.py` & `judo-0.0.9/judo/functions/hashing.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,83 +1,64 @@
-try:
-    from torch.multiprocessing.pool import Pool
-except ImportError:
-    from multiprocessing.pool import Pool
+import uuid
 
 import numpy
 import xxhash
 
 import judo
 from judo.judo_backend import Backend
 
 
 class Hasher:
-
-    _true_hash = bool(Backend.use_true_hash())
-
     def __init__(self, seed: int = 0):
         self._seed = seed
-        if self._true_hash:
-            self.pool = Pool()
 
     @property
     def uses_true_hash(self) -> bool:
-        return self._true_hash
+        return Backend.use_true_hash()
 
     @staticmethod
     def hash_numpy(x: numpy.ndarray) -> int:
         """Return a value that uniquely identifies a numpy array."""
         x = x.astype("|S576") if x.dtype == "O" else x
         return xxhash.xxh64_hexdigest(x.tobytes())
 
     @staticmethod
     def hash_torch(x):
         bytes = judo.to_numpy(x).tobytes()
         return xxhash.xxh32_intdigest(bytes)
 
+    @staticmethod
+    def get_one_id():
+        return uuid.uuid1().int >> 64
+
     @classmethod
     def true_hash_tensor(cls, x):
         funcs = {
             "numpy": cls.hash_numpy,
             "torch": cls.hash_torch,
         }
         return Backend.execute(x, funcs)
 
-    def __del__(self):
-        self.pool.close()
-
-    def get_one_id(self):
-        self._seed += 1
-        return self._seed
-
-    def get_array_of_ids(self, n: int):
-        ids = numpy.arange(n) + self._seed + 1
-        self._seed += n + 1
-        return judo.as_tensor(ids)
-
     def hash_tensor(self, x):
-        if self._true_hash:
+        if self.uses_true_hash:
             return self.true_hash_tensor(x)
-        return 0
+        return self.get_one_id()
 
-    def hash_walkers(self, x):
-        if self._true_hash:
-            # hashes = self.pool.map(self.true_hash_tensor, x)
-            hashes = [self.true_hash_tensor(x_i) for x_i in x]
-            return judo.as_tensor(hashes)
-        return self.get_array_of_ids(x.shape[0])
+    def hash_iterable(self, x):
+        hashes = [self.hash_tensor(xi) for xi in x]
+        return judo.as_tensor(hashes, dtype=judo.dtype.hash_type)
 
     def hash_state(self, state):
-        if self._true_hash:
+        if self.uses_true_hash:
             _hash = hash(
                 tuple(
                     [
                         self.hash_tensor(x) if k in state._tensor_names else hash(x)
                         for k, x in state.items()
                     ],
                 ),
             )
             return _hash
-        return 0
+        return self.get_one_id()
 
 
 hasher = Hasher()
```

### Comparing `judo-0.0.8/judo/functions/images.py` & `judo-0.0.9/judo/functions/images.py`

 * *Files identical despite different names*

### Comparing `judo-0.0.8/judo/functions/notebook.py` & `judo-0.0.9/judo/functions/notebook.py`

 * *Files identical despite different names*

### Comparing `judo-0.0.8/judo/functions/pytorch.py` & `judo-0.0.9/judo/functions/pytorch.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from judo.data_types import dtype
 from judo.judo_backend import torch
 from judo.judo_tensor import astype, tensor
 
 
 AVAILABLE_FUNCTIONS = [
+    "abs",
     "argmax",
     "hash_numpy",
     "hash_tensor",
     "concatenate",
     "stack",
     "clip",
     "repeat",
@@ -16,14 +17,19 @@
     "norm",
     "unsqueeze",
     "where",
     "sqrt",
     "tile",
     "logical_or",
     "logical_and",
+    "ones",
+    "zeros",
+    "arange",
+    "full_like",
+    "allclose",
 ]
 
 
 def parse_dim(axis, dim):
     if axis is not None:
         return axis
     return dim
@@ -121,7 +127,31 @@
 
 def logical_or(a, b):
     return a + b
 
 
 def logical_and(a, b):
     return a & b
+
+
+def ones(*args, **kwargs):
+    return torch.ones(*args, **kwargs)
+
+
+def zeros(*args, **kwargs):
+    return torch.zeros(*args, **kwargs)
+
+
+def arange(*args, **kwargs):
+    return torch.arange(*args, **kwargs)
+
+
+def abs(*args, **kwargs):
+    return torch.abs(*args, **kwargs)
+
+
+def allclose(*args, **kwargs):
+    return torch.allclose(*args, **kwargs)
+
+
+def full_like(*args, **kwargs):
+    return torch.full_like(*args, **kwargs)
```

### Comparing `judo-0.0.8/judo/functions/random.py` & `judo-0.0.9/judo/functions/random.py`

 * *Files identical despite different names*

### Comparing `judo-0.0.8/judo/judo_backend.py` & `judo-0.0.9/judo/judo_backend.py`

 * *Files identical despite different names*

### Comparing `judo-0.0.8/judo/judo_tensor.py` & `judo-0.0.9/judo/judo_tensor.py`

 * *Files identical despite different names*

### Comparing `judo-0.0.8/judo.egg-info/PKG-INFO` & `judo-0.0.9/judo.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 Metadata-Version: 2.1
 Name: judo
-Version: 0.0.8
+Version: 0.0.9
 Summary: API and data structures for efficient AI research.
 Home-page: https://github.com/FragileTech/judo
 Author: FragileTech
 Author-email: info@fragile.tech
 License: MIT
 Keywords: Machine learning,artificial intelligence
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/markdown
+Provides-Extra: torch
+Provides-Extra: image
+Provides-Extra: ipython
+Provides-Extra: data-structures
+Provides-Extra: all
 License-File: LICENSE
 
 # judo
 [![Travis build status](https://travis-ci.com/fragiletech/judo.svg)](https://travis-ci.com/fragiletech/judo)
 [![Documentation Status](https://readthedocs.org/projects/fragile/badge/?version=latest)](https://judo.readthedocs.io/en/latest/?badge=latest)
 [![Code coverage](https://codecov.io/github/fragiletech/judo/coverage.svg)](https://codecov.io/github/fragiletech/judo)
 [![PyPI package](https://badgen.net/pypi/v/judo)](https://pypi.org/project/judo/)
```

### Comparing `judo-0.0.8/judo.egg-info/SOURCES.txt` & `judo-0.0.9/judo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `judo-0.0.8/pyproject.toml` & `judo-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `judo-0.0.8/setup.py` & `judo-0.0.9/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,42 +9,50 @@
     "judo.version",
     str(Path(__file__).parent / "judo" / "version.py"),
 ).load_module()
 
 with open(Path(__file__).with_name("README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
+# Module-specific dependencies.
+extras = {
+    "torch": ["torch>=1.0.0"],
+    "image": ["pillow>=7.0.0"],
+    "ipython": ["ipython >= 7.0.0"],
+    "data-structures": ["networkx > 2.0.0"],
+}
+
+# Meta dependency groups.
+extras["all"] = [item for group in extras.values() for item in group]
+
 setup(
     name="judo",
     description="API and data structures for efficient AI research.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     version=version.__version__,
     license="MIT",
     author="FragileTech",
     author_email="info@fragile.tech",
     url="https://github.com/FragileTech/judo",
     keywords=["Machine learning", "artificial intelligence"],
     test_suite="tests",
     tests_require=["pytest>=5.3.5", "hypothesis>=5.6.0"],
-    extras_require={},
+    extras_require=extras,
     install_requires=[
         "numpy>=1.0.0",
         "pyyaml>=5.0.0",
         "xxhash>=1.1.0",
-        "pillow>=7.0.0",
-        "networkx > 2.0.0",
-        "ipython >= 7.0.0",
-        "torch>=1.0.0",
     ],
     package_data={"": ["README.md"], "judo": ["config.yml"]},
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Topic :: Software Development :: Libraries",
     ],
 )
```

### Comparing `judo-0.0.8/tests/test_backend.py` & `judo-0.0.9/tests/test_backend.py`

 * *Files identical despite different names*

### Comparing `judo-0.0.8/tests/test_bounds.py` & `judo-0.0.9/tests/test_bounds.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-# import numpy
 import pytest
 
 import judo
-from judo import tensor
+from judo import dtype, tensor
 from judo.data_structures.bounds import Bounds
+from judo.functions.api import API
 
 
 def create_bounds(name):
     if name == "scalars":
         return lambda: Bounds(high=5, low=-5, shape=(3,))
     elif name == "high_array":
-        return lambda: Bounds(high=tensor([1, 2, 5], dtype=judo.float), low=-5)
+        return lambda: Bounds(high=tensor([1, 2, 5], dtype=dtype.float), low=-5)
     elif name == "low_array":
-        return lambda: Bounds(low=tensor([-1, -5, -3], dtype=judo.float), high=5)
+        return lambda: Bounds(low=tensor([-1, -5, -3], dtype=dtype.float), high=5)
     elif name == "both_array":
-        array = tensor([1, 2, 5], dtype=judo.float)
+        array = tensor([1, 2, 5], dtype=dtype.float)
         return lambda: Bounds(high=array, low=-array)
     elif name == "high_list":
         return lambda: Bounds(
-            low=tensor([-5, -2, -3], dtype=judo.float), high=[5, 5, 5], dtype=judo.float
+            low=tensor([-5, -2, -3], dtype=dtype.float), high=[5, 5, 5], dtype=dtype.float
         )
 
 
 bounds_fixture_params = ["scalars", "high_array", "low_array", "both_array", "high_list"]
 
 
 @pytest.fixture(params=bounds_fixture_params, scope="class")
@@ -60,147 +60,147 @@
         array = tensor([[0, 0, 0], [11, 0, 0], [0, 11, 0], [11, 11, 11]])
         bounds = Bounds.from_array(array)
         assert (bounds.low == tensor([0, 0, 0])).all()
         assert (bounds.high == tensor([11, 11, 11])).all()
         assert bounds.shape == (3,)
 
     def test_from_array_with_scale_positive(self):
-        array = tensor([[0, 0, 0], [10, 0, 0], [0, 10, 0], [10, 10, 10]], dtype=judo.float)
+        array = tensor([[0, 0, 0], [10, 0, 0], [0, 10, 0], [10, 10, 10]], dtype=dtype.float)
         bounds = Bounds.from_array(array, scale=1.1)
-        assert (bounds.low == tensor([0, 0, 0], dtype=judo.float)).all(), (
+        assert (bounds.low == tensor([0, 0, 0], dtype=dtype.float)).all(), (
             bounds.low,
             array.min(axis=0),
         )
-        assert (bounds.high == tensor([11, 11, 11], dtype=judo.float)).all(), (
+        assert (bounds.high == tensor([11, 11, 11], dtype=dtype.float)).all(), (
             bounds.high,
             array.max(axis=0),
         )
         assert bounds.shape == (3,)
 
-        array = tensor([[-10, 0, 0], [-10, 0, 0], [0, -10, 0], [-10, -10, -10]], dtype=judo.float)
+        array = tensor([[-10, 0, 0], [-10, 0, 0], [0, -10, 0], [-10, -10, -10]], dtype=dtype.float)
         bounds = Bounds.from_array(array, scale=1.1)
-        assert (bounds.high == tensor([0, 0, 0], dtype=judo.float)).all(), (
+        assert (bounds.high == tensor([0, 0, 0], dtype=dtype.float)).all(), (
             bounds.high,
             array.max(axis=0),
         )
-        assert (bounds.low == tensor([-11, -11, -11], dtype=judo.float)).all(), (
+        assert (bounds.low == tensor([-11, -11, -11], dtype=dtype.float)).all(), (
             bounds.low,
             array.min(axis=0),
         )
         assert bounds.shape == (3,)
 
         array = tensor(
-            [[10, 10, 10], [100, 10, 10], [10, 100, 10], [100, 100, 100]], dtype=judo.float
+            [[10, 10, 10], [100, 10, 10], [10, 100, 10], [100, 100, 100]], dtype=dtype.float
         )
         bounds = Bounds.from_array(array, scale=1.1)
-        assert judo.allclose(bounds.low, tensor([9.0, 9.0, 9], dtype=judo.float)), (
+        assert API.allclose(bounds.low, tensor([9.0, 9.0, 9], dtype=dtype.float)), (
             bounds.low,
             array.min(axis=0),
         )
-        assert judo.allclose(bounds.high, tensor([110, 110, 110], dtype=judo.float)), (
+        assert API.allclose(bounds.high, tensor([110, 110, 110], dtype=dtype.float)), (
             bounds.high,
             array.max(axis=0),
         )
         assert bounds.shape == (3,)
 
     def test_from_array_with_scale_negative(self):
         # high +, low +, scale > 1
-        array = tensor([[-10, 0, 0], [-10, 0, 0], [0, -10, 0], [-10, -10, -10]], dtype=judo.float)
+        array = tensor([[-10, 0, 0], [-10, 0, 0], [0, -10, 0], [-10, -10, -10]], dtype=dtype.float)
         bounds = Bounds.from_array(array, scale=0.9)
-        assert (bounds.high == tensor([0, 0, 0], dtype=judo.float)).all(), (
+        assert (bounds.high == tensor([0, 0, 0], dtype=dtype.float)).all(), (
             bounds.high,
             array.max(axis=0),
         )
-        assert (bounds.low == tensor([-9, -9, -9], dtype=judo.float)).all(), (
+        assert (bounds.low == tensor([-9, -9, -9], dtype=dtype.float)).all(), (
             bounds.low,
             array.min(axis=0),
         )
         assert bounds.shape == (3,)
-        array = tensor([[0, 0, 0], [10, 0, 0], [0, 10, 0], [10, 10, 10]], dtype=judo.float)
+        array = tensor([[0, 0, 0], [10, 0, 0], [0, 10, 0], [10, 10, 10]], dtype=dtype.float)
         bounds = Bounds.from_array(array, scale=0.9)
-        assert (bounds.low == tensor([0, 0, 0], dtype=judo.float)).all(), (bounds, array)
-        assert (bounds.high == tensor([9, 9, 9], dtype=judo.float)).all()
+        assert (bounds.low == tensor([0, 0, 0], dtype=dtype.float)).all(), (bounds, array)
+        assert (bounds.high == tensor([9, 9, 9], dtype=dtype.float)).all()
         assert bounds.shape == (3,)
         # high +, low +, scale < 1
         array = tensor(
-            [[10, 10, 10], [100, 10, 10], [10, 100, 10], [100, 100, 100]], dtype=judo.float
+            [[10, 10, 10], [100, 10, 10], [10, 100, 10], [100, 100, 100]], dtype=dtype.float
         )
         bounds = Bounds.from_array(array, scale=0.9)
-        assert judo.allclose(bounds.low, tensor([9.0, 9.0, 9.0], dtype=judo.float)), (
+        assert API.allclose(bounds.low, tensor([9.0, 9.0, 9.0], dtype=dtype.float)), (
             bounds.low,
             array.min(axis=0),
         )
-        assert judo.allclose(bounds.high, tensor([90, 90, 90], dtype=judo.float)), (
+        assert API.allclose(bounds.high, tensor([90, 90, 90], dtype=dtype.float)), (
             bounds.high,
             array.max(axis=0),
         )
         assert bounds.shape == (3,)
         # high -, low -, scale > 1
         array = tensor(
             [[-100, -10, -10], [-100, -10, -10], [-10, -100, -10], [-100, -100, -100]],
-            dtype=judo.float,
+            dtype=dtype.float,
         )
         bounds = Bounds.from_array(array, scale=1.1)
-        assert judo.allclose(bounds.high, tensor([-9, -9, -9], dtype=judo.float)), (
+        assert API.allclose(bounds.high, tensor([-9, -9, -9], dtype=dtype.float)), (
             bounds.high,
             array.max(axis=0),
         )
-        assert judo.allclose(bounds.low, tensor([-110, -110, -110], dtype=judo.float)), (
+        assert API.allclose(bounds.low, tensor([-110, -110, -110], dtype=dtype.float)), (
             bounds.low,
             array.min(axis=0),
         )
         assert bounds.shape == (3,)
         # high -, low -, scale < 1
         array = tensor(
             [[-100, -10, -10], [-100, -10, -10], [-10, -100, -10], [-100, -100, -100]],
-            dtype=judo.float,
+            dtype=dtype.float,
         )
         bounds = Bounds.from_array(array, scale=0.9)
-        assert judo.allclose(bounds.high, tensor([-11, -11, -11], dtype=judo.float)), (
+        assert API.allclose(bounds.high, tensor([-11, -11, -11], dtype=dtype.float)), (
             bounds.high,
             array.max(axis=0),
         )
-        assert judo.allclose(bounds.low, tensor([-90, -90, -90], dtype=judo.float)), (
+        assert API.allclose(bounds.low, tensor([-90, -90, -90], dtype=dtype.float)), (
             bounds.low,
             array.min(axis=0),
         )
         assert bounds.shape == (3,)
 
     def test_clip(self):
         tup = ((-1, 10), (-3, 4), (2, 5))
-        array = tensor([[-10, 0, 0], [11, 0, 0], [0, 11, 0], [11, 11, 11]], dtype=judo.float)
+        array = tensor([[-10, 0, 0], [11, 0, 0], [0, 11, 0], [11, 11, 11]], dtype=dtype.float)
         bounds = Bounds.from_tuples(tup)
         clipped = bounds.clip(array)
         target = tensor(
-            [[-1.0, 0.0, 2.0], [10.0, 0.0, 2.0], [0.0, 4.0, 2], [10, 4, 5]], dtype=judo.float
+            [[-1.0, 0.0, 2.0], [10.0, 0.0, 2.0], [0.0, 4.0, 2], [10, 4, 5]], dtype=dtype.float
         )
-        assert judo.allclose(clipped, target), (clipped.dtype, target.dtype)
+        assert API.allclose(clipped, target), (clipped.dtype, target.dtype)
 
     @pytest.mark.parametrize("bounds_fixture", bounds_fixture_params, indirect=True)
     def test_to_tuples(self, bounds_fixture):
         tuples = bounds_fixture.to_tuples()
         assert len(tuples) == 3
         assert min([x[0] for x in tuples]) == -5
         assert max([x[1] for x in tuples]) == 5
 
     @pytest.mark.parametrize("bounds_fixture", bounds_fixture_params, indirect=True)
     def test_points_in_bounds(self, bounds_fixture):
-        zeros = judo.zeros((3, 3))
+        zeros = API.zeros((3, 3))
         assert all(bounds_fixture.points_in_bounds(zeros))
-        tens = judo.ones((3, 3)) * 10.0
+        tens = API.ones((3, 3)) * 10.0
         res = bounds_fixture.points_in_bounds(tens)
         assert not res.any(), (res, tens)
         tens = tensor([[-10, 0, 1], [0, 0, 0], [10, 10, 10]])
         assert sum(bounds_fixture.points_in_bounds(tens)) == 1
 
     @pytest.mark.parametrize("bounds_fixture", bounds_fixture_params, indirect=True)
     def test_safe_margin(self, bounds_fixture: Bounds):
         new_bounds = bounds_fixture.safe_margin()
-        assert judo.allclose(new_bounds.low, bounds_fixture.low)
-        assert judo.allclose(new_bounds.high, bounds_fixture.high)
-        low = judo.full_like(bounds_fixture.low, -10)
+        assert API.allclose(new_bounds.low, bounds_fixture.low)
+        assert API.allclose(new_bounds.high, bounds_fixture.high)
+        low = API.full_like(bounds_fixture.low, -10)
         new_bounds = bounds_fixture.safe_margin(low=low)
-        assert judo.allclose(new_bounds.high, bounds_fixture.high)
-        assert judo.allclose(new_bounds.low, low)
+        assert API.allclose(new_bounds.high, bounds_fixture.high)
+        assert API.allclose(new_bounds.low, low)
         new_bounds = bounds_fixture.safe_margin(low=low, scale=2)
-        assert judo.allclose(new_bounds.high, bounds_fixture.high * 2)
-        assert judo.allclose(new_bounds.low, low * 2)
+        assert API.allclose(new_bounds.high, bounds_fixture.high * 2)
+        assert API.allclose(new_bounds.low, low * 2)
```

### Comparing `judo-0.0.8/tests/test_states.py` & `judo-0.0.9/tests/test_states.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import pytest
 
-import judo
+from judo import dtype
 from judo.data_structures.states import States
+from judo.functions.api import API
 
 
 states_classes = [States]
 
 
 @pytest.fixture(scope="class", params=states_classes)
 def states_class(request):
     return request.param
 
 
 class TestStates:
     def test_init_dict(self, states_class):
-        state_dict = {"name_1": {"size": tuple([1]), "dtype": judo.float32}}
+        state_dict = {"name_1": {"size": tuple([1]), "dtype": dtype.float32}}
         new_states = states_class(state_dict=state_dict, batch_size=2)
         assert new_states.n == 2
 
     def test_init_kwargs(self, states_class):
         name = "miau"
         new_states = states_class(batch_size=2, miau=name)
         assert new_states._batch_size == 2
@@ -30,15 +31,15 @@
         new_states = states_class(batch_size=2, miau=name)
         assert new_states[name] == name, type(new_states)
 
     def test_setitem(self, states_class):
         name_1 = "miau"
         val_1 = name_1
         name_2 = "elephant"
-        val_2 = judo.arange(10)
+        val_2 = API.arange(10)
         new_states = states_class(batch_size=2)
         new_states[name_1] = val_1
         new_states[name_2] = val_2
         assert new_states[name_1] == val_1, type(new_states)
         assert (new_states[name_2] == val_2).all(), type(new_states)
 
     def test_repr(self, states_class):
@@ -58,56 +59,56 @@
 
     def test_split_states(self, states_class):
         batch_size = 20
         new_states = states_class(batch_size=batch_size, test="test")
         for s in new_states.split_states(batch_size):
             assert len(s) == 1
             assert s.test == "test"
-        data = judo.repeat(judo.arange(5).reshape(1, -1), batch_size, 0)
+        data = API.repeat(API.arange(5).reshape(1, -1), batch_size, 0)
         new_states = states_class(batch_size=batch_size, test="test", data=data)
         for s in new_states.split_states(batch_size):
             assert len(s) == 1
             assert s.test == "test"
-            assert bool((s.data == judo.arange(5)).all()), s.data
+            assert bool((s.data == API.arange(5)).all()), s.data
         chunk_len = 4
-        test_data = judo.repeat(judo.arange(5).reshape(1, -1), chunk_len, 0)
+        test_data = API.repeat(API.arange(5).reshape(1, -1), chunk_len, 0)
         for s in new_states.split_states(5):
             assert len(s) == chunk_len
             assert s.test == "test"
             assert (s.data == test_data).all(), (s.data.shape, test_data.shape)
 
         batch_size = 21
-        data = judo.repeat(judo.arange(5).reshape(1, -1), batch_size, 0)
+        data = API.repeat(API.arange(5).reshape(1, -1), batch_size, 0)
         new_states = states_class(batch_size=batch_size, test="test", data=data)
         chunk_len = 5
-        test_data = judo.repeat(judo.arange(5).reshape(1, -1), chunk_len, 0)
+        test_data = API.repeat(API.arange(5).reshape(1, -1), chunk_len, 0)
         split_states = list(new_states.split_states(5))
         for s in split_states[:-1]:
             assert len(s) == chunk_len
             assert s.test == "test"
             assert (s.data == test_data).all(), (s.data.shape, test_data.shape)
 
         assert len(split_states[-1]) == 1
         assert split_states[-1].test == "test"
-        assert (split_states[-1].data == judo.arange(5)).all(), (s.data.shape, test_data.shape)
+        assert (split_states[-1].data == API.arange(5)).all(), (s.data.shape, test_data.shape)
 
     def test_get_params_dir(self, states_class):
-        state_dict = {"name_1": {"size": tuple([1]), "dtype": judo.float32}}
+        state_dict = {"name_1": {"size": tuple([1]), "dtype": dtype.float32}}
         new_states = states_class(state_dict=state_dict, batch_size=2)
         params_dict = new_states.get_params_dict()
         assert isinstance(params_dict, dict)
         for k, v in params_dict.items():
             assert isinstance(k, str)
             assert isinstance(v, dict)
             for ki, _ in v.items():
                 assert isinstance(ki, str)
 
     def test_merge_states(self, states_class):
         batch_size = 21
-        data = judo.repeat(judo.arange(5).reshape(1, -1), batch_size, 0)
+        data = API.repeat(API.arange(5).reshape(1, -1), batch_size, 0)
         new_states = states_class(batch_size=batch_size, test="test", data=data)
         split_states = tuple(new_states.split_states(batch_size))
         merged = new_states.merge_states(split_states)
         assert len(merged) == batch_size
         assert merged.test == "test"
         assert (merged.data == data).all()
```

### Comparing `judo-0.0.8/tests/test_tree.py` & `judo-0.0.9/tests/test_tree.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,32 @@
-import networkx
 import pytest
 
-import judo
-from judo.data_structures.tree import HistoryTree, NetworkxTree, to_node_id
+
+try:
+    import networkx
+
+    from judo.data_structures.tree import HistoryTree, NetworkxTree, to_node_id
+    from judo.functions.api import API
+
+    MISSING_IMPORTS = False
+except ImportError:
+    MISSING_IMPORTS = True
 
 
 def random_powerlaw():
     g = networkx.DiGraph()
     t = networkx.random_powerlaw_tree(500, gamma=3, tries=1000, seed=160290)
     graph = networkx.compose(g, t)
     mapping = {n: to_node_id(n) for n in graph.nodes}
     return networkx.relabel_nodes(graph, mapping)
 
 
 def small_tree():
-    node_data = {"a": judo.arange(10), "b": judo.zeros(10)}
-    edge_data = {"c": judo.ones(10)}
+    node_data = {"a": API.arange(10), "b": API.zeros(10)}
+    edge_data = {"c": API.ones(10)}
     g = networkx.DiGraph()
     for i in range(8):
         g.add_node(to_node_id(i), **node_data)
     pairs = [(0, 1), (1, 2), (2, 3), (2, 4), (2, 5), (3, 6), (3, 7)]
     for a, b in pairs:
         g.add_edge(to_node_id(a), to_node_id(b), **edge_data)
     return g
@@ -28,14 +35,15 @@
 @pytest.fixture(params=[random_powerlaw, small_tree], scope="function")
 def tree(request):
     tree = HistoryTree()
     tree.data = request.param()
     return tree
 
 
+@pytest.mark.skipif(MISSING_IMPORTS, reason="networkx not installed")
 class TestNetworkxTree:
     def test_init(self, tree):
         pass
 
     def test_reset_graph(self, tree):
         node_data = {"miau": 2104}
         root_id = to_node_id(421)
@@ -43,15 +51,15 @@
         assert tree.root_id == root_id
         assert isinstance(tree.data.nodes[root_id], dict)
         assert tree.data.nodes[root_id]["epoch"] == 0
         assert len(tree) == 1
         assert tree.data.nodes[root_id]["miau"] == 2104
 
     def test_append_leaf(self, tree):
-        node_data = {"node": judo.arange(10)}
+        node_data = {"node": API.arange(10)}
         edge_data = {"edge": False}
         leaf_id = to_node_id(-421)
         epoch = 123
         tree.append_leaf(
             leaf_id=leaf_id,
             parent_id=tree.root_id,
             node_data=node_data,
```

