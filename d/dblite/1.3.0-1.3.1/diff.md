# Comparing `tmp/dblite-1.3.0.tar.gz` & `tmp/dblite-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dblite-1.3.0.tar", last modified: Mon Mar 27 15:26:15 2023, max compression
+gzip compressed data, was "dblite-1.3.1.tar", last modified: Tue Apr 18 16:02:58 2023, max compression
```

## Comparing `dblite-1.3.0.tar` & `dblite-1.3.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-03-27 15:26:15.532277 dblite-1.3.0/
--rw-rw-r--   0 user      (1000) user      (1000)      967 2023-03-27 15:24:26.000000 dblite-1.3.0/CHANGELOG.md
--rw-rw-r--   0 user      (1000) user      (1000)     6417 2023-03-27 15:25:53.000000 dblite-1.3.0/Doxyfile
--rw-rw-r--   0 user      (1000) user      (1000)     1078 2023-03-27 15:24:26.000000 dblite-1.3.0/LICENSE.md
--rw-rw-r--   0 user      (1000) user      (1000)       95 2023-03-27 15:24:26.000000 dblite-1.3.0/MANIFEST.in
--rw-rw-r--   0 user      (1000) user      (1000)    27112 2023-03-27 15:26:15.532277 dblite-1.3.0/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    21888 2023-03-27 15:24:26.000000 dblite-1.3.0/README.md
--rw-rw-r--   0 user      (1000) user      (1000)       29 2023-03-27 15:24:26.000000 dblite-1.3.0/requirements.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-03-27 15:26:15.532277 dblite-1.3.0/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     2632 2023-03-27 15:24:26.000000 dblite-1.3.0/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-03-27 15:26:15.524277 dblite-1.3.0/src/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-03-27 15:26:15.528277 dblite-1.3.0/src/dblite/
--rw-rw-r--   0 user      (1000) user      (1000)      455 2023-03-27 15:24:26.000000 dblite-1.3.0/src/dblite/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    23720 2023-03-27 15:24:26.000000 dblite-1.3.0/src/dblite/api.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-03-27 15:26:15.528277 dblite-1.3.0/src/dblite/engines/
--rw-rw-r--   0 user      (1000) user      (1000)      925 2023-03-27 15:24:26.000000 dblite-1.3.0/src/dblite/engines/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)    43139 2023-03-27 15:25:53.000000 dblite-1.3.0/src/dblite/engines/postgres.py
--rw-rw-r--   0 user      (1000) user      (1000)    25257 2023-03-27 15:24:26.000000 dblite-1.3.0/src/dblite/engines/sqlite.py
--rw-rw-r--   0 user      (1000) user      (1000)     9970 2023-03-27 15:24:26.000000 dblite-1.3.0/src/dblite/util.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-03-27 15:26:15.528277 dblite-1.3.0/src/dblite.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    27112 2023-03-27 15:26:14.000000 dblite-1.3.0/src/dblite.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      527 2023-03-27 15:26:15.000000 dblite-1.3.0/src/dblite.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-03-27 15:26:14.000000 dblite-1.3.0/src/dblite.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        4 2023-03-27 15:26:14.000000 dblite-1.3.0/src/dblite.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        7 2023-03-27 15:26:14.000000 dblite-1.3.0/src/dblite.egg-info/top_level.txt
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-03-27 15:26:15.528277 dblite-1.3.0/test/
--rwxrwxr-x   0 user      (1000) user      (1000)    30225 2023-03-27 15:24:26.000000 dblite-1.3.0/test/test_api.py
--rwxrwxr-x   0 user      (1000) user      (1000)    15854 2023-03-27 15:24:26.000000 dblite-1.3.0/test/test_orm.py
--rwxrwxr-x   0 user      (1000) user      (1000)     5345 2023-03-27 15:24:26.000000 dblite-1.3.0/test/test_postgres.py
--rwxrwxr-x   0 user      (1000) user      (1000)     7075 2023-03-27 15:24:26.000000 dblite-1.3.0/test/test_row_factory.py
--rwxrwxr-x   0 user      (1000) user      (1000)     5017 2023-03-27 15:24:26.000000 dblite-1.3.0/test/test_sqlite.py
--rwxrwxr-x   0 user      (1000) user      (1000)     4766 2023-03-27 15:24:26.000000 dblite-1.3.0/test/test_transformers.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-18 16:02:58.237924 dblite-1.3.1/
+-rw-rw-r--   0 user      (1000) user      (1000)     1056 2023-04-18 16:01:17.000000 dblite-1.3.1/CHANGELOG.md
+-rw-rw-r--   0 user      (1000) user      (1000)     6417 2023-04-18 16:01:17.000000 dblite-1.3.1/Doxyfile
+-rw-rw-r--   0 user      (1000) user      (1000)     1078 2023-04-18 16:01:17.000000 dblite-1.3.1/LICENSE.md
+-rw-rw-r--   0 user      (1000) user      (1000)       95 2023-04-18 16:01:17.000000 dblite-1.3.1/MANIFEST.in
+-rw-rw-r--   0 user      (1000) user      (1000)    27112 2023-04-18 16:02:58.237924 dblite-1.3.1/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    21888 2023-04-18 16:01:17.000000 dblite-1.3.1/README.md
+-rw-rw-r--   0 user      (1000) user      (1000)       29 2023-04-18 16:01:17.000000 dblite-1.3.1/requirements.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-04-18 16:02:58.237924 dblite-1.3.1/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     2632 2023-04-18 16:01:17.000000 dblite-1.3.1/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-18 16:02:58.233924 dblite-1.3.1/src/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-18 16:02:58.233924 dblite-1.3.1/src/dblite/
+-rw-rw-r--   0 user      (1000) user      (1000)      455 2023-04-18 16:01:17.000000 dblite-1.3.1/src/dblite/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    23720 2023-04-18 16:01:17.000000 dblite-1.3.1/src/dblite/api.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-18 16:02:58.237924 dblite-1.3.1/src/dblite/engines/
+-rw-rw-r--   0 user      (1000) user      (1000)      925 2023-04-18 16:01:17.000000 dblite-1.3.1/src/dblite/engines/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    43223 2023-04-18 16:01:17.000000 dblite-1.3.1/src/dblite/engines/postgres.py
+-rw-rw-r--   0 user      (1000) user      (1000)    25257 2023-04-18 16:01:17.000000 dblite-1.3.1/src/dblite/engines/sqlite.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9970 2023-04-18 16:01:17.000000 dblite-1.3.1/src/dblite/util.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-18 16:02:58.237924 dblite-1.3.1/src/dblite.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    27112 2023-04-18 16:02:57.000000 dblite-1.3.1/src/dblite.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      527 2023-04-18 16:02:57.000000 dblite-1.3.1/src/dblite.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-04-18 16:02:57.000000 dblite-1.3.1/src/dblite.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        4 2023-04-18 16:02:57.000000 dblite-1.3.1/src/dblite.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        7 2023-04-18 16:02:57.000000 dblite-1.3.1/src/dblite.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-04-18 16:02:58.237924 dblite-1.3.1/test/
+-rwxrwxr-x   0 user      (1000) user      (1000)    30225 2023-04-18 16:01:17.000000 dblite-1.3.1/test/test_api.py
+-rwxrwxr-x   0 user      (1000) user      (1000)    15854 2023-04-18 16:01:17.000000 dblite-1.3.1/test/test_orm.py
+-rwxrwxr-x   0 user      (1000) user      (1000)     5345 2023-04-18 16:01:17.000000 dblite-1.3.1/test/test_postgres.py
+-rwxrwxr-x   0 user      (1000) user      (1000)     7075 2023-04-18 16:01:17.000000 dblite-1.3.1/test/test_row_factory.py
+-rwxrwxr-x   0 user      (1000) user      (1000)     5017 2023-04-18 16:01:17.000000 dblite-1.3.1/test/test_sqlite.py
+-rwxrwxr-x   0 user      (1000) user      (1000)     5372 2023-04-18 16:01:17.000000 dblite-1.3.1/test/test_transformers.py
```

### Comparing `dblite-1.3.0/CHANGELOG.md` & `dblite-1.3.1/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 CHANGELOG
 =========
 
+1.3.1, 2023-04-18
+-----------------
+- fix adapting JSON values in Postgres transactions
+
 1.3.0, 2023-03-26
 -----------------
 - add insertmany() and executemany()
 - add attributes Database.ENGINE and Transaction.ENGINE
 
 1.2.0, 2022-12-07
 -----------------
```

### Comparing `dblite-1.3.0/Doxyfile` & `dblite-1.3.1/Doxyfile`

 * *Files identical despite different names*

### Comparing `dblite-1.3.0/LICENSE.md` & `dblite-1.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dblite-1.3.0/PKG-INFO` & `dblite-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dblite
-Version: 1.3.0
+Version: 1.3.1
 Summary: Simple query interface for SQL databases
 Home-page: https://github.com/suurjaak/dblite
 Author: Erki Suurjaak
 Author-email: erki@lap.ee
 License: MIT
 Description: dblite
         ======
```

### Comparing `dblite-1.3.0/README.md` & `dblite-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `dblite-1.3.0/setup.py` & `dblite-1.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `dblite-1.3.0/src/dblite/api.py` & `dblite-1.3.1/src/dblite/api.py`

 * *Files identical despite different names*

### Comparing `dblite-1.3.0/src/dblite/engines/__init__.py` & `dblite-1.3.1/src/dblite/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `dblite-1.3.0/src/dblite/engines/postgres.py` & `dblite-1.3.1/src/dblite/engines/postgres.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 ------------------------------------------------------------------------------
 This file is part of dblite - simple query interface for SQL databases.
 Released under the MIT License.
 
 @author      Erki Suurjaak
 @created     08.05.2020
-@modified    26.03.2023
+@modified    18.04.2023
 ------------------------------------------------------------------------------
 """
 import collections
 from contextlib import contextmanager
 import inspect
 import logging
 import re
@@ -271,15 +271,16 @@
 
 
     def _adapt_value(self, value, typename):
         """
         Returns value as JSON if field is a JSON type and no adapter registered for value type,
         or original value.
         """
-        if typename in ("json", "jsonb") and type(value) not in self.ADAPTERS.values():
+        ADAPTERS = self._db.ADAPTERS if isinstance(self, Transaction) else self.ADAPTERS
+        if typename in ("json", "jsonb") and type(value) not in ADAPTERS.values():
             return psycopg2.extras.Json(value, dumps=util.json_dumps)
         return value
 
 
     def _cast(self, col, val, table=None, tablename=None):
         """Returns column value cast to correct type for use in psycopg."""
         col = col.name if isinstance(col, Identifier) else \
```

### Comparing `dblite-1.3.0/src/dblite/engines/sqlite.py` & `dblite-1.3.1/src/dblite/engines/sqlite.py`

 * *Files identical despite different names*

### Comparing `dblite-1.3.0/src/dblite/util.py` & `dblite-1.3.1/src/dblite/util.py`

 * *Files identical despite different names*

### Comparing `dblite-1.3.0/src/dblite.egg-info/PKG-INFO` & `dblite-1.3.1/src/dblite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dblite
-Version: 1.3.0
+Version: 1.3.1
 Summary: Simple query interface for SQL databases
 Home-page: https://github.com/suurjaak/dblite
 Author: Erki Suurjaak
 Author-email: erki@lap.ee
 License: MIT
 Description: dblite
         ======
```

### Comparing `dblite-1.3.0/src/dblite.egg-info/SOURCES.txt` & `dblite-1.3.1/src/dblite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dblite-1.3.0/test/test_api.py` & `dblite-1.3.1/test/test_api.py`

 * *Files identical despite different names*

### Comparing `dblite-1.3.0/test/test_orm.py` & `dblite-1.3.1/test/test_orm.py`

 * *Files identical despite different names*

### Comparing `dblite-1.3.0/test/test_postgres.py` & `dblite-1.3.1/test/test_postgres.py`

 * *Files identical despite different names*

### Comparing `dblite-1.3.0/test/test_row_factory.py` & `dblite-1.3.1/test/test_row_factory.py`

 * *Files identical despite different names*

### Comparing `dblite-1.3.0/test/test_sqlite.py` & `dblite-1.3.1/test/test_sqlite.py`

 * *Files identical despite different names*

### Comparing `dblite-1.3.0/test/test_transformers.py` & `dblite-1.3.1/test/test_transformers.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 ------------------------------------------------------------------------------
 This file is part of dblite - simple query interface for SQL databases.
 Released under the MIT License.
 
 @author      Erki Suurjaak
 @created     22.11.2022
-@modified    06.12.2022
+@modified    18.04.2023
 ------------------------------------------------------------------------------
 """
 import collections
 import contextlib
 import datetime
 import json
 import logging
@@ -95,36 +95,47 @@
         for i, (engine, (opts, kwargs)) in enumerate(self._connections.items()):
             dblite.api.Engines.DATABASES.clear()  # Clear cache of default databases
             with self.subTest(engine) if hasattr(self, "subTest") else contextlib.nested():  # Py3/2
                 if i: logger.info("-" * 60)
                 dblite.init(opts, **kwargs)
                 dblite.register_adapter(json.dumps, dict)
                 dblite.register_converter(json.loads, "JSON")
-                self.verify_transformers(engine)
+                self.verify_transformers(dblite, engine)
+                self.verify_transformers(dblite.init(), engine)
+                with dblite.transaction() as tx: self.verify_transformers(tx, engine)
                 dblite.close()
 
 
-    def verify_transformers(self, engine):
+    def verify_transformers(self, obj, engine):
         """Verifies adapters and converters."""
-        logger.info("Verifying adapters and converters for %s.", engine)
+        logger.info("Verifying adapters and converters for %s %s.", engine, label(obj))
         for table, cols in self.TABLES.items():
-            dblite.executescript("DROP TABLE IF EXISTS %s" % table)
+            obj.executescript("DROP TABLE IF EXISTS %s" % table)
             if "postgres" == engine:
                 cols = [dict(c, type="TIMESTAMPTZ") if "TIMESTAMP" in c["type"] else c
                         for c in cols]
-            dblite.executescript("CREATE TABLE %s (%s)" %
+            obj.executescript("CREATE TABLE %s (%s)" %
                               (table, ", ".join("%(name)s %(type)s" % c for c in cols)))
 
             for data in self.DATAS[table]:
-                dblite.insert(table, data)
-                row = dblite.fetchone(table, id=data["id"])
-                row["dt"], data["dt"] = (x["dt"].replace(tzinfo=None) for x in (row, data))
-                self.assertEqual(row, data, "Unexpected value from dblite.select().")
+                obj.insert(table, data)
+                row, data = obj.fetchone(table, id=data["id"]), dict(data)
+                row_dt, data_dt = row.pop("dt"), data.pop("dt")  # Zone handling differs in engines
+                self.assertEqual(row, data, "Unexpected value from %s.select()." % label(obj))
+                self.assertEqual(type(row_dt), type(data_dt),
+                                 "Unexpected type for timestamp from %s.select()." % label(obj))
+
+            obj.executescript("DROP TABLE %s" % table)
 
-            dblite.executescript("DROP TABLE %s" % table)
+
+def label(obj):
+    """Returns readable name for logging, for `dblite` module or class instances."""
+    if isinstance(obj, dblite.api.Queryable):
+        return "%s.%s" % (obj.__class__.__module__, obj.__class__.__name__)
+    return obj.__name__
 
 
 
 if "__main__" == __name__:
     logging.basicConfig(
         level=logging.INFO,
         format="[%(levelname)s]\t[%(created).06f] [test_transformers] %(message)s"
```

