# Comparing `tmp/indxr-0.1.2.tar.gz` & `tmp/indxr-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/indxr-0.1.2.tar", last modified: Wed Feb 15 15:27:04 2023, max compression
+gzip compressed data, was "dist/indxr-0.1.3.tar", last modified: Tue Apr 18 09:08:49 2023, max compression
```

## Comparing `indxr-0.1.2.tar` & `indxr-0.1.3.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 elias      (501) staff       (20)        0 2023-02-15 15:27:04.000000 indxr-0.1.2/
--rw-r--r--   0 elias      (501) staff       (20)     1069 2022-12-02 22:32:06.000000 indxr-0.1.2/LICENSE
--rw-r--r--   0 elias      (501) staff       (20)     7240 2023-02-15 15:27:04.000000 indxr-0.1.2/PKG-INFO
--rw-r--r--   0 elias      (501) staff       (20)     6598 2022-12-02 22:32:06.000000 indxr-0.1.2/README.md
-drwxr-xr-x   0 elias      (501) staff       (20)        0 2023-02-15 15:27:04.000000 indxr-0.1.2/indxr/
--rw-r--r--   0 elias      (501) staff       (20)       53 2022-12-02 22:32:06.000000 indxr-0.1.2/indxr/__init__.py
-drwxr-xr-x   0 elias      (501) staff       (20)        0 2023-02-15 15:27:04.000000 indxr-0.1.2/indxr/handlers/
--rw-r--r--   0 elias      (501) staff       (20)        0 2022-12-02 22:32:06.000000 indxr-0.1.2/indxr/handlers/__init__.py
--rw-r--r--   0 elias      (501) staff       (20)     2542 2022-12-02 22:32:06.000000 indxr-0.1.2/indxr/handlers/csv_handler.py
--rw-r--r--   0 elias      (501) staff       (20)      966 2022-12-02 22:32:06.000000 indxr-0.1.2/indxr/handlers/custom_handler.py
--rw-r--r--   0 elias      (501) staff       (20)     1062 2022-12-02 22:32:06.000000 indxr-0.1.2/indxr/handlers/jsonl_handler.py
--rw-r--r--   0 elias      (501) staff       (20)     1106 2023-02-15 14:36:56.000000 indxr-0.1.2/indxr/handlers/numpy_handler.py
--rw-r--r--   0 elias      (501) staff       (20)      978 2023-02-15 13:58:15.000000 indxr-0.1.2/indxr/handlers/txt_handler.py
--rw-r--r--   0 elias      (501) staff       (20)     6396 2023-02-15 14:38:22.000000 indxr-0.1.2/indxr/indxr.py
-drwxr-xr-x   0 elias      (501) staff       (20)        0 2023-02-15 15:27:04.000000 indxr-0.1.2/indxr.egg-info/
--rw-r--r--   0 elias      (501) staff       (20)     7240 2023-02-15 15:27:04.000000 indxr-0.1.2/indxr.egg-info/PKG-INFO
--rw-r--r--   0 elias      (501) staff       (20)      387 2023-02-15 15:27:04.000000 indxr-0.1.2/indxr.egg-info/SOURCES.txt
--rw-r--r--   0 elias      (501) staff       (20)        1 2023-02-15 15:27:04.000000 indxr-0.1.2/indxr.egg-info/dependency_links.txt
--rw-r--r--   0 elias      (501) staff       (20)       13 2023-02-15 15:27:04.000000 indxr-0.1.2/indxr.egg-info/requires.txt
--rw-r--r--   0 elias      (501) staff       (20)        6 2023-02-15 15:27:04.000000 indxr-0.1.2/indxr.egg-info/top_level.txt
--rw-r--r--   0 elias      (501) staff       (20)       38 2023-02-15 15:27:04.000000 indxr-0.1.2/setup.cfg
--rw-r--r--   0 elias      (501) staff       (20)     1010 2023-02-15 15:27:00.000000 indxr-0.1.2/setup.py
+drwxr-xr-x   0 elias      (501) staff       (20)        0 2023-04-18 09:08:49.000000 indxr-0.1.3/
+-rw-r--r--   0 elias      (501) staff       (20)     1069 2022-12-02 22:32:06.000000 indxr-0.1.3/LICENSE
+-rw-r--r--   0 elias      (501) staff       (20)     7240 2023-04-18 09:08:49.000000 indxr-0.1.3/PKG-INFO
+-rw-r--r--   0 elias      (501) staff       (20)     6598 2022-12-02 22:32:06.000000 indxr-0.1.3/README.md
+drwxr-xr-x   0 elias      (501) staff       (20)        0 2023-04-18 09:08:49.000000 indxr-0.1.3/indxr/
+-rw-r--r--   0 elias      (501) staff       (20)       53 2022-12-02 22:32:06.000000 indxr-0.1.3/indxr/__init__.py
+drwxr-xr-x   0 elias      (501) staff       (20)        0 2023-04-18 09:08:49.000000 indxr-0.1.3/indxr/handlers/
+-rw-r--r--   0 elias      (501) staff       (20)        0 2022-12-02 22:32:06.000000 indxr-0.1.3/indxr/handlers/__init__.py
+-rw-r--r--   0 elias      (501) staff       (20)     2542 2022-12-02 22:32:06.000000 indxr-0.1.3/indxr/handlers/csv_handler.py
+-rw-r--r--   0 elias      (501) staff       (20)      966 2022-12-02 22:32:06.000000 indxr-0.1.3/indxr/handlers/custom_handler.py
+-rw-r--r--   0 elias      (501) staff       (20)     1062 2022-12-02 22:32:06.000000 indxr-0.1.3/indxr/handlers/jsonl_handler.py
+-rw-r--r--   0 elias      (501) staff       (20)      788 2023-04-18 08:53:58.000000 indxr-0.1.3/indxr/handlers/multi_vector_handler.py
+-rw-r--r--   0 elias      (501) staff       (20)     1106 2023-02-15 14:36:56.000000 indxr-0.1.3/indxr/handlers/numpy_handler.py
+-rw-r--r--   0 elias      (501) staff       (20)      978 2023-02-15 13:58:15.000000 indxr-0.1.3/indxr/handlers/txt_handler.py
+-rw-r--r--   0 elias      (501) staff       (20)     7396 2023-04-18 09:05:15.000000 indxr-0.1.3/indxr/indxr.py
+drwxr-xr-x   0 elias      (501) staff       (20)        0 2023-04-18 09:08:49.000000 indxr-0.1.3/indxr.egg-info/
+-rw-r--r--   0 elias      (501) staff       (20)     7240 2023-04-18 09:08:49.000000 indxr-0.1.3/indxr.egg-info/PKG-INFO
+-rw-r--r--   0 elias      (501) staff       (20)      426 2023-04-18 09:08:49.000000 indxr-0.1.3/indxr.egg-info/SOURCES.txt
+-rw-r--r--   0 elias      (501) staff       (20)        1 2023-04-18 09:08:49.000000 indxr-0.1.3/indxr.egg-info/dependency_links.txt
+-rw-r--r--   0 elias      (501) staff       (20)       13 2023-04-18 09:08:49.000000 indxr-0.1.3/indxr.egg-info/requires.txt
+-rw-r--r--   0 elias      (501) staff       (20)        6 2023-04-18 09:08:49.000000 indxr-0.1.3/indxr.egg-info/top_level.txt
+-rw-r--r--   0 elias      (501) staff       (20)       38 2023-04-18 09:08:49.000000 indxr-0.1.3/setup.cfg
+-rw-r--r--   0 elias      (501) staff       (20)     1010 2023-04-18 09:08:12.000000 indxr-0.1.3/setup.py
```

### Comparing `indxr-0.1.2/LICENSE` & `indxr-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `indxr-0.1.2/PKG-INFO` & `indxr-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indxr
-Version: 0.1.2
+Version: 0.1.3
 Summary: indxr: A Python utility for indexing long files.
 Home-page: https://github.com/AmenRa/indxr
 Author: Elias Bassani
 Author-email: elias.bssn@gmail.com
 Keywords: text index,file index,index,indexer,indexing,information retrieval,natural language processing
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `indxr-0.1.2/README.md` & `indxr-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `indxr-0.1.2/indxr/handlers/csv_handler.py` & `indxr-0.1.3/indxr/handlers/csv_handler.py`

 * *Files identical despite different names*

### Comparing `indxr-0.1.2/indxr/handlers/custom_handler.py` & `indxr-0.1.3/indxr/handlers/custom_handler.py`

 * *Files identical despite different names*

### Comparing `indxr-0.1.2/indxr/handlers/jsonl_handler.py` & `indxr-0.1.3/indxr/handlers/jsonl_handler.py`

 * *Files identical despite different names*

### Comparing `indxr-0.1.2/indxr/handlers/numpy_handler.py` & `indxr-0.1.3/indxr/handlers/numpy_handler.py`

 * *Files identical despite different names*

### Comparing `indxr-0.1.2/indxr/handlers/txt_handler.py` & `indxr-0.1.3/indxr/handlers/txt_handler.py`

 * *Files identical despite different names*

### Comparing `indxr-0.1.2/indxr/indxr.py` & `indxr-0.1.3/indxr/indxr.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import numpy as np
 import orjson
 
 from .handlers import (
     csv_handler,
     custom_handler,
     jsonl_handler,
+    multi_vector_handler,
     numpy_handler,
     txt_handler,
 )
 
 
 class Indxr:
     def __init__(
@@ -66,17 +67,24 @@
 
         elif self.kind in {"csv", "tsv"}:
             fieldnames, index = csv_handler.index(self.path, **self.kwargs)
             self.kwargs["fieldnames"] = fieldnames
             return index
 
         elif self.kind == "dat":
-            return numpy_handler.index(
-                self.kwargs["dtype"], self.kwargs["shape"]
-            )
+            if "mapping" in self.kwargs:
+                return multi_vector_handler.index(
+                    self.kwargs["dtype"],
+                    self.kwargs["shape"],
+                    self.kwargs["mapping"],
+                )
+            else:
+                return numpy_handler.index(
+                    self.kwargs["dtype"], self.kwargs["shape"]
+                )
 
         elif self.kind == "custom":
             return custom_handler.index(self.path)
 
         raise NotImplementedError("Specified `kind` not supported.")
 
     def get(self, idx: Union[str, int]) -> Union[str, Dict, np.ndarray]:
@@ -93,30 +101,41 @@
                 idx=idx,
                 delimiter=self.kwargs["delimiter"],
                 fieldnames=self.kwargs["fieldnames"],
                 return_dict=self.kwargs["return_dict"],
             )
 
         elif self.kind == "dat":
-            x = numpy_handler.get(
-                path=self.path, index=self.index, idx=str(idx)
-            )
+            if "mapping" in self.kwargs:
+                x = multi_vector_handler.get(
+                    path=self.path,
+                    index=self.index,
+                    mapping=self.kwargs["mapping"],
+                    idx=str(idx),
+                )
+            else:
+                x = numpy_handler.get(
+                    path=self.path, index=self.index, idx=str(idx)
+                )
 
         elif self.kind == "custom":
             x = custom_handler.get(path=self.path, index=self.index, idx=idx)
 
         else:
             raise NotImplementedError()
 
         return self.callback(x) if self.callback else x
 
     def mget(self, indices: List[str]) -> List[Union[str, Dict, np.ndarray]]:
         if self.kind == "txt":
             xs = txt_handler.mget(
-                path=self.path, index=self.index, indices=indices
+                path=self.path,
+                index=self.index,
+                mapping=self.kwargs["mapping"],
+                indices=indices,
             )
 
         elif self.kind == "jsonl":
             xs = jsonl_handler.mget(
                 path=self.path, index=self.index, indices=indices
             )
 
@@ -127,19 +146,27 @@
                 indices=indices,
                 delimiter=self.kwargs["delimiter"],
                 fieldnames=self.kwargs["fieldnames"],
                 return_dict=self.kwargs["return_dict"],
             )
 
         elif self.kind == "dat":
-            xs = numpy_handler.mget(
-                path=self.path,
-                index=self.index,
-                indices=[str(idx) for idx in indices],
-            )
+            if "mapping" in self.kwargs:
+                xs = multi_vector_handler.mget(
+                    path=self.path,
+                    index=self.index,
+                    mapping=self.kwargs["mapping"],
+                    indices=[str(idx) for idx in indices],
+                )
+            else:
+                xs = numpy_handler.mget(
+                    path=self.path,
+                    index=self.index,
+                    indices=[str(idx) for idx in indices],
+                )
 
         elif self.kind == "custom":
             xs = custom_handler.mget(
                 path=self.path, index=self.index, indices=indices
             )
 
         else:
```

### Comparing `indxr-0.1.2/indxr.egg-info/PKG-INFO` & `indxr-0.1.3/indxr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indxr
-Version: 0.1.2
+Version: 0.1.3
 Summary: indxr: A Python utility for indexing long files.
 Home-page: https://github.com/AmenRa/indxr
 Author: Elias Bassani
 Author-email: elias.bssn@gmail.com
 Keywords: text index,file index,index,indexer,indexing,information retrieval,natural language processing
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `indxr-0.1.2/setup.py` & `indxr-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="indxr",
-    version="0.1.2",
+    version="0.1.3",
     author="Elias Bassani",
     author_email="elias.bssn@gmail.com",
     description="indxr: A Python utility for indexing long files.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/AmenRa/indxr",
     packages=setuptools.find_packages(),
```

