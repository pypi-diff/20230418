# Comparing `tmp/koza-0.3.0.tar.gz` & `tmp/koza-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "koza-0.3.0.tar", max compression
+gzip compressed data, was "koza-0.3.1.tar", max compression
```

## Comparing `koza-0.3.0.tar` & `koza-0.3.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1526 2023-04-03 20:39:48.141150 koza-0.3.0/LICENSE
--rw-r--r--   0        0        0     2569 2023-04-03 20:39:48.145150 koza-0.3.0/README.md
--rw-r--r--   0        0        0     1193 2023-04-03 20:39:48.145150 koza-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       69 2023-04-03 20:39:48.145150 koza-0.3.0/src/koza/__init__.py
--rw-r--r--   0        0        0     8827 2023-04-03 20:39:48.145150 koza-0.3.0/src/koza/app.py
--rw-r--r--   0        0        0     5169 2023-04-03 20:39:48.145150 koza-0.3.0/src/koza/cli_runner.py
--rw-r--r--   0        0        0        0 2023-04-03 20:39:48.145150 koza-0.3.0/src/koza/converter/__init__.py
--rw-r--r--   0        0        0      880 2023-04-03 20:39:48.145150 koza-0.3.0/src/koza/converter/biolink_converter.py
--rw-r--r--   0        0        0     1719 2023-04-03 20:39:48.145150 koza-0.3.0/src/koza/converter/kgx_converter.py
--rw-r--r--   0        0        0      250 2023-04-03 20:39:48.145150 koza-0.3.0/src/koza/io/__init__.py
--rw-r--r--   0        0        0       62 2023-04-03 20:39:48.145150 koza-0.3.0/src/koza/io/reader/__init__.py
--rw-r--r--   0        0        0    10020 2023-04-03 20:39:48.145150 koza-0.3.0/src/koza/io/reader/csv_reader.py
--rw-r--r--   0        0        0     2963 2023-04-03 20:39:48.145150 koza-0.3.0/src/koza/io/reader/json_reader.py
--rw-r--r--   0        0        0     2118 2023-04-03 20:39:48.145150 koza-0.3.0/src/koza/io/reader/jsonl_reader.py
--rw-r--r--   0        0        0     7540 2023-04-03 20:39:48.149150 koza-0.3.0/src/koza/io/utils.py
--rw-r--r--   0        0        0        0 2023-04-03 20:39:48.149150 koza-0.3.0/src/koza/io/writer/__init__.py
--rw-r--r--   0        0        0     1351 2023-04-03 20:39:48.149150 koza-0.3.0/src/koza/io/writer/jsonl_writer.py
--rw-r--r--   0        0        0     5886 2023-04-03 20:39:48.149150 koza-0.3.0/src/koza/io/writer/tsv_writer.py
--rw-r--r--   0        0        0      370 2023-04-03 20:39:48.149150 koza-0.3.0/src/koza/io/writer/writer.py
--rw-r--r--   0        0        0     1592 2023-04-03 20:39:48.149150 koza-0.3.0/src/koza/io/yaml_loader.py
--rwxr-xr-x   0        0        0     2839 2023-04-03 20:39:48.149150 koza-0.3.0/src/koza/main.py
--rw-r--r--   0        0        0       28 2023-04-03 20:39:48.149150 koza-0.3.0/src/koza/model/__init__.py
--rw-r--r--   0        0        0        0 2023-04-03 20:39:48.149150 koza-0.3.0/src/koza/model/config/__init__.py
--rw-r--r--   0        0        0      235 2023-04-03 20:39:48.149150 koza-0.3.0/src/koza/model/config/pydantic_config.py
--rw-r--r--   0        0        0    10538 2023-04-03 20:39:48.149150 koza-0.3.0/src/koza/model/config/source_config.py
--rw-r--r--   0        0        0      396 2023-04-03 20:39:48.149150 koza-0.3.0/src/koza/model/curie_cleaner.py
--rw-r--r--   0        0        0      356 2023-04-03 20:39:48.149150 koza-0.3.0/src/koza/model/map_dict.py
--rw-r--r--   0        0        0     3604 2023-04-03 20:39:48.149150 koza-0.3.0/src/koza/model/source.py
--rw-r--r--   0        0        0     2943 2023-04-03 20:39:48.149150 koza-0.3.0/src/koza/model/translation_table.py
--rw-r--r--   0        0        0        0 2023-04-03 20:39:48.149150 koza-0.3.0/src/koza/utils/__init__
--rw-r--r--   0        0        0      294 2023-04-03 20:39:48.149150 koza-0.3.0/src/koza/utils/exceptions.py
--rw-r--r--   0        0        0      813 2023-04-03 20:39:48.149150 koza-0.3.0/src/koza/utils/log_utils.py
--rw-r--r--   0        0        0     1849 2023-04-03 20:39:48.149150 koza-0.3.0/src/koza/utils/row_filter.py
--rw-r--r--   0        0        0     3446 1970-01-01 00:00:00.000000 koza-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1526 2023-04-18 02:44:51.677717 koza-0.3.1/LICENSE
+-rw-r--r--   0        0        0     2569 2023-04-18 02:44:51.677717 koza-0.3.1/README.md
+-rw-r--r--   0        0        0     1194 2023-04-18 02:44:51.681717 koza-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0       69 2023-04-18 02:44:51.681717 koza-0.3.1/src/koza/__init__.py
+-rw-r--r--   0        0        0     8827 2023-04-18 02:44:51.681717 koza-0.3.1/src/koza/app.py
+-rw-r--r--   0        0        0     5169 2023-04-18 02:44:51.681717 koza-0.3.1/src/koza/cli_runner.py
+-rw-r--r--   0        0        0        0 2023-04-18 02:44:51.681717 koza-0.3.1/src/koza/converter/__init__.py
+-rw-r--r--   0        0        0      880 2023-04-18 02:44:51.681717 koza-0.3.1/src/koza/converter/biolink_converter.py
+-rw-r--r--   0        0        0     1719 2023-04-18 02:44:51.681717 koza-0.3.1/src/koza/converter/kgx_converter.py
+-rw-r--r--   0        0        0      250 2023-04-18 02:44:51.681717 koza-0.3.1/src/koza/io/__init__.py
+-rw-r--r--   0        0        0       62 2023-04-18 02:44:51.681717 koza-0.3.1/src/koza/io/reader/__init__.py
+-rw-r--r--   0        0        0    10020 2023-04-18 02:44:51.681717 koza-0.3.1/src/koza/io/reader/csv_reader.py
+-rw-r--r--   0        0        0     2963 2023-04-18 02:44:51.681717 koza-0.3.1/src/koza/io/reader/json_reader.py
+-rw-r--r--   0        0        0     2118 2023-04-18 02:44:51.681717 koza-0.3.1/src/koza/io/reader/jsonl_reader.py
+-rw-r--r--   0        0        0     7540 2023-04-18 02:44:51.681717 koza-0.3.1/src/koza/io/utils.py
+-rw-r--r--   0        0        0        0 2023-04-18 02:44:51.681717 koza-0.3.1/src/koza/io/writer/__init__.py
+-rw-r--r--   0        0        0     1351 2023-04-18 02:44:51.681717 koza-0.3.1/src/koza/io/writer/jsonl_writer.py
+-rw-r--r--   0        0        0     5886 2023-04-18 02:44:51.681717 koza-0.3.1/src/koza/io/writer/tsv_writer.py
+-rw-r--r--   0        0        0      370 2023-04-18 02:44:51.681717 koza-0.3.1/src/koza/io/writer/writer.py
+-rw-r--r--   0        0        0     1592 2023-04-18 02:44:51.681717 koza-0.3.1/src/koza/io/yaml_loader.py
+-rwxr-xr-x   0        0        0     2839 2023-04-18 02:44:51.681717 koza-0.3.1/src/koza/main.py
+-rw-r--r--   0        0        0       28 2023-04-18 02:44:51.681717 koza-0.3.1/src/koza/model/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-18 02:44:51.681717 koza-0.3.1/src/koza/model/config/__init__.py
+-rw-r--r--   0        0        0      235 2023-04-18 02:44:51.681717 koza-0.3.1/src/koza/model/config/pydantic_config.py
+-rw-r--r--   0        0        0    10538 2023-04-18 02:44:51.681717 koza-0.3.1/src/koza/model/config/source_config.py
+-rw-r--r--   0        0        0      396 2023-04-18 02:44:51.681717 koza-0.3.1/src/koza/model/curie_cleaner.py
+-rw-r--r--   0        0        0      356 2023-04-18 02:44:51.681717 koza-0.3.1/src/koza/model/map_dict.py
+-rw-r--r--   0        0        0     3604 2023-04-18 02:44:51.681717 koza-0.3.1/src/koza/model/source.py
+-rw-r--r--   0        0        0     2943 2023-04-18 02:44:51.681717 koza-0.3.1/src/koza/model/translation_table.py
+-rw-r--r--   0        0        0        0 2023-04-18 02:44:51.681717 koza-0.3.1/src/koza/utils/__init__
+-rw-r--r--   0        0        0      294 2023-04-18 02:44:51.681717 koza-0.3.1/src/koza/utils/exceptions.py
+-rw-r--r--   0        0        0      813 2023-04-18 02:44:51.681717 koza-0.3.1/src/koza/utils/log_utils.py
+-rw-r--r--   0        0        0     1849 2023-04-18 02:44:51.681717 koza-0.3.1/src/koza/utils/row_filter.py
+-rw-r--r--   0        0        0     3439 1970-01-01 00:00:00.000000 koza-0.3.1/PKG-INFO
```

### Comparing `koza-0.3.0/LICENSE` & `koza-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `koza-0.3.0/README.md` & `koza-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `koza-0.3.0/pyproject.toml` & `koza-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "koza"
-version = "0.3.0"
+version = "0.3.1"
 description = "Data transformation framework for LinkML data models"
 authors = [
     "The Monarch Initiative <info@monarchinitiative.org>",
     "Kevin Schaper <kevinschaper@gmail.com>",
     "Glass Elsarboukh <g.elsarboukh@gmail.com>",
     "Kent Shefchek <kent@tislab.org>",
     ]
@@ -14,15 +14,15 @@
     { include = "koza", from = "src"}
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 linkml-validator = ">=0.4.4"
 pydantic = "^1.0.0"
-pyyaml = "^5.3.1"
+pyyaml = ">=5.0.0"
 requests = "^2.24.0"
 ordered-set = ">=4.1.0"
 typer = "^0.7.0"
 typer-cli = "^0.0.13"
 loguru = "*"
 
 [tool.poetry.dev-dependencies]
```

### Comparing `koza-0.3.0/src/koza/app.py` & `koza-0.3.1/src/koza/app.py`

 * *Files identical despite different names*

### Comparing `koza-0.3.0/src/koza/cli_runner.py` & `koza-0.3.1/src/koza/cli_runner.py`

 * *Files identical despite different names*

### Comparing `koza-0.3.0/src/koza/converter/biolink_converter.py` & `koza-0.3.1/src/koza/converter/biolink_converter.py`

 * *Files identical despite different names*

### Comparing `koza-0.3.0/src/koza/converter/kgx_converter.py` & `koza-0.3.1/src/koza/converter/kgx_converter.py`

 * *Files identical despite different names*

### Comparing `koza-0.3.0/src/koza/io/reader/csv_reader.py` & `koza-0.3.1/src/koza/io/reader/csv_reader.py`

 * *Files identical despite different names*

### Comparing `koza-0.3.0/src/koza/io/reader/json_reader.py` & `koza-0.3.1/src/koza/io/reader/json_reader.py`

 * *Files identical despite different names*

### Comparing `koza-0.3.0/src/koza/io/reader/jsonl_reader.py` & `koza-0.3.1/src/koza/io/reader/jsonl_reader.py`

 * *Files identical despite different names*

### Comparing `koza-0.3.0/src/koza/io/utils.py` & `koza-0.3.1/src/koza/io/utils.py`

 * *Files identical despite different names*

### Comparing `koza-0.3.0/src/koza/io/writer/jsonl_writer.py` & `koza-0.3.1/src/koza/io/writer/jsonl_writer.py`

 * *Files identical despite different names*

### Comparing `koza-0.3.0/src/koza/io/writer/tsv_writer.py` & `koza-0.3.1/src/koza/io/writer/tsv_writer.py`

 * *Files identical despite different names*

### Comparing `koza-0.3.0/src/koza/io/yaml_loader.py` & `koza-0.3.1/src/koza/io/yaml_loader.py`

 * *Files identical despite different names*

### Comparing `koza-0.3.0/src/koza/main.py` & `koza-0.3.1/src/koza/main.py`

 * *Files identical despite different names*

### Comparing `koza-0.3.0/src/koza/model/config/source_config.py` & `koza-0.3.1/src/koza/model/config/source_config.py`

 * *Files identical despite different names*

### Comparing `koza-0.3.0/src/koza/model/source.py` & `koza-0.3.1/src/koza/model/source.py`

 * *Files identical despite different names*

### Comparing `koza-0.3.0/src/koza/model/translation_table.py` & `koza-0.3.1/src/koza/model/translation_table.py`

 * *Files identical despite different names*

### Comparing `koza-0.3.0/src/koza/utils/log_utils.py` & `koza-0.3.1/src/koza/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `koza-0.3.0/src/koza/utils/row_filter.py` & `koza-0.3.1/src/koza/utils/row_filter.py`

 * *Files identical despite different names*

### Comparing `koza-0.3.0/PKG-INFO` & `koza-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: koza
-Version: 0.3.0
+Version: 0.3.1
 Summary: Data transformation framework for LinkML data models
 License: BSD License
 Author: The Monarch Initiative
 Author-email: info@monarchinitiative.org
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: linkml-validator (>=0.4.4)
 Requires-Dist: loguru
 Requires-Dist: ordered-set (>=4.1.0)
 Requires-Dist: pydantic (>=1.0.0,<2.0.0)
-Requires-Dist: pyyaml (>=5.3.1,<6.0.0)
+Requires-Dist: pyyaml (>=5.0.0)
 Requires-Dist: requests (>=2.24.0,<3.0.0)
 Requires-Dist: typer (>=0.7.0,<0.8.0)
 Requires-Dist: typer-cli (>=0.0.13,<0.0.14)
 Description-Content-Type: text/markdown
 
 # Koza - a data transformation framework
```

