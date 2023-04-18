# Comparing `tmp/followthemoney-store-3.0.3.tar.gz` & `tmp/followthemoney-store-3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "followthemoney-store-3.0.3.tar", last modified: Tue Apr 13 06:10:21 2021, max compression
+gzip compressed data, was "followthemoney-store-3.0.5.tar", last modified: Tue Apr 18 15:43:27 2023, max compression
```

## Comparing `followthemoney-store-3.0.3.tar` & `followthemoney-store-3.0.5.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-13 06:10:21.350467 followthemoney-store-3.0.3/
--rw-r--r--   0 runner    (1001) docker     (121)     1794 2021-04-13 06:10:21.350467 followthemoney-store-3.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      795 2021-04-13 06:09:51.000000 followthemoney-store-3.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-13 06:10:21.346467 followthemoney-store-3.0.3/followthemoney_store.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1794 2021-04-13 06:10:21.000000 followthemoney-store-3.0.3/followthemoney_store.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      466 2021-04-13 06:10:21.000000 followthemoney-store-3.0.3/followthemoney_store.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-13 06:10:21.000000 followthemoney-store-3.0.3/followthemoney_store.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       47 2021-04-13 06:10:21.000000 followthemoney-store-3.0.3/followthemoney_store.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       76 2021-04-13 06:10:21.000000 followthemoney-store-3.0.3/followthemoney_store.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2021-04-13 06:10:21.000000 followthemoney-store-3.0.3/followthemoney_store.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-13 06:10:18.000000 followthemoney-store-3.0.3/followthemoney_store.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-13 06:10:21.350467 followthemoney-store-3.0.3/ftmstore/
--rw-r--r--   0 runner    (1001) docker     (121)      664 2021-04-13 06:09:51.000000 followthemoney-store-3.0.3/ftmstore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3605 2021-04-13 06:09:51.000000 followthemoney-store-3.0.3/ftmstore/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     5895 2021-04-13 06:09:51.000000 followthemoney-store-3.0.3/ftmstore/dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     3809 2021-04-13 06:09:51.000000 followthemoney-store-3.0.3/ftmstore/loader.py
--rw-r--r--   0 runner    (1001) docker     (121)      260 2021-04-13 06:09:51.000000 followthemoney-store-3.0.3/ftmstore/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     1393 2021-04-13 06:09:51.000000 followthemoney-store-3.0.3/ftmstore/store.py
--rw-r--r--   0 runner    (1001) docker     (121)      357 2021-04-13 06:09:51.000000 followthemoney-store-3.0.3/ftmstore/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)       67 2021-04-13 06:10:21.350467 followthemoney-store-3.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1235 2021-04-13 06:09:51.000000 followthemoney-store-3.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:27.422640 followthemoney-store-3.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-18 15:40:58.000000 followthemoney-store-3.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-04-18 15:43:27.422640 followthemoney-store-3.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-18 15:40:58.000000 followthemoney-store-3.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:27.422640 followthemoney-store-3.0.5/followthemoney_store.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-04-18 15:43:27.000000 followthemoney-store-3.0.5/followthemoney_store.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-18 15:43:27.000000 followthemoney-store-3.0.5/followthemoney_store.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 15:43:27.000000 followthemoney-store-3.0.5/followthemoney_store.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-18 15:43:27.000000 followthemoney-store-3.0.5/followthemoney_store.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-18 15:43:27.000000 followthemoney-store-3.0.5/followthemoney_store.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-18 15:43:27.000000 followthemoney-store-3.0.5/followthemoney_store.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 15:41:14.000000 followthemoney-store-3.0.5/followthemoney_store.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:27.422640 followthemoney-store-3.0.5/ftmstore/
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-18 15:40:58.000000 followthemoney-store-3.0.5/ftmstore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-04-18 15:40:58.000000 followthemoney-store-3.0.5/ftmstore/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6036 2023-04-18 15:40:58.000000 followthemoney-store-3.0.5/ftmstore/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-04-18 15:40:58.000000 followthemoney-store-3.0.5/ftmstore/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-18 15:40:58.000000 followthemoney-store-3.0.5/ftmstore/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-18 15:40:58.000000 followthemoney-store-3.0.5/ftmstore/store.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-18 15:40:58.000000 followthemoney-store-3.0.5/ftmstore/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-18 15:43:27.422640 followthemoney-store-3.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-04-18 15:40:58.000000 followthemoney-store-3.0.5/setup.py
```

### Comparing `followthemoney-store-3.0.3/PKG-INFO` & `followthemoney-store-3.0.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,50 +1,50 @@
 Metadata-Version: 2.1
 Name: followthemoney-store
-Version: 3.0.3
+Version: 3.0.5
 Summary: Store raw and structured FollowTheMoney data from different datasets in a data lake
 Home-page: http://github.com/alephdata/followthemoney-store
 Author: Organized Crime and Corruption Reporting Project
 Author-email: data@occrp.org
 License: MIT
-Description: # followthemoney-store
-        
-        This library provides methods to store, fetch and list entities formatted as
-        `followthemoney` data as datasets stored in a SQL backend.
-        
-        ## Usage
-        
-        ### Command-line usage
-        
-        ```bash
-        # Insert a bunch of FtM entities into a store:
-        $ cat ftm-entities.ijson | ftm store write -d my_dataset
-        # Re-create the entities in aggregated form:
-        $ ftm store iterate -d my_dataset | alephclient write-entities -f my_dataset
-        ```
-        
-        If you don't want to keep the balkhash dataset generated above, there's a
-        shortcut that combines the write and iterate functions:
-        
-        ```bash
-        $ cat ftm-entities.ijson | ftm store aggregate | alephclient write-entities -f my_dataset
-        ```
-        
-        ### Python Library
-        
-        ```python
-        from ftmstore import Dataset
-        
-        dataset = Dataset("US-OFAC")
-        dataset.put(entity, fragment='1')
-        ```
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 Provides-Extra: postgresql
+License-File: LICENSE
+
+# followthemoney-store
+
+This library provides methods to store, fetch and list entities formatted as
+`followthemoney` data as datasets stored in a SQL backend.
+
+## Usage
+
+### Command-line usage
+
+```bash
+# Insert a bunch of FtM entities into a store:
+$ cat ftm-entities.ijson | ftm store write -d my_dataset
+# Re-create the entities in aggregated form:
+$ ftm store iterate -d my_dataset | alephclient write-entities -f my_dataset
+```
+
+If you don't want to keep the balkhash dataset generated above, there's a
+shortcut that combines the write and iterate functions:
+
+```bash
+$ cat ftm-entities.ijson | ftm store aggregate | alephclient write-entities -f my_dataset
+```
+
+### Python Library
+
+```python
+from ftmstore import Dataset
+
+dataset = Dataset("US-OFAC")
+dataset.put(entity, fragment='1')
+```
```

### Comparing `followthemoney-store-3.0.3/README.md` & `followthemoney-store-3.0.5/README.md`

 * *Files identical despite different names*

### Comparing `followthemoney-store-3.0.3/followthemoney_store.egg-info/PKG-INFO` & `followthemoney-store-3.0.5/followthemoney_store.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,50 +1,50 @@
 Metadata-Version: 2.1
 Name: followthemoney-store
-Version: 3.0.3
+Version: 3.0.5
 Summary: Store raw and structured FollowTheMoney data from different datasets in a data lake
 Home-page: http://github.com/alephdata/followthemoney-store
 Author: Organized Crime and Corruption Reporting Project
 Author-email: data@occrp.org
 License: MIT
-Description: # followthemoney-store
-        
-        This library provides methods to store, fetch and list entities formatted as
-        `followthemoney` data as datasets stored in a SQL backend.
-        
-        ## Usage
-        
-        ### Command-line usage
-        
-        ```bash
-        # Insert a bunch of FtM entities into a store:
-        $ cat ftm-entities.ijson | ftm store write -d my_dataset
-        # Re-create the entities in aggregated form:
-        $ ftm store iterate -d my_dataset | alephclient write-entities -f my_dataset
-        ```
-        
-        If you don't want to keep the balkhash dataset generated above, there's a
-        shortcut that combines the write and iterate functions:
-        
-        ```bash
-        $ cat ftm-entities.ijson | ftm store aggregate | alephclient write-entities -f my_dataset
-        ```
-        
-        ### Python Library
-        
-        ```python
-        from ftmstore import Dataset
-        
-        dataset = Dataset("US-OFAC")
-        dataset.put(entity, fragment='1')
-        ```
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 Provides-Extra: postgresql
+License-File: LICENSE
+
+# followthemoney-store
+
+This library provides methods to store, fetch and list entities formatted as
+`followthemoney` data as datasets stored in a SQL backend.
+
+## Usage
+
+### Command-line usage
+
+```bash
+# Insert a bunch of FtM entities into a store:
+$ cat ftm-entities.ijson | ftm store write -d my_dataset
+# Re-create the entities in aggregated form:
+$ ftm store iterate -d my_dataset | alephclient write-entities -f my_dataset
+```
+
+If you don't want to keep the balkhash dataset generated above, there's a
+shortcut that combines the write and iterate functions:
+
+```bash
+$ cat ftm-entities.ijson | ftm store aggregate | alephclient write-entities -f my_dataset
+```
+
+### Python Library
+
+```python
+from ftmstore import Dataset
+
+dataset = Dataset("US-OFAC")
+dataset.put(entity, fragment='1')
+```
```

### Comparing `followthemoney-store-3.0.3/ftmstore/__init__.py` & `followthemoney-store-3.0.5/ftmstore/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from ftmstore import settings
 from ftmstore.store import Store
 from ftmstore.dataset import Dataset
 from ftmstore.utils import NULL_ORIGIN
 
 
-__version__ = "3.0.3"
+__version__ = "3.0.5"
 __all__ = ["Dataset", "Store", "get_store", "get_dataset"]
 
 
 @lru_cache(maxsize=6)
 def get_store(database_uri, **config):
     return Store(database_uri=database_uri, **config)
```

### Comparing `followthemoney-store-3.0.3/ftmstore/cli.py` & `followthemoney-store-3.0.5/ftmstore/cli.py`

 * *Files identical despite different names*

### Comparing `followthemoney-store-3.0.3/ftmstore/dataset.py` & `followthemoney-store-3.0.5/ftmstore/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,17 @@
         if entity_id is not None:
             stmt = stmt.where(table.c.id == entity_id)
         if fragment is not None:
             stmt = stmt.where(table.c.fragment == fragment)
         if origin is not None:
             stmt = stmt.where(table.c.origin == origin)
         try:
-            self.store.engine.execute(stmt)
+            with self.store.engine.connect() as conn:
+                conn.execute(stmt)
+                conn.commit()
         except UNDEFINED:
             self.reset()
             raise
 
     def put(self, entity, fragment=None, origin=None):
         bulk = self.bulk()
         bulk.put(entity, fragment=fragment, origin=origin)
@@ -161,12 +163,15 @@
         for entity in self.iterate(entity_id=entity_id):
             return entity
 
     def __iter__(self):
         return self.iterate()
 
     def __len__(self):
-        q = select([func.count(distinct(self.table.c.id))])
-        return self.store.engine.execute(q).scalar()
+        q = select(func.count(distinct(self.table.c.id)))
+        with self.store.engine.connect() as conn:
+            res = conn.execute(q)
+        
+        return res.scalar()
 
     def __repr__(self):
         return "<Dataset(%r, %r)>" % (self.store, self.name)
```

### Comparing `followthemoney-store-3.0.3/ftmstore/loader.py` & `followthemoney-store-3.0.5/ftmstore/loader.py`

 * *Files identical despite different names*

### Comparing `followthemoney-store-3.0.3/ftmstore/store.py` & `followthemoney-store-3.0.5/ftmstore/store.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from normality import slugify
 from sqlalchemy import create_engine, MetaData
-from sqlalchemy.engine.reflection import Inspector
+from sqlalchemy import inspect as sqlalchemy_inspect
 
 from ftmstore import settings
 from ftmstore.dataset import Dataset
 from ftmstore.utils import NULL_ORIGIN
 
 
 class Store(object):
@@ -18,22 +18,22 @@
         **config,
     ):
         self.prefix = prefix
         self.database_uri = database_uri
         # config.setdefault('pool_size', 1)
         self.engine = create_engine(database_uri, **config)
         self.is_postgres = self.engine.dialect.name == "postgresql"
-        self.meta = MetaData(self.engine)
+        self.meta = MetaData()
 
     def get(self, name, origin=NULL_ORIGIN):
         return Dataset(self, name, origin=origin)
 
     def all(self, origin=NULL_ORIGIN):
         prefix = slugify("%s " % self.prefix, sep="_") + "_"
-        inspect = Inspector.from_engine(self.engine)
+        inspect = sqlalchemy_inspect(self.engine)
         for table in inspect.get_table_names():
             if table.startswith(prefix):
                 name = table[len(prefix) :]
                 yield Dataset(self, name, origin=origin)
 
     def close(self):
         self.engine.dispose()
```

### Comparing `followthemoney-store-3.0.3/setup.py` & `followthemoney-store-3.0.5/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md") as f:
     long_description = f.read()
 
-
 setup(
     name="followthemoney-store",
-    version="3.0.3",
+    version="3.0.5",
     description="Store raw and structured FollowTheMoney data from "
     "different datasets in a data lake",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
@@ -23,12 +22,12 @@
     author="Organized Crime and Corruption Reporting Project",
     author_email="data@occrp.org",
     url="http://github.com/alephdata/followthemoney-store",
     license="MIT",
     packages=find_packages(exclude=["ez_setup", "tests"]),
     include_package_data=True,
     zip_safe=True,
-    install_requires=["followthemoney>=1.31.1", "SQLAlchemy>=1.3.1"],
+    install_requires=[],
     extras_require={"postgresql": ["psycopg2-binary>=2.7"]},
     tests_require=[],
     entry_points={"followthemoney.cli": ["store = ftmstore.cli:cli"]},
 )
```

