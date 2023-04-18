# Comparing `tmp/dask_histogram-2023.4.2.tar.gz` & `tmp/dask_histogram-2023.4.3.tar.gz`

## Comparing `dask_histogram-2023.4.2.tar` & `dask_histogram-2023.4.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 dask_histogram-2023.4.2/src/dask_histogram/__init__.py
--rw-r--r--   0        0        0     6417 2020-02-02 00:00:00.000000 dask_histogram-2023.4.2/src/dask_histogram/bins.py
--rw-r--r--   0        0        0    29278 2020-02-02 00:00:00.000000 dask_histogram-2023.4.2/src/dask_histogram/boost.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 dask_histogram-2023.4.2/src/dask_histogram/config.py
--rw-r--r--   0        0        0    39039 2020-02-02 00:00:00.000000 dask_histogram-2023.4.2/src/dask_histogram/core.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 dask_histogram-2023.4.2/src/dask_histogram/histogram.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dask_histogram-2023.4.2/src/dask_histogram/py.typed
--rw-r--r--   0        0        0    16836 2020-02-02 00:00:00.000000 dask_histogram-2023.4.2/src/dask_histogram/routines.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 dask_histogram-2023.4.2/src/dask_histogram/sizeof.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 dask_histogram-2023.4.2/src/dask_histogram/typing.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 dask_histogram-2023.4.2/src/dask_histogram/version.py
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 dask_histogram-2023.4.2/.gitignore
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 dask_histogram-2023.4.2/LICENSE
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 dask_histogram-2023.4.2/README.md
--rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 dask_histogram-2023.4.2/pyproject.toml
--rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 dask_histogram-2023.4.2/PKG-INFO
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 dask_histogram-2023.4.3/src/dask_histogram/__init__.py
+-rw-r--r--   0        0        0     6417 2020-02-02 00:00:00.000000 dask_histogram-2023.4.3/src/dask_histogram/bins.py
+-rw-r--r--   0        0        0    29283 2020-02-02 00:00:00.000000 dask_histogram-2023.4.3/src/dask_histogram/boost.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 dask_histogram-2023.4.3/src/dask_histogram/config.py
+-rw-r--r--   0        0        0    38929 2020-02-02 00:00:00.000000 dask_histogram-2023.4.3/src/dask_histogram/core.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 dask_histogram-2023.4.3/src/dask_histogram/histogram.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dask_histogram-2023.4.3/src/dask_histogram/py.typed
+-rw-r--r--   0        0        0    16836 2020-02-02 00:00:00.000000 dask_histogram-2023.4.3/src/dask_histogram/routines.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 dask_histogram-2023.4.3/src/dask_histogram/sizeof.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 dask_histogram-2023.4.3/src/dask_histogram/typing.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 dask_histogram-2023.4.3/src/dask_histogram/version.py
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 dask_histogram-2023.4.3/.gitignore
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 dask_histogram-2023.4.3/LICENSE
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 dask_histogram-2023.4.3/README.md
+-rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 dask_histogram-2023.4.3/pyproject.toml
+-rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 dask_histogram-2023.4.3/PKG-INFO
```

### Comparing `dask_histogram-2023.4.2/src/dask_histogram/__init__.py` & `dask_histogram-2023.4.3/src/dask_histogram/__init__.py`

 * *Files identical despite different names*

### Comparing `dask_histogram-2023.4.2/src/dask_histogram/bins.py` & `dask_histogram-2023.4.3/src/dask_histogram/bins.py`

 * *Files identical despite different names*

### Comparing `dask_histogram-2023.4.2/src/dask_histogram/boost.py` & `dask_histogram-2023.4.3/src/dask_histogram/boost.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
     def __radd__(self, other):
         return other.__iadd__(self)
 
     def __dask_graph__(self) -> HighLevelGraph:
         return self.dask
 
     def __dask_keys__(self) -> list[str]:
-        return [self.dask_name]
+        return [(self.dask_name, 0)]
 
     def __dask_layers__(self) -> tuple[str, ...]:
         if isinstance(self.dask, HighLevelGraph) and len(self.dask.layers) == 1:
             return tuple(self.dask.layers)
         return (self.dask_name,)
 
     def __dask_tokenize__(self) -> str:
```

### Comparing `dask_histogram-2023.4.2/src/dask_histogram/core.py` & `dask_histogram-2023.4.3/src/dask_histogram/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 """Dask Histogram core High Level Graph API."""
 
 from __future__ import annotations
 
 import operator
-from typing import TYPE_CHECKING, Any, Callable, Hashable, Mapping, Sequence
+from typing import TYPE_CHECKING, Any, Callable, Hashable, Literal, Mapping, Sequence
 
 import boost_histogram as bh
 import dask.config
 import numpy as np
 from dask.base import DaskMethodsMixin, dont_optimize, is_dask_collection, tokenize
 from dask.blockwise import BlockwiseDep, blockwise, fuse_roots, optimize_blockwise
 from dask.context import globalmethod
 from dask.core import flatten
 from dask.delayed import Delayed
 from dask.highlevelgraph import HighLevelGraph
 from dask.threaded import get as tget
 from dask.utils import is_dataframe_like, key_split
-from tlz import partition_all
 
 if TYPE_CHECKING:
     from dask.blockwise import Blockwise
     from numpy.typing import NDArray
 
     from dask_histogram.typing import DaskCollection
 
@@ -445,23 +444,23 @@
                 f"Layer {self._layer} not in the HighLevelGraph's layers: {list(dsk.layers)}"
             )
 
     def __dask_graph__(self) -> HighLevelGraph:
         return self._dask
 
     def __dask_keys__(self) -> list[str]:
-        return [self.name]
+        return [self.key]
 
     def __dask_layers__(self) -> tuple[str, ...]:
         if isinstance(self._dask, HighLevelGraph) and len(self._dask.layers) == 1:
             return tuple(self._dask.layers)
         return (self.name,)
 
-    def __dask_tokenize__(self) -> str:
-        return self.name
+    def __dask_tokenize__(self) -> Any:
+        return self.key
 
     def __dask_postcompute__(self) -> Any:
         return _finalize_agg_histogram, ()
 
     def __dask_postpersist__(self) -> Any:
         return self._rebuild, ()
 
@@ -487,14 +486,18 @@
         return self._name
 
     @property
     def dask(self) -> HighLevelGraph:
         return self._dask
 
     @property
+    def key(self) -> tuple[str, Literal[0]]:
+        return (self.name, 0)
+
+    @property
     def histref(self) -> bh.Histogram:
         """Empty reference boost-histogram object."""
         return self._meta
 
     @property
     def _storage_type(self) -> type[bh.storage.Storage]:
         """Storage type of the histogram."""
@@ -725,49 +728,46 @@
         return [Delayed(k, graph, layer=layer) for k in keys]
 
 
 def _reduction(
     ph: PartitionedHistogram,
     split_every: int | None = None,
 ) -> AggHistogram:
-    from dask.bag.core import empty_safe_aggregate
+    from dask.layers import DataFrameTreeReduction
 
     if split_every is None:
         split_every = dask.config.get("histogram.aggregation.split_every", 8)
     if split_every is False:
         split_every = ph.npartitions
 
     token = tokenize(ph, sum, split_every)
-    name = f"hist-aggregate-{token}"
-    k = ph.npartitions
-    b = ph.name
-    d = 0
-    dsk = {}
-    while k > split_every:
-        c = f"{name}{d}"
-        for i, inds in enumerate(partition_all(split_every, range(k))):
-            dsk[(c, i)] = (
-                empty_safe_aggregate,
-                sum,
-                [(b, j) for j in inds],
-                False,
-            )
-        k = i + 1
-        b = c
-        d += 1
-    dsk[(name, 0)] = (
-        empty_safe_aggregate,
-        sum,
-        [(b, j) for j in range(k)],
-        True,
+
+    label = "histreduce"
+
+    name_comb = f"{label}-combine-{token}"
+    name_agg = f"{label}-agg-{token}"
+
+    def hist_safe_sum(items):
+        safe_items = [item for item in items if not isinstance(item, tuple)]
+        return sum(safe_items)
+
+    dftr = DataFrameTreeReduction(
+        name=name_agg,
+        name_input=ph.name,
+        npartitions_input=ph.npartitions,
+        concat_func=hist_safe_sum,
+        tree_node_func=lambda x: x,
+        finalize_func=lambda x: x,
+        split_every=split_every,
+        tree_node_name=name_comb,
     )
 
-    dsk[name] = dsk.pop((name, 0))  # type: ignore
-    g = HighLevelGraph.from_collections(name, dsk, dependencies=[ph])
-    return AggHistogram(g, name, histref=ph.histref)
+    graph = HighLevelGraph.from_collections(name_agg, dftr, dependencies=(ph,))
+
+    return AggHistogram(graph, name_agg, histref=ph.histref)
 
 
 def _dependencies(
     *args: DaskCollection,
     weights: DaskCollection | None = None,
     sample: DaskCollection | None = None,
 ) -> tuple[DaskCollection, ...]:
@@ -988,15 +988,15 @@
     name = f"to-dask-array-{tokenize(agghist)}"
     thehist = agghist.histref
     if isinstance(thehist, tuple):
         thehist = bh.Histogram(
             *agghist.histref[0], storage=agghist.histref[1], metadata=agghist.histref[2]
         )
     zeros = (0,) * thehist.ndim
-    dsk = {(name, *zeros): (lambda x, f: x.to_numpy(flow=f)[0], agghist.name, flow)}
+    dsk = {(name, *zeros): (lambda x, f: x.to_numpy(flow=f)[0], agghist.key, flow)}
     graph = HighLevelGraph.from_collections(name, dsk, dependencies=(agghist,))
     shape = thehist.shape
     if flow:
         shape = tuple(i + 2 for i in shape)
     int_storage = thehist.storage_type in (
         bh.storage.Int64,
         bh.storage.AtomicInt64,
@@ -1026,25 +1026,19 @@
         self.__name__ = func.__name__ if name is None else name
 
     def __call__(self, a: AggHistogram, b: AggHistogram) -> AggHistogram:
         name = f"{self.__name__}-hist-{tokenize(a, b)}"
         deps = []
         if is_dask_collection(a):
             deps.append(a)
-            k1 = a.name
-        else:
-            k1 = a  # type: ignore
         if is_dask_collection(b):
             deps.append(b)
-            k2 = b.name
-        else:
-            k2 = b  # type: ignore
-        k1 = a.__dask_tokenize__() if is_dask_collection(a) else a  # type: ignore
-        k2 = b.__dask_tokenize__() if is_dask_collection(b) else b  # type: ignore
-        llg = {name: (self.func, k1, k2)}
+        k1 = a.__dask_keys__()[0] if is_dask_collection(a) else a  # type: ignore
+        k2 = b.__dask_keys__()[0] if is_dask_collection(b) else b  # type: ignore
+        llg = {(name, 0): (self.func, k1, k2)}
         g = HighLevelGraph.from_collections(name, llg, dependencies=deps)
         try:
             ref = a.histref
         except AttributeError:
             ref = b.histref
         return AggHistogram(g, name, histref=ref)
```

### Comparing `dask_histogram-2023.4.2/src/dask_histogram/routines.py` & `dask_histogram-2023.4.3/src/dask_histogram/routines.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,15 @@
     >>> h, edges = dh.histogram(x, bins=bins)
 
     Now with weights and the object return style:
 
     >>> w = da.random.uniform(0.0, 1.0, size=x.shape[0], chunks=x.chunksize[0])
     >>> h = dh.histogram(x, bins=bins, weights=w, histogram=True)
     >>> h
-    dask_histogram.AggHistogram<hist-aggregate, ndim=1, storage=Double()>
+    dask_histogram.AggHistogram<histreduce-agg, ndim=1, storage=Double()>
 
     """
     h = histogramdd(
         (x,),
         bins=bins,
         range=range,
         normed=normed,
@@ -374,15 +374,15 @@
     >>> bins = [
     ...    [-3, -2, 0, 1, 3],
     ...    [-3, -1, 1, 2, 3],
     ...    [-3, -2, 0, 2, 3],
     ... ]
     >>> h = dh.histogramdd((x, y, z), bins=bins, histogram=True)
     >>> h
-    dask_histogram.AggHistogram<hist-aggregate, ndim=3, storage=Double()>
+    dask_histogram.AggHistogram<histreduce-agg, ndim=3, storage=Double()>
     >>> h.ndim
     3
     >>> h = h.compute()
     >>> h  # doctest: +SKIP
     Histogram(
       Variable([-3, -2, 0, 1, 3]),
       Variable([-3, -1, 1, 2, 3]),
@@ -402,15 +402,15 @@
     ...     bins=bins,
     ...     range=range,
     ...     weights=w,
     ...     histogram=True,
     ...     storage=dh.storage.Weight()
     ... )
     >>> h
-    dask_histogram.AggHistogram<hist-aggregate, ndim=3, storage=Weight()>
+    dask_histogram.AggHistogram<histreduce-agg, ndim=3, storage=Weight()>
 
     """
     # Check for invalid argument combinations.
     if normed is not None:
         raise KeyError(
             "normed=True is deprecated in NumPy and not supported by dask-histogram."
         )
```

### Comparing `dask_histogram-2023.4.2/src/dask_histogram/sizeof.py` & `dask_histogram-2023.4.3/src/dask_histogram/sizeof.py`

 * *Files identical despite different names*

### Comparing `dask_histogram-2023.4.2/.gitignore` & `dask_histogram-2023.4.3/.gitignore`

 * *Files identical despite different names*

### Comparing `dask_histogram-2023.4.2/LICENSE` & `dask_histogram-2023.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dask_histogram-2023.4.2/README.md` & `dask_histogram-2023.4.3/README.md`

 * *Files identical despite different names*

### Comparing `dask_histogram-2023.4.2/pyproject.toml` & `dask_histogram-2023.4.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dask_histogram-2023.4.2/PKG-INFO` & `dask_histogram-2023.4.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-histogram
-Version: 2023.4.2
+Version: 2023.4.3
 Summary: Histogramming with Dask.
 Project-URL: Homepage, https://github.com/dask-contrib/dask-histogram
 Project-URL: Documentation, https://dask-histogram.readthedocs.io/
 Project-URL: Bug Tracker, https://github.com/dask-contrib/dask-histogram/issues
 Author-email: Doug Davis <ddavis@ddavis.io>
 License: BSD-3-Clause
 License-File: LICENSE
```

