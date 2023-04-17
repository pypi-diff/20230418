# Comparing `tmp/kgx-2.0.4.tar.gz` & `tmp/kgx-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kgx-2.0.4.tar", max compression
+gzip compressed data, was "kgx-2.0.5.tar", max compression
```

## Comparing `kgx-2.0.4.tar` & `kgx-2.0.5.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     1526 2023-04-14 23:05:45.561249 kgx-2.0.4/LICENSE
--rw-r--r--   0        0        0     6472 2023-04-14 23:05:45.561249 kgx-2.0.4/README.md
--rw-r--r--   0        0        0       42 2023-04-14 23:06:15.201541 kgx-2.0.4/kgx/__init__.py
--rw-r--r--   0        0        0    16105 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/cli/__init__.py
--rw-r--r--   0        0        0    39538 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/cli/cli_utils.py
--rw-r--r--   0        0        0     3900 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/config.py
--rw-r--r--   0        0        0      731 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/config.yml
--rw-r--r--   0        0        0     1942 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/curie_lookup_service.py
--rw-r--r--   0        0        0     5094 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/error_detection.py
--rw-r--r--   0        0        0        0 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/graph/__init__.py
--rw-r--r--   0        0        0    10649 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/graph/base_graph.py
--rw-r--r--   0        0        0    13455 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/graph/nx_graph.py
--rw-r--r--   0        0        0     8498 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/graph_operations/__init__.py
--rw-r--r--   0        0        0    28863 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/graph_operations/clique_merge.py
--rw-r--r--   0        0        0     5776 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/graph_operations/graph_merge.py
--rw-r--r--   0        0        0    36314 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/graph_operations/meta_knowledge_graph.py
--rw-r--r--   0        0        0    30601 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/graph_operations/summarize_graph.py
--rw-r--r--   0        0        0        0 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/parsers/__init__.py
--rw-r--r--   0        0        0     2156 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/parsers/ntriples_parser.py
--rw-r--r--   0        0        0     6617 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/prefix_manager.py
--rw-r--r--   0        0        0      274 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/sink/__init__.py
--rw-r--r--   0        0        0     1703 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/sink/graph_sink.py
--rw-r--r--   0        0        0     2335 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/sink/json_sink.py
--rw-r--r--   0        0        0     2242 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/sink/jsonl_sink.py
--rw-r--r--   0        0        0     9073 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/sink/neo_sink.py
--rw-r--r--   0        0        0     1356 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/sink/null_sink.py
--rw-r--r--   0        0        0    20014 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/sink/rdf_sink.py
--rw-r--r--   0        0        0     1436 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/sink/sink.py
--rw-r--r--   0        0        0    10327 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/sink/sql_sink.py
--rw-r--r--   0        0        0     8070 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/sink/tsv_sink.py
--rw-r--r--   0        0        0      395 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/source/__init__.py
--rw-r--r--   0        0        0     2526 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/source/graph_source.py
--rw-r--r--   0        0        0     2399 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/source/json_source.py
--rw-r--r--   0        0        0     1821 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/source/jsonl_source.py
--rw-r--r--   0        0        0    18963 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/source/neo_source.py
--rw-r--r--   0        0        0    11785 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/source/obograph_source.py
--rw-r--r--   0        0        0     7503 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/source/owl_source.py
--rw-r--r--   0        0        0    30464 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/source/rdf_source.py
--rw-r--r--   0        0        0    12162 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/source/source.py
--rw-r--r--   0        0        0     8221 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/source/sssom_source.py
--rw-r--r--   0        0        0     3665 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/source/trapi_source.py
--rw-r--r--   0        0        0     9150 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/source/tsv_source.py
--rw-r--r--   0        0        0    16628 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/transformer.py
--rw-r--r--   0        0        0        0 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/utils/__init__.py
--rw-r--r--   0        0        0     4575 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/utils/graph_utils.py
--rw-r--r--   0        0        0    18032 2023-04-14 23:05:45.565249 kgx-2.0.4/kgx/utils/infores.py
--rw-r--r--   0        0        0    31762 2023-04-14 23:05:45.569249 kgx-2.0.4/kgx/utils/kgx_utils.py
--rw-r--r--   0        0        0     8159 2023-04-14 23:05:45.569249 kgx-2.0.4/kgx/utils/rdf_utils.py
--rw-r--r--   0        0        0    28313 2023-04-14 23:05:45.569249 kgx-2.0.4/kgx/validator.py
--rw-r--r--   0        0        0     1591 2023-04-14 23:06:15.197540 kgx-2.0.4/pyproject.toml
--rw-r--r--   0        0        0     8531 1970-01-01 00:00:00.000000 kgx-2.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1526 2023-04-17 23:39:33.857345 kgx-2.0.5/LICENSE
+-rw-r--r--   0        0        0     6473 2023-04-17 23:39:33.857345 kgx-2.0.5/README.md
+-rw-r--r--   0        0        0       42 2023-04-17 23:39:49.169428 kgx-2.0.5/kgx/__init__.py
+-rw-r--r--   0        0        0    16105 2023-04-17 23:39:33.861345 kgx-2.0.5/kgx/cli/__init__.py
+-rw-r--r--   0        0        0    39538 2023-04-17 23:39:33.861345 kgx-2.0.5/kgx/cli/cli_utils.py
+-rw-r--r--   0        0        0     3900 2023-04-17 23:39:33.861345 kgx-2.0.5/kgx/config.py
+-rw-r--r--   0        0        0      731 2023-04-17 23:39:33.861345 kgx-2.0.5/kgx/config.yml
+-rw-r--r--   0        0        0     1942 2023-04-17 23:39:33.861345 kgx-2.0.5/kgx/curie_lookup_service.py
+-rw-r--r--   0        0        0     5094 2023-04-17 23:39:33.861345 kgx-2.0.5/kgx/error_detection.py
+-rw-r--r--   0        0        0        0 2023-04-17 23:39:33.861345 kgx-2.0.5/kgx/graph/__init__.py
+-rw-r--r--   0        0        0    10649 2023-04-17 23:39:33.861345 kgx-2.0.5/kgx/graph/base_graph.py
+-rw-r--r--   0        0        0    13455 2023-04-17 23:39:33.861345 kgx-2.0.5/kgx/graph/nx_graph.py
+-rw-r--r--   0        0        0     8498 2023-04-17 23:39:33.861345 kgx-2.0.5/kgx/graph_operations/__init__.py
+-rw-r--r--   0        0        0    28863 2023-04-17 23:39:33.861345 kgx-2.0.5/kgx/graph_operations/clique_merge.py
+-rw-r--r--   0        0        0     5776 2023-04-17 23:39:33.861345 kgx-2.0.5/kgx/graph_operations/graph_merge.py
+-rw-r--r--   0        0        0    36314 2023-04-17 23:39:33.861345 kgx-2.0.5/kgx/graph_operations/meta_knowledge_graph.py
+-rw-r--r--   0        0        0    30601 2023-04-17 23:39:33.861345 kgx-2.0.5/kgx/graph_operations/summarize_graph.py
+-rw-r--r--   0        0        0        0 2023-04-17 23:39:33.861345 kgx-2.0.5/kgx/parsers/__init__.py
+-rw-r--r--   0        0        0     2156 2023-04-17 23:39:33.861345 kgx-2.0.5/kgx/parsers/ntriples_parser.py
+-rw-r--r--   0        0        0     6617 2023-04-17 23:39:33.861345 kgx-2.0.5/kgx/prefix_manager.py
+-rw-r--r--   0        0        0      274 2023-04-17 23:39:33.861345 kgx-2.0.5/kgx/sink/__init__.py
+-rw-r--r--   0        0        0     1703 2023-04-17 23:39:33.861345 kgx-2.0.5/kgx/sink/graph_sink.py
+-rw-r--r--   0        0        0     2335 2023-04-17 23:39:33.861345 kgx-2.0.5/kgx/sink/json_sink.py
+-rw-r--r--   0        0        0     2242 2023-04-17 23:39:33.861345 kgx-2.0.5/kgx/sink/jsonl_sink.py
+-rw-r--r--   0        0        0     9073 2023-04-17 23:39:33.861345 kgx-2.0.5/kgx/sink/neo_sink.py
+-rw-r--r--   0        0        0     1356 2023-04-17 23:39:33.861345 kgx-2.0.5/kgx/sink/null_sink.py
+-rw-r--r--   0        0        0    20032 2023-04-17 23:39:33.861345 kgx-2.0.5/kgx/sink/rdf_sink.py
+-rw-r--r--   0        0        0     1436 2023-04-17 23:39:33.861345 kgx-2.0.5/kgx/sink/sink.py
+-rw-r--r--   0        0        0    10327 2023-04-17 23:39:33.861345 kgx-2.0.5/kgx/sink/sql_sink.py
+-rw-r--r--   0        0        0     8070 2023-04-17 23:39:33.861345 kgx-2.0.5/kgx/sink/tsv_sink.py
+-rw-r--r--   0        0        0      395 2023-04-17 23:39:33.861345 kgx-2.0.5/kgx/source/__init__.py
+-rw-r--r--   0        0        0     2526 2023-04-17 23:39:33.861345 kgx-2.0.5/kgx/source/graph_source.py
+-rw-r--r--   0        0        0     2399 2023-04-17 23:39:33.861345 kgx-2.0.5/kgx/source/json_source.py
+-rw-r--r--   0        0        0     1821 2023-04-17 23:39:33.861345 kgx-2.0.5/kgx/source/jsonl_source.py
+-rw-r--r--   0        0        0    18963 2023-04-17 23:39:33.861345 kgx-2.0.5/kgx/source/neo_source.py
+-rw-r--r--   0        0        0    11785 2023-04-17 23:39:33.861345 kgx-2.0.5/kgx/source/obograph_source.py
+-rw-r--r--   0        0        0     7503 2023-04-17 23:39:33.861345 kgx-2.0.5/kgx/source/owl_source.py
+-rw-r--r--   0        0        0    30464 2023-04-17 23:39:33.861345 kgx-2.0.5/kgx/source/rdf_source.py
+-rw-r--r--   0        0        0    12162 2023-04-17 23:39:33.861345 kgx-2.0.5/kgx/source/source.py
+-rw-r--r--   0        0        0     8221 2023-04-17 23:39:33.861345 kgx-2.0.5/kgx/source/sssom_source.py
+-rw-r--r--   0        0        0     3665 2023-04-17 23:39:33.861345 kgx-2.0.5/kgx/source/trapi_source.py
+-rw-r--r--   0        0        0     9150 2023-04-17 23:39:33.861345 kgx-2.0.5/kgx/source/tsv_source.py
+-rw-r--r--   0        0        0    16660 2023-04-17 23:39:33.861345 kgx-2.0.5/kgx/transformer.py
+-rw-r--r--   0        0        0        0 2023-04-17 23:39:33.861345 kgx-2.0.5/kgx/utils/__init__.py
+-rw-r--r--   0        0        0     4575 2023-04-17 23:39:33.861345 kgx-2.0.5/kgx/utils/graph_utils.py
+-rw-r--r--   0        0        0    18032 2023-04-17 23:39:33.861345 kgx-2.0.5/kgx/utils/infores.py
+-rw-r--r--   0        0        0    31762 2023-04-17 23:39:33.861345 kgx-2.0.5/kgx/utils/kgx_utils.py
+-rw-r--r--   0        0        0     8159 2023-04-17 23:39:33.861345 kgx-2.0.5/kgx/utils/rdf_utils.py
+-rw-r--r--   0        0        0    28313 2023-04-17 23:39:33.861345 kgx-2.0.5/kgx/validator.py
+-rw-r--r--   0        0        0     1591 2023-04-17 23:39:49.165428 kgx-2.0.5/pyproject.toml
+-rw-r--r--   0        0        0     8532 1970-01-01 00:00:00.000000 kgx-2.0.5/PKG-INFO
```

### Comparing `kgx-2.0.4/LICENSE` & `kgx-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `kgx-2.0.4/README.md` & `kgx-2.0.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # Knowledge Graph Exchange
 
+
 [![Python](https://img.shields.io/badge/python-3.9+-blue.svg)]()
 ![Run tests](https://github.com/biolink/kgx/workflows/Run%20tests/badge.svg)[![Documentation Status](https://readthedocs.org/projects/kgx/badge/?version=latest)](https://kgx.readthedocs.io/en/latest/?badge=latest)
 [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=biolink_kgx&metric=alert_status)](https://sonarcloud.io/dashboard?id=biolink_kgx)
 [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=biolink_kgx&metric=sqale_rating)](https://sonarcloud.io/dashboard?id=biolink_kgx)
 [![Coverage](https://sonarcloud.io/api/project_badges/measure?project=biolink_kgx&metric=coverage)](https://sonarcloud.io/dashboard?id=biolink_kgx)
 [![PyPI](https://img.shields.io/pypi/v/kgx)](https://img.shields.io/pypi/v/kgx)
 [![Docker](https://img.shields.io/static/v1?label=Docker&message=biolink/kgx:latest&color=orange&logo=docker)](https://hub.docker.com/r/biolink/kgx)
```

### Comparing `kgx-2.0.4/kgx/cli/__init__.py` & `kgx-2.0.5/kgx/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.4/kgx/cli/cli_utils.py` & `kgx-2.0.5/kgx/cli/cli_utils.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.4/kgx/config.py` & `kgx-2.0.5/kgx/config.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.4/kgx/config.yml` & `kgx-2.0.5/kgx/config.yml`

 * *Files identical despite different names*

### Comparing `kgx-2.0.4/kgx/curie_lookup_service.py` & `kgx-2.0.5/kgx/curie_lookup_service.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.4/kgx/error_detection.py` & `kgx-2.0.5/kgx/error_detection.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.4/kgx/graph/base_graph.py` & `kgx-2.0.5/kgx/graph/base_graph.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.4/kgx/graph/nx_graph.py` & `kgx-2.0.5/kgx/graph/nx_graph.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.4/kgx/graph_operations/__init__.py` & `kgx-2.0.5/kgx/graph_operations/__init__.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.4/kgx/graph_operations/clique_merge.py` & `kgx-2.0.5/kgx/graph_operations/clique_merge.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.4/kgx/graph_operations/graph_merge.py` & `kgx-2.0.5/kgx/graph_operations/graph_merge.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.4/kgx/graph_operations/meta_knowledge_graph.py` & `kgx-2.0.5/kgx/graph_operations/meta_knowledge_graph.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.4/kgx/graph_operations/summarize_graph.py` & `kgx-2.0.5/kgx/graph_operations/summarize_graph.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.4/kgx/parsers/ntriples_parser.py` & `kgx-2.0.5/kgx/parsers/ntriples_parser.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.4/kgx/prefix_manager.py` & `kgx-2.0.5/kgx/prefix_manager.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.4/kgx/sink/graph_sink.py` & `kgx-2.0.5/kgx/sink/graph_sink.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.4/kgx/sink/json_sink.py` & `kgx-2.0.5/kgx/sink/json_sink.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.4/kgx/sink/jsonl_sink.py` & `kgx-2.0.5/kgx/sink/jsonl_sink.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.4/kgx/sink/neo_sink.py` & `kgx-2.0.5/kgx/sink/neo_sink.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.4/kgx/sink/null_sink.py` & `kgx-2.0.5/kgx/sink/null_sink.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.4/kgx/sink/rdf_sink.py` & `kgx-2.0.5/kgx/sink/rdf_sink.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import gzip
 from collections import OrderedDict
 from typing import Optional, Union, Tuple, Any, Dict
-
 import rdflib
 from linkml_runtime.linkml_model.meta import Element, ClassDefinition, SlotDefinition
 from rdflib import URIRef, Literal, Namespace, RDF
 from rdflib.plugins.serializers.nt import _nt_row
 from rdflib.term import _is_valid_uri
 
 from kgx.error_detection import ErrorType
@@ -389,14 +388,15 @@
             "biolink:object",
             "biolink:relation",
             "biolink:predicate",
             "rdf:type",
             "rdf:subject",
             "rdf:predicate",
             "rdf:object",
+            "type"
         }
         if p in default_uri_types:
             t = "uriorcurie"
         else:
             if p in self.property_types:
                 t = self.property_types[p]
             elif f":{p}" in self.property_types:
```

### Comparing `kgx-2.0.4/kgx/sink/sink.py` & `kgx-2.0.5/kgx/sink/sink.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.4/kgx/sink/sql_sink.py` & `kgx-2.0.5/kgx/sink/sql_sink.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.4/kgx/sink/tsv_sink.py` & `kgx-2.0.5/kgx/sink/tsv_sink.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.4/kgx/source/graph_source.py` & `kgx-2.0.5/kgx/source/graph_source.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.4/kgx/source/json_source.py` & `kgx-2.0.5/kgx/source/json_source.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.4/kgx/source/jsonl_source.py` & `kgx-2.0.5/kgx/source/jsonl_source.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.4/kgx/source/neo_source.py` & `kgx-2.0.5/kgx/source/neo_source.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.4/kgx/source/obograph_source.py` & `kgx-2.0.5/kgx/source/obograph_source.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.4/kgx/source/owl_source.py` & `kgx-2.0.5/kgx/source/owl_source.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.4/kgx/source/rdf_source.py` & `kgx-2.0.5/kgx/source/rdf_source.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.4/kgx/source/source.py` & `kgx-2.0.5/kgx/source/source.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.4/kgx/source/sssom_source.py` & `kgx-2.0.5/kgx/source/sssom_source.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.4/kgx/source/trapi_source.py` & `kgx-2.0.5/kgx/source/trapi_source.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.4/kgx/source/tsv_source.py` & `kgx-2.0.5/kgx/source/tsv_source.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.4/kgx/transformer.py` & `kgx-2.0.5/kgx/transformer.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     GraphSink,
     TsvSink,
     JsonSink,
     JsonlSink,
     NeoSink,
     RdfSink,
     NullSink,
+    SqlSink,
 )
 from kgx.utils.kgx_utils import (
     apply_graph_operations,
     GraphEntityType,
     knowledge_provenance_properties,
 )
 
@@ -55,14 +56,15 @@
     "csv": TsvSink,
     "graph": GraphSink,
     "json": JsonSink,
     "jsonl": JsonlSink,
     "neo4j": NeoSink,
     "nt": RdfSink,
     "null": NullSink,
+    "sql": SqlSink
 }
 
 
 log = get_logger()
 
 
 class Transformer(ErrorDetecting):
```

### Comparing `kgx-2.0.4/kgx/utils/graph_utils.py` & `kgx-2.0.5/kgx/utils/graph_utils.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.4/kgx/utils/infores.py` & `kgx-2.0.5/kgx/utils/infores.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.4/kgx/utils/kgx_utils.py` & `kgx-2.0.5/kgx/utils/kgx_utils.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.4/kgx/utils/rdf_utils.py` & `kgx-2.0.5/kgx/utils/rdf_utils.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.4/kgx/validator.py` & `kgx-2.0.5/kgx/validator.py`

 * *Files identical despite different names*

### Comparing `kgx-2.0.4/pyproject.toml` & `kgx-2.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kgx"
-version = "2.0.4"
+version = "2.0.5"
 description = "A Python library and set of command line utilities for exchanging Knowledge Graphs (KGs) that conform to or are aligned to the Biolink Model."
 authors = ["Deepak Unni <deepak.unni3@gmail.com>", "Richard Bruskiewich <richard.bruskiewich@delphinai.com>", "Sierra Moxon <smoxon@lbl.gov>"]
 
 license = "BSD"
 readme = "README.md"
 classifiers = [
     "Intended Audience :: Science/Research",
```

### Comparing `kgx-2.0.4/PKG-INFO` & `kgx-2.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kgx
-Version: 2.0.4
+Version: 2.0.5
 Summary: A Python library and set of command line utilities for exchanging Knowledge Graphs (KGs) that conform to or are aligned to the Biolink Model.
 License: BSD
 Author: Deepak Unni
 Author-email: deepak.unni3@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
@@ -49,14 +49,15 @@
 Requires-Dist: terminaltables (>=3.1.0,<4.0.0)
 Requires-Dist: tox (>=3.0,<4.0)
 Requires-Dist: validators (>=0.20.0,<0.21.0)
 Description-Content-Type: text/markdown
 
 # Knowledge Graph Exchange
 
+
 [![Python](https://img.shields.io/badge/python-3.9+-blue.svg)]()
 ![Run tests](https://github.com/biolink/kgx/workflows/Run%20tests/badge.svg)[![Documentation Status](https://readthedocs.org/projects/kgx/badge/?version=latest)](https://kgx.readthedocs.io/en/latest/?badge=latest)
 [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=biolink_kgx&metric=alert_status)](https://sonarcloud.io/dashboard?id=biolink_kgx)
 [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=biolink_kgx&metric=sqale_rating)](https://sonarcloud.io/dashboard?id=biolink_kgx)
 [![Coverage](https://sonarcloud.io/api/project_badges/measure?project=biolink_kgx&metric=coverage)](https://sonarcloud.io/dashboard?id=biolink_kgx)
 [![PyPI](https://img.shields.io/pypi/v/kgx)](https://img.shields.io/pypi/v/kgx)
 [![Docker](https://img.shields.io/static/v1?label=Docker&message=biolink/kgx:latest&color=orange&logo=docker)](https://hub.docker.com/r/biolink/kgx)
```

