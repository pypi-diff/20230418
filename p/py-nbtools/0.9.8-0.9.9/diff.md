# Comparing `tmp/py-nbtools-0.9.8.tar.gz` & `tmp/py-nbtools-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-nbtools-0.9.8.tar", last modified: Tue Feb 28 14:05:52 2023, max compression
+gzip compressed data, was "py-nbtools-0.9.9.tar", last modified: Tue Apr 18 09:57:40 2023, max compression
```

## Comparing `py-nbtools-0.9.8.tar` & `py-nbtools-0.9.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 14:05:52.766579 py-nbtools-0.9.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-28 14:05:48.000000 py-nbtools-0.9.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-02-28 14:05:52.766579 py-nbtools-0.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-02-28 14:05:48.000000 py-nbtools-0.9.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 14:05:52.762579 py-nbtools-0.9.8/nbtools/
--rwxr-xr-x   0 runner    (1001) docker     (123)      179 2023-02-28 14:05:48.000000 py-nbtools-0.9.8/nbtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8456 2023-02-28 14:05:48.000000 py-nbtools-0.9.8/nbtools/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 14:05:52.766579 py-nbtools-0.9.8/nbtools/nbstat/
--rwxr-xr-x   0 runner    (1001) docker     (123)      422 2023-02-28 14:05:48.000000 py-nbtools-0.9.8/nbtools/nbstat/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14316 2023-02-28 14:05:48.000000 py-nbtools-0.9.8/nbtools/nbstat/cli.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7093 2023-02-28 14:05:48.000000 py-nbtools-0.9.8/nbtools/nbstat/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     8516 2023-02-28 14:05:48.000000 py-nbtools-0.9.8/nbtools/nbstat/resource_entry.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10022 2023-02-28 14:05:48.000000 py-nbtools-0.9.8/nbtools/nbstat/resource_formatter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    29423 2023-02-28 14:05:48.000000 py-nbtools-0.9.8/nbtools/nbstat/resource_inspector.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24196 2023-02-28 14:05:48.000000 py-nbtools-0.9.8/nbtools/nbstat/resource_table.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3606 2023-02-28 14:05:48.000000 py-nbtools-0.9.8/nbtools/nbstat/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7282 2023-02-28 14:05:48.000000 py-nbtools-0.9.8/nbtools/pylint_notebook.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15931 2023-02-28 14:05:48.000000 py-nbtools-0.9.8/nbtools/run_notebook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 14:05:52.766579 py-nbtools-0.9.8/py_nbtools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-02-28 14:05:52.000000 py-nbtools-0.9.8/py_nbtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-02-28 14:05:52.000000 py-nbtools-0.9.8/py_nbtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-28 14:05:52.000000 py-nbtools-0.9.8/py_nbtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-02-28 14:05:52.000000 py-nbtools-0.9.8/py_nbtools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-28 14:05:52.000000 py-nbtools-0.9.8/py_nbtools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-02-28 14:05:52.000000 py-nbtools-0.9.8/py_nbtools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-28 14:05:52.000000 py-nbtools-0.9.8/py_nbtools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-28 14:05:52.766579 py-nbtools-0.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-02-28 14:05:48.000000 py-nbtools-0.9.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:57:40.782610 py-nbtools-0.9.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-18 09:57:33.000000 py-nbtools-0.9.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-04-18 09:57:40.782610 py-nbtools-0.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-04-18 09:57:33.000000 py-nbtools-0.9.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:57:40.778609 py-nbtools-0.9.9/nbtools/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      179 2023-04-18 09:57:33.000000 py-nbtools-0.9.9/nbtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8456 2023-04-18 09:57:33.000000 py-nbtools-0.9.9/nbtools/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:57:40.782610 py-nbtools-0.9.9/nbtools/nbstat/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      422 2023-04-18 09:57:33.000000 py-nbtools-0.9.9/nbtools/nbstat/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14316 2023-04-18 09:57:33.000000 py-nbtools-0.9.9/nbtools/nbstat/cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7093 2023-04-18 09:57:33.000000 py-nbtools-0.9.9/nbtools/nbstat/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8516 2023-04-18 09:57:33.000000 py-nbtools-0.9.9/nbtools/nbstat/resource_entry.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10022 2023-04-18 09:57:33.000000 py-nbtools-0.9.9/nbtools/nbstat/resource_formatter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29814 2023-04-18 09:57:33.000000 py-nbtools-0.9.9/nbtools/nbstat/resource_inspector.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24196 2023-04-18 09:57:33.000000 py-nbtools-0.9.9/nbtools/nbstat/resource_table.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3606 2023-04-18 09:57:33.000000 py-nbtools-0.9.9/nbtools/nbstat/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7282 2023-04-18 09:57:33.000000 py-nbtools-0.9.9/nbtools/pylint_notebook.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15931 2023-04-18 09:57:33.000000 py-nbtools-0.9.9/nbtools/run_notebook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:57:40.782610 py-nbtools-0.9.9/py_nbtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-04-18 09:57:40.000000 py-nbtools-0.9.9/py_nbtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-18 09:57:40.000000 py-nbtools-0.9.9/py_nbtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 09:57:40.000000 py-nbtools-0.9.9/py_nbtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-18 09:57:40.000000 py-nbtools-0.9.9/py_nbtools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 09:57:40.000000 py-nbtools-0.9.9/py_nbtools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-18 09:57:40.000000 py-nbtools-0.9.9/py_nbtools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-18 09:57:40.000000 py-nbtools-0.9.9/py_nbtools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 09:57:40.782610 py-nbtools-0.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-04-18 09:57:33.000000 py-nbtools-0.9.9/setup.py
```

### Comparing `py-nbtools-0.9.8/LICENSE` & `py-nbtools-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `py-nbtools-0.9.8/PKG-INFO` & `py-nbtools-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-nbtools
-Version: 0.9.8
+Version: 0.9.9
 Summary: A collection of tools for using inside Jupyter Notebooks
 Home-page: https://github.com/analysiscenter/nbtools
 Author: Sergey Tsimfer
 Author-email: sergeytsimfer@gmail.com
 License: Apache License 2.0
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `py-nbtools-0.9.8/README.md` & `py-nbtools-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `py-nbtools-0.9.8/nbtools/core.py` & `py-nbtools-0.9.9/nbtools/core.py`

 * *Files identical despite different names*

### Comparing `py-nbtools-0.9.8/nbtools/nbstat/cli.py` & `py-nbtools-0.9.9/nbtools/nbstat/cli.py`

 * *Files identical despite different names*

### Comparing `py-nbtools-0.9.8/nbtools/nbstat/resource.py` & `py-nbtools-0.9.9/nbtools/nbstat/resource.py`

 * *Files identical despite different names*

### Comparing `py-nbtools-0.9.8/nbtools/nbstat/resource_entry.py` & `py-nbtools-0.9.9/nbtools/nbstat/resource_entry.py`

 * *Files identical despite different names*

### Comparing `py-nbtools-0.9.8/nbtools/nbstat/resource_formatter.py` & `py-nbtools-0.9.9/nbtools/nbstat/resource_formatter.py`

 * *Files identical despite different names*

### Comparing `py-nbtools-0.9.8/nbtools/nbstat/resource_inspector.py` & `py-nbtools-0.9.9/nbtools/nbstat/resource_inspector.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,16 +72,18 @@
         exist in the container namespace. Currently, we don't have a reliable and not overly hacky way of matching it to
         a PID inside the container: we circumwent this problem in the `process_table`.
         """
         formatter = formatter or self.formatter
         device_table, device_process_table = ResourceTable(), ResourceTable()
 
         for device_id, handle in self.device_handles.items():
+            device_name = nvidia_smi.nvmlDeviceGetName(handle)
+            device_name = device_name.decode() if isinstance(device_name, bytes) else device_name
             common_info = {Resource.DEVICE_ID : device_id,
-                           Resource.DEVICE_NAME : nvidia_smi.nvmlDeviceGetName(handle).decode()}
+                           Resource.DEVICE_NAME : device_name}
 
             # Inseparable device information like memory, temperature, power, etc. Request it only if needed
             if (formatter.get(Resource.DEVICE_UTIL, False) or
                 formatter.get(Resource.DEVICE_UTIL_MA, False)):
                 utilization = nvidia_smi.nvmlDeviceGetUtilizationRates(handle)
                 common_info[Resource.DEVICE_UTIL] = utilization.gpu
                 common_info[Resource.DEVICE_MEMORY_UTIL] = utilization.memory
@@ -562,16 +564,22 @@
             lines.insert(separator_position, terminal.separator_symbol * terminal.length(added_line))
         return lines
 
     def add_supheader(self, lines, terminal, interval=None, underline=True, bold=True, separate=True):
         """ Add a supheader with info about current time, driver and CUDA versions. """
         timestamp = time.strftime('%Y-%m-%d %H:%M:%S')
         interval_info = f'Interval: {interval:2.1f}s' if interval is not None else ''
-        driver_version = '.'.join(nvidia_smi.nvmlSystemGetDriverVersion().decode().split('.')[:-1])
-        cuda_version = nvidia_smi.nvmlSystemGetNVMLVersion().decode()[:4]
+
+        driver_version = nvidia_smi.nvmlSystemGetDriverVersion()
+        driver_version = driver_version.decode() if isinstance(driver_version, bytes) else driver_version
+        driver_version = '.'.join(driver_version.split('.')[:-1])
+
+        cuda_version = nvidia_smi.nvmlSystemGetNVMLVersion()
+        cuda_version = cuda_version.decode() if isinstance(cuda_version, bytes) else cuda_version
+        cuda_version = cuda_version[:4]
 
         parts = [
             timestamp,
             f'Driver Version: {driver_version}',
             f'CUDA Version: {cuda_version}',
             interval_info,
         ]
```

### Comparing `py-nbtools-0.9.8/nbtools/nbstat/resource_table.py` & `py-nbtools-0.9.9/nbtools/nbstat/resource_table.py`

 * *Files identical despite different names*

### Comparing `py-nbtools-0.9.8/nbtools/nbstat/utils.py` & `py-nbtools-0.9.9/nbtools/nbstat/utils.py`

 * *Files identical despite different names*

### Comparing `py-nbtools-0.9.8/nbtools/pylint_notebook.py` & `py-nbtools-0.9.9/nbtools/pylint_notebook.py`

 * *Files identical despite different names*

### Comparing `py-nbtools-0.9.8/nbtools/run_notebook.py` & `py-nbtools-0.9.9/nbtools/run_notebook.py`

 * *Files identical despite different names*

### Comparing `py-nbtools-0.9.8/py_nbtools.egg-info/PKG-INFO` & `py-nbtools-0.9.9/py_nbtools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-nbtools
-Version: 0.9.8
+Version: 0.9.9
 Summary: A collection of tools for using inside Jupyter Notebooks
 Home-page: https://github.com/analysiscenter/nbtools
 Author: Sergey Tsimfer
 Author-email: sergeytsimfer@gmail.com
 License: Apache License 2.0
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `py-nbtools-0.9.8/py_nbtools.egg-info/SOURCES.txt` & `py-nbtools-0.9.9/py_nbtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-nbtools-0.9.8/setup.py` & `py-nbtools-0.9.9/setup.py`

 * *Files identical despite different names*

