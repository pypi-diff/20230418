# Comparing `tmp/djclient-0.0.1a2.tar.gz` & `tmp/djclient-0.0.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djclient-0.0.1a2.tar", max compression
+gzip compressed data, was "djclient-0.0.1a3.tar", max compression
```

## Comparing `djclient-0.0.1a2.tar` & `djclient-0.0.1a3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1081 2023-03-26 08:42:43.476435 djclient-0.0.1a2/LICENSE.txt
--rw-r--r--   0        0        0     2321 2023-04-13 18:17:17.321034 djclient-0.0.1a2/README.md
--rw-r--r--   0        0        0      390 2023-04-18 15:55:39.736912 djclient-0.0.1a2/djclient/__init__.py
--rw-r--r--   0        0        0    21205 2023-04-18 16:44:02.299051 djclient-0.0.1a2/djclient/dj.py
--rw-r--r--   0        0        0      108 2023-04-13 18:17:17.322528 djclient-0.0.1a2/djclient/exceptions.py
--rw-r--r--   0        0        0     1027 2023-04-18 16:01:47.962228 djclient-0.0.1a2/pyproject.toml
--rw-r--r--   0        0        0     3329 1970-01-01 00:00:00.000000 djclient-0.0.1a2/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-03-26 08:42:43.476435 djclient-0.0.1a3/LICENSE.txt
+-rw-r--r--   0        0        0     2475 2023-04-18 18:15:45.682126 djclient-0.0.1a3/README.md
+-rw-r--r--   0        0        0      390 2023-04-18 15:55:39.736912 djclient-0.0.1a3/djclient/__init__.py
+-rw-r--r--   0        0        0    21205 2023-04-18 16:44:02.299051 djclient-0.0.1a3/djclient/dj.py
+-rw-r--r--   0        0        0      108 2023-04-13 18:17:17.322528 djclient-0.0.1a3/djclient/exceptions.py
+-rw-r--r--   0        0        0     1027 2023-04-18 18:19:53.513969 djclient-0.0.1a3/pyproject.toml
+-rw-r--r--   0        0        0     3483 1970-01-01 00:00:00.000000 djclient-0.0.1a3/PKG-INFO
```

### Comparing `djclient-0.0.1a2/LICENSE.txt` & `djclient-0.0.1a3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `djclient-0.0.1a2/README.md` & `djclient-0.0.1a3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -49,91 +49,89 @@
 To attach an engine to a catalog:
 ```python
 catalog.add_engine(engine)
 ```
 
 ### Nodes
 
-All nodes can be found with:
+All nodes for a given namespace can be found with:
 ```python
-dj.nodes()
+dj.namespace("default").nodes()
 ```
 
 Specific node types can be retrieved with:
 ```python
-dj.sources()
-dj.dimensions()
-dj.metrics()
-dj.transforms()
-dj.cubes()
+dj.namespace("default").sources()
+dj.namespace("default").dimensions()
+dj.namespace("default").metrics()
+dj.namespace("default").transforms()
+dj.namespace("default").cubes()
 ```
 
 To create a source node:
 ```python
-from djclient import Source
-repair_orders = Source(
+from djclient import NodeMode
+repair_orders = dj.new_source(
     name="repair_orders",
     display_name="Repair Orders",
     description="Repair orders",
     catalog="dj",
     schema_="roads",
     table="repair_orders",
 )
-repair_orders.publish()
+repair_orders.save(mode=NodeMode.PUBLISHED)
 ```
 
 Nodes can also be created as drafts with:
 ```python
-repair_orders.draft()
+repair_orders.save(mode=NodeMode.DRAFT)
 ```
 
 To create a dimension node:
 ```python
-from djclient import Dimension
-repair_order = Dimension(
+repair_order = dj.new_dimension(
     name="repair_order",
     query="""
     SELECT
       repair_order_id,
       municipality_id,
       hard_hat_id,
       dispatcher_id
     FROM repair_orders
     """,
     description="Repair order dimension",
+    primary_key=["repair_order_id"],
 )
-repair_order.publish()
+repair_order.save()
 ```
 
 To create a transform node:
 ```python
-from djclient import Transform
-large_revenue_payments_only = Transform(
+large_revenue_payments_only = dj.new_transform(
     name="large_revenue_payments_only",
     query="""
     SELECT
       payment_id,
       payment_amount,
       customer_id,
       account_type
     FROM revenue
     WHERE payment_amount > 1000000
     """,
     description="Only large revenue payments",
 )
-large_revenue_payments_only.publish()
+large_revenue_payments_only.save()
 ```
 
 To create a metric:
 ```python
-from djclient import Metric
-num_repair_orders = Metric(
+num_repair_orders = dj.new_metric(
     name="num_repair_orders",
     query="""
     SELECT
       count(repair_order_id) AS num_repair_orders
     FROM repair_orders
     """,
     description="Number of repair orders",
 )
-num_repair_orders.publish()
+num_repair_orders.save()
 ```
```

### Comparing `djclient-0.0.1a2/djclient/dj.py` & `djclient-0.0.1a3/djclient/dj.py`

 * *Files identical despite different names*

### Comparing `djclient-0.0.1a2/pyproject.toml` & `djclient-0.0.1a3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "djclient"
-version = "0.0.1a2"
+version = "0.0.1a3"
 readme = "README.md"
 repository = "https://github.com/DataJunction/dj"
 description = "DataJunction client library for connecting to a DataJunction server"
 authors = ["DataJunction Authors"]
 license = "MIT"
 packages = [
     { include = "djclient" },
```

### Comparing `djclient-0.0.1a2/PKG-INFO` & `djclient-0.0.1a3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djclient
-Version: 0.0.1a2
+Version: 0.0.1a3
 Summary: DataJunction client library for connecting to a DataJunction server
 Home-page: https://github.com/DataJunction/dj
 License: MIT
 Author: DataJunction Authors
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -74,92 +74,90 @@
 To attach an engine to a catalog:
 ```python
 catalog.add_engine(engine)
 ```
 
 ### Nodes
 
-All nodes can be found with:
+All nodes for a given namespace can be found with:
 ```python
-dj.nodes()
+dj.namespace("default").nodes()
 ```
 
 Specific node types can be retrieved with:
 ```python
-dj.sources()
-dj.dimensions()
-dj.metrics()
-dj.transforms()
-dj.cubes()
+dj.namespace("default").sources()
+dj.namespace("default").dimensions()
+dj.namespace("default").metrics()
+dj.namespace("default").transforms()
+dj.namespace("default").cubes()
 ```
 
 To create a source node:
 ```python
-from djclient import Source
-repair_orders = Source(
+from djclient import NodeMode
+repair_orders = dj.new_source(
     name="repair_orders",
     display_name="Repair Orders",
     description="Repair orders",
     catalog="dj",
     schema_="roads",
     table="repair_orders",
 )
-repair_orders.publish()
+repair_orders.save(mode=NodeMode.PUBLISHED)
 ```
 
 Nodes can also be created as drafts with:
 ```python
-repair_orders.draft()
+repair_orders.save(mode=NodeMode.DRAFT)
 ```
 
 To create a dimension node:
 ```python
-from djclient import Dimension
-repair_order = Dimension(
+repair_order = dj.new_dimension(
     name="repair_order",
     query="""
     SELECT
       repair_order_id,
       municipality_id,
       hard_hat_id,
       dispatcher_id
     FROM repair_orders
     """,
     description="Repair order dimension",
+    primary_key=["repair_order_id"],
 )
-repair_order.publish()
+repair_order.save()
 ```
 
 To create a transform node:
 ```python
-from djclient import Transform
-large_revenue_payments_only = Transform(
+large_revenue_payments_only = dj.new_transform(
     name="large_revenue_payments_only",
     query="""
     SELECT
       payment_id,
       payment_amount,
       customer_id,
       account_type
     FROM revenue
     WHERE payment_amount > 1000000
     """,
     description="Only large revenue payments",
 )
-large_revenue_payments_only.publish()
+large_revenue_payments_only.save()
 ```
 
 To create a metric:
 ```python
-from djclient import Metric
-num_repair_orders = Metric(
+num_repair_orders = dj.new_metric(
     name="num_repair_orders",
     query="""
     SELECT
       count(repair_order_id) AS num_repair_orders
     FROM repair_orders
     """,
     description="Number of repair orders",
 )
-num_repair_orders.publish()
+num_repair_orders.save()
 ```
```

