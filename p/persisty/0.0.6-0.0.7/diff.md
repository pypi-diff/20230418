# Comparing `tmp/persisty-0.0.6.tar.gz` & `tmp/persisty-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/persisty-0.0.6.tar", last modified: Tue Apr 18 14:28:13 2023, max compression
+gzip compressed data, was "dist/persisty-0.0.7.tar", last modified: Tue Apr 18 21:40:16 2023, max compression
```

## Comparing `persisty-0.0.6.tar` & `persisty-0.0.7.tar`

### file list

```diff
@@ -1,196 +1,196 @@
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 14:28:13.000000 persisty-0.0.6/
--rw-r--r--   0 tofarr     (501) staff       (20)     4051 2023-04-18 14:28:13.000000 persisty-0.0.6/PKG-INFO
--rw-r--r--   0 tofarr     (501) staff       (20)     3629 2023-04-16 16:31:32.000000 persisty-0.0.6/README.md
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 14:28:13.000000 persisty-0.0.6/marshy_config_persisty/
--rw-r--r--   0 tofarr     (501) staff       (20)     5933 2023-04-18 00:07:16.000000 persisty-0.0.6/marshy_config_persisty/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1670 2023-01-17 18:43:12.000000 persisty-0.0.6/marshy_config_persisty/sqlalchemy_config.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 14:28:13.000000 persisty-0.0.6/persisty/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-10 11:54:34.000000 persisty-0.0.6/persisty/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)       22 2023-04-18 14:27:46.000000 persisty-0.0.6/persisty/__version__.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 14:28:13.000000 persisty-0.0.6/persisty/attr/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-17 18:43:12.000000 persisty-0.0.6/persisty/attr/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2290 2023-04-18 14:22:16.000000 persisty-0.0.6/persisty/attr/attr.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2033 2023-03-19 15:06:43.000000 persisty-0.0.6/persisty/attr/attr_filter.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2499 2023-03-19 15:06:43.000000 persisty-0.0.6/persisty/attr/attr_filter_op.py
--rw-r--r--   0 tofarr     (501) staff       (20)      868 2023-03-19 15:06:43.000000 persisty-0.0.6/persisty/attr/attr_type.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 14:28:13.000000 persisty-0.0.6/persisty/attr/generator/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-17 18:43:12.000000 persisty-0.0.6/persisty/attr/generator/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)      168 2023-01-17 18:43:12.000000 persisty-0.0.6/persisty/attr/generator/attr_value_generator_abc.py
--rw-r--r--   0 tofarr     (501) staff       (20)      375 2023-01-17 18:43:12.000000 persisty-0.0.6/persisty/attr/generator/default_value_generator.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1203 2023-01-17 18:43:12.000000 persisty-0.0.6/persisty/attr/generator/defaults.py
--rw-r--r--   0 tofarr     (501) staff       (20)      749 2023-03-19 15:06:43.000000 persisty-0.0.6/persisty/attr/generator/int_sequence_generator.py
--rw-r--r--   0 tofarr     (501) staff       (20)      798 2023-01-17 18:43:12.000000 persisty-0.0.6/persisty/attr/generator/str_sequence_generator.py
--rw-r--r--   0 tofarr     (501) staff       (20)      382 2023-01-17 18:43:12.000000 persisty-0.0.6/persisty/attr/generator/timestamp_generator.py
--rw-r--r--   0 tofarr     (501) staff       (20)      328 2023-01-17 18:43:12.000000 persisty-0.0.6/persisty/attr/generator/uuid_generator.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1304 2023-01-17 18:43:12.000000 persisty-0.0.6/persisty/batch_edit.py
--rw-r--r--   0 tofarr     (501) staff       (20)      983 2023-01-17 18:43:12.000000 persisty-0.0.6/persisty/batch_edit_result.py
--rw-r--r--   0 tofarr     (501) staff       (20)       41 2023-01-12 05:23:25.000000 persisty-0.0.6/persisty/errors.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 14:28:13.000000 persisty-0.0.6/persisty/factory/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-03-19 15:06:43.000000 persisty-0.0.6/persisty/factory/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)      625 2023-03-19 15:06:43.000000 persisty-0.0.6/persisty/factory/default_store_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1725 2023-03-30 15:13:54.000000 persisty-0.0.6/persisty/factory/owned_store_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)     3275 2023-03-19 15:06:43.000000 persisty-0.0.6/persisty/factory/store_factory_abc.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 14:28:13.000000 persisty-0.0.6/persisty/finder/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-05 19:31:01.000000 persisty-0.0.6/persisty/finder/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1776 2023-03-30 17:29:52.000000 persisty-0.0.6/persisty/finder/module_store_finder.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1134 2023-03-30 21:59:07.000000 persisty-0.0.6/persisty/finder/store_finder_abc.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 14:28:13.000000 persisty-0.0.6/persisty/impl/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-05 17:22:52.000000 persisty-0.0.6/persisty/impl/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1461 2023-03-30 21:09:21.000000 persisty-0.0.6/persisty/impl/default_store.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 14:28:13.000000 persisty-0.0.6/persisty/impl/dynamodb/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-05 17:22:52.000000 persisty-0.0.6/persisty/impl/dynamodb/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1461 2023-01-17 18:43:12.000000 persisty-0.0.6/persisty/impl/dynamodb/dynamodb_key_config.py
--rw-r--r--   0 tofarr     (501) staff       (20)     6672 2023-04-18 00:07:16.000000 persisty-0.0.6/persisty/impl/dynamodb/dynamodb_store_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)    17588 2023-04-18 00:07:16.000000 persisty-0.0.6/persisty/impl/dynamodb/dynamodb_table_store.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2423 2023-04-18 00:06:51.000000 persisty-0.0.6/persisty/impl/dynamodb/partition_sort_index.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 14:28:13.000000 persisty-0.0.6/persisty/impl/mem/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-05 17:22:52.000000 persisty-0.0.6/persisty/impl/mem/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     3951 2023-03-19 15:06:43.000000 persisty-0.0.6/persisty/impl/mem/mem_store.py
--rw-r--r--   0 tofarr     (501) staff       (20)      915 2023-03-30 15:48:00.000000 persisty-0.0.6/persisty/impl/mem/mem_store_factory.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 14:28:13.000000 persisty-0.0.6/persisty/impl/sqlalchemy/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-05 17:22:52.000000 persisty-0.0.6/persisty/impl/sqlalchemy/__init__.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 14:28:13.000000 persisty-0.0.6/persisty/impl/sqlalchemy/search_filter/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-05 17:22:52.000000 persisty-0.0.6/persisty/impl/sqlalchemy/search_filter/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1412 2023-01-17 18:43:12.000000 persisty-0.0.6/persisty/impl/sqlalchemy/search_filter/and_filter_converter.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2162 2023-01-17 18:43:12.000000 persisty-0.0.6/persisty/impl/sqlalchemy/search_filter/field_filter_converter.py
--rw-r--r--   0 tofarr     (501) staff       (20)      607 2023-01-17 18:43:12.000000 persisty-0.0.6/persisty/impl/sqlalchemy/search_filter/include_all_converter.py
--rw-r--r--   0 tofarr     (501) staff       (20)      827 2023-01-17 18:43:12.000000 persisty-0.0.6/persisty/impl/sqlalchemy/search_filter/not_filter_converter.py
--rw-r--r--   0 tofarr     (501) staff       (20)      845 2023-01-17 18:43:12.000000 persisty-0.0.6/persisty/impl/sqlalchemy/search_filter/or_filter_converter.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1015 2023-01-17 18:43:12.000000 persisty-0.0.6/persisty/impl/sqlalchemy/search_filter/query_filter_converter.py
--rw-r--r--   0 tofarr     (501) staff       (20)      677 2023-01-17 18:43:12.000000 persisty-0.0.6/persisty/impl/sqlalchemy/search_filter/search_filter_converter_abc.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1362 2023-01-17 18:43:12.000000 persisty-0.0.6/persisty/impl/sqlalchemy/search_filter/search_filter_converter_context.py
--rw-r--r--   0 tofarr     (501) staff       (20)     3648 2023-01-17 18:43:12.000000 persisty-0.0.6/persisty/impl/sqlalchemy/sqlalchemy_column_converter.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1353 2023-03-30 17:49:46.000000 persisty-0.0.6/persisty/impl/sqlalchemy/sqlalchemy_constraint_converter.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1394 2023-03-30 20:09:21.000000 persisty-0.0.6/persisty/impl/sqlalchemy/sqlalchemy_context.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1088 2023-03-30 20:09:02.000000 persisty-0.0.6/persisty/impl/sqlalchemy/sqlalchemy_context_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)      894 2023-03-30 02:34:01.000000 persisty-0.0.6/persisty/impl/sqlalchemy/sqlalchemy_context_factory_abc.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2529 2023-04-17 22:52:15.000000 persisty-0.0.6/persisty/impl/sqlalchemy/sqlalchemy_table_converter.py
--rw-r--r--   0 tofarr     (501) staff       (20)    18019 2023-04-17 21:07:20.000000 persisty-0.0.6/persisty/impl/sqlalchemy/sqlalchemy_table_store.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1189 2023-03-30 15:48:06.000000 persisty-0.0.6/persisty/impl/sqlalchemy/sqlalchemy_table_store_factory.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 14:28:13.000000 persisty-0.0.6/persisty/index/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-04-17 20:43:57.000000 persisty-0.0.6/persisty/index/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)      259 2023-04-17 20:40:30.000000 persisty-0.0.6/persisty/index/attr_index.py
--rw-r--r--   0 tofarr     (501) staff       (20)       52 2023-04-17 20:39:42.000000 persisty-0.0.6/persisty/index/index_abc.py
--rw-r--r--   0 tofarr     (501) staff       (20)      271 2023-04-17 20:41:37.000000 persisty-0.0.6/persisty/index/unique_index.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 14:28:13.000000 persisty-0.0.6/persisty/io/
--rw-r--r--   0 tofarr     (501) staff       (20)     3200 2023-03-19 15:06:43.000000 persisty-0.0.6/persisty/io/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1290 2023-03-30 21:14:52.000000 persisty-0.0.6/persisty/io/seed.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 14:28:13.000000 persisty-0.0.6/persisty/key_config/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-05 17:22:52.000000 persisty-0.0.6/persisty/key_config/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2041 2023-01-17 18:43:12.000000 persisty-0.0.6/persisty/key_config/attr_key_config.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1265 2023-01-17 18:43:12.000000 persisty-0.0.6/persisty/key_config/composite_key_config.py
--rw-r--r--   0 tofarr     (501) staff       (20)      777 2023-03-24 21:18:32.000000 persisty-0.0.6/persisty/key_config/key_config_abc.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 14:28:13.000000 persisty-0.0.6/persisty/link/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-10 12:25:11.000000 persisty-0.0.6/persisty/link/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2958 2023-03-30 22:16:51.000000 persisty-0.0.6/persisty/link/belongs_to.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1702 2023-03-19 15:06:43.000000 persisty-0.0.6/persisty/link/has_count.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2250 2023-03-30 22:18:04.000000 persisty-0.0.6/persisty/link/has_many.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1125 2023-03-19 15:06:43.000000 persisty-0.0.6/persisty/link/link_abc.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1681 2023-03-19 15:06:43.000000 persisty-0.0.6/persisty/link/linked_store_abc.py
--rw-r--r--   0 tofarr     (501) staff       (20)      114 2023-01-05 17:22:52.000000 persisty-0.0.6/persisty/link/on_delete.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 14:28:13.000000 persisty-0.0.6/persisty/migration/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-03-30 00:58:05.000000 persisty-0.0.6/persisty/migration/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1229 2023-03-30 21:59:55.000000 persisty-0.0.6/persisty/migration/alembic.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 14:28:13.000000 persisty-0.0.6/persisty/migration/serverless/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-03-30 01:07:24.000000 persisty-0.0.6/persisty/migration/serverless/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     4126 2023-04-06 13:26:22.000000 persisty-0.0.6/persisty/migration/serverless/dynamodb_yml_config.py
--rw-r--r--   0 tofarr     (501) staff       (20)      569 2023-01-17 18:43:12.000000 persisty-0.0.6/persisty/result_set.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 14:28:13.000000 persisty-0.0.6/persisty/search_filter/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-05 17:22:52.000000 persisty-0.0.6/persisty/search_filter/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2777 2023-04-18 13:52:30.000000 persisty-0.0.6/persisty/search_filter/and_filter.py
--rw-r--r--   0 tofarr     (501) staff       (20)      827 2023-03-19 15:06:43.000000 persisty-0.0.6/persisty/search_filter/exclude_all.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1412 2023-01-17 18:43:12.000000 persisty-0.0.6/persisty/search_filter/filter_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)      624 2023-03-19 15:06:43.000000 persisty-0.0.6/persisty/search_filter/include_all.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1032 2023-01-17 18:43:12.000000 persisty-0.0.6/persisty/search_filter/not_filter.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2397 2023-04-18 13:52:30.000000 persisty-0.0.6/persisty/search_filter/or_filter.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1908 2023-01-17 18:43:12.000000 persisty-0.0.6/persisty/search_filter/query_filter.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1631 2023-01-17 18:43:12.000000 persisty-0.0.6/persisty/search_filter/search_filter_abc.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2003 2023-04-18 14:02:40.000000 persisty-0.0.6/persisty/search_filter/search_filter_factory.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 14:28:13.000000 persisty-0.0.6/persisty/search_order/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-05 17:22:52.000000 persisty-0.0.6/persisty/search_order/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)      919 2023-01-17 18:43:12.000000 persisty-0.0.6/persisty/search_order/search_order.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1112 2023-04-17 14:04:58.000000 persisty-0.0.6/persisty/search_order/search_order_attr.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1178 2023-03-19 15:06:43.000000 persisty-0.0.6/persisty/search_order/search_order_factory.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 14:28:13.000000 persisty-0.0.6/persisty/servey/
--rw-r--r--   0 tofarr     (501) staff       (20)      540 2023-03-19 15:06:43.000000 persisty-0.0.6/persisty/servey/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)    11179 2023-04-18 14:25:35.000000 persisty-0.0.6/persisty/servey/actions.py
--rw-r--r--   0 tofarr     (501) staff       (20)       87 2023-01-17 18:43:12.000000 persisty-0.0.6/persisty/servey/generated.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 14:28:13.000000 persisty-0.0.6/persisty/store/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-17 18:43:12.000000 persisty-0.0.6/persisty/store/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1483 2023-01-17 18:43:12.000000 persisty-0.0.6/persisty/store/filtered_store.py
--rw-r--r--   0 tofarr     (501) staff       (20)     8672 2023-01-17 18:43:12.000000 persisty-0.0.6/persisty/store/filtered_store_abc.py
--rw-r--r--   0 tofarr     (501) staff       (20)      379 2023-01-17 18:43:12.000000 persisty-0.0.6/persisty/store/logging_store.py
--rw-r--r--   0 tofarr     (501) staff       (20)     6401 2023-03-30 15:14:07.000000 persisty-0.0.6/persisty/store/owned_store.py
--rw-r--r--   0 tofarr     (501) staff       (20)     5020 2023-01-17 18:43:12.000000 persisty-0.0.6/persisty/store/restrict_access_store.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2609 2023-01-17 18:43:12.000000 persisty-0.0.6/persisty/store/schema_validating_store.py
--rw-r--r--   0 tofarr     (501) staff       (20)     8608 2023-01-17 18:43:12.000000 persisty-0.0.6/persisty/store/store_abc.py
--rw-r--r--   0 tofarr     (501) staff       (20)     5537 2023-01-17 18:43:12.000000 persisty-0.0.6/persisty/store/ttl_cache_store.py
--rw-r--r--   0 tofarr     (501) staff       (20)     3261 2023-04-17 21:34:03.000000 persisty-0.0.6/persisty/store/unique_index_store.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2371 2023-03-19 15:06:43.000000 persisty-0.0.6/persisty/store/wrapper_store_abc.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1074 2023-01-17 18:43:12.000000 persisty-0.0.6/persisty/store_access.py
--rw-r--r--   0 tofarr     (501) staff       (20)     6996 2023-04-17 21:07:20.000000 persisty-0.0.6/persisty/store_meta.py
--rw-r--r--   0 tofarr     (501) staff       (20)     6610 2023-04-18 13:20:04.000000 persisty-0.0.6/persisty/stored.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 14:28:13.000000 persisty-0.0.6/persisty/trigger/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-07 17:19:03.000000 persisty-0.0.6/persisty/trigger/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)      156 2023-01-17 18:43:12.000000 persisty-0.0.6/persisty/trigger/after_create_trigger.py
--rw-r--r--   0 tofarr     (501) staff       (20)      156 2023-01-17 18:43:12.000000 persisty-0.0.6/persisty/trigger/after_delete_trigger.py
--rw-r--r--   0 tofarr     (501) staff       (20)      156 2023-01-17 18:43:12.000000 persisty-0.0.6/persisty/trigger/after_update_trigger.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2334 2023-01-17 18:43:12.000000 persisty-0.0.6/persisty/trigger/asyncio_trigger_store.py
--rw-r--r--   0 tofarr     (501) staff       (20)      985 2023-01-17 18:43:12.000000 persisty-0.0.6/persisty/trigger/celery_store_trigger_config.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2553 2023-01-17 18:43:12.000000 persisty-0.0.6/persisty/trigger/celery_trigger_store.py
--rw-r--r--   0 tofarr     (501) staff       (20)     3164 2023-01-17 18:43:12.000000 persisty-0.0.6/persisty/trigger/dynamodb_post_process_event_handler.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1504 2023-01-17 18:43:12.000000 persisty-0.0.6/persisty/trigger/serverless_trigger_handler.py
--rw-r--r--   0 tofarr     (501) staff       (20)     3287 2023-03-30 15:47:07.000000 persisty-0.0.6/persisty/trigger/store_triggers.py
--rw-r--r--   0 tofarr     (501) staff       (20)      638 2023-01-17 18:43:12.000000 persisty-0.0.6/persisty/trigger/wrapper.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 14:28:13.000000 persisty-0.0.6/persisty/util/
--rw-r--r--   0 tofarr     (501) staff       (20)     2023 2023-01-11 03:09:38.000000 persisty-0.0.6/persisty/util/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1094 2023-01-05 17:22:52.000000 persisty-0.0.6/persisty/util/encrypt_at_rest.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1866 2023-01-17 18:43:12.000000 persisty-0.0.6/persisty/util/logify.py
--rw-r--r--   0 tofarr     (501) staff       (20)      754 2023-01-17 18:43:12.000000 persisty-0.0.6/persisty/util/undefined.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 14:28:13.000000 persisty-0.0.6/persisty.egg-info/
--rw-r--r--   0 tofarr     (501) staff       (20)     4051 2023-04-18 14:28:12.000000 persisty-0.0.6/persisty.egg-info/PKG-INFO
--rw-r--r--   0 tofarr     (501) staff       (20)     5783 2023-04-18 14:28:13.000000 persisty-0.0.6/persisty.egg-info/SOURCES.txt
--rw-r--r--   0 tofarr     (501) staff       (20)        1 2023-04-18 14:28:12.000000 persisty-0.0.6/persisty.egg-info/dependency_links.txt
--rw-r--r--   0 tofarr     (501) staff       (20)       48 2023-04-18 14:28:12.000000 persisty-0.0.6/persisty.egg-info/requires.txt
--rw-r--r--   0 tofarr     (501) staff       (20)       38 2023-04-18 14:28:12.000000 persisty-0.0.6/persisty.egg-info/top_level.txt
--rw-r--r--   0 tofarr     (501) staff       (20)       38 2023-04-18 14:28:13.000000 persisty-0.0.6/setup.cfg
--rw-r--r--   0 tofarr     (501) staff       (20)      946 2023-04-13 14:34:44.000000 persisty-0.0.6/setup.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 14:28:13.000000 persisty-0.0.6/tests/
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 14:28:13.000000 persisty-0.0.6/tests/attr/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-03-19 15:06:43.000000 persisty-0.0.6/tests/attr/__init__.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 14:28:13.000000 persisty-0.0.6/tests/attr/generator/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-03-19 15:06:43.000000 persisty-0.0.6/tests/attr/generator/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)      636 2023-03-19 15:06:43.000000 persisty-0.0.6/tests/attr/generator/test_defaults.py
--rw-r--r--   0 tofarr     (501) staff       (20)      915 2023-03-19 15:06:43.000000 persisty-0.0.6/tests/attr/test_attr.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2492 2023-03-19 15:06:43.000000 persisty-0.0.6/tests/attr/test_attr_filter.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1321 2023-03-19 15:06:43.000000 persisty-0.0.6/tests/attr/test_attr_filter_op.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 14:28:13.000000 persisty-0.0.6/tests/factory/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-03-19 15:06:43.000000 persisty-0.0.6/tests/factory/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)      664 2023-03-19 15:06:43.000000 persisty-0.0.6/tests/factory/test_default_store_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2439 2023-04-17 21:46:14.000000 persisty-0.0.6/tests/factory/test_owned_store_factory.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 14:28:13.000000 persisty-0.0.6/tests/finder/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-03-19 15:06:43.000000 persisty-0.0.6/tests/finder/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)      361 2023-03-19 15:06:43.000000 persisty-0.0.6/tests/finder/fixtures.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1702 2023-03-19 15:06:43.000000 persisty-0.0.6/tests/finder/test_module_store_finder.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 14:28:13.000000 persisty-0.0.6/tests/fixtures/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-07-19 13:13:59.000000 persisty-0.0.6/tests/fixtures/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1464 2023-04-18 03:18:56.000000 persisty-0.0.6/tests/fixtures/number_name.py
--rw-r--r--   0 tofarr     (501) staff       (20)    21310 2023-01-17 18:43:12.000000 persisty-0.0.6/tests/fixtures/storage_tst_abc.py
--rw-r--r--   0 tofarr     (501) staff       (20)    14045 2023-04-17 22:14:54.000000 persisty-0.0.6/tests/fixtures/super_bowl_results.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 14:28:13.000000 persisty-0.0.6/tests/impl/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-08-07 19:20:56.000000 persisty-0.0.6/tests/impl/__init__.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 14:28:13.000000 persisty-0.0.6/tests/impl/dynamodb/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-05 16:41:50.000000 persisty-0.0.6/tests/impl/dynamodb/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     6078 2023-04-18 00:07:16.000000 persisty-0.0.6/tests/impl/dynamodb/test_dynamodb_store.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 14:28:13.000000 persisty-0.0.6/tests/impl/mem/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-07-20 13:33:37.000000 persisty-0.0.6/tests/impl/mem/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     3478 2023-01-17 18:43:12.000000 persisty-0.0.6/tests/impl/mem/test_mem_store.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 14:28:13.000000 persisty-0.0.6/tests/impl/sqlalchemy/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-08-07 19:22:30.000000 persisty-0.0.6/tests/impl/sqlalchemy/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     4970 2023-01-17 18:43:12.000000 persisty-0.0.6/tests/impl/sqlalchemy/test_sqlalchemy_table_store.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 14:28:13.000000 persisty-0.0.6/tests/util/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-07-20 13:34:03.000000 persisty-0.0.6/tests/util/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)      595 2022-07-21 04:14:28.000000 persisty-0.0.6/tests/util/test_encrypt_at_rest.py
--rw-r--r--   0 tofarr     (501) staff       (20)     3262 2023-03-19 15:06:43.000000 persisty-0.0.6/tests/util/test_logify.py
--rw-r--r--   0 tofarr     (501) staff       (20)      377 2022-07-20 14:03:55.000000 persisty-0.0.6/tests/util/test_undefined.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1368 2022-07-21 04:14:28.000000 persisty-0.0.6/tests/util/test_util.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:40:16.000000 persisty-0.0.7/
+-rw-r--r--   0 tofarr     (501) staff       (20)     4051 2023-04-18 21:40:16.000000 persisty-0.0.7/PKG-INFO
+-rw-r--r--   0 tofarr     (501) staff       (20)     3629 2023-04-16 16:31:32.000000 persisty-0.0.7/README.md
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:40:16.000000 persisty-0.0.7/marshy_config_persisty/
+-rw-r--r--   0 tofarr     (501) staff       (20)     5933 2023-04-18 00:07:16.000000 persisty-0.0.7/marshy_config_persisty/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1670 2023-01-17 18:43:12.000000 persisty-0.0.7/marshy_config_persisty/sqlalchemy_config.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:40:16.000000 persisty-0.0.7/persisty/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-10 11:54:34.000000 persisty-0.0.7/persisty/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)       22 2023-04-18 21:36:36.000000 persisty-0.0.7/persisty/__version__.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:40:16.000000 persisty-0.0.7/persisty/attr/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-17 18:43:12.000000 persisty-0.0.7/persisty/attr/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     2290 2023-04-18 14:22:16.000000 persisty-0.0.7/persisty/attr/attr.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     2033 2023-03-19 15:06:43.000000 persisty-0.0.7/persisty/attr/attr_filter.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     2499 2023-03-19 15:06:43.000000 persisty-0.0.7/persisty/attr/attr_filter_op.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      868 2023-03-19 15:06:43.000000 persisty-0.0.7/persisty/attr/attr_type.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:40:16.000000 persisty-0.0.7/persisty/attr/generator/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-17 18:43:12.000000 persisty-0.0.7/persisty/attr/generator/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      168 2023-01-17 18:43:12.000000 persisty-0.0.7/persisty/attr/generator/attr_value_generator_abc.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      375 2023-01-17 18:43:12.000000 persisty-0.0.7/persisty/attr/generator/default_value_generator.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1203 2023-01-17 18:43:12.000000 persisty-0.0.7/persisty/attr/generator/defaults.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      749 2023-03-19 15:06:43.000000 persisty-0.0.7/persisty/attr/generator/int_sequence_generator.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      798 2023-01-17 18:43:12.000000 persisty-0.0.7/persisty/attr/generator/str_sequence_generator.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      382 2023-01-17 18:43:12.000000 persisty-0.0.7/persisty/attr/generator/timestamp_generator.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      328 2023-01-17 18:43:12.000000 persisty-0.0.7/persisty/attr/generator/uuid_generator.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1304 2023-01-17 18:43:12.000000 persisty-0.0.7/persisty/batch_edit.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      983 2023-01-17 18:43:12.000000 persisty-0.0.7/persisty/batch_edit_result.py
+-rw-r--r--   0 tofarr     (501) staff       (20)       41 2023-01-12 05:23:25.000000 persisty-0.0.7/persisty/errors.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:40:16.000000 persisty-0.0.7/persisty/factory/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-03-19 15:06:43.000000 persisty-0.0.7/persisty/factory/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      625 2023-03-19 15:06:43.000000 persisty-0.0.7/persisty/factory/default_store_factory.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1725 2023-03-30 15:13:54.000000 persisty-0.0.7/persisty/factory/owned_store_factory.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     3275 2023-03-19 15:06:43.000000 persisty-0.0.7/persisty/factory/store_factory_abc.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:40:16.000000 persisty-0.0.7/persisty/finder/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-05 19:31:01.000000 persisty-0.0.7/persisty/finder/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1776 2023-03-30 17:29:52.000000 persisty-0.0.7/persisty/finder/module_store_finder.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1134 2023-03-30 21:59:07.000000 persisty-0.0.7/persisty/finder/store_finder_abc.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:40:16.000000 persisty-0.0.7/persisty/impl/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-05 17:22:52.000000 persisty-0.0.7/persisty/impl/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1461 2023-03-30 21:09:21.000000 persisty-0.0.7/persisty/impl/default_store.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:40:16.000000 persisty-0.0.7/persisty/impl/dynamodb/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-05 17:22:52.000000 persisty-0.0.7/persisty/impl/dynamodb/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1461 2023-01-17 18:43:12.000000 persisty-0.0.7/persisty/impl/dynamodb/dynamodb_key_config.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     6672 2023-04-18 00:07:16.000000 persisty-0.0.7/persisty/impl/dynamodb/dynamodb_store_factory.py
+-rw-r--r--   0 tofarr     (501) staff       (20)    17588 2023-04-18 00:07:16.000000 persisty-0.0.7/persisty/impl/dynamodb/dynamodb_table_store.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     2423 2023-04-18 00:06:51.000000 persisty-0.0.7/persisty/impl/dynamodb/partition_sort_index.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:40:16.000000 persisty-0.0.7/persisty/impl/mem/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-05 17:22:52.000000 persisty-0.0.7/persisty/impl/mem/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     3951 2023-03-19 15:06:43.000000 persisty-0.0.7/persisty/impl/mem/mem_store.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      915 2023-03-30 15:48:00.000000 persisty-0.0.7/persisty/impl/mem/mem_store_factory.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:40:16.000000 persisty-0.0.7/persisty/impl/sqlalchemy/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-05 17:22:52.000000 persisty-0.0.7/persisty/impl/sqlalchemy/__init__.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:40:16.000000 persisty-0.0.7/persisty/impl/sqlalchemy/search_filter/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-05 17:22:52.000000 persisty-0.0.7/persisty/impl/sqlalchemy/search_filter/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1412 2023-01-17 18:43:12.000000 persisty-0.0.7/persisty/impl/sqlalchemy/search_filter/and_filter_converter.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     2162 2023-01-17 18:43:12.000000 persisty-0.0.7/persisty/impl/sqlalchemy/search_filter/field_filter_converter.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      607 2023-01-17 18:43:12.000000 persisty-0.0.7/persisty/impl/sqlalchemy/search_filter/include_all_converter.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      827 2023-01-17 18:43:12.000000 persisty-0.0.7/persisty/impl/sqlalchemy/search_filter/not_filter_converter.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      845 2023-01-17 18:43:12.000000 persisty-0.0.7/persisty/impl/sqlalchemy/search_filter/or_filter_converter.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1015 2023-01-17 18:43:12.000000 persisty-0.0.7/persisty/impl/sqlalchemy/search_filter/query_filter_converter.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      677 2023-01-17 18:43:12.000000 persisty-0.0.7/persisty/impl/sqlalchemy/search_filter/search_filter_converter_abc.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1362 2023-01-17 18:43:12.000000 persisty-0.0.7/persisty/impl/sqlalchemy/search_filter/search_filter_converter_context.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     3648 2023-01-17 18:43:12.000000 persisty-0.0.7/persisty/impl/sqlalchemy/sqlalchemy_column_converter.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1353 2023-03-30 17:49:46.000000 persisty-0.0.7/persisty/impl/sqlalchemy/sqlalchemy_constraint_converter.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1394 2023-03-30 20:09:21.000000 persisty-0.0.7/persisty/impl/sqlalchemy/sqlalchemy_context.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1088 2023-03-30 20:09:02.000000 persisty-0.0.7/persisty/impl/sqlalchemy/sqlalchemy_context_factory.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      894 2023-03-30 02:34:01.000000 persisty-0.0.7/persisty/impl/sqlalchemy/sqlalchemy_context_factory_abc.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     2529 2023-04-17 22:52:15.000000 persisty-0.0.7/persisty/impl/sqlalchemy/sqlalchemy_table_converter.py
+-rw-r--r--   0 tofarr     (501) staff       (20)    18019 2023-04-17 21:07:20.000000 persisty-0.0.7/persisty/impl/sqlalchemy/sqlalchemy_table_store.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1189 2023-03-30 15:48:06.000000 persisty-0.0.7/persisty/impl/sqlalchemy/sqlalchemy_table_store_factory.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:40:16.000000 persisty-0.0.7/persisty/index/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-04-17 20:43:57.000000 persisty-0.0.7/persisty/index/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      259 2023-04-17 20:40:30.000000 persisty-0.0.7/persisty/index/attr_index.py
+-rw-r--r--   0 tofarr     (501) staff       (20)       52 2023-04-17 20:39:42.000000 persisty-0.0.7/persisty/index/index_abc.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      271 2023-04-17 20:41:37.000000 persisty-0.0.7/persisty/index/unique_index.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:40:16.000000 persisty-0.0.7/persisty/io/
+-rw-r--r--   0 tofarr     (501) staff       (20)     3200 2023-03-19 15:06:43.000000 persisty-0.0.7/persisty/io/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1290 2023-03-30 21:14:52.000000 persisty-0.0.7/persisty/io/seed.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:40:16.000000 persisty-0.0.7/persisty/key_config/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-05 17:22:52.000000 persisty-0.0.7/persisty/key_config/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     2041 2023-01-17 18:43:12.000000 persisty-0.0.7/persisty/key_config/attr_key_config.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1265 2023-01-17 18:43:12.000000 persisty-0.0.7/persisty/key_config/composite_key_config.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      777 2023-03-24 21:18:32.000000 persisty-0.0.7/persisty/key_config/key_config_abc.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:40:16.000000 persisty-0.0.7/persisty/link/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-10 12:25:11.000000 persisty-0.0.7/persisty/link/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     2958 2023-03-30 22:16:51.000000 persisty-0.0.7/persisty/link/belongs_to.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1702 2023-03-19 15:06:43.000000 persisty-0.0.7/persisty/link/has_count.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     2250 2023-03-30 22:18:04.000000 persisty-0.0.7/persisty/link/has_many.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1125 2023-03-19 15:06:43.000000 persisty-0.0.7/persisty/link/link_abc.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1681 2023-03-19 15:06:43.000000 persisty-0.0.7/persisty/link/linked_store_abc.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      114 2023-01-05 17:22:52.000000 persisty-0.0.7/persisty/link/on_delete.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:40:16.000000 persisty-0.0.7/persisty/migration/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-03-30 00:58:05.000000 persisty-0.0.7/persisty/migration/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1229 2023-03-30 21:59:55.000000 persisty-0.0.7/persisty/migration/alembic.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:40:16.000000 persisty-0.0.7/persisty/migration/serverless/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-03-30 01:07:24.000000 persisty-0.0.7/persisty/migration/serverless/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     4126 2023-04-06 13:26:22.000000 persisty-0.0.7/persisty/migration/serverless/dynamodb_yml_config.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      569 2023-01-17 18:43:12.000000 persisty-0.0.7/persisty/result_set.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:40:16.000000 persisty-0.0.7/persisty/search_filter/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-05 17:22:52.000000 persisty-0.0.7/persisty/search_filter/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     2777 2023-04-18 13:52:30.000000 persisty-0.0.7/persisty/search_filter/and_filter.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      827 2023-03-19 15:06:43.000000 persisty-0.0.7/persisty/search_filter/exclude_all.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1412 2023-01-17 18:43:12.000000 persisty-0.0.7/persisty/search_filter/filter_factory.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      624 2023-03-19 15:06:43.000000 persisty-0.0.7/persisty/search_filter/include_all.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1032 2023-01-17 18:43:12.000000 persisty-0.0.7/persisty/search_filter/not_filter.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     2397 2023-04-18 13:52:30.000000 persisty-0.0.7/persisty/search_filter/or_filter.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1908 2023-01-17 18:43:12.000000 persisty-0.0.7/persisty/search_filter/query_filter.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1631 2023-01-17 18:43:12.000000 persisty-0.0.7/persisty/search_filter/search_filter_abc.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     2003 2023-04-18 14:02:40.000000 persisty-0.0.7/persisty/search_filter/search_filter_factory.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:40:16.000000 persisty-0.0.7/persisty/search_order/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-05 17:22:52.000000 persisty-0.0.7/persisty/search_order/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      919 2023-01-17 18:43:12.000000 persisty-0.0.7/persisty/search_order/search_order.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1112 2023-04-17 14:04:58.000000 persisty-0.0.7/persisty/search_order/search_order_attr.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1178 2023-03-19 15:06:43.000000 persisty-0.0.7/persisty/search_order/search_order_factory.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:40:16.000000 persisty-0.0.7/persisty/servey/
+-rw-r--r--   0 tofarr     (501) staff       (20)      540 2023-03-19 15:06:43.000000 persisty-0.0.7/persisty/servey/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)    11179 2023-04-18 14:25:35.000000 persisty-0.0.7/persisty/servey/actions.py
+-rw-r--r--   0 tofarr     (501) staff       (20)       87 2023-01-17 18:43:12.000000 persisty-0.0.7/persisty/servey/generated.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:40:16.000000 persisty-0.0.7/persisty/store/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-17 18:43:12.000000 persisty-0.0.7/persisty/store/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1483 2023-01-17 18:43:12.000000 persisty-0.0.7/persisty/store/filtered_store.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     8672 2023-01-17 18:43:12.000000 persisty-0.0.7/persisty/store/filtered_store_abc.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      379 2023-01-17 18:43:12.000000 persisty-0.0.7/persisty/store/logging_store.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     6401 2023-03-30 15:14:07.000000 persisty-0.0.7/persisty/store/owned_store.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     5020 2023-01-17 18:43:12.000000 persisty-0.0.7/persisty/store/restrict_access_store.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     2609 2023-01-17 18:43:12.000000 persisty-0.0.7/persisty/store/schema_validating_store.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     8608 2023-01-17 18:43:12.000000 persisty-0.0.7/persisty/store/store_abc.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     5537 2023-01-17 18:43:12.000000 persisty-0.0.7/persisty/store/ttl_cache_store.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     3261 2023-04-17 21:34:03.000000 persisty-0.0.7/persisty/store/unique_index_store.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     2371 2023-03-19 15:06:43.000000 persisty-0.0.7/persisty/store/wrapper_store_abc.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1074 2023-01-17 18:43:12.000000 persisty-0.0.7/persisty/store_access.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     6996 2023-04-17 21:07:20.000000 persisty-0.0.7/persisty/store_meta.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     6610 2023-04-18 13:20:04.000000 persisty-0.0.7/persisty/stored.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:40:16.000000 persisty-0.0.7/persisty/trigger/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-07 17:19:03.000000 persisty-0.0.7/persisty/trigger/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      156 2023-01-17 18:43:12.000000 persisty-0.0.7/persisty/trigger/after_create_trigger.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      156 2023-01-17 18:43:12.000000 persisty-0.0.7/persisty/trigger/after_delete_trigger.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      156 2023-01-17 18:43:12.000000 persisty-0.0.7/persisty/trigger/after_update_trigger.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     2334 2023-01-17 18:43:12.000000 persisty-0.0.7/persisty/trigger/asyncio_trigger_store.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      985 2023-01-17 18:43:12.000000 persisty-0.0.7/persisty/trigger/celery_store_trigger_config.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     2553 2023-01-17 18:43:12.000000 persisty-0.0.7/persisty/trigger/celery_trigger_store.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     3164 2023-01-17 18:43:12.000000 persisty-0.0.7/persisty/trigger/dynamodb_post_process_event_handler.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1504 2023-01-17 18:43:12.000000 persisty-0.0.7/persisty/trigger/serverless_trigger_handler.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     3287 2023-03-30 15:47:07.000000 persisty-0.0.7/persisty/trigger/store_triggers.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      638 2023-01-17 18:43:12.000000 persisty-0.0.7/persisty/trigger/wrapper.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:40:16.000000 persisty-0.0.7/persisty/util/
+-rw-r--r--   0 tofarr     (501) staff       (20)     2023 2023-01-11 03:09:38.000000 persisty-0.0.7/persisty/util/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1094 2023-01-05 17:22:52.000000 persisty-0.0.7/persisty/util/encrypt_at_rest.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1866 2023-01-17 18:43:12.000000 persisty-0.0.7/persisty/util/logify.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      754 2023-01-17 18:43:12.000000 persisty-0.0.7/persisty/util/undefined.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:40:16.000000 persisty-0.0.7/persisty.egg-info/
+-rw-r--r--   0 tofarr     (501) staff       (20)     4051 2023-04-18 21:40:16.000000 persisty-0.0.7/persisty.egg-info/PKG-INFO
+-rw-r--r--   0 tofarr     (501) staff       (20)     5783 2023-04-18 21:40:16.000000 persisty-0.0.7/persisty.egg-info/SOURCES.txt
+-rw-r--r--   0 tofarr     (501) staff       (20)        1 2023-04-18 21:40:16.000000 persisty-0.0.7/persisty.egg-info/dependency_links.txt
+-rw-r--r--   0 tofarr     (501) staff       (20)       48 2023-04-18 21:40:16.000000 persisty-0.0.7/persisty.egg-info/requires.txt
+-rw-r--r--   0 tofarr     (501) staff       (20)       38 2023-04-18 21:40:16.000000 persisty-0.0.7/persisty.egg-info/top_level.txt
+-rw-r--r--   0 tofarr     (501) staff       (20)       38 2023-04-18 21:40:16.000000 persisty-0.0.7/setup.cfg
+-rw-r--r--   0 tofarr     (501) staff       (20)      946 2023-04-18 21:35:52.000000 persisty-0.0.7/setup.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:40:16.000000 persisty-0.0.7/tests/
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:40:16.000000 persisty-0.0.7/tests/attr/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-03-19 15:06:43.000000 persisty-0.0.7/tests/attr/__init__.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:40:16.000000 persisty-0.0.7/tests/attr/generator/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-03-19 15:06:43.000000 persisty-0.0.7/tests/attr/generator/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      636 2023-03-19 15:06:43.000000 persisty-0.0.7/tests/attr/generator/test_defaults.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      915 2023-03-19 15:06:43.000000 persisty-0.0.7/tests/attr/test_attr.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     2492 2023-03-19 15:06:43.000000 persisty-0.0.7/tests/attr/test_attr_filter.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1321 2023-03-19 15:06:43.000000 persisty-0.0.7/tests/attr/test_attr_filter_op.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:40:16.000000 persisty-0.0.7/tests/factory/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-03-19 15:06:43.000000 persisty-0.0.7/tests/factory/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      664 2023-03-19 15:06:43.000000 persisty-0.0.7/tests/factory/test_default_store_factory.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     2439 2023-04-17 21:46:14.000000 persisty-0.0.7/tests/factory/test_owned_store_factory.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:40:16.000000 persisty-0.0.7/tests/finder/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-03-19 15:06:43.000000 persisty-0.0.7/tests/finder/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      361 2023-03-19 15:06:43.000000 persisty-0.0.7/tests/finder/fixtures.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1702 2023-03-19 15:06:43.000000 persisty-0.0.7/tests/finder/test_module_store_finder.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:40:16.000000 persisty-0.0.7/tests/fixtures/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-07-19 13:13:59.000000 persisty-0.0.7/tests/fixtures/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1464 2023-04-18 03:18:56.000000 persisty-0.0.7/tests/fixtures/number_name.py
+-rw-r--r--   0 tofarr     (501) staff       (20)    21310 2023-01-17 18:43:12.000000 persisty-0.0.7/tests/fixtures/storage_tst_abc.py
+-rw-r--r--   0 tofarr     (501) staff       (20)    14045 2023-04-17 22:14:54.000000 persisty-0.0.7/tests/fixtures/super_bowl_results.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:40:16.000000 persisty-0.0.7/tests/impl/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-08-07 19:20:56.000000 persisty-0.0.7/tests/impl/__init__.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:40:16.000000 persisty-0.0.7/tests/impl/dynamodb/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2023-01-05 16:41:50.000000 persisty-0.0.7/tests/impl/dynamodb/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     6078 2023-04-18 00:07:16.000000 persisty-0.0.7/tests/impl/dynamodb/test_dynamodb_store.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:40:16.000000 persisty-0.0.7/tests/impl/mem/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-07-20 13:33:37.000000 persisty-0.0.7/tests/impl/mem/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     3478 2023-01-17 18:43:12.000000 persisty-0.0.7/tests/impl/mem/test_mem_store.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:40:16.000000 persisty-0.0.7/tests/impl/sqlalchemy/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-08-07 19:22:30.000000 persisty-0.0.7/tests/impl/sqlalchemy/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     4970 2023-01-17 18:43:12.000000 persisty-0.0.7/tests/impl/sqlalchemy/test_sqlalchemy_table_store.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:40:16.000000 persisty-0.0.7/tests/util/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-07-20 13:34:03.000000 persisty-0.0.7/tests/util/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      595 2022-07-21 04:14:28.000000 persisty-0.0.7/tests/util/test_encrypt_at_rest.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     3262 2023-03-19 15:06:43.000000 persisty-0.0.7/tests/util/test_logify.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      377 2022-07-20 14:03:55.000000 persisty-0.0.7/tests/util/test_undefined.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1368 2022-07-21 04:14:28.000000 persisty-0.0.7/tests/util/test_util.py
```

### Comparing `persisty-0.0.6/PKG-INFO` & `persisty-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: persisty
-Version: 0.0.6
+Version: 0.0.7
 Summary: A better persistence layer for python
 Home-page: https://github.com/tofarr/lambsync
 Author: Tim O'Farrell
 Author-email: tofarr@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `persisty-0.0.6/README.md` & `persisty-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/marshy_config_persisty/__init__.py` & `persisty-0.0.7/marshy_config_persisty/__init__.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/marshy_config_persisty/sqlalchemy_config.py` & `persisty-0.0.7/marshy_config_persisty/sqlalchemy_config.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/attr/attr.py` & `persisty-0.0.7/persisty/attr/attr.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/attr/attr_filter.py` & `persisty-0.0.7/persisty/attr/attr_filter.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/attr/attr_filter_op.py` & `persisty-0.0.7/persisty/attr/attr_filter_op.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/attr/attr_type.py` & `persisty-0.0.7/persisty/attr/attr_type.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/attr/generator/defaults.py` & `persisty-0.0.7/persisty/attr/generator/defaults.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/attr/generator/int_sequence_generator.py` & `persisty-0.0.7/persisty/attr/generator/int_sequence_generator.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/attr/generator/str_sequence_generator.py` & `persisty-0.0.7/persisty/attr/generator/str_sequence_generator.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/batch_edit.py` & `persisty-0.0.7/persisty/batch_edit.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/batch_edit_result.py` & `persisty-0.0.7/persisty/batch_edit_result.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/factory/default_store_factory.py` & `persisty-0.0.7/persisty/factory/default_store_factory.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/factory/owned_store_factory.py` & `persisty-0.0.7/persisty/factory/owned_store_factory.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/factory/store_factory_abc.py` & `persisty-0.0.7/persisty/factory/store_factory_abc.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/finder/module_store_finder.py` & `persisty-0.0.7/persisty/finder/module_store_finder.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/finder/store_finder_abc.py` & `persisty-0.0.7/persisty/finder/store_finder_abc.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/impl/default_store.py` & `persisty-0.0.7/persisty/impl/default_store.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/impl/dynamodb/dynamodb_key_config.py` & `persisty-0.0.7/persisty/impl/dynamodb/dynamodb_key_config.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/impl/dynamodb/dynamodb_store_factory.py` & `persisty-0.0.7/persisty/impl/dynamodb/dynamodb_store_factory.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/impl/dynamodb/dynamodb_table_store.py` & `persisty-0.0.7/persisty/impl/dynamodb/dynamodb_table_store.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/impl/dynamodb/partition_sort_index.py` & `persisty-0.0.7/persisty/impl/dynamodb/partition_sort_index.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/impl/mem/mem_store.py` & `persisty-0.0.7/persisty/impl/mem/mem_store.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/impl/mem/mem_store_factory.py` & `persisty-0.0.7/persisty/impl/mem/mem_store_factory.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/impl/sqlalchemy/search_filter/and_filter_converter.py` & `persisty-0.0.7/persisty/impl/sqlalchemy/search_filter/and_filter_converter.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/impl/sqlalchemy/search_filter/field_filter_converter.py` & `persisty-0.0.7/persisty/impl/sqlalchemy/search_filter/field_filter_converter.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/impl/sqlalchemy/search_filter/include_all_converter.py` & `persisty-0.0.7/persisty/impl/sqlalchemy/search_filter/include_all_converter.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/impl/sqlalchemy/search_filter/not_filter_converter.py` & `persisty-0.0.7/persisty/impl/sqlalchemy/search_filter/not_filter_converter.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/impl/sqlalchemy/search_filter/or_filter_converter.py` & `persisty-0.0.7/persisty/impl/sqlalchemy/search_filter/or_filter_converter.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/impl/sqlalchemy/search_filter/query_filter_converter.py` & `persisty-0.0.7/persisty/impl/sqlalchemy/search_filter/query_filter_converter.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/impl/sqlalchemy/search_filter/search_filter_converter_abc.py` & `persisty-0.0.7/persisty/impl/sqlalchemy/search_filter/search_filter_converter_abc.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/impl/sqlalchemy/search_filter/search_filter_converter_context.py` & `persisty-0.0.7/persisty/impl/sqlalchemy/search_filter/search_filter_converter_context.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/impl/sqlalchemy/sqlalchemy_column_converter.py` & `persisty-0.0.7/persisty/impl/sqlalchemy/sqlalchemy_column_converter.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/impl/sqlalchemy/sqlalchemy_constraint_converter.py` & `persisty-0.0.7/persisty/impl/sqlalchemy/sqlalchemy_constraint_converter.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/impl/sqlalchemy/sqlalchemy_context.py` & `persisty-0.0.7/persisty/impl/sqlalchemy/sqlalchemy_context.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/impl/sqlalchemy/sqlalchemy_context_factory.py` & `persisty-0.0.7/persisty/impl/sqlalchemy/sqlalchemy_context_factory.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/impl/sqlalchemy/sqlalchemy_context_factory_abc.py` & `persisty-0.0.7/persisty/impl/sqlalchemy/sqlalchemy_context_factory_abc.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/impl/sqlalchemy/sqlalchemy_table_converter.py` & `persisty-0.0.7/persisty/impl/sqlalchemy/sqlalchemy_table_converter.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/impl/sqlalchemy/sqlalchemy_table_store.py` & `persisty-0.0.7/persisty/impl/sqlalchemy/sqlalchemy_table_store.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/impl/sqlalchemy/sqlalchemy_table_store_factory.py` & `persisty-0.0.7/persisty/impl/sqlalchemy/sqlalchemy_table_store_factory.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/io/__init__.py` & `persisty-0.0.7/persisty/io/__init__.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/io/seed.py` & `persisty-0.0.7/persisty/io/seed.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/key_config/attr_key_config.py` & `persisty-0.0.7/persisty/key_config/attr_key_config.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/key_config/composite_key_config.py` & `persisty-0.0.7/persisty/key_config/composite_key_config.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/key_config/key_config_abc.py` & `persisty-0.0.7/persisty/key_config/key_config_abc.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/link/belongs_to.py` & `persisty-0.0.7/persisty/link/belongs_to.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/link/has_count.py` & `persisty-0.0.7/persisty/link/has_count.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/link/has_many.py` & `persisty-0.0.7/persisty/link/has_many.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/link/link_abc.py` & `persisty-0.0.7/persisty/link/link_abc.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/link/linked_store_abc.py` & `persisty-0.0.7/persisty/link/linked_store_abc.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/migration/alembic.py` & `persisty-0.0.7/persisty/migration/alembic.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/migration/serverless/dynamodb_yml_config.py` & `persisty-0.0.7/persisty/migration/serverless/dynamodb_yml_config.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/result_set.py` & `persisty-0.0.7/persisty/result_set.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/search_filter/and_filter.py` & `persisty-0.0.7/persisty/search_filter/and_filter.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/search_filter/exclude_all.py` & `persisty-0.0.7/persisty/search_filter/exclude_all.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/search_filter/filter_factory.py` & `persisty-0.0.7/persisty/search_filter/filter_factory.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/search_filter/include_all.py` & `persisty-0.0.7/persisty/search_filter/include_all.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/search_filter/not_filter.py` & `persisty-0.0.7/persisty/search_filter/not_filter.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/search_filter/or_filter.py` & `persisty-0.0.7/persisty/search_filter/or_filter.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/search_filter/query_filter.py` & `persisty-0.0.7/persisty/search_filter/query_filter.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/search_filter/search_filter_abc.py` & `persisty-0.0.7/persisty/search_filter/search_filter_abc.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/search_filter/search_filter_factory.py` & `persisty-0.0.7/persisty/search_filter/search_filter_factory.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/search_order/search_order.py` & `persisty-0.0.7/persisty/search_order/search_order.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/search_order/search_order_attr.py` & `persisty-0.0.7/persisty/search_order/search_order_attr.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/search_order/search_order_factory.py` & `persisty-0.0.7/persisty/search_order/search_order_factory.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/servey/__init__.py` & `persisty-0.0.7/persisty/servey/__init__.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/servey/actions.py` & `persisty-0.0.7/persisty/servey/actions.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/store/filtered_store.py` & `persisty-0.0.7/persisty/store/filtered_store.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/store/filtered_store_abc.py` & `persisty-0.0.7/persisty/store/filtered_store_abc.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/store/owned_store.py` & `persisty-0.0.7/persisty/store/owned_store.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/store/restrict_access_store.py` & `persisty-0.0.7/persisty/store/restrict_access_store.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/store/schema_validating_store.py` & `persisty-0.0.7/persisty/store/schema_validating_store.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/store/store_abc.py` & `persisty-0.0.7/persisty/store/store_abc.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/store/ttl_cache_store.py` & `persisty-0.0.7/persisty/store/ttl_cache_store.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/store/unique_index_store.py` & `persisty-0.0.7/persisty/store/unique_index_store.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/store/wrapper_store_abc.py` & `persisty-0.0.7/persisty/store/wrapper_store_abc.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/store_access.py` & `persisty-0.0.7/persisty/store_access.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/store_meta.py` & `persisty-0.0.7/persisty/store_meta.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/stored.py` & `persisty-0.0.7/persisty/stored.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/trigger/asyncio_trigger_store.py` & `persisty-0.0.7/persisty/trigger/asyncio_trigger_store.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/trigger/celery_store_trigger_config.py` & `persisty-0.0.7/persisty/trigger/celery_store_trigger_config.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/trigger/celery_trigger_store.py` & `persisty-0.0.7/persisty/trigger/celery_trigger_store.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/trigger/dynamodb_post_process_event_handler.py` & `persisty-0.0.7/persisty/trigger/dynamodb_post_process_event_handler.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/trigger/serverless_trigger_handler.py` & `persisty-0.0.7/persisty/trigger/serverless_trigger_handler.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/trigger/store_triggers.py` & `persisty-0.0.7/persisty/trigger/store_triggers.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/trigger/wrapper.py` & `persisty-0.0.7/persisty/trigger/wrapper.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/util/__init__.py` & `persisty-0.0.7/persisty/util/__init__.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/util/encrypt_at_rest.py` & `persisty-0.0.7/persisty/util/encrypt_at_rest.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/util/logify.py` & `persisty-0.0.7/persisty/util/logify.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty/util/undefined.py` & `persisty-0.0.7/persisty/util/undefined.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/persisty.egg-info/PKG-INFO` & `persisty-0.0.7/persisty.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: persisty
-Version: 0.0.6
+Version: 0.0.7
 Summary: A better persistence layer for python
 Home-page: https://github.com/tofarr/lambsync
 Author: Tim O'Farrell
 Author-email: tofarr@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `persisty-0.0.6/persisty.egg-info/SOURCES.txt` & `persisty-0.0.7/persisty.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/setup.py` & `persisty-0.0.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,33 +3,33 @@
 from persisty.__version__ import __version__
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 extras_require = {
     "sql": ["SQLAlchemy~=1.4"],
-    "server": ["servey[server]~=2.7"],
-    "serverless": ["servey[serverless]~=2.7"]
+    "server": ["servey[server]~=2.8"],
+    "serverless": ["servey[serverless]~=2.8"]
 }
 
 setuptools.setup(
     name="persisty",
     version=__version__,
     author="Tim O'Farrell",
     author_email="tofarr@gmail.com",
     description="A better persistence layer for python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/tofarr/lambsync",
     packages=setuptools.find_packages(exclude=("tests",)),
     install_requires=[
-        "marshy~=3.0",
+        "marshy~=4.0",
         "pyaes~=1.6",
-        "schemey~=5.7",
-        "servey~=2.7",
+        "schemey~=6.0",
+        "servey~=2.8",
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
 )
```

### Comparing `persisty-0.0.6/tests/attr/generator/test_defaults.py` & `persisty-0.0.7/tests/attr/generator/test_defaults.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/tests/attr/test_attr.py` & `persisty-0.0.7/tests/attr/test_attr.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/tests/attr/test_attr_filter.py` & `persisty-0.0.7/tests/attr/test_attr_filter.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/tests/attr/test_attr_filter_op.py` & `persisty-0.0.7/tests/attr/test_attr_filter_op.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/tests/factory/test_default_store_factory.py` & `persisty-0.0.7/tests/factory/test_default_store_factory.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/tests/factory/test_owned_store_factory.py` & `persisty-0.0.7/tests/factory/test_owned_store_factory.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/tests/finder/test_module_store_finder.py` & `persisty-0.0.7/tests/finder/test_module_store_finder.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/tests/fixtures/number_name.py` & `persisty-0.0.7/tests/fixtures/number_name.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/tests/fixtures/storage_tst_abc.py` & `persisty-0.0.7/tests/fixtures/storage_tst_abc.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/tests/fixtures/super_bowl_results.py` & `persisty-0.0.7/tests/fixtures/super_bowl_results.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/tests/impl/dynamodb/test_dynamodb_store.py` & `persisty-0.0.7/tests/impl/dynamodb/test_dynamodb_store.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/tests/impl/mem/test_mem_store.py` & `persisty-0.0.7/tests/impl/mem/test_mem_store.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/tests/impl/sqlalchemy/test_sqlalchemy_table_store.py` & `persisty-0.0.7/tests/impl/sqlalchemy/test_sqlalchemy_table_store.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/tests/util/test_encrypt_at_rest.py` & `persisty-0.0.7/tests/util/test_encrypt_at_rest.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/tests/util/test_logify.py` & `persisty-0.0.7/tests/util/test_logify.py`

 * *Files identical despite different names*

### Comparing `persisty-0.0.6/tests/util/test_util.py` & `persisty-0.0.7/tests/util/test_util.py`

 * *Files identical despite different names*

