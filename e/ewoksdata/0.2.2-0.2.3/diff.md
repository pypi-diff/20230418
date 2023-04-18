# Comparing `tmp/ewoksdata-0.2.2.tar.gz` & `tmp/ewoksdata-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ewoksdata-0.2.2.tar", last modified: Tue Apr 11 17:32:32 2023, max compression
+gzip compressed data, was "dist/ewoksdata-0.2.3.tar", last modified: Tue Apr 18 15:23:37 2023, max compression
```

## Comparing `ewoksdata-0.2.2.tar` & `ewoksdata-0.2.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:32:32.000000 ewoksdata-0.2.2/
--rw-rw-rw-   0 root         (0) root         (0)     1102 2023-04-11 11:03:11.000000 ewoksdata-0.2.2/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)     1020 2023-04-11 17:32:32.000000 ewoksdata-0.2.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      267 2023-04-11 11:03:11.000000 ewoksdata-0.2.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-04-11 11:03:11.000000 ewoksdata-0.2.2/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1256 2023-04-11 17:32:32.000000 ewoksdata-0.2.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-04-11 11:03:11.000000 ewoksdata-0.2.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:32:32.000000 ewoksdata-0.2.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:32:32.000000 ewoksdata-0.2.2/src/ewoksdata/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-04-11 17:31:40.000000 ewoksdata-0.2.2/src/ewoksdata/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:32:32.000000 ewoksdata-0.2.2/src/ewoksdata/data/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-11 17:32:26.000000 ewoksdata-0.2.2/src/ewoksdata/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5265 2023-04-11 11:03:11.000000 ewoksdata-0.2.2/src/ewoksdata/data/bliss.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:32:32.000000 ewoksdata-0.2.2/src/ewoksdata/data/hdf5/
--rw-rw-rw-   0 root         (0) root         (0)      622 2023-04-11 17:28:37.000000 ewoksdata-0.2.2/src/ewoksdata/data/hdf5/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6085 2023-04-11 11:03:11.000000 ewoksdata-0.2.2/src/ewoksdata/data/hdf5/config.py
--rw-rw-rw-   0 root         (0) root         (0)     3373 2023-04-11 17:28:37.000000 ewoksdata-0.2.2/src/ewoksdata/data/hdf5/dataset_writer.py
--rw-rw-rw-   0 root         (0) root         (0)      474 2023-04-11 11:03:11.000000 ewoksdata-0.2.2/src/ewoksdata/data/hdf5/types.py
--rw-rw-rw-   0 root         (0) root         (0)     3057 2023-04-11 17:28:37.000000 ewoksdata-0.2.2/src/ewoksdata/data/nexus.py
--rw-rw-rw-   0 root         (0) root         (0)      354 2023-04-11 11:03:11.000000 ewoksdata-0.2.2/src/ewoksdata/data/url.py
--rw-rw-rw-   0 root         (0) root         (0)      722 2023-04-11 11:03:11.000000 ewoksdata-0.2.2/src/ewoksdata/data/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:32:32.000000 ewoksdata-0.2.2/src/ewoksdata/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-11 17:32:26.000000 ewoksdata-0.2.2/src/ewoksdata/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      508 2023-04-11 11:03:11.000000 ewoksdata-0.2.2/src/ewoksdata/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:32:32.000000 ewoksdata-0.2.2/src/ewoksdata/tests/data/
--rw-rw-rw-   0 root         (0) root         (0)       40 2023-04-11 11:03:11.000000 ewoksdata-0.2.2/src/ewoksdata/tests/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3468 2023-04-11 11:03:11.000000 ewoksdata-0.2.2/src/ewoksdata/tests/data/bliss_scans.py
--rw-rw-rw-   0 root         (0) root         (0)      906 2023-04-11 11:03:11.000000 ewoksdata-0.2.2/src/ewoksdata/tests/test_data_bliss.py
--rw-rw-rw-   0 root         (0) root         (0)      505 2023-04-11 11:03:11.000000 ewoksdata-0.2.2/src/ewoksdata/tests/test_data_hdf5.py
--rw-rw-rw-   0 root         (0) root         (0)     1095 2023-04-11 17:28:37.000000 ewoksdata-0.2.2/src/ewoksdata/tests/test_data_nexus.py
--rw-rw-rw-   0 root         (0) root         (0)      570 2023-04-11 11:03:11.000000 ewoksdata-0.2.2/src/ewoksdata/tests/test_dataset_writer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 17:32:32.000000 ewoksdata-0.2.2/src/ewoksdata.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1020 2023-04-11 17:32:32.000000 ewoksdata-0.2.2/src/ewoksdata.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      850 2023-04-11 17:32:32.000000 ewoksdata-0.2.2/src/ewoksdata.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 17:32:32.000000 ewoksdata-0.2.2/src/ewoksdata.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      207 2023-04-11 17:32:32.000000 ewoksdata-0.2.2/src/ewoksdata.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-04-11 17:32:32.000000 ewoksdata-0.2.2/src/ewoksdata.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:23:37.000000 ewoksdata-0.2.3/
+-rw-rw-rw-   0 root         (0) root         (0)     1102 2023-04-18 11:03:12.000000 ewoksdata-0.2.3/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-04-18 15:23:37.000000 ewoksdata-0.2.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      267 2023-04-18 11:03:12.000000 ewoksdata-0.2.3/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-04-18 11:03:12.000000 ewoksdata-0.2.3/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1256 2023-04-18 15:23:37.000000 ewoksdata-0.2.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-04-18 11:03:12.000000 ewoksdata-0.2.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:23:37.000000 ewoksdata-0.2.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:23:37.000000 ewoksdata-0.2.3/src/ewoksdata/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-04-18 15:21:54.000000 ewoksdata-0.2.3/src/ewoksdata/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:23:37.000000 ewoksdata-0.2.3/src/ewoksdata/data/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 15:23:31.000000 ewoksdata-0.2.3/src/ewoksdata/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7007 2023-04-18 15:13:18.000000 ewoksdata-0.2.3/src/ewoksdata/data/bliss.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:23:37.000000 ewoksdata-0.2.3/src/ewoksdata/data/hdf5/
+-rw-rw-rw-   0 root         (0) root         (0)      622 2023-04-18 11:03:12.000000 ewoksdata-0.2.3/src/ewoksdata/data/hdf5/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6085 2023-04-18 11:03:12.000000 ewoksdata-0.2.3/src/ewoksdata/data/hdf5/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     3925 2023-04-18 15:13:18.000000 ewoksdata-0.2.3/src/ewoksdata/data/hdf5/dataset_writer.py
+-rw-rw-rw-   0 root         (0) root         (0)      474 2023-04-18 11:03:12.000000 ewoksdata-0.2.3/src/ewoksdata/data/hdf5/types.py
+-rw-rw-rw-   0 root         (0) root         (0)     3057 2023-04-18 11:03:12.000000 ewoksdata-0.2.3/src/ewoksdata/data/nexus.py
+-rw-rw-rw-   0 root         (0) root         (0)      354 2023-04-18 11:03:12.000000 ewoksdata-0.2.3/src/ewoksdata/data/url.py
+-rw-rw-rw-   0 root         (0) root         (0)      722 2023-04-18 11:03:12.000000 ewoksdata-0.2.3/src/ewoksdata/data/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:23:37.000000 ewoksdata-0.2.3/src/ewoksdata/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 15:23:31.000000 ewoksdata-0.2.3/src/ewoksdata/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      508 2023-04-18 11:03:12.000000 ewoksdata-0.2.3/src/ewoksdata/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:23:37.000000 ewoksdata-0.2.3/src/ewoksdata/tests/data/
+-rw-rw-rw-   0 root         (0) root         (0)       40 2023-04-18 11:03:12.000000 ewoksdata-0.2.3/src/ewoksdata/tests/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3468 2023-04-18 11:03:12.000000 ewoksdata-0.2.3/src/ewoksdata/tests/data/bliss_scans.py
+-rw-rw-rw-   0 root         (0) root         (0)      906 2023-04-18 11:03:12.000000 ewoksdata-0.2.3/src/ewoksdata/tests/test_data_bliss.py
+-rw-rw-rw-   0 root         (0) root         (0)      505 2023-04-18 11:03:12.000000 ewoksdata-0.2.3/src/ewoksdata/tests/test_data_hdf5.py
+-rw-rw-rw-   0 root         (0) root         (0)     1095 2023-04-18 11:03:12.000000 ewoksdata-0.2.3/src/ewoksdata/tests/test_data_nexus.py
+-rw-rw-rw-   0 root         (0) root         (0)      570 2023-04-18 11:03:12.000000 ewoksdata-0.2.3/src/ewoksdata/tests/test_dataset_writer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:23:37.000000 ewoksdata-0.2.3/src/ewoksdata.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-04-18 15:23:37.000000 ewoksdata-0.2.3/src/ewoksdata.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      850 2023-04-18 15:23:37.000000 ewoksdata-0.2.3/src/ewoksdata.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 15:23:37.000000 ewoksdata-0.2.3/src/ewoksdata.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      207 2023-04-18 15:23:37.000000 ewoksdata-0.2.3/src/ewoksdata.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-04-18 15:23:37.000000 ewoksdata-0.2.3/src/ewoksdata.egg-info/top_level.txt
```

### Comparing `ewoksdata-0.2.2/LICENSE.md` & `ewoksdata-0.2.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.2.2/PKG-INFO` & `ewoksdata-0.2.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ewoksdata
-Version: 0.2.2
+Version: 0.2.3
 Summary: Ewoks tasks for data access
 Home-page: https://gitlab.esrf.fr/workflow/ewoksapps/ewoksdata/
 Author: ESRF
 Author-email: wout.de_nolf@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/workflow/ewoksapps/ewoksdata/
 Project-URL: Documentation, https://ewoksdata.readthedocs.io
```

### Comparing `ewoksdata-0.2.2/setup.cfg` & `ewoksdata-0.2.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.2.2/src/ewoksdata/data/bliss.py` & `ewoksdata-0.2.3/src/ewoksdata/data/bliss.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from numpy.typing import ArrayLike
 from silx.io import h5py_utils
 from silx.utils import retry as retrymod
 from silx.io.utils import get_data as silx_get_data
 from blissdata.h5api import dynamic_hdf5
 
 try:
+    import gevent.queue  # noqa F401 bliss MR 5369
     from blissdata.data.node import get_node
 except ImportError:
     get_node = None
 
 from . import hdf5
 from . import nexus
 from . import url
@@ -128,20 +129,70 @@
 
 def _is_bliss_file(h5item: Union[h5py.Dataset, h5py.Group]) -> bool:
     return h5item.file.attrs.get("creator", "").lower() == "bliss"
 
 
 def last_lima_image(db_name: str) -> ArrayLike:
     """Get last lima image from memory"""
-    if get_node is None:
-        raise ModuleNotFoundError("No module named 'blissdata'")
-    node = get_node(db_name)
-    if node is None:
-        raise RuntimeError(f"Redis node {db_name} does not exist")
-    if node.type != "lima":
-        raise RuntimeError("Not a lima Redis node")
+    node = _get_node(db_name, "lima")
     node.from_stream = True
     dataview = node.get(-1)
-    image = dataview.get_last_live_image()
+    try:
+        image = dataview.get_last_live_image()
+    except AttributeError:
+        image = None
     if image is None or image.data is None:
         raise RuntimeError("Cannot get last image from lima")
     return image.data
+
+
+def iter_bliss_scan_data_from_memory(
+    db_name: str,
+    lima_names: List[str],
+    counter_names: List[str],
+    retry_timeout: Optional[Number],
+    retry_period: Optional[Number],
+):
+    node = _get_node(
+        db_name, "scan", retry_timeout=retry_timeout, retry_period=retry_period
+    )
+    indices = {name: 0 for name in lima_names + counter_names}
+    buffers = {name: list() for name in lima_names + counter_names}
+    for event_type, node, event_data in node.walk_events():
+        if event_type == event_type.END_SCAN:
+            break
+        if node.type == "lima":
+            name = node.db_name.split(":")[-2]
+            if name not in lima_names:
+                continue
+            dataview = node.get(indices[name], -1)
+            data = list(dataview)
+            indices[name] += len(data)
+            buffers[name].extend(data)
+        if node.type == "channel":
+            name = node.db_name.split(":")[-1]
+            if name not in counter_names:
+                continue
+            if event_data:
+                data = event_data.data
+            else:
+                data = node.get_as_array(indices[name], -1)
+            indices[name] += len(data)
+            buffers[name].extend(data)
+        n = min(len(v) for v in buffers.values())
+        if n == 0:
+            continue
+        for i in range(n):
+            yield {name: values[i] for name, values in buffers.items()}
+        buffers = {name: values[n:] for name, values in buffers.items()}
+
+
+@retrymod.retry()
+def _get_node(db_name: str, node_type: str):
+    if get_node is None:
+        raise ModuleNotFoundError("No module named 'blissdata'")
+    node = get_node(db_name)
+    if node is None:
+        raise retrymod.RetryError(f"Redis node {db_name} does not exist")
+    if node.type != node_type:
+        raise RuntimeError(f"Not a Redis {node_type} node")
+    return node
```

### Comparing `ewoksdata-0.2.2/src/ewoksdata/data/hdf5/__init__.py` & `ewoksdata-0.2.3/src/ewoksdata/data/hdf5/__init__.py`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.2.2/src/ewoksdata/data/hdf5/config.py` & `ewoksdata-0.2.3/src/ewoksdata/data/hdf5/config.py`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.2.2/src/ewoksdata/data/hdf5/dataset_writer.py` & `ewoksdata-0.2.3/src/ewoksdata/data/hdf5/dataset_writer.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import time
 from typing import Optional
 
 import h5py
 import numpy
 from numpy.typing import ArrayLike
 
 from .types import StrictPositiveIntegral
@@ -11,25 +12,28 @@
 class DatasetWriter:
     def __init__(
         self,
         parent: h5py.Group,
         name: str,
         npoints: Optional[StrictPositiveIntegral] = None,
         attrs: Optional[dict] = None,
+        flush_period: Optional[float] = None,
     ) -> None:
         self._parent = parent
         self._name = name
         self._attrs = attrs
         self._dataset_name = f"{parent.name}/{name}"
         self._dataset = None
         self._buffer = list()
         self._npoints_added = 0
         self._npoints = npoints
         self._npoints_chunk = None
         self._dataset_idx = 0
+        self._flush_period = flush_period
+        self._last_flush = None
 
     @property
     def dataset_name(self) -> str:
         return self._dataset_name
 
     def __enter__(self) -> "DatasetWriter":
         return self
@@ -85,22 +89,34 @@
             self._dataset = self._create_dataset(data[0])
         self._buffer.extend(data)
         self._npoints_added += len(data)
         return self.flush_buffer(align=True)
 
     def flush_buffer(self, align: bool = False) -> bool:
         nbuffer = len(self._buffer)
-        if align and self._npoints_chunk:
-            nflush = nbuffer // self._npoints_chunk * self._npoints_chunk
-        else:
+        if self._flush_time_expired():
             nflush = nbuffer
+        else:
+            if align and self._npoints_chunk:
+                nflush = nbuffer // self._npoints_chunk * self._npoints_chunk
+            else:
+                nflush = nbuffer
         if nflush == 0:
             return False
         npoints0 = self._dataset.shape[0]
         istart = self._dataset_idx
         npoints1 = istart + nflush
         if self._npoints_chunk and npoints1 > npoints0:
             self._dataset.resize(npoints1, axis=0)
         self._dataset[istart : istart + nflush] = self._buffer[:nflush]
         self._buffer = self._buffer[nflush:]
         self._dataset_idx += nflush
+        self._last_flush = time.time()
         return True
+
+    def _flush_time_expired(self) -> bool:
+        if self._flush_period is None:
+            return False
+        if self._last_flush is None:
+            self._last_flush = time.time()
+            return False
+        return (time.time() - self._last_flush) >= self._flush_period
```

### Comparing `ewoksdata-0.2.2/src/ewoksdata/data/nexus.py` & `ewoksdata-0.2.3/src/ewoksdata/data/nexus.py`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.2.2/src/ewoksdata/data/utils.py` & `ewoksdata-0.2.3/src/ewoksdata/data/utils.py`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.2.2/src/ewoksdata/tests/data/bliss_scans.py` & `ewoksdata-0.2.3/src/ewoksdata/tests/data/bliss_scans.py`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.2.2/src/ewoksdata/tests/test_data_bliss.py` & `ewoksdata-0.2.3/src/ewoksdata/tests/test_data_bliss.py`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.2.2/src/ewoksdata/tests/test_data_nexus.py` & `ewoksdata-0.2.3/src/ewoksdata/tests/test_data_nexus.py`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.2.2/src/ewoksdata/tests/test_dataset_writer.py` & `ewoksdata-0.2.3/src/ewoksdata/tests/test_dataset_writer.py`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.2.2/src/ewoksdata.egg-info/PKG-INFO` & `ewoksdata-0.2.3/src/ewoksdata.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ewoksdata
-Version: 0.2.2
+Version: 0.2.3
 Summary: Ewoks tasks for data access
 Home-page: https://gitlab.esrf.fr/workflow/ewoksapps/ewoksdata/
 Author: ESRF
 Author-email: wout.de_nolf@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/workflow/ewoksapps/ewoksdata/
 Project-URL: Documentation, https://ewoksdata.readthedocs.io
```

### Comparing `ewoksdata-0.2.2/src/ewoksdata.egg-info/SOURCES.txt` & `ewoksdata-0.2.3/src/ewoksdata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

