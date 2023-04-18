# Comparing `tmp/pdtable-0.0.8.tar.gz` & `tmp/pdtable-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pdtable-0.0.8.tar", last modified: Mon Feb 15 13:47:12 2021, max compression
+gzip compressed data, was "dist/pdtable-0.0.9.tar", last modified: Tue Feb 23 11:54:39 2021, max compression
```

## Comparing `pdtable-0.0.8.tar` & `pdtable-0.0.9.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-15 13:47:12.000000 pdtable-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (116)     3238 2021-02-15 13:47:12.000000 pdtable-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2233 2021-02-15 13:47:07.000000 pdtable-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-15 13:47:12.000000 pdtable-0.0.8/examples/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-02-15 13:47:07.000000 pdtable-0.0.8/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    16274 2021-02-15 13:47:07.000000 pdtable-0.0.8/examples/pdtable_demo.py
--rw-r--r--   0 runner    (1001) docker     (116)      183 2021-02-15 13:47:07.000000 pdtable-0.0.8/examples/test_pdtable_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-15 13:47:12.000000 pdtable-0.0.8/pdtable/
--rw-r--r--   0 runner    (1001) docker     (116)      469 2021-02-15 13:47:07.000000 pdtable-0.0.8/pdtable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      545 2021-02-15 13:47:07.000000 pdtable-0.0.8/pdtable/auxiliary.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-15 13:47:12.000000 pdtable-0.0.8/pdtable/demo/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-02-15 13:47:07.000000 pdtable-0.0.8/pdtable/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1929 2021-02-15 13:47:07.000000 pdtable-0.0.8/pdtable/demo/directive_handlers.py
--rw-r--r--   0 runner    (1001) docker     (116)     2435 2021-02-15 13:47:07.000000 pdtable-0.0.8/pdtable/demo/unit_converter.py
--rw-r--r--   0 runner    (1001) docker     (116)    11226 2021-02-15 13:47:07.000000 pdtable-0.0.8/pdtable/frame.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-15 13:47:12.000000 pdtable-0.0.8/pdtable/io/
--rw-r--r--   0 runner    (1001) docker     (116)      286 2021-02-15 13:47:07.000000 pdtable-0.0.8/pdtable/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2478 2021-02-15 13:47:07.000000 pdtable-0.0.8/pdtable/io/_excel_openpyxl.py
--rw-r--r--   0 runner    (1001) docker     (116)     2530 2021-02-15 13:47:07.000000 pdtable-0.0.8/pdtable/io/_json.py
--rw-r--r--   0 runner    (1001) docker     (116)     2041 2021-02-15 13:47:07.000000 pdtable-0.0.8/pdtable/io/_represent.py
--rw-r--r--   0 runner    (1001) docker     (116)     7684 2021-02-15 13:47:07.000000 pdtable-0.0.8/pdtable/io/csv.py
--rw-r--r--   0 runner    (1001) docker     (116)     3496 2021-02-15 13:47:07.000000 pdtable-0.0.8/pdtable/io/excel.py
--rw-r--r--   0 runner    (1001) docker     (116)     1353 2021-02-15 13:47:07.000000 pdtable-0.0.8/pdtable/io/json.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-15 13:47:12.000000 pdtable-0.0.8/pdtable/io/parsers/
--rw-r--r--   0 runner    (1001) docker     (116)       91 2021-02-15 13:47:07.000000 pdtable-0.0.8/pdtable/io/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    14144 2021-02-15 13:47:07.000000 pdtable-0.0.8/pdtable/io/parsers/blocks.py
--rw-r--r--   0 runner    (1001) docker     (116)     6939 2021-02-15 13:47:07.000000 pdtable-0.0.8/pdtable/io/parsers/columns.py
--rw-r--r--   0 runner    (1001) docker     (116)     4756 2021-02-15 13:47:07.000000 pdtable-0.0.8/pdtable/io/parsers/fixer.py
--rw-r--r--   0 runner    (1001) docker     (116)    16736 2021-02-15 13:47:07.000000 pdtable-0.0.8/pdtable/proxy.py
--rw-r--r--   0 runner    (1001) docker     (116)     5292 2021-02-15 13:47:07.000000 pdtable-0.0.8/pdtable/store.py
--rw-r--r--   0 runner    (1001) docker     (116)     6640 2021-02-15 13:47:07.000000 pdtable-0.0.8/pdtable/table_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-15 13:47:12.000000 pdtable-0.0.8/pdtable/test/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-02-15 13:47:07.000000 pdtable-0.0.8/pdtable/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-15 13:47:12.000000 pdtable-0.0.8/pdtable/test/input/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-02-15 13:47:07.000000 pdtable-0.0.8/pdtable/test/input/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-15 13:47:12.000000 pdtable-0.0.8/pdtable/test/io/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-02-15 13:47:07.000000 pdtable-0.0.8/pdtable/test/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-15 13:47:12.000000 pdtable-0.0.8/pdtable/test/io/input/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-02-15 13:47:07.000000 pdtable-0.0.8/pdtable/test/io/input/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-15 13:47:12.000000 pdtable-0.0.8/pdtable/test/io/input/with_errors/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-02-15 13:47:07.000000 pdtable-0.0.8/pdtable/test/io/input/with_errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4355 2021-02-15 13:47:07.000000 pdtable-0.0.8/pdtable/test/io/input/with_errors/auto_fixed.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-15 13:47:12.000000 pdtable-0.0.8/pdtable/test/io/parsers/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-02-15 13:47:07.000000 pdtable-0.0.8/pdtable/test/io/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    16073 2021-02-15 13:47:07.000000 pdtable-0.0.8/pdtable/test/io/parsers/test_block_parsers.py
--rw-r--r--   0 runner    (1001) docker     (116)     3204 2021-02-15 13:47:07.000000 pdtable-0.0.8/pdtable/test/io/parsers/test_column_parsers.py
--rw-r--r--   0 runner    (1001) docker     (116)     5400 2021-02-15 13:47:07.000000 pdtable-0.0.8/pdtable/test/io/test__excel.py
--rw-r--r--   0 runner    (1001) docker     (116)     6761 2021-02-15 13:47:07.000000 pdtable-0.0.8/pdtable/test/io/test_csv_writer.py
--rw-r--r--   0 runner    (1001) docker     (116)      944 2021-02-15 13:47:07.000000 pdtable-0.0.8/pdtable/test/io/test_formatting.py
--rw-r--r--   0 runner    (1001) docker     (116)     3439 2021-02-15 13:47:07.000000 pdtable-0.0.8/pdtable/test/io/test_read_bundle_from_csv.py
--rw-r--r--   0 runner    (1001) docker     (116)     4293 2021-02-15 13:47:07.000000 pdtable-0.0.8/pdtable/test/io/test_read_csv.py
--rw-r--r--   0 runner    (1001) docker     (116)     8609 2021-02-15 13:47:07.000000 pdtable-0.0.8/pdtable/test/io/test_read_csv_fixer.py
--rw-r--r--   0 runner    (1001) docker     (116)     8451 2021-02-15 13:47:07.000000 pdtable-0.0.8/pdtable/test/io/test_read_csv_json.py
--rw-r--r--   0 runner    (1001) docker     (116)     2490 2021-02-15 13:47:07.000000 pdtable-0.0.8/pdtable/test/io/test_read_excel.py
--rw-r--r--   0 runner    (1001) docker     (116)     1273 2021-02-15 13:47:07.000000 pdtable-0.0.8/pdtable/test/test_ancillary_blocks.py
--rw-r--r--   0 runner    (1001) docker     (116)     7045 2021-02-15 13:47:07.000000 pdtable-0.0.8/pdtable/test/test_pdtable.py
--rw-r--r--   0 runner    (1001) docker     (116)     6251 2021-02-15 13:47:07.000000 pdtable-0.0.8/pdtable/test/test_store.py
--rw-r--r--   0 runner    (1001) docker     (116)     7997 2021-02-15 13:47:07.000000 pdtable-0.0.8/pdtable/test/test_units.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-15 13:47:12.000000 pdtable-0.0.8/pdtable/units/
--rw-r--r--   0 runner    (1001) docker     (116)       62 2021-02-15 13:47:07.000000 pdtable-0.0.8/pdtable/units/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2521 2021-02-15 13:47:07.000000 pdtable-0.0.8/pdtable/units/pint.py
--rw-r--r--   0 runner    (1001) docker     (116)     2312 2021-02-15 13:47:07.000000 pdtable-0.0.8/pdtable/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-15 13:47:12.000000 pdtable-0.0.8/pdtable.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     3238 2021-02-15 13:47:12.000000 pdtable-0.0.8/pdtable.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1608 2021-02-15 13:47:12.000000 pdtable-0.0.8/pdtable.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-02-15 13:47:12.000000 pdtable-0.0.8/pdtable.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       13 2021-02-15 13:47:12.000000 pdtable-0.0.8/pdtable.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       17 2021-02-15 13:47:12.000000 pdtable-0.0.8/pdtable.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       42 2021-02-15 13:47:07.000000 pdtable-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)      417 2021-02-15 13:47:12.000000 pdtable-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     2224 2021-02-15 13:47:07.000000 pdtable-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-15 13:47:12.000000 pdtable-0.0.8/test/
--rw-r--r--   0 runner    (1001) docker     (116)     1424 2021-02-15 13:47:07.000000 pdtable-0.0.8/test/test_optional_dependencies.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-23 11:54:39.000000 pdtable-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (116)     3238 2021-02-23 11:54:39.000000 pdtable-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     2233 2021-02-23 11:54:34.000000 pdtable-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-23 11:54:39.000000 pdtable-0.0.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-02-23 11:54:34.000000 pdtable-0.0.9/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    16274 2021-02-23 11:54:34.000000 pdtable-0.0.9/examples/pdtable_demo.py
+-rw-r--r--   0 runner    (1001) docker     (116)      183 2021-02-23 11:54:34.000000 pdtable-0.0.9/examples/test_pdtable_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-23 11:54:39.000000 pdtable-0.0.9/pdtable/
+-rw-r--r--   0 runner    (1001) docker     (116)      469 2021-02-23 11:54:34.000000 pdtable-0.0.9/pdtable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      545 2021-02-23 11:54:34.000000 pdtable-0.0.9/pdtable/auxiliary.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-23 11:54:39.000000 pdtable-0.0.9/pdtable/demo/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-02-23 11:54:34.000000 pdtable-0.0.9/pdtable/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1929 2021-02-23 11:54:34.000000 pdtable-0.0.9/pdtable/demo/directive_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2435 2021-02-23 11:54:34.000000 pdtable-0.0.9/pdtable/demo/unit_converter.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11226 2021-02-23 11:54:34.000000 pdtable-0.0.9/pdtable/frame.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-23 11:54:39.000000 pdtable-0.0.9/pdtable/io/
+-rw-r--r--   0 runner    (1001) docker     (116)      286 2021-02-23 11:54:34.000000 pdtable-0.0.9/pdtable/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5393 2021-02-23 11:54:34.000000 pdtable-0.0.9/pdtable/io/_excel_openpyxl.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2530 2021-02-23 11:54:34.000000 pdtable-0.0.9/pdtable/io/_json.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2041 2021-02-23 11:54:34.000000 pdtable-0.0.9/pdtable/io/_represent.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7684 2021-02-23 11:54:34.000000 pdtable-0.0.9/pdtable/io/csv.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3866 2021-02-23 11:54:34.000000 pdtable-0.0.9/pdtable/io/excel.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1353 2021-02-23 11:54:34.000000 pdtable-0.0.9/pdtable/io/json.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-23 11:54:39.000000 pdtable-0.0.9/pdtable/io/parsers/
+-rw-r--r--   0 runner    (1001) docker     (116)       91 2021-02-23 11:54:34.000000 pdtable-0.0.9/pdtable/io/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    14144 2021-02-23 11:54:34.000000 pdtable-0.0.9/pdtable/io/parsers/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6939 2021-02-23 11:54:34.000000 pdtable-0.0.9/pdtable/io/parsers/columns.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4756 2021-02-23 11:54:34.000000 pdtable-0.0.9/pdtable/io/parsers/fixer.py
+-rw-r--r--   0 runner    (1001) docker     (116)    16736 2021-02-23 11:54:34.000000 pdtable-0.0.9/pdtable/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5292 2021-02-23 11:54:34.000000 pdtable-0.0.9/pdtable/store.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6640 2021-02-23 11:54:34.000000 pdtable-0.0.9/pdtable/table_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-23 11:54:39.000000 pdtable-0.0.9/pdtable/test/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-02-23 11:54:34.000000 pdtable-0.0.9/pdtable/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-23 11:54:39.000000 pdtable-0.0.9/pdtable/test/input/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-02-23 11:54:34.000000 pdtable-0.0.9/pdtable/test/input/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-23 11:54:39.000000 pdtable-0.0.9/pdtable/test/io/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-02-23 11:54:34.000000 pdtable-0.0.9/pdtable/test/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-23 11:54:39.000000 pdtable-0.0.9/pdtable/test/io/input/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-02-23 11:54:34.000000 pdtable-0.0.9/pdtable/test/io/input/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-23 11:54:39.000000 pdtable-0.0.9/pdtable/test/io/input/with_errors/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-02-23 11:54:34.000000 pdtable-0.0.9/pdtable/test/io/input/with_errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4355 2021-02-23 11:54:34.000000 pdtable-0.0.9/pdtable/test/io/input/with_errors/auto_fixed.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-23 11:54:39.000000 pdtable-0.0.9/pdtable/test/io/parsers/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-02-23 11:54:34.000000 pdtable-0.0.9/pdtable/test/io/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    16073 2021-02-23 11:54:34.000000 pdtable-0.0.9/pdtable/test/io/parsers/test_block_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3204 2021-02-23 11:54:34.000000 pdtable-0.0.9/pdtable/test/io/parsers/test_column_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12986 2021-02-23 11:54:34.000000 pdtable-0.0.9/pdtable/test/io/test__excel.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6761 2021-02-23 11:54:34.000000 pdtable-0.0.9/pdtable/test/io/test_csv_writer.py
+-rw-r--r--   0 runner    (1001) docker     (116)      944 2021-02-23 11:54:34.000000 pdtable-0.0.9/pdtable/test/io/test_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3439 2021-02-23 11:54:34.000000 pdtable-0.0.9/pdtable/test/io/test_read_bundle_from_csv.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4293 2021-02-23 11:54:34.000000 pdtable-0.0.9/pdtable/test/io/test_read_csv.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8609 2021-02-23 11:54:34.000000 pdtable-0.0.9/pdtable/test/io/test_read_csv_fixer.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8451 2021-02-23 11:54:34.000000 pdtable-0.0.9/pdtable/test/io/test_read_csv_json.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2490 2021-02-23 11:54:34.000000 pdtable-0.0.9/pdtable/test/io/test_read_excel.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1273 2021-02-23 11:54:34.000000 pdtable-0.0.9/pdtable/test/test_ancillary_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7045 2021-02-23 11:54:34.000000 pdtable-0.0.9/pdtable/test/test_pdtable.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6251 2021-02-23 11:54:34.000000 pdtable-0.0.9/pdtable/test/test_store.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7997 2021-02-23 11:54:34.000000 pdtable-0.0.9/pdtable/test/test_units.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-23 11:54:39.000000 pdtable-0.0.9/pdtable/units/
+-rw-r--r--   0 runner    (1001) docker     (116)       62 2021-02-23 11:54:34.000000 pdtable-0.0.9/pdtable/units/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2521 2021-02-23 11:54:34.000000 pdtable-0.0.9/pdtable/units/pint.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2312 2021-02-23 11:54:34.000000 pdtable-0.0.9/pdtable/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-23 11:54:39.000000 pdtable-0.0.9/pdtable.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     3238 2021-02-23 11:54:39.000000 pdtable-0.0.9/pdtable.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     1608 2021-02-23 11:54:39.000000 pdtable-0.0.9/pdtable.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-02-23 11:54:39.000000 pdtable-0.0.9/pdtable.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       13 2021-02-23 11:54:39.000000 pdtable-0.0.9/pdtable.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       17 2021-02-23 11:54:39.000000 pdtable-0.0.9/pdtable.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       42 2021-02-23 11:54:34.000000 pdtable-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (116)      417 2021-02-23 11:54:39.000000 pdtable-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     2224 2021-02-23 11:54:34.000000 pdtable-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-23 11:54:39.000000 pdtable-0.0.9/test/
+-rw-r--r--   0 runner    (1001) docker     (116)     1424 2021-02-23 11:54:34.000000 pdtable-0.0.9/test/test_optional_dependencies.py
```

### Comparing `pdtable-0.0.8/PKG-INFO` & `pdtable-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdtable
-Version: 0.0.8
+Version: 0.0.9
 Summary: Reads and writes data stored in StarTable format; and stores table data inmemory as a Pandas data frame for easy manipulation.
 Home-page: https://github.com/startable/pdtable/
 Author: Jean-François Corbett
 Author-email: jeaco@orsted.dk
 License: BSD-3-Clause
 Description: # pdtable
```

### Comparing `pdtable-0.0.8/README.md` & `pdtable-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pdtable-0.0.8/examples/pdtable_demo.py` & `pdtable-0.0.9/examples/pdtable_demo.py`

 * *Files identical despite different names*

### Comparing `pdtable-0.0.8/pdtable/auxiliary.py` & `pdtable-0.0.9/pdtable/auxiliary.py`

 * *Files identical despite different names*

### Comparing `pdtable-0.0.8/pdtable/demo/directive_handlers.py` & `pdtable-0.0.9/pdtable/demo/directive_handlers.py`

 * *Files identical despite different names*

### Comparing `pdtable-0.0.8/pdtable/demo/unit_converter.py` & `pdtable-0.0.9/pdtable/demo/unit_converter.py`

 * *Files identical despite different names*

### Comparing `pdtable-0.0.8/pdtable/frame.py` & `pdtable-0.0.9/pdtable/frame.py`

 * *Files identical despite different names*

### Comparing `pdtable-0.0.8/pdtable/io/_json.py` & `pdtable-0.0.9/pdtable/io/_json.py`

 * *Files identical despite different names*

### Comparing `pdtable-0.0.8/pdtable/io/_represent.py` & `pdtable-0.0.9/pdtable/io/_represent.py`

 * *Files identical despite different names*

### Comparing `pdtable-0.0.8/pdtable/io/csv.py` & `pdtable-0.0.9/pdtable/io/csv.py`

 * *Files identical despite different names*

### Comparing `pdtable-0.0.8/pdtable/io/excel.py` & `pdtable-0.0.9/pdtable/io/excel.py`

 * *Files 14% similar despite different names*

```diff
@@ -55,14 +55,16 @@
     yield from parse_blocks(read_cell_rows(source), **kwargs)
 
 
 def write_excel(
     tables: Union[Table, Iterable[Table], Dict[str, Table], Dict[str, Iterable[Table]]],
     to: Union[str, os.PathLike, BinaryIO],
     na_rep: str = "-",
+    num_blank_rows_between_tables: int = 1,
+    style: bool = False
 ):
     """Writes one or more tables to an Excel workbook.
 
     Writes table blocks to an Excel workbook file.
     Values are formatted to comply with the StarTable standard where necessary and possible.
 
     This is a thin wrapper around parse_blocks(). The only thing it does is to present the contents
@@ -79,19 +81,25 @@
             If a file path, then this file gets created/overwritten and then closed after writing.
             If a stream, then it is left open after writing; the caller is responsible for managing
             the stream.
         na_rep:
             Optional; String representation of missing values (NaN, None, NaT).
             If overriding the default '-', it is recommended to use another value compliant with
             the StarTable standard.
+        num_blank_rows_between_tables:
+            Optional; Number of blank rows between tables.
+            Default is 1.
+        style:
+            Optional; Whether or not to apply standard StarTable style to Excel workbook file.
+            Default is False.
     """
     try:
         from ._excel_openpyxl import write_excel_openpyxl as write_excel_func
 
     except ImportError as err:
         raise ImportError(
             "Unable to find a usable spreadsheet engine. "
             "Tried using: 'openpyxl'.\n"
             "Please install openpyxl for Excel I/O support."
         ) from err
 
-    write_excel_func(tables, to, na_rep)
+    write_excel_func(tables, to, na_rep, style, num_blank_rows_between_tables)
```

### Comparing `pdtable-0.0.8/pdtable/io/json.py` & `pdtable-0.0.9/pdtable/io/json.py`

 * *Files identical despite different names*

### Comparing `pdtable-0.0.8/pdtable/io/parsers/blocks.py` & `pdtable-0.0.9/pdtable/io/parsers/blocks.py`

 * *Files identical despite different names*

### Comparing `pdtable-0.0.8/pdtable/io/parsers/columns.py` & `pdtable-0.0.9/pdtable/io/parsers/columns.py`

 * *Files identical despite different names*

### Comparing `pdtable-0.0.8/pdtable/io/parsers/fixer.py` & `pdtable-0.0.9/pdtable/io/parsers/fixer.py`

 * *Files identical despite different names*

### Comparing `pdtable-0.0.8/pdtable/proxy.py` & `pdtable-0.0.9/pdtable/proxy.py`

 * *Files identical despite different names*

### Comparing `pdtable-0.0.8/pdtable/store.py` & `pdtable-0.0.9/pdtable/store.py`

 * *Files identical despite different names*

### Comparing `pdtable-0.0.8/pdtable/table_metadata.py` & `pdtable-0.0.9/pdtable/table_metadata.py`

 * *Files identical despite different names*

### Comparing `pdtable-0.0.8/pdtable/test/io/input/with_errors/auto_fixed.py` & `pdtable-0.0.9/pdtable/test/io/input/with_errors/auto_fixed.py`

 * *Files identical despite different names*

### Comparing `pdtable-0.0.8/pdtable/test/io/parsers/test_block_parsers.py` & `pdtable-0.0.9/pdtable/test/io/parsers/test_block_parsers.py`

 * *Files identical despite different names*

### Comparing `pdtable-0.0.8/pdtable/test/io/parsers/test_column_parsers.py` & `pdtable-0.0.9/pdtable/test/io/parsers/test_column_parsers.py`

 * *Files identical despite different names*

### Comparing `pdtable-0.0.8/pdtable/test/io/test_csv_writer.py` & `pdtable-0.0.9/pdtable/test/io/test_csv_writer.py`

 * *Files identical despite different names*

### Comparing `pdtable-0.0.8/pdtable/test/io/test_formatting.py` & `pdtable-0.0.9/pdtable/test/io/test_formatting.py`

 * *Files identical despite different names*

### Comparing `pdtable-0.0.8/pdtable/test/io/test_read_bundle_from_csv.py` & `pdtable-0.0.9/pdtable/test/io/test_read_bundle_from_csv.py`

 * *Files identical despite different names*

### Comparing `pdtable-0.0.8/pdtable/test/io/test_read_csv.py` & `pdtable-0.0.9/pdtable/test/io/test_read_csv.py`

 * *Files identical despite different names*

### Comparing `pdtable-0.0.8/pdtable/test/io/test_read_csv_fixer.py` & `pdtable-0.0.9/pdtable/test/io/test_read_csv_fixer.py`

 * *Files identical despite different names*

### Comparing `pdtable-0.0.8/pdtable/test/io/test_read_csv_json.py` & `pdtable-0.0.9/pdtable/test/io/test_read_csv_json.py`

 * *Files identical despite different names*

### Comparing `pdtable-0.0.8/pdtable/test/io/test_read_excel.py` & `pdtable-0.0.9/pdtable/test/io/test_read_excel.py`

 * *Files identical despite different names*

### Comparing `pdtable-0.0.8/pdtable/test/test_ancillary_blocks.py` & `pdtable-0.0.9/pdtable/test/test_ancillary_blocks.py`

 * *Files identical despite different names*

### Comparing `pdtable-0.0.8/pdtable/test/test_pdtable.py` & `pdtable-0.0.9/pdtable/test/test_pdtable.py`

 * *Files identical despite different names*

### Comparing `pdtable-0.0.8/pdtable/test/test_store.py` & `pdtable-0.0.9/pdtable/test/test_store.py`

 * *Files identical despite different names*

### Comparing `pdtable-0.0.8/pdtable/test/test_units.py` & `pdtable-0.0.9/pdtable/test/test_units.py`

 * *Files identical despite different names*

### Comparing `pdtable-0.0.8/pdtable/units/pint.py` & `pdtable-0.0.9/pdtable/units/pint.py`

 * *Files identical despite different names*

### Comparing `pdtable-0.0.8/pdtable/utils.py` & `pdtable-0.0.9/pdtable/utils.py`

 * *Files identical despite different names*

### Comparing `pdtable-0.0.8/pdtable.egg-info/PKG-INFO` & `pdtable-0.0.9/pdtable.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdtable
-Version: 0.0.8
+Version: 0.0.9
 Summary: Reads and writes data stored in StarTable format; and stores table data inmemory as a Pandas data frame for easy manipulation.
 Home-page: https://github.com/startable/pdtable/
 Author: Jean-François Corbett
 Author-email: jeaco@orsted.dk
 License: BSD-3-Clause
 Description: # pdtable
```

### Comparing `pdtable-0.0.8/pdtable.egg-info/SOURCES.txt` & `pdtable-0.0.9/pdtable.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pdtable-0.0.8/setup.py` & `pdtable-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `pdtable-0.0.8/test/test_optional_dependencies.py` & `pdtable-0.0.9/test/test_optional_dependencies.py`

 * *Files identical despite different names*

