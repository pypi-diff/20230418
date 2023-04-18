# Comparing `tmp/unlok-0.1.8.tar.gz` & `tmp/unlok-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unlok-0.1.8.tar", max compression
+gzip compressed data, was "unlok-0.1.9.tar", max compression
```

## Comparing `unlok-0.1.8.tar` & `unlok-0.1.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      335 2023-02-24 17:44:17.297530 unlok-0.1.8/pyproject.toml
--rw-r--r--   0        0        0        8 2022-12-13 15:08:50.308739 unlok-0.1.8/unlok/README.md
--rw-r--r--   0        0        0      102 2022-11-21 14:10:43.876847 unlok-0.1.8/unlok/__init__.py
--rw-r--r--   0        0        0     6612 2023-02-23 16:04:19.787186 unlok-0.1.8/unlok/api/schema.py
--rw-r--r--   0        0        0        0 2022-11-21 14:00:14.667168 unlok-0.1.8/unlok/composition/__init__.py
--rw-r--r--   0        0        0      206 2022-11-21 14:00:14.667168 unlok-0.1.8/unlok/composition/man.py
--rw-r--r--   0        0        0      129 2022-11-21 14:04:08.295889 unlok-0.1.8/unlok/error.py
--rw-r--r--   0        0        0      908 2022-12-15 16:54:14.126407 unlok-0.1.8/unlok/funcs.py
--rw-r--r--   0        0        0     1597 2023-01-19 09:26:52.621324 unlok-0.1.8/unlok/rath.py
--rw-r--r--   0        0        0      588 2022-12-01 12:59:32.107922 unlok-0.1.8/unlok/structures.py
--rw-r--r--   0        0        0      374 2023-01-19 09:24:35.361373 unlok-0.1.8/unlok/unlok.py
--rw-r--r--   0        0        0      621 1970-01-01 00:00:00.000000 unlok-0.1.8/setup.py
--rw-r--r--   0        0        0      395 1970-01-01 00:00:00.000000 unlok-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      335 2023-03-01 15:23:28.458688 unlok-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0        8 2022-12-13 15:08:50.308739 unlok-0.1.9/unlok/README.md
+-rw-r--r--   0        0        0      102 2022-11-21 14:10:43.876847 unlok-0.1.9/unlok/__init__.py
+-rw-r--r--   0        0        0     7020 2023-03-01 13:19:54.456888 unlok-0.1.9/unlok/api/schema.py
+-rw-r--r--   0        0        0        0 2022-11-21 14:00:14.667168 unlok-0.1.9/unlok/composition/__init__.py
+-rw-r--r--   0        0        0      206 2022-11-21 14:00:14.667168 unlok-0.1.9/unlok/composition/man.py
+-rw-r--r--   0        0        0      129 2022-11-21 14:04:08.295889 unlok-0.1.9/unlok/error.py
+-rw-r--r--   0        0        0      908 2022-12-15 16:54:14.126407 unlok-0.1.9/unlok/funcs.py
+-rw-r--r--   0        0        0     1597 2023-01-19 09:26:52.621324 unlok-0.1.9/unlok/rath.py
+-rw-r--r--   0        0        0      588 2022-12-01 12:59:32.107922 unlok-0.1.9/unlok/structures.py
+-rw-r--r--   0        0        0      374 2023-01-19 09:24:35.361373 unlok-0.1.9/unlok/unlok.py
+-rw-r--r--   0        0        0      621 1970-01-01 00:00:00.000000 unlok-0.1.9/setup.py
+-rw-r--r--   0        0        0      395 1970-01-01 00:00:00.000000 unlok-0.1.9/PKG-INFO
```

### Comparing `unlok-0.1.8/unlok/api/schema.py` & `unlok-0.1.9/unlok/api/schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from unlok.funcs import execute, aexecute
-from typing import Tuple, List, Literal, Optional
-from pydantic import Field, BaseModel
+from unlok.funcs import aexecute, execute
+from pydantic import BaseModel, Field
 from enum import Enum
-from rath.scalars import ID
+from typing import List, Literal, Optional, Tuple
 from unlok.rath import UnlokRath
+from rath.scalars import ID
 
 
 class ApplicationClientType(str, Enum):
     """An enumeration."""
 
     CONFIDENTIAL = "CONFIDENTIAL"
     "Confidential"
@@ -124,17 +124,18 @@
 
 
 class Search_scopesQuery(BaseModel):
     options: Optional[Tuple[Optional[Search_scopesQueryOptions], ...]]
 
     class Arguments(BaseModel):
         search: Optional[str] = None
+        values: Optional[List[Optional[ID]]] = None
 
     class Meta:
-        document = "query search_scopes($search: String) {\n  options: scopes(search: $search) {\n    value\n    label\n  }\n}"
+        document = "query search_scopes($search: String, $values: [ID]) {\n  options: scopes(search: $search, values: $values) {\n    value\n    label\n  }\n}"
 
 
 class MeQuery(BaseModel):
     me: Optional[UserFragment]
 
     class Arguments(BaseModel):
         pass
@@ -196,43 +197,55 @@
 
     Returns:
         Optional[ScopeFragment]"""
     return execute(Aget_scopeQuery, {"id": id}, rath=rath).scope
 
 
 async def asearch_scopes(
-    search: Optional[str] = None, rath: UnlokRath = None
+    search: Optional[str] = None,
+    values: Optional[List[Optional[ID]]] = None,
+    rath: UnlokRath = None,
 ) -> Optional[List[Optional[Search_scopesQueryOptions]]]:
     """search_scopes
 
 
 
     Arguments:
         search (Optional[str], optional): search.
+        values (Optional[List[Optional[ID]]], optional): values.
         rath (unlok.rath.UnlokRath, optional): The client we want to use (defaults to the currently active client)
 
     Returns:
         Optional[List[Optional[Search_scopesQueryScopes]]]"""
-    return (await aexecute(Search_scopesQuery, {"search": search}, rath=rath)).scopes
+    return (
+        await aexecute(
+            Search_scopesQuery, {"search": search, "values": values}, rath=rath
+        )
+    ).scopes
 
 
 def search_scopes(
-    search: Optional[str] = None, rath: UnlokRath = None
+    search: Optional[str] = None,
+    values: Optional[List[Optional[ID]]] = None,
+    rath: UnlokRath = None,
 ) -> Optional[List[Optional[Search_scopesQueryOptions]]]:
     """search_scopes
 
 
 
     Arguments:
         search (Optional[str], optional): search.
+        values (Optional[List[Optional[ID]]], optional): values.
         rath (unlok.rath.UnlokRath, optional): The client we want to use (defaults to the currently active client)
 
     Returns:
         Optional[List[Optional[Search_scopesQueryScopes]]]"""
-    return execute(Search_scopesQuery, {"search": search}, rath=rath).scopes
+    return execute(
+        Search_scopesQuery, {"search": search, "values": values}, rath=rath
+    ).scopes
 
 
 async def ame(rath: UnlokRath = None) -> Optional[UserFragment]:
     """me
```

### Comparing `unlok-0.1.8/unlok/funcs.py` & `unlok-0.1.9/unlok/funcs.py`

 * *Files identical despite different names*

### Comparing `unlok-0.1.8/unlok/rath.py` & `unlok-0.1.9/unlok/rath.py`

 * *Files identical despite different names*

### Comparing `unlok-0.1.8/unlok/structures.py` & `unlok-0.1.9/unlok/structures.py`

 * *Files identical despite different names*

### Comparing `unlok-0.1.8/setup.py` & `unlok-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['koil>=0.2.10', 'rath>=0.3.3']
 
 setup_kwargs = {
     'name': 'unlok',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': '',
     'long_description': 'None',
     'author': 'jhnnsrs',
     'author_email': 'jhnnsrs@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

