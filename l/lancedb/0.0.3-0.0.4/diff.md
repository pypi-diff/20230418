# Comparing `tmp/lancedb-0.0.3.tar.gz` & `tmp/lancedb-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lancedb-0.0.3.tar", last modified: Fri Mar 31 02:20:12 2023, max compression
+gzip compressed data, was "lancedb-0.0.4.tar", last modified: Tue Apr 18 16:23:07 2023, max compression
```

## Comparing `lancedb-0.0.3.tar` & `lancedb-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 changshe   (501) staff       (20)        0 2023-03-31 02:20:12.998544 lancedb-0.0.3/
--rw-r--r--   0 changshe   (501) staff       (20)      996 2023-03-31 02:20:12.998421 lancedb-0.0.3/PKG-INFO
-drwxr-xr-x   0 changshe   (501) staff       (20)        0 2023-03-31 02:20:12.997038 lancedb-0.0.3/lancedb/
--rw-r--r--   0 changshe   (501) staff       (20)      922 2023-03-18 17:14:30.000000 lancedb-0.0.3/lancedb/__init__.py
--rw-r--r--   0 changshe   (501) staff       (20)      889 2023-03-22 23:02:41.000000 lancedb-0.0.3/lancedb/common.py
--rw-r--r--   0 changshe   (501) staff       (20)     2981 2023-03-24 06:56:52.000000 lancedb-0.0.3/lancedb/context.py
--rw-r--r--   0 changshe   (501) staff       (20)     2756 2023-03-24 06:56:52.000000 lancedb-0.0.3/lancedb/db.py
--rw-r--r--   0 changshe   (501) staff       (20)     3644 2023-03-31 02:15:49.000000 lancedb-0.0.3/lancedb/embeddings.py
--rw-r--r--   0 changshe   (501) staff       (20)     3336 2023-03-24 06:56:52.000000 lancedb-0.0.3/lancedb/query.py
--rw-r--r--   0 changshe   (501) staff       (20)     6561 2023-03-31 02:15:49.000000 lancedb-0.0.3/lancedb/table.py
-drwxr-xr-x   0 changshe   (501) staff       (20)        0 2023-03-31 02:20:12.997581 lancedb-0.0.3/lancedb.egg-info/
--rw-r--r--   0 changshe   (501) staff       (20)      996 2023-03-31 02:20:12.000000 lancedb-0.0.3/lancedb.egg-info/PKG-INFO
--rw-r--r--   0 changshe   (501) staff       (20)      386 2023-03-31 02:20:12.000000 lancedb-0.0.3/lancedb.egg-info/SOURCES.txt
--rw-r--r--   0 changshe   (501) staff       (20)        1 2023-03-31 02:20:12.000000 lancedb-0.0.3/lancedb.egg-info/dependency_links.txt
--rw-r--r--   0 changshe   (501) staff       (20)      143 2023-03-31 02:20:12.000000 lancedb-0.0.3/lancedb.egg-info/requires.txt
--rw-r--r--   0 changshe   (501) staff       (20)        8 2023-03-31 02:20:12.000000 lancedb-0.0.3/lancedb.egg-info/top_level.txt
--rw-r--r--   0 changshe   (501) staff       (20)     1318 2023-03-31 02:19:08.000000 lancedb-0.0.3/pyproject.toml
--rw-r--r--   0 changshe   (501) staff       (20)       38 2023-03-31 02:20:12.998581 lancedb-0.0.3/setup.cfg
--rw-r--r--   0 changshe   (501) staff       (20)      660 2023-03-23 18:53:47.000000 lancedb-0.0.3/setup.py
-drwxr-xr-x   0 changshe   (501) staff       (20)        0 2023-03-31 02:20:12.998219 lancedb-0.0.3/tests/
--rw-r--r--   0 changshe   (501) staff       (20)     1346 2023-03-23 01:47:48.000000 lancedb-0.0.3/tests/test_db.py
--rw-r--r--   0 changshe   (501) staff       (20)     1527 2023-03-31 02:15:49.000000 lancedb-0.0.3/tests/test_embeddings.py
--rw-r--r--   0 changshe   (501) staff       (20)     1814 2023-03-23 01:47:48.000000 lancedb-0.0.3/tests/test_query.py
--rw-r--r--   0 changshe   (501) staff       (20)     2186 2023-03-23 01:47:48.000000 lancedb-0.0.3/tests/test_table.py
+drwxr-xr-x   0 changshe   (501) staff       (20)        0 2023-04-18 16:23:07.529026 lancedb-0.0.4/
+-rw-r--r--   0 changshe   (501) staff       (20)      996 2023-04-18 16:23:07.528901 lancedb-0.0.4/PKG-INFO
+drwxr-xr-x   0 changshe   (501) staff       (20)        0 2023-04-18 16:23:07.527813 lancedb-0.0.4/lancedb/
+-rw-r--r--   0 changshe   (501) staff       (20)      922 2023-03-18 17:14:30.000000 lancedb-0.0.4/lancedb/__init__.py
+-rw-r--r--   0 changshe   (501) staff       (20)      889 2023-03-22 23:02:41.000000 lancedb-0.0.4/lancedb/common.py
+-rw-r--r--   0 changshe   (501) staff       (20)     2981 2023-03-24 06:56:52.000000 lancedb-0.0.4/lancedb/context.py
+-rw-r--r--   0 changshe   (501) staff       (20)     2756 2023-03-24 06:56:52.000000 lancedb-0.0.4/lancedb/db.py
+-rw-r--r--   0 changshe   (501) staff       (20)     3644 2023-03-31 02:15:49.000000 lancedb-0.0.4/lancedb/embeddings.py
+-rw-r--r--   0 changshe   (501) staff       (20)     3336 2023-03-24 06:56:52.000000 lancedb-0.0.4/lancedb/query.py
+-rw-r--r--   0 changshe   (501) staff       (20)     6645 2023-04-18 16:20:06.000000 lancedb-0.0.4/lancedb/table.py
+drwxr-xr-x   0 changshe   (501) staff       (20)        0 2023-04-18 16:23:07.528343 lancedb-0.0.4/lancedb.egg-info/
+-rw-r--r--   0 changshe   (501) staff       (20)      996 2023-04-18 16:23:07.000000 lancedb-0.0.4/lancedb.egg-info/PKG-INFO
+-rw-r--r--   0 changshe   (501) staff       (20)      386 2023-04-18 16:23:07.000000 lancedb-0.0.4/lancedb.egg-info/SOURCES.txt
+-rw-r--r--   0 changshe   (501) staff       (20)        1 2023-04-18 16:23:07.000000 lancedb-0.0.4/lancedb.egg-info/dependency_links.txt
+-rw-r--r--   0 changshe   (501) staff       (20)      143 2023-04-18 16:23:07.000000 lancedb-0.0.4/lancedb.egg-info/requires.txt
+-rw-r--r--   0 changshe   (501) staff       (20)        8 2023-04-18 16:23:07.000000 lancedb-0.0.4/lancedb.egg-info/top_level.txt
+-rw-r--r--   0 changshe   (501) staff       (20)     1318 2023-04-18 16:20:39.000000 lancedb-0.0.4/pyproject.toml
+-rw-r--r--   0 changshe   (501) staff       (20)       38 2023-04-18 16:23:07.529062 lancedb-0.0.4/setup.cfg
+-rw-r--r--   0 changshe   (501) staff       (20)      660 2023-03-23 18:53:47.000000 lancedb-0.0.4/setup.py
+drwxr-xr-x   0 changshe   (501) staff       (20)        0 2023-04-18 16:23:07.528726 lancedb-0.0.4/tests/
+-rw-r--r--   0 changshe   (501) staff       (20)     1346 2023-03-23 01:47:48.000000 lancedb-0.0.4/tests/test_db.py
+-rw-r--r--   0 changshe   (501) staff       (20)     1527 2023-03-31 02:15:49.000000 lancedb-0.0.4/tests/test_embeddings.py
+-rw-r--r--   0 changshe   (501) staff       (20)     1814 2023-03-23 01:47:48.000000 lancedb-0.0.4/tests/test_query.py
+-rw-r--r--   0 changshe   (501) staff       (20)     3092 2023-04-18 16:20:06.000000 lancedb-0.0.4/tests/test_table.py
```

### Comparing `lancedb-0.0.3/PKG-INFO` & `lancedb-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lancedb
-Version: 0.0.3
+Version: 0.0.4
 Summary: lancedb
 Author-email: Lance Devs <dev@eto.ai>
 Project-URL: repository, https://github.com/eto-ai/lancedb
 Keywords: data-format,data-science,machine-learning,arrow,data-analytics
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
```

### Comparing `lancedb-0.0.3/lancedb/__init__.py` & `lancedb-0.0.4/lancedb/__init__.py`

 * *Files identical despite different names*

### Comparing `lancedb-0.0.3/lancedb/common.py` & `lancedb-0.0.4/lancedb/common.py`

 * *Files identical despite different names*

### Comparing `lancedb-0.0.3/lancedb/context.py` & `lancedb-0.0.4/lancedb/context.py`

 * *Files identical despite different names*

### Comparing `lancedb-0.0.3/lancedb/db.py` & `lancedb-0.0.4/lancedb/db.py`

 * *Files identical despite different names*

### Comparing `lancedb-0.0.3/lancedb/embeddings.py` & `lancedb-0.0.4/lancedb/embeddings.py`

 * *Files identical despite different names*

### Comparing `lancedb-0.0.3/lancedb/query.py` & `lancedb-0.0.4/lancedb/query.py`

 * *Files identical despite different names*

### Comparing `lancedb-0.0.3/lancedb/table.py` & `lancedb-0.0.4/lancedb/table.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,14 +167,15 @@
         vector column to fixed_size_list(float32) if necessary.
     """
     if schema is not None:
         if data.schema == schema:
             return data
         # cast the columns to the expected types
         data = data.combine_chunks()
+        data = _sanitize_vector_column(data, vector_column_name=VECTOR_COLUMN_NAME)
         return pa.Table.from_arrays(
             [data[name] for name in schema.names], schema=schema
         )
     # just check the vector column
     return _sanitize_vector_column(data, vector_column_name=VECTOR_COLUMN_NAME)
```

### Comparing `lancedb-0.0.3/lancedb.egg-info/PKG-INFO` & `lancedb-0.0.4/lancedb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lancedb
-Version: 0.0.3
+Version: 0.0.4
 Summary: lancedb
 Author-email: Lance Devs <dev@eto.ai>
 Project-URL: repository, https://github.com/eto-ai/lancedb
 Keywords: data-format,data-science,machine-learning,arrow,data-analytics
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
```

### Comparing `lancedb-0.0.3/pyproject.toml` & `lancedb-0.0.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "lancedb"
-version = "0.0.3"
+version = "0.0.4"
 dependencies = ["pylance", "ratelimiter", "retry", "tqdm"]
 description = "lancedb"
 authors = [
     { name = "Lance Devs", email = "dev@eto.ai" },
 ]
 license = { file = "LICENSE" }
 readme = "README.md"
```

### Comparing `lancedb-0.0.3/setup.py` & `lancedb-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `lancedb-0.0.3/tests/test_db.py` & `lancedb-0.0.4/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `lancedb-0.0.3/tests/test_embeddings.py` & `lancedb-0.0.4/tests/test_embeddings.py`

 * *Files identical despite different names*

### Comparing `lancedb-0.0.3/tests/test_query.py` & `lancedb-0.0.4/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `lancedb-0.0.3/tests/test_table.py` & `lancedb-0.0.4/tests/test_table.py`

 * *Files 19% similar despite different names*

```diff
@@ -42,25 +42,25 @@
 
     table = LanceTable(db, "test")
     assert table.name == "test"
     assert table.schema == ds.schema
     assert table.to_lance().to_table() == ds.to_table()
 
 
-def test_add(db):
+def test_create_table(db):
     schema = pa.schema(
         [
-            pa.field("vector", pa.list_(pa.float32())),
+            pa.field("vector", pa.list_(pa.float32(), 2)),
             pa.field("item", pa.string()),
             pa.field("price", pa.float32()),
         ]
     )
     expected = pa.Table.from_arrays(
         [
-            pa.array([[3.1, 4.1], [5.9, 26.5]]),
+            pa.FixedSizeListArray.from_arrays(pa.array([3.1, 4.1, 5.9, 26.5]), 2),
             pa.array(["foo", "bar"]),
             pa.array([10.0, 20.0]),
         ],
         schema=schema,
     )
     data = [
         [
@@ -75,7 +75,38 @@
     for i, d in enumerate(data):
         tbl = (
             LanceTable.create(db, f"test_{i}", data=d, schema=schema)
             .to_lance()
             .to_table()
         )
         assert expected == tbl
+
+
+def test_add(db):
+    table = LanceTable.create(
+        db,
+        "test",
+        data=[
+            {"vector": [3.1, 4.1], "item": "foo", "price": 10.0},
+            {"vector": [5.9, 26.5], "item": "bar", "price": 20.0},
+        ],
+    )
+
+    # table = LanceTable(db, "test")
+    assert len(table) == 2
+
+    count = table.add([{"vector": [6.3, 100.5], "item": "new", "price": 30.0}])
+    assert count == 3
+
+    expected = pa.Table.from_arrays(
+        [
+            pa.FixedSizeListArray.from_arrays(pa.array([3.1, 4.1, 5.9, 26.5]), 2),
+            pa.array(["foo", "bar"]),
+            pa.array([10.0, 20.0]),
+        ],
+        schema=pa.schema([
+            pa.field("vector", pa.list_(pa.float32(), 2)),
+            pa.field("item", pa.string()),
+            pa.field("price", pa.float64()),
+        ]),
+    )
+    assert expected == table.to_arrow()
```

