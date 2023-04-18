# Comparing `tmp/torch-interpol-0.2.1.tar.gz` & `tmp/torch-interpol-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/torch-interpol-0.2.1.tar", last modified: Wed Jan  4 17:12:37 2023, max compression
+gzip compressed data, was "dist/torch-interpol-0.2.2.tar", last modified: Tue Apr 18 00:39:05 2023, max compression
```

## Comparing `torch-interpol-0.2.1.tar` & `torch-interpol-0.2.2.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 17:12:37.000000 torch-interpol-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-01-04 17:11:55.000000 torch-interpol-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-01-04 17:11:55.000000 torch-interpol-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11240 2023-01-04 17:12:37.000000 torch-interpol-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8249 2023-01-04 17:11:55.000000 torch-interpol-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 17:12:37.000000 torch-interpol-0.2.1/interpol/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-01-04 17:11:55.000000 torch-interpol-0.2.1/interpol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-01-04 17:12:37.000000 torch-interpol-0.2.1/interpol/_version.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18789 2023-01-04 17:11:55.000000 torch-interpol-0.2.1/interpol/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9256 2023-01-04 17:11:55.000000 torch-interpol-0.2.1/interpol/autograd.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-01-04 17:11:55.000000 torch-interpol-0.2.1/interpol/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-01-04 17:11:55.000000 torch-interpol-0.2.1/interpol/bounds.py
--rw-r--r--   0 runner    (1001) docker     (123)    10629 2023-01-04 17:11:55.000000 torch-interpol-0.2.1/interpol/coeff.py
--rw-r--r--   0 runner    (1001) docker     (123)    10756 2023-01-04 17:11:55.000000 torch-interpol-0.2.1/interpol/iso0.py
--rw-r--r--   0 runner    (1001) docker     (123)    42938 2023-01-04 17:11:55.000000 torch-interpol-0.2.1/interpol/iso1.py
--rw-r--r--   0 runner    (1001) docker     (123)    10655 2023-01-04 17:11:55.000000 torch-interpol-0.2.1/interpol/jit_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-01-04 17:11:55.000000 torch-interpol-0.2.1/interpol/jitfields.py
--rw-r--r--   0 runner    (1001) docker     (123)    15488 2023-01-04 17:11:55.000000 torch-interpol-0.2.1/interpol/nd.py
--rw-r--r--   0 runner    (1001) docker     (123)    12052 2023-01-04 17:11:55.000000 torch-interpol-0.2.1/interpol/pushpull.py
--rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-01-04 17:11:55.000000 torch-interpol-0.2.1/interpol/resize.py
--rw-r--r--   0 runner    (1001) docker     (123)     8918 2023-01-04 17:11:55.000000 torch-interpol-0.2.1/interpol/splines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 17:12:37.000000 torch-interpol-0.2.1/interpol/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-04 17:11:55.000000 torch-interpol-0.2.1/interpol/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-01-04 17:11:55.000000 torch-interpol-0.2.1/interpol/tests/test_gradcheck_pushpull.py
--rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-01-04 17:11:55.000000 torch-interpol-0.2.1/interpol/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-01-04 17:12:37.000000 torch-interpol-0.2.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-01-04 17:11:55.000000 torch-interpol-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-04 17:12:37.000000 torch-interpol-0.2.1/torch_interpol.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11240 2023-01-04 17:12:37.000000 torch-interpol-0.2.1/torch_interpol.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-01-04 17:12:37.000000 torch-interpol-0.2.1/torch_interpol.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-04 17:12:37.000000 torch-interpol-0.2.1/torch_interpol.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-01-04 17:12:37.000000 torch-interpol-0.2.1/torch_interpol.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-04 17:12:37.000000 torch-interpol-0.2.1/torch_interpol.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    78254 2023-01-04 17:11:55.000000 torch-interpol-0.2.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 00:39:05.000000 torch-interpol-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-18 00:38:20.000000 torch-interpol-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-18 00:38:20.000000 torch-interpol-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11240 2023-04-18 00:39:05.000000 torch-interpol-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8249 2023-04-18 00:38:20.000000 torch-interpol-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 00:39:05.000000 torch-interpol-0.2.2/interpol/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-18 00:38:20.000000 torch-interpol-0.2.2/interpol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-18 00:39:05.000000 torch-interpol-0.2.2/interpol/_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18789 2023-04-18 00:38:20.000000 torch-interpol-0.2.2/interpol/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9256 2023-04-18 00:38:20.000000 torch-interpol-0.2.2/interpol/autograd.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-18 00:38:20.000000 torch-interpol-0.2.2/interpol/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-04-18 00:38:20.000000 torch-interpol-0.2.2/interpol/bounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10629 2023-04-18 00:38:20.000000 torch-interpol-0.2.2/interpol/coeff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10756 2023-04-18 00:38:20.000000 torch-interpol-0.2.2/interpol/iso0.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42938 2023-04-18 00:38:20.000000 torch-interpol-0.2.2/interpol/iso1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11834 2023-04-18 00:38:20.000000 torch-interpol-0.2.2/interpol/jit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-04-18 00:38:20.000000 torch-interpol-0.2.2/interpol/jitfields.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15488 2023-04-18 00:38:20.000000 torch-interpol-0.2.2/interpol/nd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12052 2023-04-18 00:38:20.000000 torch-interpol-0.2.2/interpol/pushpull.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-04-18 00:38:20.000000 torch-interpol-0.2.2/interpol/resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-04-18 00:38:20.000000 torch-interpol-0.2.2/interpol/restrict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8918 2023-04-18 00:38:20.000000 torch-interpol-0.2.2/interpol/splines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 00:39:05.000000 torch-interpol-0.2.2/interpol/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 00:38:20.000000 torch-interpol-0.2.2/interpol/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-04-18 00:38:20.000000 torch-interpol-0.2.2/interpol/tests/test_gradcheck_pushpull.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-04-18 00:38:20.000000 torch-interpol-0.2.2/interpol/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-18 00:39:05.000000 torch-interpol-0.2.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      203 2023-04-18 00:38:20.000000 torch-interpol-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 00:39:05.000000 torch-interpol-0.2.2/torch_interpol.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11240 2023-04-18 00:39:05.000000 torch-interpol-0.2.2/torch_interpol.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-18 00:39:05.000000 torch-interpol-0.2.2/torch_interpol.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 00:39:05.000000 torch-interpol-0.2.2/torch_interpol.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-18 00:39:05.000000 torch-interpol-0.2.2/torch_interpol.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-18 00:39:05.000000 torch-interpol-0.2.2/torch_interpol.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    78254 2023-04-18 00:38:20.000000 torch-interpol-0.2.2/versioneer.py
```

### Comparing `torch-interpol-0.2.1/LICENSE` & `torch-interpol-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `torch-interpol-0.2.1/PKG-INFO` & `torch-interpol-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-interpol
-Version: 0.2.1
+Version: 0.2.2
 Summary: High-order spline interpolation in PyTorch
 Home-page: UNKNOWN
 Author: Yael Balbastre
 Author-email: yael.balbastre@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/balbasty/torch-interpol
 Description: # torch-interpol
```

### Comparing `torch-interpol-0.2.1/README.md` & `torch-interpol-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `torch-interpol-0.2.1/interpol/api.py` & `torch-interpol-0.2.2/interpol/api.py`

 * *Files identical despite different names*

### Comparing `torch-interpol-0.2.1/interpol/autograd.py` & `torch-interpol-0.2.2/interpol/autograd.py`

 * *Files identical despite different names*

### Comparing `torch-interpol-0.2.1/interpol/bounds.py` & `torch-interpol-0.2.2/interpol/bounds.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import torch
 from enum import Enum
 from typing import Optional
+from .jit_utils import floor_div
 Tensor = torch.Tensor
 
 
 class BoundType(Enum):
     zero = zeros = 0
     replicate = nearest = 1
     dct1 = mirror = 2
@@ -65,20 +66,22 @@
             one = torch.ones([1], dtype=torch.int8, device=i.device)
             zero = torch.zeros([1], dtype=torch.int8, device=i.device)
             n2 = 2 * (n + 1)
             i = torch.where(i < 0, -i + (n-1), i)
             i = i.remainder(n2)
             x = torch.where(i == 0, zero, one)
             x = torch.where(i.remainder(n + 1) == n, zero, x)
-            x = torch.where((i / (n+1)).remainder(2) > 0, -x, x)
+            i = floor_div(i, n+1)
+            x = torch.where(torch.remainder(i, 2) > 0, -x, x)
             return x
         elif self.type == 5:  # dst2
             i = torch.where(i < 0, n - 1 - i, i)
             x = torch.ones([1], dtype=torch.int8, device=i.device)
-            x = torch.where((i / n).remainder(2) > 0, -x, x)
+            i = floor_div(i, n)
+            x = torch.where(torch.remainder(i, 2) > 0, -x, x)
             return x
         elif self.type == 0:  # zero
             one = torch.ones([1], dtype=torch.int8, device=i.device)
             zero = torch.zeros([1], dtype=torch.int8, device=i.device)
             outbounds = ((i < 0) | (i >= n))
             x = torch.where(outbounds, zero, one)
             return x
```

### Comparing `torch-interpol-0.2.1/interpol/coeff.py` & `torch-interpol-0.2.2/interpol/coeff.py`

 * *Files identical despite different names*

### Comparing `torch-interpol-0.2.1/interpol/iso0.py` & `torch-interpol-0.2.2/interpol/iso0.py`

 * *Files identical despite different names*

### Comparing `torch-interpol-0.2.1/interpol/iso1.py` & `torch-interpol-0.2.2/interpol/iso1.py`

 * *Files identical despite different names*

### Comparing `torch-interpol-0.2.1/interpol/jit_utils.py` & `torch-interpol-0.2.2/interpol/jit_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -379,41 +379,65 @@
     dt = torch.matmul(x, y).squeeze(-1).squeeze(-1)
     if keepdim:
         for d in dim:
             dt.unsqueeze(d)
     return dt
 
 
-if torch_version('>=', (1, 10)):
-    @torch.jit.script
-    def meshgrid_ij(x: List[torch.Tensor]) -> List[torch.Tensor]:
-        return torch.meshgrid(x, indexing='ij')
-    @torch.jit.script
-    def meshgrid_xy(x: List[torch.Tensor]) -> List[torch.Tensor]:
-        return torch.meshgrid(x, indexing='xy')
-else:
-    @torch.jit.script
-    def meshgrid_ij(x: List[torch.Tensor]) -> List[torch.Tensor]:
-        return torch.meshgrid(x)
-    @torch.jit.script
-    def meshgrid_xy(x: List[torch.Tensor]) -> List[torch.Tensor]:
-        grid = torch.meshgrid(x)
-        if len(grid) > 1:
-            grid[0] = grid[0].transpose(0, 1)
-            grid[1] = grid[1].transpose(0, 1)
-        return grid
-
 
 # cartesian_prod takes multiple inout tensors as input in eager mode
 # but takes a list of tensor in jit mode. This is a helper that works
 # in both cases.
 if not int(os.environ.get('PYTORCH_JIT', '1')):
     cartesian_prod = lambda x: torch.cartesian_prod(*x)
-    meshgrid_ij_list = meshgrid_ij
-    meshgrid_xy_list = meshgrid_xy
-    meshgrid_ij = lambda x: meshgrid_ij_list(*x)
-    meshgrid_xy = lambda x: meshgrid_xy_list(*x)
+    if torch_version('>=', (1, 10)):
+        def meshgrid_ij(x: List[torch.Tensor]) -> List[torch.Tensor]:
+            return torch.meshgrid(*x, indexing='ij')
+        def meshgrid_xy(x: List[torch.Tensor]) -> List[torch.Tensor]:
+            return torch.meshgrid(*x, indexing='xy')
+    else:
+        def meshgrid_ij(x: List[torch.Tensor]) -> List[torch.Tensor]:
+            return torch.meshgrid(*x)
+        def meshgrid_xy(x: List[torch.Tensor]) -> List[torch.Tensor]:
+            grid = torch.meshgrid(*x)
+            if len(grid) > 1:
+                grid[0] = grid[0].transpose(0, 1)
+                grid[1] = grid[1].transpose(0, 1)
+            return grid
+
 else:
     cartesian_prod = torch.cartesian_prod
+    if torch_version('>=', (1, 10)):
+        @torch.jit.script
+        def meshgrid_ij(x: List[torch.Tensor]) -> List[torch.Tensor]:
+            return torch.meshgrid(x, indexing='ij')
+        @torch.jit.script
+        def meshgrid_xy(x: List[torch.Tensor]) -> List[torch.Tensor]:
+            return torch.meshgrid(x, indexing='xy')
+    else:
+        @torch.jit.script
+        def meshgrid_ij(x: List[torch.Tensor]) -> List[torch.Tensor]:
+            return torch.meshgrid(x)
+        @torch.jit.script
+        def meshgrid_xyt(x: List[torch.Tensor]) -> List[torch.Tensor]:
+            grid = torch.meshgrid(x)
+            if len(grid) > 1:
+                grid[0] = grid[0].transpose(0, 1)
+                grid[1] = grid[1].transpose(0, 1)
+            return grid
 
 
 meshgrid = meshgrid_ij
+
+
+# In torch < 1.6, div applied to integer tensor performed a floor_divide
+# In torch > 1.6, it performs a true divide.
+# Floor division must be done using `floor_divide`, but it was buggy
+# until torch 1.13 (it was doing a trunc divide instead of a floor divide).
+# There was at some point a deprecation warning for floor_divide, but it
+# seems to have been lifted afterwards. In torch >= 1.13, floor_divide
+# performs a correct floor division.
+# Since we only apply floor_divide ot positive values, we are fine.
+if torch_version('<', (1, 6)):
+    floor_div = torch.div
+else:
+    floor_div = torch.floor_divide
```

### Comparing `torch-interpol-0.2.1/interpol/jitfields.py` & `torch-interpol-0.2.2/interpol/jitfields.py`

 * *Files 20% similar despite different names*

```diff
@@ -78,7 +78,18 @@
     kwargs.setdefault('bound', 'nearest')
     ndim = max(len(make_list(factor or [])),
                len(make_list(shape or [])),
                len(make_list(anchor or []))) or (image.dim() - 2)
     return jitfields.resize(image, factor=factor, shape=shape, ndim=ndim,
                             anchor=anchor, order=interpolation,
                             bound=kwargs['bound'], prefilter=prefilter)
+
+
+def restrict(image, factor=None, shape=None, anchor='c',
+             interpolation=1, reduce_sum=False, **kwargs):
+    kwargs.setdefault('bound', 'nearest')
+    ndim = max(len(make_list(factor or [])),
+               len(make_list(shape or [])),
+               len(make_list(anchor or []))) or (image.dim() - 2)
+    return jitfields.restrict(image, factor=factor, shape=shape, ndim=ndim,
+                              anchor=anchor, order=interpolation,
+                              bound=kwargs['bound'], reduce_sum=reduce_sum)
```

### Comparing `torch-interpol-0.2.1/interpol/nd.py` & `torch-interpol-0.2.2/interpol/nd.py`

 * *Files identical despite different names*

### Comparing `torch-interpol-0.2.1/interpol/pushpull.py` & `torch-interpol-0.2.2/interpol/pushpull.py`

 * *Files identical despite different names*

### Comparing `torch-interpol-0.2.1/interpol/resize.py` & `torch-interpol-0.2.2/interpol/resize.py`

 * *Files identical despite different names*

### Comparing `torch-interpol-0.2.1/interpol/splines.py` & `torch-interpol-0.2.2/interpol/splines.py`

 * *Files identical despite different names*

### Comparing `torch-interpol-0.2.1/interpol/tests/test_gradcheck_pushpull.py` & `torch-interpol-0.2.2/interpol/tests/test_gradcheck_pushpull.py`

 * *Files identical despite different names*

### Comparing `torch-interpol-0.2.1/interpol/utils.py` & `torch-interpol-0.2.2/interpol/utils.py`

 * *Files identical despite different names*

### Comparing `torch-interpol-0.2.1/setup.cfg` & `torch-interpol-0.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `torch-interpol-0.2.1/torch_interpol.egg-info/PKG-INFO` & `torch-interpol-0.2.2/torch_interpol.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-interpol
-Version: 0.2.1
+Version: 0.2.2
 Summary: High-order spline interpolation in PyTorch
 Home-page: UNKNOWN
 Author: Yael Balbastre
 Author-email: yael.balbastre@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/balbasty/torch-interpol
 Description: # torch-interpol
```

### Comparing `torch-interpol-0.2.1/torch_interpol.egg-info/SOURCES.txt` & `torch-interpol-0.2.2/torch_interpol.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 interpol/iso0.py
 interpol/iso1.py
 interpol/jit_utils.py
 interpol/jitfields.py
 interpol/nd.py
 interpol/pushpull.py
 interpol/resize.py
+interpol/restrict.py
 interpol/splines.py
 interpol/utils.py
 interpol/tests/__init__.py
 interpol/tests/test_gradcheck_pushpull.py
 torch_interpol.egg-info/PKG-INFO
 torch_interpol.egg-info/SOURCES.txt
 torch_interpol.egg-info/dependency_links.txt
```

### Comparing `torch-interpol-0.2.1/versioneer.py` & `torch-interpol-0.2.2/versioneer.py`

 * *Files identical despite different names*

