# Comparing `tmp/ewoksdata-0.2.3.tar.gz` & `tmp/ewoksdata-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ewoksdata-0.2.3.tar", last modified: Tue Apr 18 15:23:37 2023, max compression
+gzip compressed data, was "dist/ewoksdata-0.2.4.tar", last modified: Tue Apr 18 16:13:46 2023, max compression
```

## Comparing `ewoksdata-0.2.3.tar` & `ewoksdata-0.2.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:23:37.000000 ewoksdata-0.2.3/
--rw-rw-rw-   0 root         (0) root         (0)     1102 2023-04-18 11:03:12.000000 ewoksdata-0.2.3/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)     1020 2023-04-18 15:23:37.000000 ewoksdata-0.2.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      267 2023-04-18 11:03:12.000000 ewoksdata-0.2.3/README.md
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-04-18 11:03:12.000000 ewoksdata-0.2.3/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1256 2023-04-18 15:23:37.000000 ewoksdata-0.2.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-04-18 11:03:12.000000 ewoksdata-0.2.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:23:37.000000 ewoksdata-0.2.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:23:37.000000 ewoksdata-0.2.3/src/ewoksdata/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-04-18 15:21:54.000000 ewoksdata-0.2.3/src/ewoksdata/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:23:37.000000 ewoksdata-0.2.3/src/ewoksdata/data/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 15:23:31.000000 ewoksdata-0.2.3/src/ewoksdata/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7007 2023-04-18 15:13:18.000000 ewoksdata-0.2.3/src/ewoksdata/data/bliss.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:23:37.000000 ewoksdata-0.2.3/src/ewoksdata/data/hdf5/
--rw-rw-rw-   0 root         (0) root         (0)      622 2023-04-18 11:03:12.000000 ewoksdata-0.2.3/src/ewoksdata/data/hdf5/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6085 2023-04-18 11:03:12.000000 ewoksdata-0.2.3/src/ewoksdata/data/hdf5/config.py
--rw-rw-rw-   0 root         (0) root         (0)     3925 2023-04-18 15:13:18.000000 ewoksdata-0.2.3/src/ewoksdata/data/hdf5/dataset_writer.py
--rw-rw-rw-   0 root         (0) root         (0)      474 2023-04-18 11:03:12.000000 ewoksdata-0.2.3/src/ewoksdata/data/hdf5/types.py
--rw-rw-rw-   0 root         (0) root         (0)     3057 2023-04-18 11:03:12.000000 ewoksdata-0.2.3/src/ewoksdata/data/nexus.py
--rw-rw-rw-   0 root         (0) root         (0)      354 2023-04-18 11:03:12.000000 ewoksdata-0.2.3/src/ewoksdata/data/url.py
--rw-rw-rw-   0 root         (0) root         (0)      722 2023-04-18 11:03:12.000000 ewoksdata-0.2.3/src/ewoksdata/data/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:23:37.000000 ewoksdata-0.2.3/src/ewoksdata/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 15:23:31.000000 ewoksdata-0.2.3/src/ewoksdata/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      508 2023-04-18 11:03:12.000000 ewoksdata-0.2.3/src/ewoksdata/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:23:37.000000 ewoksdata-0.2.3/src/ewoksdata/tests/data/
--rw-rw-rw-   0 root         (0) root         (0)       40 2023-04-18 11:03:12.000000 ewoksdata-0.2.3/src/ewoksdata/tests/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3468 2023-04-18 11:03:12.000000 ewoksdata-0.2.3/src/ewoksdata/tests/data/bliss_scans.py
--rw-rw-rw-   0 root         (0) root         (0)      906 2023-04-18 11:03:12.000000 ewoksdata-0.2.3/src/ewoksdata/tests/test_data_bliss.py
--rw-rw-rw-   0 root         (0) root         (0)      505 2023-04-18 11:03:12.000000 ewoksdata-0.2.3/src/ewoksdata/tests/test_data_hdf5.py
--rw-rw-rw-   0 root         (0) root         (0)     1095 2023-04-18 11:03:12.000000 ewoksdata-0.2.3/src/ewoksdata/tests/test_data_nexus.py
--rw-rw-rw-   0 root         (0) root         (0)      570 2023-04-18 11:03:12.000000 ewoksdata-0.2.3/src/ewoksdata/tests/test_dataset_writer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:23:37.000000 ewoksdata-0.2.3/src/ewoksdata.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1020 2023-04-18 15:23:37.000000 ewoksdata-0.2.3/src/ewoksdata.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      850 2023-04-18 15:23:37.000000 ewoksdata-0.2.3/src/ewoksdata.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 15:23:37.000000 ewoksdata-0.2.3/src/ewoksdata.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      207 2023-04-18 15:23:37.000000 ewoksdata-0.2.3/src/ewoksdata.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-04-18 15:23:37.000000 ewoksdata-0.2.3/src/ewoksdata.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 16:13:46.000000 ewoksdata-0.2.4/
+-rw-rw-rw-   0 root         (0) root         (0)     1102 2023-04-18 11:03:12.000000 ewoksdata-0.2.4/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-04-18 16:13:46.000000 ewoksdata-0.2.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      267 2023-04-18 11:03:12.000000 ewoksdata-0.2.4/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-04-18 11:03:12.000000 ewoksdata-0.2.4/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1256 2023-04-18 16:13:46.000000 ewoksdata-0.2.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-04-18 11:03:12.000000 ewoksdata-0.2.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 16:13:46.000000 ewoksdata-0.2.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 16:13:46.000000 ewoksdata-0.2.4/src/ewoksdata/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-04-18 16:12:04.000000 ewoksdata-0.2.4/src/ewoksdata/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 16:13:46.000000 ewoksdata-0.2.4/src/ewoksdata/data/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 16:13:40.000000 ewoksdata-0.2.4/src/ewoksdata/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7007 2023-04-18 15:13:18.000000 ewoksdata-0.2.4/src/ewoksdata/data/bliss.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 16:13:46.000000 ewoksdata-0.2.4/src/ewoksdata/data/hdf5/
+-rw-rw-rw-   0 root         (0) root         (0)      622 2023-04-18 11:03:12.000000 ewoksdata-0.2.4/src/ewoksdata/data/hdf5/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6085 2023-04-18 11:03:12.000000 ewoksdata-0.2.4/src/ewoksdata/data/hdf5/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     4017 2023-04-18 16:12:04.000000 ewoksdata-0.2.4/src/ewoksdata/data/hdf5/dataset_writer.py
+-rw-rw-rw-   0 root         (0) root         (0)      474 2023-04-18 11:03:12.000000 ewoksdata-0.2.4/src/ewoksdata/data/hdf5/types.py
+-rw-rw-rw-   0 root         (0) root         (0)     3057 2023-04-18 11:03:12.000000 ewoksdata-0.2.4/src/ewoksdata/data/nexus.py
+-rw-rw-rw-   0 root         (0) root         (0)      354 2023-04-18 11:03:12.000000 ewoksdata-0.2.4/src/ewoksdata/data/url.py
+-rw-rw-rw-   0 root         (0) root         (0)      722 2023-04-18 11:03:12.000000 ewoksdata-0.2.4/src/ewoksdata/data/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 16:13:46.000000 ewoksdata-0.2.4/src/ewoksdata/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 16:13:40.000000 ewoksdata-0.2.4/src/ewoksdata/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      508 2023-04-18 11:03:12.000000 ewoksdata-0.2.4/src/ewoksdata/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 16:13:46.000000 ewoksdata-0.2.4/src/ewoksdata/tests/data/
+-rw-rw-rw-   0 root         (0) root         (0)       40 2023-04-18 11:03:12.000000 ewoksdata-0.2.4/src/ewoksdata/tests/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3468 2023-04-18 11:03:12.000000 ewoksdata-0.2.4/src/ewoksdata/tests/data/bliss_scans.py
+-rw-rw-rw-   0 root         (0) root         (0)      906 2023-04-18 11:03:12.000000 ewoksdata-0.2.4/src/ewoksdata/tests/test_data_bliss.py
+-rw-rw-rw-   0 root         (0) root         (0)      505 2023-04-18 11:03:12.000000 ewoksdata-0.2.4/src/ewoksdata/tests/test_data_hdf5.py
+-rw-rw-rw-   0 root         (0) root         (0)     1095 2023-04-18 11:03:12.000000 ewoksdata-0.2.4/src/ewoksdata/tests/test_data_nexus.py
+-rw-rw-rw-   0 root         (0) root         (0)     1886 2023-04-18 16:12:04.000000 ewoksdata-0.2.4/src/ewoksdata/tests/test_dataset_writer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 16:13:46.000000 ewoksdata-0.2.4/src/ewoksdata.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-04-18 16:13:46.000000 ewoksdata-0.2.4/src/ewoksdata.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      850 2023-04-18 16:13:46.000000 ewoksdata-0.2.4/src/ewoksdata.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 16:13:46.000000 ewoksdata-0.2.4/src/ewoksdata.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      207 2023-04-18 16:13:46.000000 ewoksdata-0.2.4/src/ewoksdata.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-04-18 16:13:46.000000 ewoksdata-0.2.4/src/ewoksdata.egg-info/top_level.txt
```

### Comparing `ewoksdata-0.2.3/LICENSE.md` & `ewoksdata-0.2.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.2.3/PKG-INFO` & `ewoksdata-0.2.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ewoksdata
-Version: 0.2.3
+Version: 0.2.4
 Summary: Ewoks tasks for data access
 Home-page: https://gitlab.esrf.fr/workflow/ewoksapps/ewoksdata/
 Author: ESRF
 Author-email: wout.de_nolf@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/workflow/ewoksapps/ewoksdata/
 Project-URL: Documentation, https://ewoksdata.readthedocs.io
```

### Comparing `ewoksdata-0.2.3/setup.cfg` & `ewoksdata-0.2.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.2.3/src/ewoksdata/data/bliss.py` & `ewoksdata-0.2.4/src/ewoksdata/data/bliss.py`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.2.3/src/ewoksdata/data/hdf5/__init__.py` & `ewoksdata-0.2.4/src/ewoksdata/data/hdf5/__init__.py`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.2.3/src/ewoksdata/data/hdf5/config.py` & `ewoksdata-0.2.4/src/ewoksdata/data/hdf5/config.py`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.2.3/src/ewoksdata/data/hdf5/dataset_writer.py` & `ewoksdata-0.2.4/src/ewoksdata/data/hdf5/dataset_writer.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         self._attrs = attrs
         self._dataset_name = f"{parent.name}/{name}"
         self._dataset = None
         self._buffer = list()
         self._npoints_added = 0
         self._npoints = npoints
         self._npoints_chunk = None
-        self._dataset_idx = 0
+        self._npoints_flushed = 0
         self._flush_period = flush_period
         self._last_flush = None
 
     @property
     def dataset_name(self) -> str:
         return self._dataset_name
 
@@ -91,29 +91,30 @@
         self._npoints_added += len(data)
         return self.flush_buffer(align=True)
 
     def flush_buffer(self, align: bool = False) -> bool:
         nbuffer = len(self._buffer)
         if self._flush_time_expired():
             nflush = nbuffer
+        elif align and self._npoints_chunk:
+            n = nbuffer + (self._npoints_flushed % self._npoints_chunk)
+            nflush = n // self._npoints_chunk * self._npoints_chunk
+            nflush = min(nflush, nbuffer)
         else:
-            if align and self._npoints_chunk:
-                nflush = nbuffer // self._npoints_chunk * self._npoints_chunk
-            else:
-                nflush = nbuffer
+            nflush = nbuffer
         if nflush == 0:
             return False
         npoints0 = self._dataset.shape[0]
-        istart = self._dataset_idx
+        istart = self._npoints_flushed
         npoints1 = istart + nflush
         if self._npoints_chunk and npoints1 > npoints0:
             self._dataset.resize(npoints1, axis=0)
         self._dataset[istart : istart + nflush] = self._buffer[:nflush]
         self._buffer = self._buffer[nflush:]
-        self._dataset_idx += nflush
+        self._npoints_flushed += nflush
         self._last_flush = time.time()
         return True
 
     def _flush_time_expired(self) -> bool:
         if self._flush_period is None:
             return False
         if self._last_flush is None:
```

### Comparing `ewoksdata-0.2.3/src/ewoksdata/data/nexus.py` & `ewoksdata-0.2.4/src/ewoksdata/data/nexus.py`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.2.3/src/ewoksdata/data/utils.py` & `ewoksdata-0.2.4/src/ewoksdata/data/utils.py`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.2.3/src/ewoksdata/tests/data/bliss_scans.py` & `ewoksdata-0.2.4/src/ewoksdata/tests/data/bliss_scans.py`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.2.3/src/ewoksdata/tests/test_data_bliss.py` & `ewoksdata-0.2.4/src/ewoksdata/tests/test_data_bliss.py`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.2.3/src/ewoksdata/tests/test_data_nexus.py` & `ewoksdata-0.2.4/src/ewoksdata/tests/test_data_nexus.py`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.2.3/src/ewoksdata.egg-info/PKG-INFO` & `ewoksdata-0.2.4/src/ewoksdata.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ewoksdata
-Version: 0.2.3
+Version: 0.2.4
 Summary: Ewoks tasks for data access
 Home-page: https://gitlab.esrf.fr/workflow/ewoksapps/ewoksdata/
 Author: ESRF
 Author-email: wout.de_nolf@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/workflow/ewoksapps/ewoksdata/
 Project-URL: Documentation, https://ewoksdata.readthedocs.io
```

### Comparing `ewoksdata-0.2.3/src/ewoksdata.egg-info/SOURCES.txt` & `ewoksdata-0.2.4/src/ewoksdata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

