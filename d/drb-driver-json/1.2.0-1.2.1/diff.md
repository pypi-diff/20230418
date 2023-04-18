# Comparing `tmp/drb-driver-json-1.2.0.tar.gz` & `tmp/drb-driver-json-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drb-driver-json-1.2.0.tar", last modified: Thu Mar 23 15:57:17 2023, max compression
+gzip compressed data, was "drb-driver-json-1.2.1.tar", last modified: Tue Apr 18 12:07:38 2023, max compression
```

## Comparing `drb-driver-json-1.2.0.tar` & `drb-driver-json-1.2.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 15:57:17.910774 drb-driver-json-1.2.0/
--rw-rw-rw-   0 root         (0) root         (0)     7651 2023-01-19 13:55:19.000000 drb-driver-json-1.2.0/LICENCE.txt
--rw-rw-rw-   0 root         (0) root         (0)       59 2022-12-19 09:36:35.000000 drb-driver-json-1.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2956 2023-03-23 15:57:17.910774 drb-driver-json-1.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2413 2023-03-23 14:58:42.000000 drb-driver-json-1.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 15:57:17.898774 drb-driver-json-1.2.0/drb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 15:57:17.898774 drb-driver-json-1.2.0/drb/drivers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 15:57:17.914774 drb-driver-json-1.2.0/drb/drivers/json/
--rw-rw-rw-   0 root         (0) root         (0)      224 2022-12-15 15:25:37.000000 drb-driver-json-1.2.0/drb/drivers/json/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2023-03-23 15:57:17.914774 drb-driver-json-1.2.0/drb/drivers/json/_version.py
--rw-rw-rw-   0 root         (0) root         (0)      903 2022-12-15 15:25:37.000000 drb-driver-json-1.2.0/drb/drivers/json/factory.py
--rw-rw-rw-   0 root         (0) root         (0)     7434 2023-03-23 15:42:13.000000 drb-driver-json-1.2.0/drb/drivers/json/node.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 15:57:17.898774 drb-driver-json-1.2.0/drb/topics/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 15:57:17.906774 drb-driver-json-1.2.0/drb/topics/json/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-15 15:25:37.000000 drb-driver-json-1.2.0/drb/topics/json/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      209 2023-03-23 15:56:39.000000 drb-driver-json-1.2.0/drb/topics/json/cortex.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 15:57:17.910774 drb-driver-json-1.2.0/drb_driver_json.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2956 2023-03-23 15:57:17.000000 drb-driver-json-1.2.0/drb_driver_json.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      709 2023-03-23 15:57:17.000000 drb-driver-json-1.2.0/drb_driver_json.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-23 15:57:17.000000 drb-driver-json-1.2.0/drb_driver_json.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       89 2023-03-23 15:57:17.000000 drb-driver-json-1.2.0/drb_driver_json.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-23 15:57:17.000000 drb-driver-json-1.2.0/drb_driver_json.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       11 2023-03-23 15:57:17.000000 drb-driver-json-1.2.0/drb_driver_json.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-03-23 15:57:17.000000 drb-driver-json-1.2.0/drb_driver_json.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      104 2023-03-23 14:58:42.000000 drb-driver-json-1.2.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       10 2023-03-23 14:58:42.000000 drb-driver-json-1.2.0/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)     1092 2023-03-23 15:57:17.914774 drb-driver-json-1.2.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      134 2023-03-23 14:58:42.000000 drb-driver-json-1.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 15:57:17.910774 drb-driver-json-1.2.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)      582 2022-12-15 15:25:37.000000 drb-driver-json-1.2.0/tests/test_dbr_json_user.py
--rw-rw-rw-   0 root         (0) root         (0)     2364 2023-03-23 14:58:42.000000 drb-driver-json-1.2.0/tests/test_drb_base_node.py
--rw-rw-rw-   0 root         (0) root         (0)     5460 2023-03-23 14:58:42.000000 drb-driver-json-1.2.0/tests/test_drb_json.py
--rw-rw-rw-   0 root         (0) root         (0)      993 2022-12-15 15:25:37.000000 drb-driver-json-1.2.0/tests/test_drb_json_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     1685 2022-12-15 15:25:37.000000 drb-driver-json-1.2.0/tests/test_drb_json_load.py
--rw-rw-rw-   0 root         (0) root         (0)     1548 2023-03-23 14:58:42.000000 drb-driver-json-1.2.0/tests/test_drb_json_signature.py
--rw-rw-rw-   0 root         (0) root         (0)    80044 2023-02-22 15:30:31.000000 drb-driver-json-1.2.0/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 12:07:38.563971 drb-driver-json-1.2.1/
+-rw-rw-rw-   0 root         (0) root         (0)     7651 2023-01-19 13:55:19.000000 drb-driver-json-1.2.1/LICENCE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       59 2022-12-19 09:36:35.000000 drb-driver-json-1.2.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2956 2023-04-18 12:07:38.563971 drb-driver-json-1.2.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2413 2023-03-23 14:58:42.000000 drb-driver-json-1.2.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 12:07:38.503970 drb-driver-json-1.2.1/drb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 12:07:38.503970 drb-driver-json-1.2.1/drb/drivers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 12:07:38.567971 drb-driver-json-1.2.1/drb/drivers/json/
+-rw-rw-rw-   0 root         (0) root         (0)      224 2022-12-15 15:25:37.000000 drb-driver-json-1.2.1/drb/drivers/json/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-04-18 12:07:38.567971 drb-driver-json-1.2.1/drb/drivers/json/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)      903 2022-12-15 15:25:37.000000 drb-driver-json-1.2.1/drb/drivers/json/factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     6684 2023-04-18 11:35:14.000000 drb-driver-json-1.2.1/drb/drivers/json/node.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 12:07:38.503970 drb-driver-json-1.2.1/drb/topics/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 12:07:38.559971 drb-driver-json-1.2.1/drb/topics/json/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-15 15:25:37.000000 drb-driver-json-1.2.1/drb/topics/json/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      209 2023-04-18 12:06:55.000000 drb-driver-json-1.2.1/drb/topics/json/cortex.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 12:07:38.559971 drb-driver-json-1.2.1/drb_driver_json.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2956 2023-04-18 12:07:38.000000 drb-driver-json-1.2.1/drb_driver_json.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      709 2023-04-18 12:07:38.000000 drb-driver-json-1.2.1/drb_driver_json.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 12:07:38.000000 drb-driver-json-1.2.1/drb_driver_json.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       89 2023-04-18 12:07:38.000000 drb-driver-json-1.2.1/drb_driver_json.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 12:07:38.000000 drb-driver-json-1.2.1/drb_driver_json.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       11 2023-04-18 12:07:38.000000 drb-driver-json-1.2.1/drb_driver_json.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-04-18 12:07:38.000000 drb-driver-json-1.2.1/drb_driver_json.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      104 2023-03-23 14:58:42.000000 drb-driver-json-1.2.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       10 2023-03-23 14:58:42.000000 drb-driver-json-1.2.1/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1092 2023-04-18 12:07:38.567971 drb-driver-json-1.2.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      134 2023-03-23 14:58:42.000000 drb-driver-json-1.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 12:07:38.563971 drb-driver-json-1.2.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      582 2022-12-15 15:25:37.000000 drb-driver-json-1.2.1/tests/test_dbr_json_user.py
+-rw-rw-rw-   0 root         (0) root         (0)     2364 2023-03-23 14:58:42.000000 drb-driver-json-1.2.1/tests/test_drb_base_node.py
+-rw-rw-rw-   0 root         (0) root         (0)     5460 2023-03-23 14:58:42.000000 drb-driver-json-1.2.1/tests/test_drb_json.py
+-rw-rw-rw-   0 root         (0) root         (0)      993 2022-12-15 15:25:37.000000 drb-driver-json-1.2.1/tests/test_drb_json_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     1685 2022-12-15 15:25:37.000000 drb-driver-json-1.2.1/tests/test_drb_json_load.py
+-rw-rw-rw-   0 root         (0) root         (0)     1548 2023-03-23 14:58:42.000000 drb-driver-json-1.2.1/tests/test_drb_json_signature.py
+-rw-rw-rw-   0 root         (0) root         (0)    80044 2023-02-22 15:30:31.000000 drb-driver-json-1.2.1/versioneer.py
```

### Comparing `drb-driver-json-1.2.0/LICENCE.txt` & `drb-driver-json-1.2.1/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `drb-driver-json-1.2.0/PKG-INFO` & `drb-driver-json-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drb-driver-json
-Version: 1.2.0
+Version: 1.2.1
 Summary: DRB json driver
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
 License: LGPLv3
 Project-URL: Documentation, https://drb-python.gitlab.io/impl/json
 Project-URL: Source, https://gitlab.com/drb-python/impl/json
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `drb-driver-json-1.2.0/README.md` & `drb-driver-json-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `drb-driver-json-1.2.0/drb/drivers/json/factory.py` & `drb-driver-json-1.2.1/drb/drivers/json/factory.py`

 * *Files identical despite different names*

### Comparing `drb-driver-json-1.2.0/drb/drivers/json/node.py` & `drb-driver-json-1.2.1/drb/drivers/json/node.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,64 +64,45 @@
                 return json.dumps(self._data).encode('utf-8')
             else:
                 return json.dumps(self._data)
 
         raise DrbNotImplementationException(
             f"JsonNode doesn't implement {impl}")
 
-    def has_child(self, name: str = None, namespace: str = None) -> bool:
-        if namespace:
-            return False
-        if name:
-            if isinstance(self._data, dict):
-                for e in self._data.keys():
-                    if e == name:
-                        return True
-                    return False
-            if isinstance(self._data, list):
-                for e in self._data:
-                    if e == name:
-                        return True
-                    return False
-        return isinstance(self._data, dict) or isinstance(self._data, list)
-
     @property
     @deprecated(version='1.2.0',
                 reason='Only bracket browse should be use')
     def children(self) -> List[DrbNode]:
         if self._children is None:
             self._children = []
-            if self.has_child():
-                if isinstance(self._data, list):
-                    self._children = [
-                        JsonNode(path=self.path.path,
-                                 parent=self,
-                                 data=e)
-                        for e in self._data]
-                else:
-                    for e in self._data.keys():
-                        if isinstance(self._data[e], list):
-                            for x in self._data[e]:
-                                self._children.append(
-                                    JsonNode(
-                                        path=Path(self.path.path).joinpath(e)
-                                        .as_posix(),
-                                        parent=self,
-                                        data=x)
-                                )
-                        else:
+            if isinstance(self._data, list):
+                self._children = [
+                    JsonNode(path=self.path.path,
+                             parent=self,
+                             data=e)
+                    for e in self._data]
+            elif isinstance(self._data, dict):
+                for e in self._data.keys():
+                    if isinstance(self._data[e], list):
+                        for x in self._data[e]:
                             self._children.append(
                                 JsonNode(
                                     path=Path(self.path.path).joinpath(e)
                                     .as_posix(),
                                     parent=self,
-                                    data=self._data[e])
+                                    data=x)
                             )
-            else:
-                self._children = []
+                    else:
+                        self._children.append(
+                            JsonNode(
+                                path=Path(self.path.path).joinpath(e)
+                                .as_posix(),
+                                parent=self,
+                                data=self._data[e])
+                        )
         return self._children
 
     def __setitem__(self, key, value):
         raise NotImplementedError(
             'Not supported in this version of drb-driver-json')
 
     def __delitem__(self, key):
```

### Comparing `drb-driver-json-1.2.0/drb_driver_json.egg-info/PKG-INFO` & `drb-driver-json-1.2.1/drb_driver_json.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drb-driver-json
-Version: 1.2.0
+Version: 1.2.1
 Summary: DRB json driver
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
 License: LGPLv3
 Project-URL: Documentation, https://drb-python.gitlab.io/impl/json
 Project-URL: Source, https://gitlab.com/drb-python/impl/json
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `drb-driver-json-1.2.0/drb_driver_json.egg-info/SOURCES.txt` & `drb-driver-json-1.2.1/drb_driver_json.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `drb-driver-json-1.2.0/setup.cfg` & `drb-driver-json-1.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `drb-driver-json-1.2.0/tests/test_dbr_json_user.py` & `drb-driver-json-1.2.1/tests/test_dbr_json_user.py`

 * *Files identical despite different names*

### Comparing `drb-driver-json-1.2.0/tests/test_drb_base_node.py` & `drb-driver-json-1.2.1/tests/test_drb_base_node.py`

 * *Files identical despite different names*

### Comparing `drb-driver-json-1.2.0/tests/test_drb_json.py` & `drb-driver-json-1.2.1/tests/test_drb_json.py`

 * *Files identical despite different names*

### Comparing `drb-driver-json-1.2.0/tests/test_drb_json_factory.py` & `drb-driver-json-1.2.1/tests/test_drb_json_factory.py`

 * *Files identical despite different names*

### Comparing `drb-driver-json-1.2.0/tests/test_drb_json_load.py` & `drb-driver-json-1.2.1/tests/test_drb_json_load.py`

 * *Files identical despite different names*

### Comparing `drb-driver-json-1.2.0/tests/test_drb_json_signature.py` & `drb-driver-json-1.2.1/tests/test_drb_json_signature.py`

 * *Files identical despite different names*

### Comparing `drb-driver-json-1.2.0/versioneer.py` & `drb-driver-json-1.2.1/versioneer.py`

 * *Files identical despite different names*

