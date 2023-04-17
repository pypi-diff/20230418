# Comparing `tmp/python_roborock-0.6.5.tar.gz` & `tmp/python_roborock-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_roborock-0.6.5.tar", max compression
+gzip compressed data, was "python_roborock-0.6.6.tar", max compression
```

## Comparing `python_roborock-0.6.5.tar` & `python_roborock-0.6.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    35149 2023-04-13 17:45:45.491427 python_roborock-0.6.5/LICENSE
--rw-r--r--   0        0        0     2122 2023-04-13 17:45:45.491427 python_roborock-0.6.5/README.md
--rw-r--r--   0        0        0     1370 2023-04-13 17:45:46.427436 python_roborock-0.6.5/pyproject.toml
--rw-r--r--   0        0        0      156 2023-04-13 17:45:45.491427 python_roborock-0.6.5/roborock/__init__.py
--rw-r--r--   0        0        0    18886 2023-04-13 17:45:45.491427 python_roborock-0.6.5/roborock/api.py
--rw-r--r--   0        0        0     3991 2023-04-13 17:45:45.491427 python_roborock-0.6.5/roborock/cli.py
--rw-r--r--   0        0        0     8595 2023-04-13 17:45:45.491427 python_roborock-0.6.5/roborock/cloud_api.py
--rw-r--r--   0        0        0     4283 2023-04-13 17:45:45.491427 python_roborock-0.6.5/roborock/code_mappings.py
--rw-r--r--   0        0        0     9404 2023-04-13 17:45:45.495427 python_roborock-0.6.5/roborock/containers.py
--rw-r--r--   0        0        0     1028 2023-04-13 17:45:45.495427 python_roborock-0.6.5/roborock/exceptions.py
--rw-r--r--   0        0        0     7217 2023-04-13 17:45:45.495427 python_roborock-0.6.5/roborock/local_api.py
--rw-r--r--   0        0        0     6108 2023-04-13 17:45:45.495427 python_roborock-0.6.5/roborock/roborock_message.py
--rw-r--r--   0        0        0      644 2023-04-13 17:45:45.495427 python_roborock-0.6.5/roborock/roborock_queue.py
--rw-r--r--   0        0        0    12762 2023-04-13 17:45:45.495427 python_roborock-0.6.5/roborock/typing.py
--rw-r--r--   0        0        0      868 2023-04-13 17:45:45.495427 python_roborock-0.6.5/roborock/util.py
--rw-r--r--   0        0        0     3339 1970-01-01 00:00:00.000000 python_roborock-0.6.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-17 23:55:00.477835 python_roborock-0.6.6/LICENSE
+-rw-r--r--   0        0        0     2122 2023-04-17 23:55:00.477835 python_roborock-0.6.6/README.md
+-rw-r--r--   0        0        0     1370 2023-04-17 23:55:01.229832 python_roborock-0.6.6/pyproject.toml
+-rw-r--r--   0        0        0      156 2023-04-17 23:55:00.477835 python_roborock-0.6.6/roborock/__init__.py
+-rw-r--r--   0        0        0    18861 2023-04-17 23:55:00.477835 python_roborock-0.6.6/roborock/api.py
+-rw-r--r--   0        0        0     3991 2023-04-17 23:55:00.477835 python_roborock-0.6.6/roborock/cli.py
+-rw-r--r--   0        0        0     8595 2023-04-17 23:55:00.477835 python_roborock-0.6.6/roborock/cloud_api.py
+-rw-r--r--   0        0        0     4283 2023-04-17 23:55:00.477835 python_roborock-0.6.6/roborock/code_mappings.py
+-rw-r--r--   0        0        0     9404 2023-04-17 23:55:00.477835 python_roborock-0.6.6/roborock/containers.py
+-rw-r--r--   0        0        0     1028 2023-04-17 23:55:00.477835 python_roborock-0.6.6/roborock/exceptions.py
+-rw-r--r--   0        0        0     7230 2023-04-17 23:55:00.477835 python_roborock-0.6.6/roborock/local_api.py
+-rw-r--r--   0        0        0     6108 2023-04-17 23:55:00.477835 python_roborock-0.6.6/roborock/roborock_message.py
+-rw-r--r--   0        0        0      644 2023-04-17 23:55:00.477835 python_roborock-0.6.6/roborock/roborock_queue.py
+-rw-r--r--   0        0        0    12762 2023-04-17 23:55:00.477835 python_roborock-0.6.6/roborock/typing.py
+-rw-r--r--   0        0        0      868 2023-04-17 23:55:00.477835 python_roborock-0.6.6/roborock/util.py
+-rw-r--r--   0        0        0     3339 1970-01-01 00:00:00.000000 python_roborock-0.6.6/PKG-INFO
```

### Comparing `python_roborock-0.6.5/LICENSE` & `python_roborock-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.5/README.md` & `python_roborock-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.5/pyproject.toml` & `python_roborock-0.6.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-roborock"
-version = "0.6.5"
+version = "0.6.6"
 description = "A package to control Roborock vacuums."
 authors = ["humbertogontijo <humbertogontijo@users.noreply.github.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 repository = "https://github.com/humbertogontijo/python-roborock"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

### Comparing `python_roborock-0.6.5/roborock/api.py` & `python_roborock-0.6.6/roborock/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,16 +189,16 @@
         return None
 
     async def get_clean_summary(self, device_id: str) -> CleanSummary | None:
         try:
             clean_summary = await self.send_command(device_id, RoborockCommand.GET_CLEAN_SUMMARY)
             if isinstance(clean_summary, dict):
                 return CleanSummary.from_dict(clean_summary)
-            elif isinstance(clean_summary, bytes):
-                return CleanSummary(clean_time=int.from_bytes(clean_summary, "big"))
+            elif isinstance(clean_summary, int):
+                return CleanSummary(clean_time=clean_summary)
         except RoborockTimeout as e:
             _LOGGER.error(e)
         return None
 
     async def get_clean_record(self, device_id: str, record_id: int) -> CleanRecord | None:
         try:
             clean_record = await self.send_command(device_id, RoborockCommand.GET_CLEAN_RECORD, [record_id])
```

### Comparing `python_roborock-0.6.5/roborock/cli.py` & `python_roborock-0.6.6/roborock/cli.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.5/roborock/cloud_api.py` & `python_roborock-0.6.6/roborock/cloud_api.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.5/roborock/code_mappings.py` & `python_roborock-0.6.6/roborock/code_mappings.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.5/roborock/containers.py` & `python_roborock-0.6.6/roborock/containers.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.5/roborock/exceptions.py` & `python_roborock-0.6.6/roborock/exceptions.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.5/roborock/local_api.py` & `python_roborock-0.6.6/roborock/local_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,9 +166,9 @@
             async with self._mutex:
                 async with async_timeout.timeout(self.timeout):
                     await self.loop.sock_sendall(self.socket, data)
         except (asyncio.TimeoutError, asyncio.CancelledError):
             await self.disconnect()
             raise RoborockTimeout(f"Timeout after {self.timeout} seconds waiting for response") from None
         except BrokenPipeError as e:
-            _LOGGER.exception(e)
             await self.disconnect()
+            raise RoborockException(e) from e
```

### Comparing `python_roborock-0.6.5/roborock/roborock_message.py` & `python_roborock-0.6.6/roborock/roborock_message.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.5/roborock/roborock_queue.py` & `python_roborock-0.6.6/roborock/roborock_queue.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.5/roborock/typing.py` & `python_roborock-0.6.6/roborock/typing.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.5/roborock/util.py` & `python_roborock-0.6.6/roborock/util.py`

 * *Files identical despite different names*

### Comparing `python_roborock-0.6.5/PKG-INFO` & `python_roborock-0.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-roborock
-Version: 0.6.5
+Version: 0.6.6
 Summary: A package to control Roborock vacuums.
 Home-page: https://github.com/humbertogontijo/python-roborock
 License: GPL-3.0-only
 Author: humbertogontijo
 Author-email: humbertogontijo@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-roborock Version: 0.6.5 Summary: A package
+Metadata-Version: 2.1 Name: python-roborock Version: 0.6.6 Summary: A package
 to control Roborock vacuums. Home-page: https://github.com/humbertogontijo/
 python-roborock License: GPL-3.0-only Author: humbertogontijo Author-email:
 humbertogontijo@users.noreply.github.com Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: GNU General
 Public License v3 (GPLv3) Classifier: Natural Language :: English Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
```

