# Comparing `tmp/datajunction-0.0.1a4.tar.gz` & `tmp/datajunction-0.0.1a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datajunction-0.0.1a4.tar", max compression
+gzip compressed data, was "datajunction-0.0.1a5.tar", max compression
```

## Comparing `datajunction-0.0.1a4.tar` & `datajunction-0.0.1a5.tar`

### file list

```diff
@@ -1,65 +1,66 @@
--rw-r--r--   0        0        0     1081 2023-03-23 18:47:56.715355 datajunction-0.0.1a4/LICENSE.txt
--rw-r--r--   0        0        0     5589 2023-03-23 18:47:56.715553 datajunction-0.0.1a4/README.rst
--rw-r--r--   0        0        0      384 2023-03-23 18:47:56.716046 datajunction-0.0.1a4/dj/__init__.py
--rw-r--r--   0        0        0        0 2023-03-23 18:47:56.716107 datajunction-0.0.1a4/dj/api/__init__.py
--rw-r--r--   0        0        0     4692 2023-04-15 05:07:29.312727 datajunction-0.0.1a4/dj/api/attributes.py
--rw-r--r--   0        0        0     2862 2023-04-15 05:07:29.312961 datajunction-0.0.1a4/dj/api/catalogs.py
--rw-r--r--   0        0        0      654 2023-04-15 05:07:29.313211 datajunction-0.0.1a4/dj/api/cubes.py
--rw-r--r--   0        0        0     4437 2023-04-15 05:07:29.313555 datajunction-0.0.1a4/dj/api/data.py
--rw-r--r--   0        0        0     1457 2023-04-15 05:07:29.313966 datajunction-0.0.1a4/dj/api/engines.py
--rw-r--r--   0        0        0     1220 2023-04-15 05:07:29.314174 datajunction-0.0.1a4/dj/api/health.py
--rw-r--r--   0        0        0    12516 2023-04-15 05:07:29.314478 datajunction-0.0.1a4/dj/api/helpers.py
--rw-r--r--   0        0        0     2995 2023-04-15 05:07:29.315145 datajunction-0.0.1a4/dj/api/main.py
--rw-r--r--   0        0        0     2781 2023-04-15 05:07:29.315496 datajunction-0.0.1a4/dj/api/metrics.py
--rw-r--r--   0        0        0    31233 2023-04-15 05:07:29.316092 datajunction-0.0.1a4/dj/api/nodes.py
--rw-r--r--   0        0        0      702 2023-04-15 05:07:29.316369 datajunction-0.0.1a4/dj/api/query.py
--rw-r--r--   0        0        0     1032 2023-04-15 05:07:29.316543 datajunction-0.0.1a4/dj/api/sql.py
--rw-r--r--   0        0        0     3358 2023-04-15 05:07:29.317020 datajunction-0.0.1a4/dj/api/tags.py
--rw-r--r--   0        0        0     2239 2023-04-12 00:50:10.209059 datajunction-0.0.1a4/dj/config.py
--rw-r--r--   0        0        0      412 2023-03-23 18:47:56.717349 datajunction-0.0.1a4/dj/constants.py
--rwxr-xr-x   0        0        0        0 2023-03-23 18:47:56.717408 datajunction-0.0.1a4/dj/construction/__init__.py
--rwxr-xr-x   0        0        0    16624 2023-04-15 05:07:29.317378 datajunction-0.0.1a4/dj/construction/build.py
--rw-r--r--   0        0        0     6561 2023-04-06 16:56:36.610509 datajunction-0.0.1a4/dj/construction/dj_query.py
--rwxr-xr-x   0        0        0     1495 2023-03-23 18:47:56.717765 datajunction-0.0.1a4/dj/construction/exceptions.py
--rwxr-xr-x   0        0        0     2679 2023-04-13 20:40:03.277515 datajunction-0.0.1a4/dj/construction/utils.py
--rw-r--r--   0        0        0     5900 2023-04-06 16:56:36.610840 datajunction-0.0.1a4/dj/errors.py
--rw-r--r--   0        0        0      518 2023-03-23 19:26:05.392314 datajunction-0.0.1a4/dj/models/__init__.py
--rw-r--r--   0        0        0     2146 2023-03-23 18:47:56.718197 datajunction-0.0.1a4/dj/models/attribute.py
--rw-r--r--   0        0        0     1592 2023-03-23 18:47:56.718254 datajunction-0.0.1a4/dj/models/base.py
--rw-r--r--   0        0        0     2155 2023-03-23 18:47:56.718316 datajunction-0.0.1a4/dj/models/catalog.py
--rw-r--r--   0        0        0     2661 2023-04-06 16:56:36.610968 datajunction-0.0.1a4/dj/models/column.py
--rw-r--r--   0        0        0      858 2023-03-23 18:47:56.718484 datajunction-0.0.1a4/dj/models/cube.py
--rw-r--r--   0        0        0     2019 2023-03-23 19:26:05.392453 datajunction-0.0.1a4/dj/models/database.py
--rw-r--r--   0        0        0      478 2023-03-23 18:47:56.718608 datajunction-0.0.1a4/dj/models/engine.py
--rw-r--r--   0        0        0     1183 2023-04-07 03:44:14.893669 datajunction-0.0.1a4/dj/models/metric.py
--rw-r--r--   0        0        0    20252 2023-04-15 05:07:29.317932 datajunction-0.0.1a4/dj/models/node.py
--rw-r--r--   0        0        0     3711 2023-03-23 19:26:05.392593 datajunction-0.0.1a4/dj/models/query.py
--rw-r--r--   0        0        0     2449 2023-03-23 18:47:56.718891 datajunction-0.0.1a4/dj/models/table.py
--rw-r--r--   0        0        0     2567 2023-03-23 18:47:56.718952 datajunction-0.0.1a4/dj/models/tag.py
--rw-r--r--   0        0        0     4043 2023-04-07 03:44:14.894264 datajunction-0.0.1a4/dj/service_clients.py
--rw-r--r--   0        0        0        0 2023-03-23 18:47:56.719076 datajunction-0.0.1a4/dj/sql/__init__.py
--rw-r--r--   0        0        0     1243 2023-03-23 19:26:05.392954 datajunction-0.0.1a4/dj/sql/dag.py
--rw-r--r--   0        0        0    32092 2023-04-15 05:07:29.318209 datajunction-0.0.1a4/dj/sql/functions.py
--rw-r--r--   0        0        0      644 2023-04-06 16:56:36.611655 datajunction-0.0.1a4/dj/sql/parse.py
--rw-r--r--   0        0        0       55 2023-04-06 16:56:36.611803 datajunction-0.0.1a4/dj/sql/parsing/__init__.py
--rw-r--r--   0        0        0    65122 2023-04-15 05:07:29.318629 datajunction-0.0.1a4/dj/sql/parsing/ast.py
--rw-r--r--   0        0        0        0 2023-03-23 18:47:56.720227 datajunction-0.0.1a4/dj/sql/parsing/backends/__init__.py
--rw-r--r--   0        0        0    30496 2023-04-06 16:56:36.612502 datajunction-0.0.1a4/dj/sql/parsing/backends/antlr4.py
--rw-r--r--   0        0        0      192 2023-03-23 18:47:56.720284 datajunction-0.0.1a4/dj/sql/parsing/backends/exceptions.py
--rw-r--r--   0        0        0     8733 2023-03-27 05:02:19.596790 datajunction-0.0.1a4/dj/sql/parsing/backends/grammar/SqlBaseLexer.g4
--rw-r--r--   0        0        0    49854 2023-03-27 05:02:19.597040 datajunction-0.0.1a4/dj/sql/parsing/backends/grammar/SqlBaseParser.g4
--rw-r--r--   0        0        0        0 2023-03-27 05:02:19.597083 datajunction-0.0.1a4/dj/sql/parsing/backends/grammar/__init__.py
--rw-r--r--   0        0        0   117820 2023-03-27 05:02:19.597848 datajunction-0.0.1a4/dj/sql/parsing/backends/grammar/generated/SqlBaseLexer.interp
--rw-r--r--   0        0        0   114725 2023-03-27 05:02:19.598388 datajunction-0.0.1a4/dj/sql/parsing/backends/grammar/generated/SqlBaseLexer.py
--rw-r--r--   0        0        0     8131 2023-03-27 05:02:19.598564 datajunction-0.0.1a4/dj/sql/parsing/backends/grammar/generated/SqlBaseLexer.tokens
--rw-r--r--   0        0        0   142799 2023-03-27 05:02:19.599083 datajunction-0.0.1a4/dj/sql/parsing/backends/grammar/generated/SqlBaseParser.interp
--rw-r--r--   0        0        0  1020523 2023-03-27 05:02:19.601075 datajunction-0.0.1a4/dj/sql/parsing/backends/grammar/generated/SqlBaseParser.py
--rw-r--r--   0        0        0     8131 2023-03-27 05:02:19.601243 datajunction-0.0.1a4/dj/sql/parsing/backends/grammar/generated/SqlBaseParser.tokens
--rw-r--r--   0        0        0   102489 2023-03-27 05:02:19.601505 datajunction-0.0.1a4/dj/sql/parsing/backends/grammar/generated/SqlBaseParserListener.py
--rw-r--r--   0        0        0    60656 2023-03-27 05:02:19.601711 datajunction-0.0.1a4/dj/sql/parsing/backends/grammar/generated/SqlBaseParserVisitor.py
--rw-r--r--   0        0        0    22205 2023-04-15 05:07:29.319121 datajunction-0.0.1a4/dj/sql/parsing/types.py
--rw-r--r--   0        0        0     3812 2023-03-23 18:47:56.721099 datajunction-0.0.1a4/dj/superset.py
--rw-r--r--   0        0        0     6467 2023-04-06 16:56:36.612795 datajunction-0.0.1a4/dj/typing.py
--rw-r--r--   0        0        0     4042 2023-04-15 05:07:29.319550 datajunction-0.0.1a4/dj/utils.py
--rw-r--r--   0        0        0     1418 2023-04-15 05:53:12.084649 datajunction-0.0.1a4/pyproject.toml
--rw-r--r--   0        0        0     7328 1970-01-01 00:00:00.000000 datajunction-0.0.1a4/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-03-09 19:29:41.743091 datajunction-0.0.1a5/LICENSE.txt
+-rw-r--r--   0        0        0     5589 2023-03-09 19:29:41.743202 datajunction-0.0.1a5/README.rst
+-rw-r--r--   0        0        0      384 2023-03-09 22:42:36.169164 datajunction-0.0.1a5/dj/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-09 19:29:41.770645 datajunction-0.0.1a5/dj/api/__init__.py
+-rw-r--r--   0        0        0     4692 2023-04-13 18:17:17.325178 datajunction-0.0.1a5/dj/api/attributes.py
+-rw-r--r--   0        0        0     2862 2023-04-13 18:17:17.325699 datajunction-0.0.1a5/dj/api/catalogs.py
+-rw-r--r--   0        0        0      654 2023-04-13 18:17:17.326024 datajunction-0.0.1a5/dj/api/cubes.py
+-rw-r--r--   0        0        0     5036 2023-04-16 15:31:28.665337 datajunction-0.0.1a5/dj/api/data.py
+-rw-r--r--   0        0        0     1457 2023-04-16 03:55:14.641955 datajunction-0.0.1a5/dj/api/engines.py
+-rw-r--r--   0        0        0     1220 2023-04-13 18:17:17.327030 datajunction-0.0.1a5/dj/api/health.py
+-rw-r--r--   0        0        0    12980 2023-04-16 15:31:28.665743 datajunction-0.0.1a5/dj/api/helpers.py
+-rw-r--r--   0        0        0     3061 2023-04-17 19:39:28.361836 datajunction-0.0.1a5/dj/api/main.py
+-rw-r--r--   0        0        0     2781 2023-04-13 18:17:17.327629 datajunction-0.0.1a5/dj/api/metrics.py
+-rw-r--r--   0        0        0     2205 2023-04-17 19:39:28.362005 datajunction-0.0.1a5/dj/api/namespaces.py
+-rw-r--r--   0        0        0    30136 2023-04-17 19:39:28.362281 datajunction-0.0.1a5/dj/api/nodes.py
+-rw-r--r--   0        0        0      702 2023-04-13 18:17:17.328235 datajunction-0.0.1a5/dj/api/query.py
+-rw-r--r--   0        0        0     1345 2023-04-16 15:31:28.666447 datajunction-0.0.1a5/dj/api/sql.py
+-rw-r--r--   0        0        0     3358 2023-04-13 18:17:17.328723 datajunction-0.0.1a5/dj/api/tags.py
+-rw-r--r--   0        0        0     2239 2023-04-13 18:17:17.329272 datajunction-0.0.1a5/dj/config.py
+-rw-r--r--   0        0        0      412 2023-03-09 19:29:41.772659 datajunction-0.0.1a5/dj/constants.py
+-rwxr-xr-x   0        0        0        0 2023-03-09 19:29:41.772720 datajunction-0.0.1a5/dj/construction/__init__.py
+-rwxr-xr-x   0        0        0    18129 2023-04-16 15:31:28.666684 datajunction-0.0.1a5/dj/construction/build.py
+-rw-r--r--   0        0        0     6561 2023-04-06 15:30:00.095444 datajunction-0.0.1a5/dj/construction/dj_query.py
+-rwxr-xr-x   0        0        0     1495 2023-03-09 19:29:41.773112 datajunction-0.0.1a5/dj/construction/exceptions.py
+-rwxr-xr-x   0        0        0     2679 2023-04-06 15:30:00.095544 datajunction-0.0.1a5/dj/construction/utils.py
+-rw-r--r--   0        0        0     5900 2023-04-06 15:30:00.095933 datajunction-0.0.1a5/dj/errors.py
+-rw-r--r--   0        0        0      518 2023-03-24 07:12:07.926290 datajunction-0.0.1a5/dj/models/__init__.py
+-rw-r--r--   0        0        0     2146 2023-03-09 19:29:41.773677 datajunction-0.0.1a5/dj/models/attribute.py
+-rw-r--r--   0        0        0     1592 2023-03-09 19:29:41.773734 datajunction-0.0.1a5/dj/models/base.py
+-rw-r--r--   0        0        0     2155 2023-03-24 07:12:07.926414 datajunction-0.0.1a5/dj/models/catalog.py
+-rw-r--r--   0        0        0     2661 2023-04-06 15:30:00.096245 datajunction-0.0.1a5/dj/models/column.py
+-rw-r--r--   0        0        0      858 2023-03-24 07:12:07.926823 datajunction-0.0.1a5/dj/models/cube.py
+-rw-r--r--   0        0        0     2019 2023-03-24 07:12:07.927108 datajunction-0.0.1a5/dj/models/database.py
+-rw-r--r--   0        0        0      791 2023-04-16 15:31:28.667119 datajunction-0.0.1a5/dj/models/engine.py
+-rw-r--r--   0        0        0     1258 2023-04-16 15:31:28.667317 datajunction-0.0.1a5/dj/models/metric.py
+-rw-r--r--   0        0        0    20833 2023-04-17 19:39:28.362596 datajunction-0.0.1a5/dj/models/node.py
+-rw-r--r--   0        0        0     3711 2023-04-13 18:09:39.316286 datajunction-0.0.1a5/dj/models/query.py
+-rw-r--r--   0        0        0     2449 2023-03-24 07:12:07.927968 datajunction-0.0.1a5/dj/models/table.py
+-rw-r--r--   0        0        0     2567 2023-03-09 19:29:41.774456 datajunction-0.0.1a5/dj/models/tag.py
+-rw-r--r--   0        0        0     4043 2023-04-14 00:40:01.549543 datajunction-0.0.1a5/dj/service_clients.py
+-rw-r--r--   0        0        0        0 2023-03-09 19:29:41.774583 datajunction-0.0.1a5/dj/sql/__init__.py
+-rw-r--r--   0        0        0     1243 2023-04-13 18:09:39.316464 datajunction-0.0.1a5/dj/sql/dag.py
+-rw-r--r--   0        0        0    34351 2023-04-17 19:39:28.362882 datajunction-0.0.1a5/dj/sql/functions.py
+-rw-r--r--   0        0        0      644 2023-04-06 15:30:00.097501 datajunction-0.0.1a5/dj/sql/parse.py
+-rw-r--r--   0        0        0       55 2023-04-06 15:30:00.097814 datajunction-0.0.1a5/dj/sql/parsing/__init__.py
+-rw-r--r--   0        0        0    65402 2023-04-17 19:39:28.363345 datajunction-0.0.1a5/dj/sql/parsing/ast.py
+-rw-r--r--   0        0        0        0 2023-03-09 19:29:41.775867 datajunction-0.0.1a5/dj/sql/parsing/backends/__init__.py
+-rw-r--r--   0        0        0    30630 2023-04-16 15:31:28.668409 datajunction-0.0.1a5/dj/sql/parsing/backends/antlr4.py
+-rw-r--r--   0        0        0      192 2023-03-09 19:29:41.775929 datajunction-0.0.1a5/dj/sql/parsing/backends/exceptions.py
+-rw-r--r--   0        0        0     8733 2023-03-26 08:42:46.249360 datajunction-0.0.1a5/dj/sql/parsing/backends/grammar/SqlBaseLexer.g4
+-rw-r--r--   0        0        0    49854 2023-03-26 08:42:46.249545 datajunction-0.0.1a5/dj/sql/parsing/backends/grammar/SqlBaseParser.g4
+-rw-r--r--   0        0        0        0 2023-03-26 08:42:46.249595 datajunction-0.0.1a5/dj/sql/parsing/backends/grammar/__init__.py
+-rw-r--r--   0        0        0   117820 2023-03-26 08:42:46.250054 datajunction-0.0.1a5/dj/sql/parsing/backends/grammar/generated/SqlBaseLexer.interp
+-rw-r--r--   0        0        0   114725 2023-03-26 08:42:46.250494 datajunction-0.0.1a5/dj/sql/parsing/backends/grammar/generated/SqlBaseLexer.py
+-rw-r--r--   0        0        0     8131 2023-03-26 08:42:46.250603 datajunction-0.0.1a5/dj/sql/parsing/backends/grammar/generated/SqlBaseLexer.tokens
+-rw-r--r--   0        0        0   142799 2023-03-26 08:42:46.251524 datajunction-0.0.1a5/dj/sql/parsing/backends/grammar/generated/SqlBaseParser.interp
+-rw-r--r--   0        0        0  1020523 2023-03-26 08:42:46.255771 datajunction-0.0.1a5/dj/sql/parsing/backends/grammar/generated/SqlBaseParser.py
+-rw-r--r--   0        0        0     8131 2023-03-26 08:42:46.255887 datajunction-0.0.1a5/dj/sql/parsing/backends/grammar/generated/SqlBaseParser.tokens
+-rw-r--r--   0        0        0   102489 2023-03-26 08:42:46.256283 datajunction-0.0.1a5/dj/sql/parsing/backends/grammar/generated/SqlBaseParserListener.py
+-rw-r--r--   0        0        0    60656 2023-03-26 08:42:46.256504 datajunction-0.0.1a5/dj/sql/parsing/backends/grammar/generated/SqlBaseParserVisitor.py
+-rw-r--r--   0        0        0    26308 2023-04-17 19:39:28.363635 datajunction-0.0.1a5/dj/sql/parsing/types.py
+-rw-r--r--   0        0        0     3812 2023-03-09 19:29:41.776529 datajunction-0.0.1a5/dj/superset.py
+-rw-r--r--   0        0        0     6467 2023-04-06 15:30:00.099751 datajunction-0.0.1a5/dj/typing.py
+-rw-r--r--   0        0        0     4042 2023-04-14 18:39:42.363510 datajunction-0.0.1a5/dj/utils.py
+-rw-r--r--   0        0        0     1418 2023-04-18 03:34:03.317288 datajunction-0.0.1a5/pyproject.toml
+-rw-r--r--   0        0        0     7328 1970-01-01 00:00:00.000000 datajunction-0.0.1a5/PKG-INFO
```

### Comparing `datajunction-0.0.1a4/LICENSE.txt` & `datajunction-0.0.1a5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a4/README.rst` & `datajunction-0.0.1a5/README.rst`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a4/dj/api/attributes.py` & `datajunction-0.0.1a5/dj/api/attributes.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a4/dj/api/catalogs.py` & `datajunction-0.0.1a5/dj/api/catalogs.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a4/dj/api/cubes.py` & `datajunction-0.0.1a5/dj/api/cubes.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a4/dj/api/data.py` & `datajunction-0.0.1a5/dj/api/data.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """
 Data related APIs.
 """
 
 import logging
-from typing import List
+from typing import List, Optional
 
 from fastapi import APIRouter, Depends, Query
 from fastapi.responses import JSONResponse
 from sqlmodel import Session
 
-from dj.api.helpers import get_node_by_name, get_query
-from dj.errors import DJException
+from dj.api.helpers import get_engine, get_node_by_name, get_query
+from dj.errors import DJException, DJInvalidInputException
 from dj.models.metric import TranslatedSQL
 from dj.models.node import AvailabilityState, AvailabilityStateBase, NodeType
 from dj.models.query import ColumnMetadata, QueryCreate, QueryWithResults
 from dj.service_clients import QueryServiceClient
 from dj.utils import get_query_service_client, get_session
 
 _logger = logging.getLogger(__name__)
@@ -86,47 +86,62 @@
     return JSONResponse(
         status_code=200,
         content={"message": "Availability state successfully posted"},
     )
 
 
 @router.get("/data/{node_name}/")
-def get_data(
+def get_data(  # pylint: disable=too-many-locals
     node_name: str,
     *,
     dimensions: List[str] = Query([]),
     filters: List[str] = Query([]),
     async_: bool = False,
     session: Session = Depends(get_session),
     query_service_client: QueryServiceClient = Depends(get_query_service_client),
+    engine_name: Optional[str] = None,
+    engine_version: Optional[str] = None,
 ) -> QueryWithResults:
     """
     Gets data for a node
     """
     node = get_node_by_name(session, node_name)
+
+    available_engines = node.current.catalog.engines
+    engine = (
+        get_engine(session, engine_name, engine_version)  # type: ignore
+        if engine_name
+        else available_engines[0]
+    )
+    if engine not in available_engines:
+        raise DJInvalidInputException(  # pragma: no cover
+            f"The selected engine is not available for the node {node_name}. "
+            f"Available engines include: {', '.join(engine.name for engine in available_engines)}",
+        )
+
     query_ast = get_query(
         session=session,
         node_name=node_name,
         dimensions=dimensions,
         filters=filters,
+        engine=engine,
     )
     columns = [
         ColumnMetadata(name=col.alias_or_name.name, type=str(col.type))  # type: ignore
         for col in query_ast.select.projection
     ]
     query = TranslatedSQL(
         sql=str(query_ast),
         columns=columns,
     )
 
-    available_engines = node.current.catalog.engines
     query_create = QueryCreate(
-        engine_name=available_engines[0].name,
+        engine_name=engine.name,
         catalog_name=node.current.catalog.name,
-        engine_version=available_engines[0].version,
+        engine_version=engine.version,
         submitted_query=query.sql,
         async_=async_,
     )
     result = query_service_client.submit_query(query_create)
     # Inject column info if there are results
     if result.results.__root__:  # pragma: no cover
         result.results.__root__[0].columns = columns
```

### Comparing `datajunction-0.0.1a4/dj/api/engines.py` & `datajunction-0.0.1a5/dj/api/engines.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a4/dj/api/health.py` & `datajunction-0.0.1a5/dj/api/health.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a4/dj/api/helpers.py` & `datajunction-0.0.1a5/dj/api/helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,17 @@
 from sqlmodel import Session, select
 
 from dj.construction.build import build_node
 from dj.construction.dj_query import build_dj_metric_query
 from dj.errors import DJError, DJException, DJInvalidInputException, ErrorCode
 from dj.models import AttributeType, Catalog, Column, Engine
 from dj.models.attribute import RESERVED_ATTRIBUTE_NAMESPACE
+from dj.models.engine import Dialect
 from dj.models.node import (
+    BuildCriteria,
     MissingParent,
     Node,
     NodeMissingParents,
     NodeMode,
     NodeNamespace,
     NodeRelationship,
     NodeRevision,
@@ -141,33 +143,45 @@
 
 
 def get_query(  # pylint: disable=too-many-arguments
     session: Session,
     node_name: str,
     dimensions: List[str],
     filters: List[str],
+    engine: Optional[Engine],
 ) -> ast.Query:
     """
     Get a query for a metric, dimensions, and filters
     """
     node = get_node_by_name(session=session, name=node_name)
 
     if node.type in (NodeType.DIMENSION, NodeType.SOURCE):
         if dimensions:
             raise DJInvalidInputException(
                 message=f"Cannot set dimensions for node type {node.type}!",
             )
 
+    # Builds the node for the engine's dialect if one is set or defaults to Spark
+    if (
+        not engine
+        and node.current
+        and node.current.catalog
+        and node.current.catalog.engines
+    ):
+        engine = node.current.catalog.engines[0]
+    build_criteria = BuildCriteria(
+        dialect=(engine.dialect if engine and engine.dialect else Dialect.SPARK),
+    )
+
     query_ast = build_node(
         session=session,
         node=node.current,
-        dialect=None,
         filters=filters,
         dimensions=dimensions,
-        build_criteria=None,
+        build_criteria=build_criteria,
     )
     return query_ast
 
 
 def get_dj_query(
     session: Session,
     query: str,
```

### Comparing `datajunction-0.0.1a4/dj/api/main.py` & `datajunction-0.0.1a5/dj/api/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     attributes,
     catalogs,
     cubes,
     data,
     engines,
     health,
     metrics,
+    namespaces,
     nodes,
     query,
     sql,
     tags,
 )
 from dj.api.attributes import default_attribute_types
 from dj.errors import DJException
@@ -70,14 +71,15 @@
     )
 
     application.include_router(catalogs.router)
     application.include_router(engines.router)
     application.include_router(metrics.router)
     application.include_router(query.router)
     application.include_router(nodes.router)
+    application.include_router(namespaces.router)
     application.include_router(data.router)
     application.include_router(health.router)
     application.include_router(cubes.router)
     application.include_router(tags.router)
     application.include_router(attributes.router)
     application.include_router(sql.router)
```

### Comparing `datajunction-0.0.1a4/dj/api/metrics.py` & `datajunction-0.0.1a5/dj/api/metrics.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a4/dj/api/nodes.py` & `datajunction-0.0.1a5/dj/api/nodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,14 @@
     CreateCubeNode,
     CreateNode,
     CreateSourceNode,
     MaterializationConfig,
     MissingParent,
     Node,
     NodeMode,
-    NodeNamespace,
     NodeOutput,
     NodeRevision,
     NodeRevisionBase,
     NodeRevisionOutput,
     NodeStatus,
     NodeType,
     NodeValidation,
@@ -180,15 +179,15 @@
                         scopes_map[item]
                         for item in attribute.attribute_type.uniqueness_scope
                     ),
                 )
             ].add(column.name)
 
     for (attribute, _), columns in attributes_columns_map.items():
-        if len(columns) > 1:
+        if len(columns) > 1 and attribute.uniqueness_scope:
             for col in columns:
                 modified_columns_map[col].attributes = []
             raise DJException(
                 message=f"The column attribute `{attribute.name}` is scoped to be "
                 f"unique to the `{attribute.uniqueness_scope}` level, but there "
                 "is more than one column tagged with it: "
                 f"`{', '.join(sorted(list(columns)))}`",
@@ -516,46 +515,48 @@
     query_service_client: QueryServiceClient = Depends(get_query_service_client),
 ) -> NodeOutput:
     """
     Create a source node. If columns are not provided, the source node's schema
     will be inferred using the configured query service.
     """
     raise_if_node_exists(session, data.name)
-    node = Node(
-        name=data.name,
-        namespace=data.namespace,
-        type=NodeType.SOURCE,
-        current_version=0,
-    )
-    catalog = get_catalog(session=session, name=data.catalog)
 
+    # Extract and assign namespace if one exists
     namespace = get_namespace_from_name(data.name)
     get_node_namespace(
         session=session,
         namespace=namespace,
     )  # Will return 404 if namespace doesn't exist
     data.namespace = namespace
 
+    node = Node(
+        name=data.name,
+        namespace=data.namespace,
+        type=NodeType.SOURCE,
+        current_version=0,
+    )
+    catalog = get_catalog(session=session, name=data.catalog)
+
     # When no columns are provided, attempt to find actual table columns
     # if a query service is set
     columns = (
         [
             Column(
-                name=column_name,
+                name=column_data.name,
                 type=column_data.type,
                 dimension=(
                     get_node_by_name(
                         session,
                         name=column_data.dimension,
                         node_type=NodeType.DIMENSION,
                         raise_if_not_exists=False,
                     )
                 ),
             )
-            for column_name, column_data in data.columns.items()
+            for column_data in data.columns
         ]
         if data.columns
         else None
     )
     if not columns:
         if not query_service_client:
             raise DJException(
@@ -586,59 +587,14 @@
     )
 
     # Point the node to the new node revision.
     save_node(session, node_revision, node, data.mode)
     return node  # type: ignore
 
 
-@router.post("/namespaces/{namespace}/", status_code=201)
-def create_a_node_namespace(
-    namespace: str,
-    session: Session = Depends(get_session),
-) -> JSONResponse:
-    """
-    Create a node namespace
-    """
-    if get_node_namespace(
-        session=session,
-        namespace=namespace,
-        raise_if_not_exists=False,
-    ):  # pragma: no cover
-        return JSONResponse(
-            status_code=409,
-            content={
-                "message": (f"Node namespace`{namespace}` already exists"),
-            },
-        )
-    node_namespace = NodeNamespace(namespace=namespace)
-    session.add(node_namespace)
-    session.commit()
-    return JSONResponse(
-        status_code=201,
-        content={
-            "message": (f"Node namespace`{namespace}` has been successfully created"),
-        },
-    )
-
-
-@router.get(
-    "/namespaces/all/",
-    response_model=List[NodeNamespace],
-    status_code=201,
-)
-def list_node_namespaces(
-    session: Session = Depends(get_session),
-) -> List[NodeNamespace]:
-    """
-    List node namespaces
-    """
-    namespaces = session.exec(select(NodeNamespace)).all()
-    return namespaces
-
-
 @router.post("/nodes/transform/", response_model=NodeOutput, status_code=201)
 @router.post("/nodes/dimension/", response_model=NodeOutput, status_code=201)
 @router.post("/nodes/metric/", response_model=NodeOutput, status_code=201)
 def create_a_node(
     data: CreateNode,
     request: Request,
     *,
@@ -745,15 +701,15 @@
 
     target_column = get_column(node.current, column)
     if dimension_column:
         # Check that the dimension column exists
         column_from_dimension = get_column(dimension_node.current, dimension_column)
 
         # Check the dimension column's type is compatible with the target column's type
-        if column_from_dimension.type != target_column.type:
+        if not column_from_dimension.type.is_compatible(target_column.type):
             raise DJInvalidInputException(
                 f"The column {target_column.name} has type {target_column.type} "
                 f"and is being linked to the dimension {dimension} via the dimension"
                 f" column {dimension_column}, which has type {column_from_dimension.type}."
                 " These column types are incompatible and the dimension cannot be linked!",
             )
 
@@ -855,19 +811,19 @@
         description=(
             data.description if data and data.description else old_revision.description
         ),
         query=(data.query if data and data.query else old_revision.query),
         type=old_revision.type,
         columns=[
             Column(
-                name=column_name,
+                name=column_data.name,
                 type=column_data.type,
                 dimension_column=column_data.dimension,
             )
-            for column_name, column_data in data.columns.items()
+            for column_data in data.columns
         ]
         if data and data.columns
         else old_revision.columns,
         catalog=old_revision.catalog,
         schema_=old_revision.schema_,
         table=old_revision.table,
         parents=[],
```

### Comparing `datajunction-0.0.1a4/dj/api/query.py` & `datajunction-0.0.1a5/dj/api/query.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a4/dj/api/sql.py` & `datajunction-0.0.1a5/dj/api/sql.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """
 SQL related APIs.
 """
 
 import logging
-from typing import List
+from typing import List, Optional
 
 from fastapi import APIRouter, Depends, Query
 from sqlmodel import Session
 
-from dj.api.helpers import get_query
+from dj.api.helpers import get_engine, get_query
 from dj.models.metric import TranslatedSQL
 from dj.models.query import ColumnMetadata
 from dj.utils import get_session
 
 _logger = logging.getLogger(__name__)
 router = APIRouter()
 
@@ -20,25 +20,34 @@
 @router.get("/sql/{node_name}/", response_model=TranslatedSQL)
 def get_sql(
     node_name: str,
     dimensions: List[str] = Query([]),
     filters: List[str] = Query([]),
     *,
     session: Session = Depends(get_session),
+    engine_name: Optional[str] = None,
+    engine_version: Optional[str] = None,
 ) -> TranslatedSQL:
     """
     Return SQL for a node.
     """
+    engine = (
+        get_engine(session, engine_name, engine_version)  # type: ignore
+        if engine_name
+        else None
+    )
     query_ast = get_query(
         session=session,
         node_name=node_name,
         dimensions=dimensions,
         filters=filters,
+        engine=engine,
     )
     columns = [
         ColumnMetadata(name=col.alias_or_name.name, type=str(col.type))  # type: ignore
         for col in query_ast.select.projection
     ]
     return TranslatedSQL(
         sql=str(query_ast),
         columns=columns,
+        dialect=engine.dialect if engine else None,
     )
```

### Comparing `datajunction-0.0.1a4/dj/api/tags.py` & `datajunction-0.0.1a5/dj/api/tags.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a4/dj/config.py` & `datajunction-0.0.1a5/dj/config.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a4/dj/construction/build.py` & `datajunction-0.0.1a5/dj/construction/build.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from typing import DefaultDict, Deque, Dict, List, Optional, Set, Tuple, Union, cast
 
 from sqlmodel import Session
 
 from dj.construction.utils import amenable_name, to_namespaced_name
 from dj.errors import DJException, DJInvalidInputException
 from dj.models.column import Column
+from dj.models.engine import Dialect
 from dj.models.node import BuildCriteria, NodeRevision, NodeType
 from dj.sql.parsing.ast import CompileContext
 from dj.sql.parsing.backends.antlr4 import ast, parse
 
 
 def _get_tables_from_select(
     select: ast.SelectExpression,
@@ -96,16 +97,16 @@
         _get_node_table(table_node, build_criteria),
     )
     if not join_table:  # pragma: no cover
         join_query = parse(cast(str, table_node.query))
         join_table = build_ast(session, join_query)  # type: ignore
         join_table.parenthesized = True  # type: ignore
 
-    ctx = CompileContext(session=session, exception=DJException())
-    join_table.compile(ctx)  # type: ignore
+    for col in join_table.columns:
+        col._table = join_table  # pylint: disable=protected-access
 
     join_table = cast(ast.TableExpression, join_table)  # type: ignore
     right_alias = ast.Name(table_node_alias)
     join_right = ast.Alias(  # type: ignore
         right_alias,
         child=join_table,
         as_=True,
@@ -139,32 +140,53 @@
             else tables[start_node][0]
         )
         join_left_columns = {
             col.alias_or_name.name: col for col in left_table.columns  # type: ignore
         }
 
         # Assemble table on right of join
-        join_right = _get_or_build_join_table(session, table_node, build_criteria)
+        join_right = _get_or_build_join_table(
+            session,
+            table_node,
+            build_criteria,
+        )
+
+        # Optimize query by filtering down to only the necessary columns
+        selected_columns = {col.name.name for col in required_dimension_columns}
+        available_join_columns = {
+            col.dimension_column for col in join_columns if col.dimension_column
+        }
+        primary_key_columns = {col.name for col in table_node.primary_key()}
+        joinable_dim_columns = {
+            col.name for col in table_node.columns if col.dimension_id
+        }
+        required_mapping = (
+            selected_columns.union(available_join_columns)
+            .union(primary_key_columns)
+            .union(joinable_dim_columns)
+        )
+        join_right.child.select.projection = [
+            col
+            for col in join_right.child.select.projection
+            if col.alias_or_name.name in required_mapping
+        ]
+
         initial_nodes.add(table_node)
         tables[table_node].append(join_right)  # type: ignore
         join_right_columns = {
             col.alias_or_name.name: col  # type: ignore
             for col in join_right.child.columns
         }
 
         # Assemble join ON clause
         for join_col in join_columns:
             join_table_pk = table_node.primary_key()
-            if (
-                len(join_table_pk) == 1
-                and join_col.name in join_left_columns
-                and (
-                    join_col.dimension_column in join_right_columns
-                    or join_table_pk[0].name in join_right_columns
-                )
+            if join_col.name in join_left_columns and (
+                join_col.dimension_column in join_right_columns
+                or join_table_pk[0].name in join_right_columns
             ):
                 left_table.add_ref_column(
                     cast(ast.Column, join_left_columns[join_col.name]),
                 )
                 join_on.append(
                     ast.BinaryOp.Eq(
                         join_left_columns[join_col.name],
@@ -206,15 +228,14 @@
     onto the select expression.
 
     In some cases, the necessary tables will already be on the select and
     no additional joins will be needed. However, if the tables are not in
     the select, it will traverse through available linked tables (via dimension
     nodes) and join them in.
     """
-
     for dim_node, required_dimension_columns in sorted(
         dimension_nodes_to_columns.items(),
         key=lambda x: x[0].name,
     ):
         # Find all the selects that contain the different dimension columns
         selects_map = {
             cast(ast.Select, dim_col.get_nearest_parent_of_type(ast.Select))
@@ -264,14 +285,20 @@
             node_table.parenthesized = True  # type: ignore
 
         alias = amenable_name(node.node.name)
         context = CompileContext(session=session, exception=DJException())
 
         node_ast = ast.Alias(ast.Name(alias), child=node_table, as_=True)  # type: ignore
         for tbl in tbls:
+            if isinstance(node_ast.child, ast.Select) and isinstance(tbl, ast.Alias):
+                node_ast.child.projection = [
+                    col
+                    for col in node_ast.child.projection
+                    if col in set(tbl.child.select.projection)
+                ]
             node_ast.compile(context)
             select.replace(tbl, node_ast)
 
 
 def dimension_columns_mapping(
     select: ast.SelectExpression,
 ) -> Dict[NodeRevision, List[ast.Column]]:
@@ -354,15 +381,15 @@
 
 def _get_node_table(
     node: NodeRevision,
     build_criteria: Optional[BuildCriteria] = None,
     as_select: bool = False,
 ) -> Optional[Union[ast.Select, ast.Table]]:
     """
-    If a node is available, return a table for the available state
+    If a node has a materialization available, return the materialized table
     """
     table = None
     if node.type == NodeType.SOURCE:
         if node.table:
             name = ast.Name(
                 node.table,
                 namespace=ast.Name(node.schema_) if node.schema_ else None,
@@ -391,22 +418,33 @@
         )
     return table
 
 
 def build_node(  # pylint: disable=too-many-arguments
     session: Session,
     node: NodeRevision,
-    dialect: Optional[str] = None,
     filters: Optional[List[str]] = None,
     dimensions: Optional[List[str]] = None,
     build_criteria: Optional[BuildCriteria] = None,
 ) -> ast.Query:
     """
     Determines the optimal way to build the Node and does so
     """
+    # Set the dialect by finding available engines for this node, or default to Spark
+    if not build_criteria:
+        build_criteria = BuildCriteria(
+            dialect=(
+                node.catalog.engines[0].dialect
+                if node.catalog
+                and node.catalog.engines
+                and node.catalog.engines[0].dialect
+                else Dialect.SPARK
+            ),
+        )
+
     # if no dimensions need to be added then we can see if the node is directly materialized
     if not (filters or dimensions):
         if select := cast(
             ast.Select,
             _get_node_table(node, build_criteria, as_select=True),
         ):
             return ast.Query(select=select)  # pragma: no cover
@@ -414,15 +452,15 @@
     if node.query:
         query = parse(node.query)
     else:
         query = build_source_node_query(node)
 
     add_filters_and_dimensions_to_query_ast(
         query,
-        dialect,
+        build_criteria.dialect,
         filters,
         dimensions,
     )
 
     return build_ast(session, query, build_criteria)
```

### Comparing `datajunction-0.0.1a4/dj/construction/dj_query.py` & `datajunction-0.0.1a5/dj/construction/dj_query.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a4/dj/construction/exceptions.py` & `datajunction-0.0.1a5/dj/construction/exceptions.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a4/dj/construction/utils.py` & `datajunction-0.0.1a5/dj/construction/utils.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a4/dj/errors.py` & `datajunction-0.0.1a5/dj/errors.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a4/dj/models/__init__.py` & `datajunction-0.0.1a5/dj/models/__init__.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a4/dj/models/attribute.py` & `datajunction-0.0.1a5/dj/models/attribute.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a4/dj/models/base.py` & `datajunction-0.0.1a5/dj/models/base.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a4/dj/models/catalog.py` & `datajunction-0.0.1a5/dj/models/catalog.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a4/dj/models/column.py` & `datajunction-0.0.1a5/dj/models/column.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a4/dj/models/cube.py` & `datajunction-0.0.1a5/dj/models/cube.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a4/dj/models/database.py` & `datajunction-0.0.1a5/dj/models/database.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a4/dj/models/metric.py` & `datajunction-0.0.1a5/dj/models/metric.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Models for metrics.
 """
 from typing import List, Optional
 
 from sqlmodel import SQLModel
 
+from dj.models.engine import Dialect
 from dj.models.node import Node
 from dj.models.query import ColumnMetadata
 from dj.sql.dag import get_dimensions
 from dj.typing import UTCDatetime
 
 
 class Metric(SQLModel):
@@ -49,7 +50,8 @@
     Class for SQL generated from a given metric.
     """
 
     # TODO: once type-inference is added to /query/ endpoint  # pylint: disable=fixme
     # columns attribute can be required
     sql: str
     columns: Optional[List[ColumnMetadata]] = None  # pragma: no-cover
+    dialect: Optional[Dialect] = None
```

### Comparing `datajunction-0.0.1a4/dj/models/node.py` & `datajunction-0.0.1a5/dj/models/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from typing_extensions import TypedDict
 
 from dj.errors import DJInvalidInputException
 from dj.models.base import BaseSQLModel, generate_display_name
 from dj.models.catalog import Catalog
 from dj.models.column import Column, ColumnYAML
 from dj.models.database import Database
-from dj.models.engine import Engine, EngineInfo
+from dj.models.engine import Dialect, Engine, EngineInfo
 from dj.models.tag import Tag, TagNodeRelationship
 from dj.sql.parse import is_metric
 from dj.sql.parsing.types import ColumnType
 from dj.typing import UTCDatetime
 from dj.utils import Version
 
 DEFAULT_DRAFT_VERSION = Version(major=0, minor=1)
@@ -38,14 +38,15 @@
 class BuildCriteria:
     """
     Criterion used for building
         - used to deterimine whether to use an availability state
     """
 
     timestamp: Optional[UTCDatetime] = None
+    dialect: Dialect = Dialect.SPARK
 
 
 class NodeRelationship(BaseSQLModel, table=True):  # type: ignore
     """
     Join table for self-referential many-to-many relationships between nodes.
     """
 
@@ -368,15 +369,20 @@
     __table_args__ = (UniqueConstraint("version", "node_id"),)
 
     id: Optional[int] = Field(default=None, primary_key=True)
     version: Optional[str] = Field(default=str(DEFAULT_DRAFT_VERSION))
     node_id: Optional[int] = Field(foreign_key="node.id")
     node: Node = Relationship(back_populates="revisions")
     catalog_id: int = Field(default=None, foreign_key="catalog.id")
-    catalog: Catalog = Relationship(back_populates="node_revisions")
+    catalog: Catalog = Relationship(
+        back_populates="node_revisions",
+        sa_relationship_kwargs={
+            "lazy": "joined",
+        },
+    )
     schema_: Optional[str] = None
     table: Optional[str] = None
     cube_elements: List["Node"] = Relationship(  # Only used by cube nodes
         back_populates="cubes",
         link_model=CubeRelationship,
         sa_relationship_kwargs={
             "primaryjoin": "NodeRevision.id==CubeRelationship.cube_id",
@@ -505,32 +511,100 @@
     """
     Query field for node.
     """
 
     query: str
 
 
-class SourceNodeColumnType(BaseSQLModel):
+class NodeNameOutput(SQLModel):
+    """
+    Node name only
+    """
+
+    name: str
+
+
+class AttributeTypeName(BaseSQLModel):
+    """
+    Attribute type name.
+    """
+
+    namespace: str
+    name: str
+
+
+class AttributeOutput(BaseSQLModel):
+    """
+    Column attribute output.
+    """
+
+    attribute_type: AttributeTypeName
+
+
+class ColumnOutput(SQLModel):
+    """
+    A simplified column schema, without ID or dimensions.
+    """
+
+    name: str
+    type: ColumnType
+    attributes: Optional[List[AttributeOutput]]
+    dimension: Optional[NodeNameOutput]
+
+    class Config:  # pylint: disable=too-few-public-methods
+        """
+        Should perform validation on assignment
+        """
+
+        validate_assignment = True
+
+    @root_validator
+    def type_string(cls, values):  # pylint: disable=no-self-argument
+        """
+        Extracts the type as a string
+        """
+        values["type"] = str(values.get("type"))
+        return values
+
+
+class SourceColumnOutput(SQLModel):
     """
-    Schema of a column for a table defined in a source node
+    A column used in creation of a source node
     """
 
+    name: str
     type: ColumnType
+    attributes: Optional[List[AttributeOutput]]
     dimension: Optional[str]
 
+    class Config:  # pylint: disable=too-few-public-methods
+        """
+        Should perform validation on assignment
+        """
+
+        validate_assignment = True
+
+    @root_validator
+    def type_string(cls, values):  # pylint: disable=no-self-argument
+        """
+        Extracts the type as a string
+        """
+        values["type"] = str(values.get("type"))
+        return values
+
 
 class SourceNodeFields(BaseSQLModel):
     """
     Source node fields that can be changed.
     """
 
     catalog: str
     schema_: str
     table: str
-    columns: Optional[Dict[str, SourceNodeColumnType]]
+    columns: Optional[List["SourceColumnOutput"]] = []
 
 
 class CubeNodeFields(BaseSQLModel):
     """
     Cube node fields that can be changed
     """
 
@@ -623,65 +697,14 @@
                 assert isinstance(value, dict)
                 for key, val in value.items():
                     yield key, val
             else:
                 yield dict_key, value
 
 
-class AttributeTypeName(BaseSQLModel):
-    """
-    Attribute type name.
-    """
-
-    namespace: str
-    name: str
-
-
-class AttributeOutput(BaseSQLModel):
-    """
-    Column attribute output.
-    """
-
-    attribute_type: AttributeTypeName
-
-
-class NodeNameOutput(SQLModel):
-    """
-    Node name only
-    """
-
-    name: str
-
-
-class ColumnOutput(SQLModel):
-    """
-    A simplified column schema, without ID or dimensions.
-    """
-
-    name: str
-    type: ColumnType
-    attributes: List[AttributeOutput]
-    dimension: Optional[NodeNameOutput]
-
-    class Config:  # pylint: disable=too-few-public-methods
-        """
-        Should perform validation on assignment
-        """
-
-        validate_assignment = True
-
-    @root_validator
-    def type_string(cls, values):  # pylint: disable=no-self-argument
-        """
-        Extracts the type as a string
-        """
-        values["type"] = str(values.get("type"))
-        return values
-
-
 class TableOutput(SQLModel):
     """
     Output for table information.
     """
 
     id: Optional[int]
     catalog: Optional[Catalog]
```

### Comparing `datajunction-0.0.1a4/dj/models/query.py` & `datajunction-0.0.1a5/dj/models/query.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a4/dj/models/table.py` & `datajunction-0.0.1a5/dj/models/table.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a4/dj/models/tag.py` & `datajunction-0.0.1a5/dj/models/tag.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a4/dj/service_clients.py` & `datajunction-0.0.1a5/dj/service_clients.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a4/dj/sql/dag.py` & `datajunction-0.0.1a5/dj/sql/dag.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a4/dj/sql/functions.py` & `datajunction-0.0.1a5/dj/sql/functions.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 nodes. The functions are used to infer types.
 
 Spark function reference
 https://github.com/apache/spark/tree/74cddcfda3ac4779de80696cdae2ba64d53fc635/sql/catalyst/src/main/scala/org/apache/spark/sql/catalyst/expressions
 
 Java strictmath reference
 https://docs.oracle.com/javase/8/docs/api/java/lang/StrictMath.html
+
+Databricks reference:
+https://docs.databricks.com/sql/language-manual/sql-ref-functions-builtin-alpha.html
 """
 
 import inspect
 import re
 from itertools import zip_longest
 
 # pylint: disable=unused-argument, missing-function-docstring, arguments-differ, too-many-return-statements
@@ -45,28 +48,27 @@
     from dj.sql.parsing.ast import Expression
 
 
 def compare_registers(types, register) -> bool:
     """
     Comparing registers
     """
-    saved_a = None
-    for ((_, register_a), (type_b, register_b)) in zip_longest(
+    for ((type_a, register_a), (type_b, register_b)) in zip_longest(
         types,
         register,
-        fillvalue=register[-1],
+        fillvalue=(-1, None),
     ):
-        if register_a is None:
-            if type_b != -1:  # pragma: no cover
+        if type_b == -1 and register_b is None:
+            if register[-1][0] == -1:  # args
+                register_b = register[-1][1]
+            else:
                 return False  # pragma: no cover
-        else:
-            saved_a = register_a
-        if register_b is None:
-            return False  # pragma: no cover
-        if not issubclass(saved_a, register_b):  # type: ignore
+        if type_a == -1:
+            register_a = type(register_a)
+        if not issubclass(register_a, register_b):  # type: ignore
             return False
     return True
 
 
 class DispatchMeta(type):
     """
     Dispatch abstract class for function registry
@@ -183,30 +185,28 @@
     is_aggregation = True
 
 
 @Avg.register
 def infer_type(
     arg: ct.DecimalType,
 ) -> ct.DecimalType:  # noqa: F811  # pylint: disable=function-redefined
-    type_ = arg
-    if hasattr(arg, "type") and isinstance(arg.type, ct.DecimalType):
-        type_ = arg.type
+    type_ = arg.type
     return ct.DecimalType(type_.precision + 4, type_.scale + 4)
 
 
 @Avg.register  # type: ignore
 def infer_type(  # noqa: F811  # pylint: disable=function-redefined
     arg: ct.IntervalTypeBase,
 ) -> ct.IntervalTypeBase:
     return type(arg.type)()
 
 
 @Avg.register  # type: ignore
 def infer_type(  # noqa: F811  # pylint: disable=function-redefined
-    arg: ct.ColumnType,
+    arg: ct.NumberType,
 ) -> ct.DoubleType:
     return ct.DoubleType()
 
 
 class Min(Function):  # pylint: disable=abstract-method
     """
     Computes the minimum value of the input column or expression.
@@ -240,49 +240,114 @@
 @Max.register  # type: ignore
 def infer_type(  # noqa: F811  # pylint: disable=function-redefined
     arg: ct.StringType,
 ) -> ct.StringType:
     return arg.type
 
 
-class Sum(Function):
+class Sum(Function):  # pylint: disable=abstract-method
     """
     Computes the sum of the input column or expression.
     """
 
     is_aggregation = True
 
-    @staticmethod
-    def infer_type(arg: "Expression") -> ct.ColumnType:  # type: ignore
-        return arg.type  # type: ignore
+
+@Sum.register  # type: ignore
+def infer_type(  # noqa: F811  # pylint: disable=function-redefined
+    arg: ct.IntegerBase,
+) -> ct.BigIntType:
+    return ct.BigIntType()
+
+
+@Sum.register  # type: ignore
+def infer_type(  # noqa: F811  # pylint: disable=function-redefined
+    arg: ct.DecimalType,
+) -> ct.DecimalType:
+    precision = arg.type.precision
+    scale = arg.type.scale
+    return ct.DecimalType(precision + min(10, 31 - precision), scale)
 
 
-class Ceil(Function):
+@Sum.register  # type: ignore
+def infer_type(  # noqa: F811  # pylint: disable=function-redefined
+    arg: Union[ct.NumberType, ct.IntervalTypeBase],
+) -> ct.DoubleType:
+    return ct.DoubleType()
+
+
+class Ceil(Function):  # pylint: disable=abstract-method
     """
     Computes the smallest integer greater than or equal to the input value.
     """
 
-    @staticmethod
-    def infer_type(arg: "Expression") -> ct.IntegerType:  # type: ignore
-        return ct.IntegerType()
+
+@Ceil.register
+def infer_type(  # noqa: F811  # pylint: disable=function-redefined
+    args: ct.NumberType,
+    _target_scale: ct.IntegerType,
+) -> ct.DecimalType:
+    target_scale = _target_scale.value
+    if isinstance(args.type, ct.DecimalType):
+        precision = max(args.type.precision - args.type.scale + 1, -target_scale + 1)
+        scale = min(args.type.scale, max(0, target_scale))
+        return ct.DecimalType(precision, scale)
+    if args.type == ct.TinyIntType():
+        precision = max(3, -target_scale + 1)
+        return ct.DecimalType(precision, 0)
+    if args.type == ct.SmallIntType():
+        precision = max(5, -target_scale + 1)
+        return ct.DecimalType(precision, 0)
+    if args.type == ct.IntegerType():
+        precision = max(10, -target_scale + 1)
+        return ct.DecimalType(precision, 0)
+    if args.type == ct.BigIntType():
+        precision = max(20, -target_scale + 1)
+        return ct.DecimalType(precision, 0)
+    if args.type == ct.FloatType():
+        precision = max(14, -target_scale + 1)
+        scale = min(7, max(0, target_scale))
+        return ct.DecimalType(precision, scale)
+    if args.type == ct.DoubleType():
+        precision = max(30, -target_scale + 1)
+        scale = min(15, max(0, target_scale))
+        return ct.DecimalType(precision, scale)
+
+    raise DJParseException(
+        f"Unhandled numeric type in Ceil `{args.type}`",
+    )  # pragma: no cover
+
+
+@Ceil.register
+def infer_type(  # noqa: F811  # pylint: disable=function-redefined
+    args: ct.DecimalType,
+) -> ct.DecimalType:
+    return ct.DecimalType(args.type.precision - args.type.scale + 1, 0)
+
+
+@Ceil.register
+def infer_type(  # noqa: F811  # pylint: disable=function-redefined
+    args: ct.NumberType,
+) -> ct.BigIntType:
+    return ct.BigIntType()
 
 
 class Count(Function):  # pylint: disable=abstract-method
     """
     Counts the number of non-null values in the input column or expression.
     """
 
     is_aggregation = True
 
 
 @Count.register  # type: ignore
 def infer_type(  # noqa: F811  # pylint: disable=function-redefined
     *args: ct.ColumnType,
-) -> ct.LongType:
-    return ct.LongType()
+) -> ct.BigIntType:
+    return ct.BigIntType()
 
 
 class Coalesce(Function):  # pylint: disable=abstract-method
     """
     Computes the average of the input column or expression.
     """
 
@@ -450,44 +515,14 @@
 def infer_type(  # noqa: F811  # pylint: disable=function-redefined
     start_date: ct.StringType,
     end_date: ct.StringType,
 ) -> ct.IntegerType:
     return ct.IntegerType()
 
 
-class DatetimeAdd(Function):
-    """
-    Adds a specified number of seconds to a timestamp.
-    """
-
-    @staticmethod
-    def infer_type(*arg: "Expression") -> ct.TimestampType:
-        return ct.TimestampType()
-
-
-class DatetimeSub(Function):
-    """
-    Subtracts a specified number of seconds from a timestamp.
-    """
-
-    @staticmethod
-    def infer_type(*arg: "Expression") -> ct.TimestampType:
-        return ct.TimestampType()
-
-
-class DatetimeDiff(Function):
-    """
-    Computes the difference in seconds between two timestamps.
-    """
-
-    @staticmethod
-    def infer_type(*arg: "Expression") -> ct.IntegerType:
-        return ct.IntegerType()
-
-
 class Extract(Function):
     """
     Returns a specified component of a timestamp, such as year, month or day.
     """
 
     @staticmethod
     def infer_type(  # type: ignore
@@ -495,122 +530,39 @@
         source: "Expression",
     ) -> Union[ct.DecimalType, ct.IntegerType]:
         if str(field.name) == "SECOND":  # type: ignore
             return ct.DecimalType(8, 6)
         return ct.IntegerType()
 
 
-class TimestampAdd(Function):
-    """
-    Adds a specified amount of time to a timestamp.
-    """
-
-    @staticmethod
-    def infer_type(*arg: "Expression") -> ct.TimestampType:
-        return ct.TimestampType()
-
-
-class TimestampSub(Function):
-    """
-    Subtracts a specified amount of time from a timestamp.
-    """
-
-    @staticmethod
-    def infer_type(*arg: "Expression") -> ct.TimestampType:
-        return ct.TimestampType()
-
-
-class TimestampDiff(Function):
-    """
-    Computes the difference in seconds between two timestamps.
-    """
-
-    @staticmethod
-    def infer_type(*arg: "Expression") -> ct.IntegerType:
-        return ct.IntegerType()
-
-
-class TimeAdd(Function):
-    """
-    Adds a specified amount of time to a time value.
-    """
-
-    @staticmethod
-    def infer_type(*arg: "Expression") -> ct.TimestampType:
-        return ct.TimestampType()
-
-
-class TimeSub(Function):
-    """
-    Subtracts a specified amount of time from a time value.
-    """
-
-    @staticmethod
-    def infer_type(*arg: "Expression") -> ct.TimestampType:
-        return ct.TimestampType()
-
-
-class TimeDiff(Function):
-    """
-    Computes the difference in seconds between two time values.
-    """
-
-    @staticmethod
-    def infer_type(*arg: "Expression") -> ct.IntegerType:
-        return ct.IntegerType()
-
-
-class DateStrToDate(Function):  # pragma: no cover
+class ToDate(Function):  # pragma: no cover # pylint: disable=abstract-method
     """
     Converts a date string to a date value.
     """
 
-    @staticmethod
-    def infer_type(arg: "Expression") -> ct.DateType:  # type: ignore
-        return ct.DateType()
-
 
-class DateToDateStr(Function):  # pragma: no cover
-    """
-    Converts a date value to a date string.
-    """
-
-    @staticmethod
-    def infer_type(arg: "Expression") -> ct.StringType:  # type: ignore
-        return ct.StringType()
-
-
-class DateToDi(Function):  # pragma: no cover
-    """
-    Returns the day of the year for a specified date.
-    """
-
-    @staticmethod
-    def infer_type(arg: "Expression") -> ct.IntegerType:  # type: ignore
-        return ct.IntegerType()
+@ToDate.register  # type: ignore
+def infer_type(  # noqa: F811  # pylint: disable=function-redefined
+    expr: ct.StringType,
+    fmt: Optional[ct.StringType] = None,
+) -> ct.DateType:
+    return ct.DateType()
 
 
-class Day(Function):
+class Day(Function):  # pylint: disable=abstract-method
     """
     Returns the day of the month for a specified date.
     """
 
-    @staticmethod
-    def infer_type(arg: "Expression") -> ct.TinyIntType:  # type: ignore
-        return ct.TinyIntType()
-
-
-class DiToDate(Function):  # pragma: no cover
-    """
-    Converts a day of the year and a year to a date value.
-    """
 
-    @staticmethod
-    def infer_type(arg: "Expression") -> ct.DateType:  # type: ignore
-        return ct.DateType()
+@Day.register  # type: ignore
+def infer_type(  # noqa: F811  # pylint: disable=function-redefined
+    arg: Union[ct.StringType, ct.DateType, ct.TimestampType],
+) -> ct.IntegerType:  # type: ignore
+    return ct.IntegerType()
 
 
 class Exp(Function):  # pylint: disable=abstract-method
     """
     Returns e to the power of expr.
     """
 
@@ -618,22 +570,68 @@
 @Exp.register  # type: ignore
 def infer_type(  # noqa: F811  # pylint: disable=function-redefined
     args: ct.ColumnType,
 ) -> ct.DoubleType:
     return ct.DoubleType()
 
 
-class Floor(Function):
+class Floor(Function):  # pylint: disable=abstract-method
     """
     Returns the largest integer less than or equal to a specified number.
     """
 
-    @staticmethod
-    def infer_type(arg: "Expression") -> ct.IntegerType:  # type: ignore
-        return ct.IntegerType()
+
+@Floor.register  # type: ignore
+def infer_type(  # noqa: F811  # pylint: disable=function-redefined
+    args: ct.DecimalType,
+) -> ct.DecimalType:
+    return ct.DecimalType(args.type.precision - args.type.scale + 1, 0)
+
+
+@Floor.register  # type: ignore
+def infer_type(  # noqa: F811  # pylint: disable=function-redefined
+    args: ct.NumberType,
+) -> ct.BigIntType:
+    return ct.BigIntType()
+
+
+@Floor.register  # type: ignore
+def infer_type(  # noqa: F811  # pylint: disable=function-redefined
+    args: ct.NumberType,
+    _target_scale: ct.IntegerType,
+) -> ct.DecimalType:
+    target_scale = _target_scale.value
+    if isinstance(args.type, ct.DecimalType):  # pylint: disable=R1705
+        precision = max(args.type.precision - args.type.scale + 1, -target_scale + 1)
+        scale = min(args.type.scale, max(0, target_scale))
+        return ct.DecimalType(precision, scale)
+    if args.type == ct.TinyIntType():
+        precision = max(3, -target_scale + 1)
+        return ct.DecimalType(precision, 0)
+    if args.type == ct.SmallIntType():
+        precision = max(5, -target_scale + 1)
+        return ct.DecimalType(precision, 0)
+    if args.type == ct.IntegerType():
+        precision = max(10, -target_scale + 1)
+        return ct.DecimalType(precision, 0)
+    if args.type == ct.BigIntType():
+        precision = max(20, -target_scale + 1)
+        return ct.DecimalType(precision, 0)
+    if args.type == ct.FloatType():
+        precision = max(14, -target_scale + 1)
+        scale = min(7, max(0, target_scale))
+        return ct.DecimalType(precision, scale)
+    if args.type == ct.DoubleType():
+        precision = max(30, -target_scale + 1)
+        scale = min(15, max(0, target_scale))
+        return ct.DecimalType(precision, scale)
+
+    raise DJParseException(
+        f"Unhandled numeric type in Floor `{args.type}`",
+    )  # pragma: no cover
 
 
 class IfNull(Function):
     """
     Returns the second expression if the first is null, else returns the first expression.
     """
 
@@ -1227,14 +1225,36 @@
 @Explode.register
 def infer_type(  # noqa: F811  # pylint: disable=function-redefined
     arg: ct.MapType,
 ) -> List[ct.NestedField]:
     return [arg.key, arg.value]
 
 
+class Unnest(TableFunction):  # pylint: disable=abstract-method
+    """
+    The unnest function is used to explode the specified array,
+    nested array, or map column into multiple rows.
+    It will generate a new row for each element in the specified column.
+    """
+
+
+@Unnest.register
+def infer_type(  # noqa: F811  # pylint: disable=function-redefined
+    arg: ct.ListType,
+) -> List[ct.NestedField]:
+    return [arg.element]  # pragma: no cover
+
+
+@Unnest.register
+def infer_type(  # noqa: F811  # pylint: disable=function-redefined
+    arg: ct.MapType,
+) -> List[ct.NestedField]:
+    return [arg.key, arg.value]
+
+
 function_registry = FunctionRegistryDict()
 for cls in Function.__subclasses__():
     snake_cased = re.sub(r"(?<!^)(?=[A-Z])", "_", cls.__name__)
     function_registry[cls.__name__.upper()] = cls
     function_registry[snake_cased.upper()] = cls
```

### Comparing `datajunction-0.0.1a4/dj/sql/parse.py` & `datajunction-0.0.1a5/dj/sql/parse.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a4/dj/sql/parsing/ast.py` & `datajunction-0.0.1a5/dj/sql/parsing/ast.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,22 +33,23 @@
 from dj.models.node import NodeRevision
 from dj.models.node import NodeRevision as DJNode
 from dj.models.node import NodeType
 from dj.models.node import NodeType as DJNodeType
 from dj.sql.functions import function_registry, table_function_registry
 from dj.sql.parsing.backends.exceptions import DJParseException
 from dj.sql.parsing.types import (
+    BigIntType,
     BooleanType,
     ColumnType,
     DayTimeIntervalType,
     DecimalType,
     DoubleType,
     FloatType,
+    IntegerBase,
     IntegerType,
-    LongType,
     MapType,
     NestedField,
     NullType,
     StringType,
     WildcardType,
     YearMonthIntervalType,
 )
@@ -821,15 +822,15 @@
         source_table = cast(TableExpression, found_sources[0])
         source_table.add_ref_column(self, ctx)
         self._is_compiled = True
 
     def __str__(self) -> str:
         as_ = " AS " if self.as_ else " "
         alias = "" if not self.alias else f"{as_}{self.alias}"
-        if self.table is not None:
+        if self.table is not None and not isinstance(self.table, FunctionTable):
             ret = f"{self.table.alias_or_name.name}.{self.name.quote_style}{self.name.name}{self.name.quote_style}"
         else:
             ret = str(self.name)
         if self.parenthesized:
             ret = f"({ret})"
         return ret + alias
 
@@ -915,46 +916,42 @@
             if ctx is None:
                 raise DJErrorException(
                     "Uncompiled Table expression requested to "
                     "add Column ref without a compilation context.",
                 )
             self.compile(ctx)
 
+        # For table-valued functions, add the list of columns that gets
+        # returned as reference columns and compile them
         if isinstance(self, FunctionTable):
-            matched = False
-            if not self.alias and not column.namespace:
-                matched = True
-            elif (
-                self.alias
-                and column.name.namespace
-                and self.alias == column.name.namespace
+            if (
+                not self.alias
+                and not column.name.namespace
+                or (
+                    self.alias
+                    and column.name.namespace
+                    and self.alias == column.name.namespace
+                )
             ):
-                matched = True
-            if matched:
                 for col in self.column_list:
-                    if (
-                        column.name == col.alias_or_name
-                        and column.name.namespace == col.alias_or_name.namespace
-                    ):
+                    if column.name.name == col.alias_or_name.name:
                         self._ref_columns.append(column)
                         column.add_table(self)
                         column.add_expression(col)
                         column.add_type(col.type)
                         return True
 
         for col in self.columns:
-            if not isinstance(col, (Aliasable, Named)):
-                continue
-
-            if column.name.name == col.alias_or_name.identifier(False):
-                self._ref_columns.append(column)
-                column.add_table(self)
-                column.add_expression(col)
-                column.add_type(col.type)
-                return True
+            if isinstance(col, (Aliasable, Named)):
+                if column.name.name == col.alias_or_name.identifier(False):
+                    self._ref_columns.append(column)
+                    column.add_table(self)
+                    column.add_expression(col)
+                    column.add_type(col.type)
+                    return True
         return False
 
     def is_compiled(self) -> bool:  # noqa: F811
         return bool(self._columns) or self._is_compiled
 
     def in_from_or_lateral(self) -> bool:
         """
@@ -1195,15 +1192,15 @@
 
         numeric_types = {
             type_: idx
             for idx, type_ in enumerate(
                 [
                     str(DoubleType()),
                     str(FloatType()),
-                    str(LongType()),
+                    str(BigIntType()),
                     str(IntegerType()),
                 ],
             )
         }
 
         def resolve_numeric_types_binary_operations(
             left: ColumnType,
@@ -1391,14 +1388,15 @@
 @dataclass(eq=False)
 class Number(Value):
     """
     Number value
     """
 
     value: Union[float, int, decimal.Decimal]
+    _type: Optional[IntegerBase] = None
 
     def __post_init__(self):
         super().__post_init__()
 
         if (
             not isinstance(self.value, float)
             and not isinstance(self.value, int)
@@ -1421,17 +1419,22 @@
     @property
     def type(self) -> ColumnType:
         """
         Determine the type of the numeric expression.
         """
         # We won't assume that anyone wants SHORT by default
         if isinstance(self.value, int):
-            if self.value <= IntegerType.min or self.value >= IntegerType.max:
-                return LongType()
-            return IntegerType()
+            check_types = (self._type,) if self._type else (IntegerType(), BigIntType())
+            for integer_type in check_types:
+                if integer_type.check_bounds(self.value):
+                    return integer_type
+
+            raise DJParseException(
+                f"No Integer type of {check_types} can hold the value {self.value}.",
+            )
         #
         # # Arbitrary-precision floating point
         # if isinstance(self.value, decimal.Decimal):
         #     return DecimalType.parse(self.value)
 
         # Double-precision floating point
         if not (1.18e-38 <= abs(self.value) <= 3.4e38):
@@ -1844,21 +1847,20 @@
         alias = f" {self.alias}" if self.alias else ""
         as_ = " AS " if self.as_ else ""
         cols = (
             f" {', '.join(str(col) for col in self.column_list)}"
             if self.column_list
             else ""
         )
-        if len(self.column_list) > 1:
-            cols = f"({cols})"
+        column_list_str = f"({cols})" if alias else str(cols)
         args_str = f"({', '.join(str(col) for col in self.args)})" if self.args else ""
-        return f"{self.name}{args_str}{alias}{as_}{cols}"
+        return f"{self.name}{args_str}{alias}{as_}{column_list_str}"
 
-    def set_alias(self: TNode, alias: List[Column]) -> TNode:
-        self.column_list = alias
+    def set_alias(self: TNode, alias: Name) -> TNode:
+        self.alias = alias
         return self
 
     def _type(self, ctx: Optional[CompileContext] = None) -> List[NestedField]:
         name = self.name.name.upper()
         dj_func = table_function_registry[name]
         arg_types = []
         for arg in self.args:
```

### Comparing `datajunction-0.0.1a4/dj/sql/parsing/backends/antlr4.py` & `datajunction-0.0.1a5/dj/sql/parsing/backends/antlr4.py`

 * *Files 0% similar despite different names*

```diff
@@ -678,23 +678,23 @@
 def _(ctx: sbp.LateralViewContext):
     outer = bool(ctx.OUTER())
     func_name = visit(ctx.qualifiedName())
     func_args = visit(ctx.expression())
     table_name = visit(ctx.tblName)
     function_table_name = table_name if table_name != ast.Name(name="AS") else None
     func = ast.FunctionTable(func_name, args=func_args, alias=function_table_name)
-    func.set_alias(table_name)
+    func.set_alias(function_table_name)
     if function_table_name:
         func.column_list = [
             ast.Column(name=ast.Name(name=name.name, namespace=function_table_name))
             for name in visit(ctx.colName)
         ]
     else:
         func.column_list = [ast.Column(name=name) for name in visit(ctx.colName)]
-    if ctx.AS():
+    if ctx.AS() or table_name == ast.Name(name="AS"):
         func.set_as(True)
     return ast.LateralView(outer, func)
 
 
 @visit.register
 def _(ctx: sbp.RelationContext):
     primary_relation = visit(ctx.relationPrimary())
@@ -739,19 +739,23 @@
 
 
 @visit.register
 def _(ctx: sbp.FunctionTableContext):
     name = visit(ctx.funcName)
     args = visit(ctx.expression())
     alias, cols = visit(ctx.tableAlias())
-    return ast.FunctionTable(
+    func_table = ast.FunctionTable(
         name,
         args=args,
         column_list=[ast.Column(name) for name in cols],
-    ).set_alias(alias)
+        alias=alias,
+    )
+    if not cols:
+        func_table.column_list = alias
+    return func_table
 
 
 @visit.register
 def _(ctx: sbp.TableAliasContext):
     if ident := ctx.strictIdentifier():
         identifier_list = visit(ctx.identifierList()) if ctx.identifierList() else []
         return visit(ident), identifier_list
```

### Comparing `datajunction-0.0.1a4/dj/sql/parsing/backends/grammar/SqlBaseLexer.g4` & `datajunction-0.0.1a5/dj/sql/parsing/backends/grammar/SqlBaseLexer.g4`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a4/dj/sql/parsing/backends/grammar/SqlBaseParser.g4` & `datajunction-0.0.1a5/dj/sql/parsing/backends/grammar/SqlBaseParser.g4`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a4/dj/sql/parsing/backends/grammar/generated/SqlBaseLexer.interp` & `datajunction-0.0.1a5/dj/sql/parsing/backends/grammar/generated/SqlBaseLexer.interp`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a4/dj/sql/parsing/backends/grammar/generated/SqlBaseLexer.py` & `datajunction-0.0.1a5/dj/sql/parsing/backends/grammar/generated/SqlBaseLexer.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a4/dj/sql/parsing/backends/grammar/generated/SqlBaseLexer.tokens` & `datajunction-0.0.1a5/dj/sql/parsing/backends/grammar/generated/SqlBaseLexer.tokens`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a4/dj/sql/parsing/backends/grammar/generated/SqlBaseParser.interp` & `datajunction-0.0.1a5/dj/sql/parsing/backends/grammar/generated/SqlBaseParser.interp`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a4/dj/sql/parsing/backends/grammar/generated/SqlBaseParser.py` & `datajunction-0.0.1a5/dj/sql/parsing/backends/grammar/generated/SqlBaseParser.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a4/dj/sql/parsing/backends/grammar/generated/SqlBaseParser.tokens` & `datajunction-0.0.1a5/dj/sql/parsing/backends/grammar/generated/SqlBaseParser.tokens`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a4/dj/sql/parsing/backends/grammar/generated/SqlBaseParserListener.py` & `datajunction-0.0.1a5/dj/sql/parsing/backends/grammar/generated/SqlBaseParserListener.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a4/dj/sql/parsing/backends/grammar/generated/SqlBaseParserVisitor.py` & `datajunction-0.0.1a5/dj/sql/parsing/backends/grammar/generated/SqlBaseParserVisitor.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a4/dj/sql/parsing/types.py` & `datajunction-0.0.1a5/dj/sql/parsing/types.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 field_type=StringType(), is_optional=False, doc='a required field'), \
 NestedField(name=Name(name='optional_field', quote_style='', namespace=None), \
 field_type=IntegerType(), is_optional=True, doc='an optional field'))
 
 """
 
 import re
+from enum import Enum
 from typing import TYPE_CHECKING, Any, ClassVar, Dict, Generator, Optional, Tuple, cast
 
 from pydantic import BaseModel, Extra
 from pydantic.class_validators import AnyCallable
 
 if TYPE_CHECKING:
     from dj.sql.parsing import ast
@@ -103,14 +104,47 @@
 
     def __hash__(self):
         """
         Equality is dependent on the string representation of the column type.
         """
         return hash(str(self))
 
+    def is_compatible(self, other: "ColumnType") -> bool:
+        """
+        Returns whether the two types are compatible with each other by
+        checking their ancestors.
+        """
+        if self == other:
+            return True  # quick return
+
+        def has_common_ancestor(type1, type2) -> bool:
+            """
+            Helper function to check whether two column types have common ancestors,
+            other than the highest-level ancestor types like ColumnType itself. This
+            determines whether they're part of the same type group and are compatible
+            with each other when performing type compatibility checks.
+            """
+            base_types = (ColumnType, Singleton, PrimitiveType)
+            if type1 in base_types or type2 in base_types:
+                return False
+            if type1 == type2:
+                return True
+            current_has = False
+            for ancestor in type1.__bases__:
+                for ancestor2 in type2.__bases__:
+                    current_has = current_has or has_common_ancestor(
+                        ancestor,
+                        ancestor2,
+                    )
+                    if current_has:
+                        return current_has
+            return False
+
+        return has_common_ancestor(self.__class__, other.__class__)
+
 
 class PrimitiveType(ColumnType):  # pylint: disable=too-few-public-methods
     """Base class for all Column Primitive Types"""
 
 
 class NumberType(PrimitiveType):  # pylint: disable=too-few-public-methods
     """Base class for all Column Number Types"""
@@ -121,16 +155,15 @@
 
     Example:
         >>> NullType()
         NullType()
     """
 
     def __init__(self):
-        if not self._initialized:
-            super().__init__("NULL", "NullType()")
+        super().__init__("NULL", "NullType()")
 
 
 class FixedType(PrimitiveType):
     """A fixed data type.
 
     Example:
         >>> FixedType(8)
@@ -177,20 +210,22 @@
             min(precision, DecimalType.max_precision),
             min(scale, DecimalType.max_scale),
         )
         cls._instances[key] = cls._instances.get(key) or object.__new__(cls)
         return cls._instances[key]
 
     def __init__(self, precision: int, scale: int):
-        super().__init__(
-            f"decimal({precision}, {scale})",
-            f"DecimalType(precision={precision}, scale={scale})",
-        )
-        self._precision = min(precision, DecimalType.max_precision)
-        self._scale = min(scale, DecimalType.max_scale)
+
+        if not self._initialized:
+            super().__init__(
+                f"decimal({precision}, {scale})",
+                f"DecimalType(precision={precision}, scale={scale})",
+            )
+            self._precision = min(precision, DecimalType.max_precision)
+            self._scale = min(scale, DecimalType.max_scale)
 
     @property
     def precision(self) -> int:  # pragma: no cover
         """
         Decimal's precision
         """
         return self._precision
@@ -235,22 +270,21 @@
     def __init__(
         self,
         name: "ast.Name",
         field_type: ColumnType,
         is_optional: bool = True,
         doc: Optional[str] = None,
     ):
-        if isinstance(name, str):  # pragma: no cover
-            from dj.sql.parsing.ast import (  # pylint: disable=import-outside-toplevel
-                Name,
-            )
-
-            name = Name(name)
-
         if not self._initialized:
+            if isinstance(name, str):  # pragma: no cover
+                from dj.sql.parsing.ast import (  # pylint: disable=import-outside-toplevel
+                    Name,
+                )
+
+                name = Name(name)
             doc_string = "" if doc is None else f", doc={repr(doc)}"
             super().__init__(
                 (
                     f"{name}: {field_type}"
                     f"{' NOT NULL' if not is_optional else ''}"
                     + ("" if doc is None else f" {doc}")
                 ),
@@ -354,20 +388,20 @@
         cls._instances[key] = cls._instances.get(key) or object.__new__(cls)  # type: ignore
         return cls._instances[key]  # type: ignore
 
     def __init__(
         self,
         element_type: ColumnType,
     ):
+
         if not self._initialized:
             super().__init__(
                 f"array<{element_type}>",
                 f"ListType(element_type={repr(element_type)})",
             )
-
             self._element_field = NestedField(
                 name="col",  # type: ignore
                 field_type=element_type,
                 is_optional=False,  # type: ignore
             )
 
     @property
@@ -393,14 +427,15 @@
         return cls._instances[impl_key]
 
     def __init__(
         self,
         key_type: ColumnType,
         value_type: ColumnType,
     ):
+
         if not self._initialized:
             super().__init__(
                 f"map<{key_type}, {value_type}>",
             )
             self._key_field = NestedField(
                 name="key",  # type: ignore
                 field_type=key_type,
@@ -433,21 +468,29 @@
     Example:
         >>> column_foo = BooleanType()
         >>> isinstance(column_foo, BooleanType)
         True
     """
 
     def __init__(self):
-        # if not self._initialized:
         super().__init__("boolean", "BooleanType()")
 
 
 class IntegerBase(NumberType, Singleton):
     """Base class for all integer types"""
 
+    max: ClassVar[int]
+    min: ClassVar[int]
+
+    def check_bounds(self, value: int) -> bool:
+        """
+        Check whether a value fits within the Integer min and max
+        """
+        return self.__class__.min < value < self.__class__.max
+
 
 class IntegerType(IntegerBase):
     """An Integer data type can be represented using an instance of this class. Integers are
     32-bit signed and can be promoted to Longs.
 
     Example:
         >>> column_foo = IntegerType()
@@ -464,16 +507,15 @@
     """
 
     max: ClassVar[int] = 2147483647
 
     min: ClassVar[int] = -2147483648
 
     def __init__(self):
-        if not self._initialized:
-            super().__init__("int", "IntegerType()")
+        super().__init__("int", "IntegerType()")
 
 
 class TinyIntType(IntegerBase):
     """A TinyInt data type can be represented using an instance of this class. TinyInts are
     8-bit signed integers.
 
     Example:
@@ -487,25 +529,46 @@
     """
 
     max: ClassVar[int] = 127
 
     min: ClassVar[int] = -128
 
     def __init__(self):
-        if not self._initialized:
-            super().__init__("tinyint", "TinyIntType()")
+        super().__init__("tinyint", "TinyIntType()")
+
+
+class SmallIntType(IntegerBase):  # pylint: disable=R0901
+    """A SmallInt data type can be represented using an instance of this class. SmallInts are
+    16-bit signed integers.
+
+    Example:
+        >>> column_foo = SmallIntType()
+        >>> isinstance(column_foo, SmallIntType)
+        True
+
+    Attributes:
+        max (int): The maximum allowed value for SmallInts (returns `32767`).
+        min (int): The minimum allowed value for SmallInts (returns `-32768`).
+    """
 
+    max: ClassVar[int] = 32767
 
-class LongType(IntegerBase):
+    min: ClassVar[int] = -32768
+
+    def __init__(self):
+        super().__init__("smallint", "SmallIntType()")
+
+
+class BigIntType(IntegerBase):
     """A Long data type can be represented using an instance of this class. Longs are
     64-bit signed integers.
 
     Example:
-        >>> column_foo = LongType()
-        >>> isinstance(column_foo, LongType)
+        >>> column_foo = BigIntType()
+        >>> isinstance(column_foo, BigIntType)
         True
 
     Attributes:
         max (int): The maximum allowed value for Longs, inherited from the
         canonical Column implementation
           in Java. (returns `9223372036854775807`)
         min (int): The minimum allowed value for Longs, inherited from the
@@ -514,108 +577,39 @@
     """
 
     max: ClassVar[int] = 9223372036854775807
 
     min: ClassVar[int] = -9223372036854775808
 
     def __init__(self):
-        if not self._initialized:
-            super().__init__("long", "LongType()")
-
+        super().__init__("bigint", "BigIntType()")
 
-class IntervalTypeBase(PrimitiveType):
-    """A base class for all interval types"""
 
-
-class DayTimeIntervalType(IntervalTypeBase):
-    """A DayTimeIntervalType type.
+class LongType(BigIntType):  # pylint: disable=R0901
+    """A Long data type can be represented using an instance of this class. Longs are
+    64-bit signed integers.
 
     Example:
-        >>> DayTimeIntervalType()==DayTimeIntervalType("DAY", "SECOND")
+        >>> column_foo = LongType()
+        >>> column_foo == LongType()
         True
-    """
 
-    _instances: Dict[Tuple[str, str], "DayTimeIntervalType"] = {}
-
-    def __new__(
-        cls,
-        from_: Optional[str] = "DAY",
-        to_: Optional[str] = "SECOND",
-    ):
-        key = (from_.upper(), to_.upper())  # type: ignore
-        cls._instances[key] = cls._instances.get(key) or object.__new__(cls)
-        return cls._instances[key]
-
-    def __init__(
-        self,
-        from_: str = "DAY",
-        to_: Optional[str] = "SECOND",
-    ):
-        from_ = from_.upper()
-        to_ = to_.upper()  # type: ignore
-        to_str = f" TO {to_}" if to_ else ""
-        to_repr = f', to="{to_}"' if to_ else ""
-        super().__init__(
-            f"INTERVAL {from_}{to_str}",
-            f'DayTimeIntervalType(from="{from_}"{to_repr})',
-        )
-        self._from = from_
-        self._to = to_
-
-    @property
-    def from_(self) -> str:  # pylint: disable=missing-function-docstring
-        return self._from  # pragma: no cover
-
-    @property
-    def to_(  # pylint: disable=missing-function-docstring
-        self,
-    ) -> Optional[str]:
-        return self._to  # pragma: no cover
-
-
-class YearMonthIntervalType(IntervalTypeBase):
-    """A YearMonthIntervalType type.
-
-    Example:
-        >>> YearMonthIntervalType()==YearMonthIntervalType("YEAR", "MONTH")
-        True
+    Attributes:
+        max (int): The maximum allowed value for Longs, inherited from the
+        canonical Column implementation
+          in Java. (returns `9223372036854775807`)
+        min (int): The minimum allowed value for Longs, inherited from the
+        canonical Column implementation
+          in Java (returns `-9223372036854775808`)
     """
 
-    _instances: Dict[Tuple[str, str], "YearMonthIntervalType"] = {}
-
-    def __new__(cls, from_: Optional[str] = "YEAR", to_: Optional[str] = "MONTH"):
-        key = (from_.upper(), to_.upper())  # type: ignore
-        cls._instances[key] = cls._instances.get(key) or object.__new__(cls)
-        return cls._instances[key]
-
-    def __init__(
-        self,
-        from_: str = "YEAR",
-        to_: Optional[str] = "MONTH",
-    ):
-        from_ = from_.upper()
-        to_ = to_.upper()  # type: ignore
-        to_str = f" TO {to_}" if to_ else ""
-        to_repr = f', to="{to_}"' if to_ else ""
-        super().__init__(
-            f"INTERVAL {from_}{to_str}",
-            f'YearMonthIntervalType(from="{from_}"{to_repr})',
-        )
-        self._from = from_
-        self._to = to_
-
-    @property
-    def from_(self) -> str:  # pylint: disable=missing-function-docstring
-        return self._from  # pragma: no cover
-
-    @property
-    def to_(  # pylint: disable=missing-function-docstring
-        self,
-    ) -> Optional[str]:
-        return self._to  # pragma: no cover
+    def __new__(cls, *args, **kwargs):
+        self = super().__new__(BigIntType, *args, **kwargs)
+        super(BigIntType, self).__init__("long", "LongType()")
+        return self
 
 
 class FloatingBase(NumberType, Singleton):
     """Base class for all floating types"""
 
 
 class FloatType(FloatingBase):
@@ -625,158 +619,293 @@
     Example:
         >>> column_foo = FloatType()
         >>> isinstance(column_foo, FloatType)
         True
     """
 
     def __init__(self):
-        if not self._initialized:
-            super().__init__("float", "FloatType()")
+        super().__init__("float", "FloatType()")
 
 
 class DoubleType(FloatingBase):
     """A Double data type can be represented using an instance of this class. Doubles are
     64-bit IEEE 754 floating points.
 
     Example:
         >>> column_foo = DoubleType()
         >>> isinstance(column_foo, DoubleType)
         True
     """
 
     def __init__(self):
-        if not self._initialized:
-            super().__init__("double", "DoubleType()")
+        super().__init__("double", "DoubleType()")
+
+
+class DateTimeBase(PrimitiveType, Singleton):
+    """
+    Base class for date and time types.
+    """
+
+    # pylint: disable=invalid-name
+    class Unit(str, Enum):
+        """
+        Units used for date and time functions and intervals
+        """
 
+        dayofyear = "DAYOFYEAR"
+        year = "YEAR"
+        day = "DAY"
+        microsecond = "MICROSECOND"
+        month = "MONTH"
+        week = "WEEK"
+        minute = "MINUTE"
+        second = "SECOND"
+        quarter = "QUARTER"
+        hour = "HOUR"
+        millisecond = "MILLISECOND"
 
-class DateType(PrimitiveType, Singleton):
+    # pylint: enable=invalid-name
+
+
+class DateType(DateTimeBase):
     """A Date data type can be represented using an instance of this class. Dates are
     calendar dates without a timezone or time.
 
     Example:
         >>> column_foo = DateType()
         >>> isinstance(column_foo, DateType)
         True
     """
 
     def __init__(self):
-        if not self._initialized:
-            super().__init__("date", "DateType()")
+        super().__init__("date", "DateType()")
 
 
-class TimeType(PrimitiveType, Singleton):
+class TimeType(DateTimeBase):
     """A Time data type can be represented using an instance of this class. Times
     have microsecond precision and are a time of day without a date or timezone.
 
     Example:
         >>> column_foo = TimeType()
         >>> isinstance(column_foo, TimeType)
         True
     """
 
     def __init__(self):
-        if not self._initialized:
-            super().__init__("time", "TimeType()")
+        super().__init__("time", "TimeType()")
 
 
 class TimestampType(PrimitiveType, Singleton):
     """A Timestamp data type can be represented using an instance of this class. Timestamps in
     Column have microsecond precision and include a date and a time of day without a timezone.
 
     Example:
         >>> column_foo = TimestampType()
         >>> isinstance(column_foo, TimestampType)
         True
     """
 
     def __init__(self):
-        if not self._initialized:
-            super().__init__("timestamp", "TimestampType()")
+        super().__init__("timestamp", "TimestampType()")
 
 
 class TimestamptzType(PrimitiveType, Singleton):
     """A Timestamptz data type can be represented using an instance of this class. Timestamptzs in
     Column are stored as UTC and include a date and a time of day with a timezone.
 
     Example:
         >>> column_foo = TimestamptzType()
         >>> isinstance(column_foo, TimestamptzType)
         True
     """
 
     def __init__(self):
+        super().__init__("timestamptz", "TimestamptzType()")
+
+
+class IntervalTypeBase(PrimitiveType):
+    """A base class for all interval types"""
+
+
+class DayTimeIntervalType(IntervalTypeBase):
+    """A DayTimeIntervalType type.
+
+    Example:
+        >>> DayTimeIntervalType()==DayTimeIntervalType("DAY", "SECOND")
+        True
+    """
+
+    _instances: Dict[Tuple[str, str], "DayTimeIntervalType"] = {}
+
+    def __new__(
+        cls,
+        from_: DateTimeBase.Unit = DateTimeBase.Unit.day,
+        to_: Optional[DateTimeBase.Unit] = DateTimeBase.Unit.second,
+    ):
+        key = (from_.upper(), to_.upper())  # type: ignore
+        cls._instances[key] = cls._instances.get(key) or object.__new__(cls)
+        return cls._instances[key]
+
+    def __init__(
+        self,
+        from_: DateTimeBase.Unit = DateTimeBase.Unit.day,
+        to_: Optional[DateTimeBase.Unit] = DateTimeBase.Unit.second,
+    ):
+        if not self._initialized:
+            from_ = from_.upper()  # type: ignore
+            to_ = to_.upper()  # type: ignore
+            to_str = f" TO {to_}" if to_ else ""
+            to_repr = f', to="{to_}"' if to_ else ""
+            super().__init__(
+                f"INTERVAL {from_}{to_str}",
+                f'DayTimeIntervalType(from="{from_}"{to_repr})',
+            )
+            self._from = from_
+            self._to = to_
+
+    @property
+    def from_(self) -> str:  # pylint: disable=missing-function-docstring
+        return self._from  # pragma: no cover
+
+    @property
+    def to_(  # pylint: disable=missing-function-docstring
+        self,
+    ) -> Optional[str]:
+        return self._to  # pragma: no cover
+
+
+class YearMonthIntervalType(IntervalTypeBase):
+    """A YearMonthIntervalType type.
+
+    Example:
+        >>> YearMonthIntervalType()==YearMonthIntervalType("YEAR", "MONTH")
+        True
+    """
+
+    _instances: Dict[Tuple[str, str], "YearMonthIntervalType"] = {}
+
+    def __new__(
+        cls,
+        from_: DateTimeBase.Unit = DateTimeBase.Unit.year,
+        to_: Optional[DateTimeBase.Unit] = DateTimeBase.Unit.month,
+    ):
+        key = (from_.upper(), to_.upper())  # type: ignore
+        cls._instances[key] = cls._instances.get(key) or object.__new__(cls)
+        return cls._instances[key]
+
+    def __init__(
+        self,
+        from_: DateTimeBase.Unit = DateTimeBase.Unit.year,
+        to_: Optional[DateTimeBase.Unit] = DateTimeBase.Unit.month,
+    ):
         if not self._initialized:
-            super().__init__("timestamptz", "TimestamptzType()")
+            from_ = from_.upper()  # type: ignore
+            to_ = to_.upper()  # type: ignore
+            to_str = f" TO {to_}" if to_ else ""
+            to_repr = f', to="{to_}"' if to_ else ""
+            super().__init__(
+                f"INTERVAL {from_}{to_str}",
+                f'YearMonthIntervalType(from="{from_}"{to_repr})',
+            )
+            self._from = from_
+            self._to = to_
+
+    @property
+    def from_(self) -> str:  # pylint: disable=missing-function-docstring
+        return self._from  # pragma: no cover
+
+    @property
+    def to_(  # pylint: disable=missing-function-docstring
+        self,
+    ) -> Optional[str]:
+        return self._to  # pragma: no cover
+
 
+class StringBase(PrimitiveType, Singleton):
+    """Base class for all string types"""
 
-class StringType(PrimitiveType, Singleton):
+
+class StringType(StringBase):
     """A String data type can be represented using an instance of this class. Strings in
     Column are arbitrary-length character sequences and are encoded with UTF-8.
 
     Example:
         >>> column_foo = StringType()
         >>> isinstance(column_foo, StringType)
         True
     """
 
     def __init__(self):
-        if not self._initialized:
-            super().__init__("string", "StringType()")
+        super().__init__("string", "StringType()")
+
+
+class VarcharType(StringBase):
+    """A VarcharType data type can be represented using an instance of this class.
+    Varchars in Column are arbitrary-length character sequences and are
+    encoded with UTF-8.
+
+    Example:
+        >>> column_foo = VarcharType()
+        >>> isinstance(column_foo, VarcharType)
+        True
+    """
+
+    def __init__(self):
+        super().__init__("varchar", "VarcharType()")
 
 
 class UUIDType(PrimitiveType, Singleton):
     """A UUID data type can be represented using an instance of this class. UUIDs in
     Column are universally unique identifiers.
 
     Example:
         >>> column_foo = UUIDType()
         >>> isinstance(column_foo, UUIDType)
         True
     """
 
     def __init__(self):
-        if not self._initialized:
-            super().__init__("uuid", "UUIDType()")
+        super().__init__("uuid", "UUIDType()")
 
 
 class BinaryType(PrimitiveType, Singleton):
     """A Binary data type can be represented using an instance of this class. Binarys in
     Column are arbitrary-length byte arrays.
 
     Example:
         >>> column_foo = BinaryType()
         >>> isinstance(column_foo, BinaryType)
         True
     """
 
     def __init__(self):
-        if not self._initialized:
-            super().__init__("binary", "BinaryType()")
+        super().__init__("binary", "BinaryType()")
 
 
 class WildcardType(PrimitiveType, Singleton):
     """A Wildcard datatype.
 
     Example:
         >>> column_foo = WildcardType()
         >>> isinstance(column_foo, WildcardType)
         True
     """
 
     def __init__(self):
-        if not self._initialized:
-            super().__init__("wildcard", "WildcardType()")
+        super().__init__("wildcard", "WildcardType()")
 
 
 # Define the primitive data types and their corresponding Python classes
 PRIMITIVE_TYPES: Dict[str, PrimitiveType] = {
     "bool": BooleanType(),
     "boolean": BooleanType(),
+    "varchar": VarcharType(),
+    "bigint": BigIntType(),
     "int": IntegerType(),
-    "long": LongType(),
+    "long": BigIntType(),
     "float": FloatType(),
     "double": DoubleType(),
     "date": DateType(),
     "time": TimeType(),
     "timestamp": TimestampType(),
     "timestamptz": TimestamptzType(),
     "string": StringType(),
```

### Comparing `datajunction-0.0.1a4/dj/superset.py` & `datajunction-0.0.1a5/dj/superset.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a4/dj/typing.py` & `datajunction-0.0.1a5/dj/typing.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a4/dj/utils.py` & `datajunction-0.0.1a5/dj/utils.py`

 * *Files identical despite different names*

### Comparing `datajunction-0.0.1a4/pyproject.toml` & `datajunction-0.0.1a5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 [tool.setuptools_scm]
 # See configuration details in https://github.com/pypa/setuptools_scm
 version_scheme = "no-guess-dev"
 
 [tool.poetry]
 name = "datajunction"
-version = "0.0.1a4"
+version = "0.0.1a5"
 readme = "README.rst"
 repository = "https://github.com/DataJunction/dj"
 description = "DataJunction server library for running to a DataJunction server"
 authors = ["DataJunction Authors"]
 license = "MIT"
 packages = [
     { include = "dj" },
```

### Comparing `datajunction-0.0.1a4/PKG-INFO` & `datajunction-0.0.1a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datajunction
-Version: 0.0.1a4
+Version: 0.0.1a5
 Summary: DataJunction server library for running to a DataJunction server
 Home-page: https://github.com/DataJunction/dj
 License: MIT
 Author: DataJunction Authors
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

