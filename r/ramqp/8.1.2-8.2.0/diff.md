# Comparing `tmp/ramqp-8.1.2.tar.gz` & `tmp/ramqp-8.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ramqp-8.1.2.tar", max compression
+gzip compressed data, was "ramqp-8.2.0.tar", max compression
```

## Comparing `ramqp-8.1.2.tar` & `ramqp-8.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0        0        0        0 2023-04-14 23:49:34.753397 ramqp-8.1.2/LICENSES/
--rw-r--r--   0        0        0    15177 2023-04-14 23:49:34.754397 ramqp-8.1.2/LICENSES/MPL-2.0.txt
--rw-r--r--   0        0        0     7466 2023-04-14 23:49:34.754397 ramqp-8.1.2/README.md
--rw-r--r--   0        0        0     1460 2023-04-14 23:50:01.868992 ramqp-8.1.2/pyproject.toml
--rw-r--r--   0        0        0      321 2023-04-14 23:49:34.756398 ramqp-8.1.2/ramqp/__init__.py
--rw-r--r--   0        0        0    13047 2023-04-14 23:49:34.756398 ramqp-8.1.2/ramqp/abstract.py
--rw-r--r--   0        0        0      668 2023-04-14 23:49:34.756398 ramqp-8.1.2/ramqp/amqp.py
--rw-r--r--   0        0        0     2729 2023-04-14 23:49:34.759398 ramqp-8.1.2/ramqp/config.py
--rw-r--r--   0        0        0     8841 2023-04-14 23:49:34.759398 ramqp-8.1.2/ramqp/depends.py
--rw-r--r--   0        0        0     7010 2023-04-14 23:49:34.759398 ramqp-8.1.2/ramqp/metrics.py
--rw-r--r--   0        0        0     8249 2023-04-14 23:49:34.759398 ramqp-8.1.2/ramqp/mo.py
--rw-r--r--   0        0        0        0 2023-04-14 23:49:34.937408 ramqp-8.1.2/ramqp/py.typed
--rw-r--r--   0        0        0     1367 2023-04-14 23:49:34.760398 ramqp-8.1.2/ramqp/utils.py
--rw-r--r--   0        0        0     8361 1970-01-01 00:00:00.000000 ramqp-8.1.2/PKG-INFO
+drwxr-xr-x   0        0        0        0 2023-04-18 12:28:38.373985 ramqp-8.2.0/LICENSES/
+-rw-r--r--   0        0        0    15177 2023-04-18 12:28:38.373985 ramqp-8.2.0/LICENSES/MPL-2.0.txt
+-rw-r--r--   0        0        0     7466 2023-04-18 12:28:38.373985 ramqp-8.2.0/README.md
+-rw-r--r--   0        0        0     1460 2023-04-18 12:28:51.925891 ramqp-8.2.0/pyproject.toml
+-rw-r--r--   0        0        0      321 2023-04-18 12:28:38.375985 ramqp-8.2.0/ramqp/__init__.py
+-rw-r--r--   0        0        0    13047 2023-04-18 12:28:38.375985 ramqp-8.2.0/ramqp/abstract.py
+-rw-r--r--   0        0        0      668 2023-04-18 12:28:38.375985 ramqp-8.2.0/ramqp/amqp.py
+-rw-r--r--   0        0        0     2729 2023-04-18 12:28:38.375985 ramqp-8.2.0/ramqp/config.py
+-rw-r--r--   0        0        0     8841 2023-04-18 12:28:38.375985 ramqp-8.2.0/ramqp/depends.py
+-rw-r--r--   0        0        0     7010 2023-04-18 12:28:38.376985 ramqp-8.2.0/ramqp/metrics.py
+-rw-r--r--   0        0        0     8537 2023-04-18 12:28:38.376985 ramqp-8.2.0/ramqp/mo.py
+-rw-r--r--   0        0        0        0 2023-04-18 12:28:38.418988 ramqp-8.2.0/ramqp/py.typed
+-rw-r--r--   0        0        0     1367 2023-04-18 12:28:38.376985 ramqp-8.2.0/ramqp/utils.py
+-rw-r--r--   0        0        0     8361 1970-01-01 00:00:00.000000 ramqp-8.2.0/PKG-INFO
```

### Comparing `ramqp-8.1.2/LICENSES/MPL-2.0.txt` & `ramqp-8.2.0/LICENSES/MPL-2.0.txt`

 * *Files identical despite different names*

### Comparing `ramqp-8.1.2/README.md` & `ramqp-8.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ramqp-8.1.2/pyproject.toml` & `ramqp-8.2.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ramqp"
-version = "8.1.2"
+version = "8.2.0"
 description = "Rammearkitektur AMQP library (aio_pika wrapper)"
 authors = ["Magenta ApS <info@magenta.dk>"]
 license = "MPL-2.0"
 readme = "README.md"
 homepage = "https://magenta.dk/"
 repository = "https://git.magenta.dk/rammearkitektur/ramqp"
 keywords = ["os2mo", "amqp"]
```

### Comparing `ramqp-8.1.2/ramqp/abstract.py` & `ramqp-8.2.0/ramqp/abstract.py`

 * *Files identical despite different names*

### Comparing `ramqp-8.1.2/ramqp/amqp.py` & `ramqp-8.2.0/ramqp/amqp.py`

 * *Files identical despite different names*

### Comparing `ramqp-8.1.2/ramqp/config.py` & `ramqp-8.2.0/ramqp/config.py`

 * *Files identical despite different names*

### Comparing `ramqp-8.1.2/ramqp/depends.py` & `ramqp-8.2.0/ramqp/depends.py`

 * *Files identical despite different names*

### Comparing `ramqp-8.1.2/ramqp/metrics.py` & `ramqp-8.2.0/ramqp/metrics.py`

 * *Files identical despite different names*

### Comparing `ramqp-8.1.2/ramqp/mo.py` & `ramqp-8.2.0/ramqp/mo.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from ramqp.abstract import AbstractPublishMixin
 from ramqp.abstract import AbstractRouter
 from ramqp.depends import get_payload_as_type
 from ramqp.depends import get_routing_key
 from ramqp.utils import CallbackType
 
 # >>> print("\n".join(((f"\"{'.'.join(x)}\"," for x in itertools.product(["employee", "org_unit", "*"], ["address", "association", "employee", "engagement", "it", "kle", "leave", "manager", "owner", "org_unit", "related_unit", "role", "*"], ["create", "edit", "terminate", "refresh", "*"])))))  # noqa: E501
-_MORoutingKey = Literal[
+_MORoutingKeyOld = Literal[
     "employee.address.create",
     "employee.address.edit",
     "employee.address.terminate",
     "employee.address.refresh",
     "employee.address.*",
     "employee.association.create",
     "employee.association.edit",
@@ -213,15 +213,35 @@
     "*.role.*",
     "*.*.create",
     "*.*.edit",
     "*.*.terminate",
     "*.*.refresh",
     "*.*.*",
 ]
-MORoutingKey = Annotated[_MORoutingKey, Depends(get_routing_key)]
+
+_MORoutingKey = Literal[
+    "address",
+    "association",
+    "class",
+    "engagement",
+    "facet",
+    "itsystem",
+    "ituser",
+    "kle",
+    "leave",
+    "manager",
+    "manager",
+    "org_unit",
+    "owner",
+    "person",
+    "related_unit",
+    "role",
+]
+
+MORoutingKey = Annotated[_MORoutingKey | _MORoutingKeyOld, Depends(get_routing_key)]
 
 
 class _PayloadType(BaseModel):
     """MO AMQP message format.
 
     Args:
         uuid: The UUID of the org-unit or employee.
```

### Comparing `ramqp-8.1.2/ramqp/utils.py` & `ramqp-8.2.0/ramqp/utils.py`

 * *Files identical despite different names*

### Comparing `ramqp-8.1.2/PKG-INFO` & `ramqp-8.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ramqp
-Version: 8.1.2
+Version: 8.2.0
 Summary: Rammearkitektur AMQP library (aio_pika wrapper)
 Home-page: https://magenta.dk/
 License: MPL-2.0
 Keywords: os2mo,amqp
 Author: Magenta ApS
 Author-email: info@magenta.dk
 Requires-Python: >=3.10,<4.0
```

